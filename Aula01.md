# Aula 01

Nesta aula serão apresentados os conceitos básicos de carga e corrente, tensão, potência e energia, além de algumas leis básicas, fundamentais para a análise de circuitos elétricos.

# Conceitos básicos


## Carga e corrente

>**Carga** é uma propriedade elétrica das partículas atômicas que compõem a matéria, medida em coulombs ($\large C$).

O conceito de carga elétrica é o princípio fundamental para explicar todos os fenômenos elétricos. A carga é a quantidade mais elementar de um circuito elétrico.

A carga $\large e^-$ de um elétron é negativa, e tem uma magnitude de $\large 1,602\times 10^{-19}C$:

$$\large e^- = -1,602\times 10^{-19}C$$

>**Corrente elétrica** é o fluxo de carga por unidade de tempo, medido em ampères ($\large A$).

Matematicamente, a relação entre a corrente $\large i$, a carga $\large q$ e o tempo $\large t$ é:

$$\large i \triangleq \frac{dq}{dt}$$

onde a corrente é medida em ampères ($\large A$) e 1 ampère = 1 coulomb/segundo.

A carga transferida entre o instante $\large t_0$ e o instante $\large t$ é obtida integrando ambos os lados da equação anterior:

$$\large Q \triangleq \int_{t_0}^{t}i\ dt$$

Nos circuitos elétricos, podemos ter dois tipos de corrente: contínua e alternada. 

>**Corrente contínua** (CC) é uma corrente que permanece constante ao longo do tempo.

<p align="center">
  <img width='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/de17139a-be7c-4d58-b713-0cce8fa93ad2" />
</p>

>**Corrente alternada** (CA) é uma corrente que varia com o tempo.

<p align="center">
  <img width='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/27135293-bcce-401a-9308-b279a7828a4b" />
</p>

Ao definirmos corrente como a movimentação de cargas, é esperado que ela tenha um sentido de fluxo associado. Esse sentido é, por convenção, tomado como o sentido de movimentação das cargas positivas. Ou ainda, é o sentido oposto ao da movimentação dos elétrons.

<p align="center">
  <img width='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/4a40187e-a3d3-4f93-a2e8-c4ec6a6929b1" />
</p>

---

### Exemplo

Qual é a quantidade de carga representada por $\large 4.600$ elétrons?


<details>
<summary>Solução</summary>

Cada elétron tem carga igual a $\large e^- = -1,602\times 10^{-19}C$. Portanto, $\large 4.600$ elétrons terão $\large 4.600 \times (-1,602\times 10^{-19}C) = -7,369\times 10^{-16}C$

</details>

---

### Exemplo

A carga total entrando em um terminal é dada por $\large q = 5t\ sen(4\pi t)mC$. Calcule a corrente no instante $\large t = 0,5s$.


<details>
<summary>Solução</summary>
  
$$\large i = \frac{dq}{dt} = \frac{d}{dt}(5t\ sen(4\pi t))mC/s = 5sen(4\pi t) + 20\pi t\ cos(4\pi t) mA$$

Para $\large t = 0,5s$:

$$\large i = 5 sen(2\pi) + 10\pi cos(2\pi) = 0 + 10\pi = 31,42mA$$

</details>

---

### Exemplo

Determine a carga total que entra em um terminal entre os instantes $\large t = 1s$ e $\large t = 2s$ se a corrente que  passa pelo terminal é $\large i = (3t^2 - t)A$.


<details>
<summary>Solução</summary>

$$\large Q = \int_{t=1}^{2}i\ dt = \int_{1}^{2}(3t^2 -t)dt = \left(t^3 - \frac{t^2}{2} \right) \Bigg|_{1}^{2} = (8 - 2) - \left( 1 - \frac{1}{2}\right) = 5,5C$$

</details>

---

## Tensão

Para deslocar um elétron em um condutor a um determinado sentido, é necessária uma força eletromotriz (FEM). Essa força também é conhecida como _tensão elétrica_ ou _diferença de potencial_. 

>A tensão $\large v_{ab}$ entre dois pontos $\large a$ e $\large b$ em um circuito elétrico é a energia necessária para deslocar uma carga unitária de $\large a$ para $\large b$. A tensão é medida em volts ($\large V$).

$$\large v_{ab} \triangleq \frac{dw}{dq}$$

em que $\large w$ é a energia em joules ($\large J$).

<p align="center">
  <img height='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/825fac87-6163-499f-96ea-1ad868142d48" />
</p>

Observe a polaridade na representação da tensão. Podemos dizer que o ponto $\large a$ se encontra a um potencial de $\large v_{ab}$ volts mais alto que o ponto $\large b$. Podemos dizer ainda que, de $\large a$ para $\large b$ houve uma queda de tensão no valor de $\large v_{ab}$.

Segue que, em geral, uma queda de tensão de $\large a$ para $\large b$ é equivalente a uma elevação de tensão de $\large b$ para $\large a$:

$$\large v_{ab} = -v_{ba}$$

## Potência e energia

>**Potência** é a velocidade com que se consome ou se absorve energia, medida em watts ($\large W$).

Matematicamente, escrevemos como:

$$\large p \triangleq \frac{dw}{dt}$$

em que $\large w$ é a energia em joules ($\large J$), $t$ é o tempo em segundos ($\large s$) e $\large p$ é a potência em watts ($\large W$).

Da equação anterior, temos ainda que:

$$\large p = \frac{dw}{dt} = \frac{dw}{dq}\cdot\frac{dq}{dt} = v\cdot i$$

$$\large p = v\cdot i$$

O sentido da corrente e a polaridade da tensão desempenham um papel fundamental na determinação do sinal da potência em um elemento. 

Pela _convenção de sinal passivo_, quando a corrente entra pela polaridade positiva da tensão, a potência nesse elemento será positiva ($\large p = +vi$). Quando a corrente entra pela polaridade negativa da tensão, a potência nesse elemento será negativa ($\large p = -vi$). 

Quando a potência é positiva, dizemos que o elemento está absorvendo (consumindo) energia. Quando a potência é negativa, o elemento está liberando (fornecendo) energia ao circuito.

<p align="center">
  <img height='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/e62a6a6d-07e3-40a1-babe-46aff57ce820" />
</p>

>A _lei da conservação da energia_ diz que a soma algébrica da potência em um circuito, a qualquer instante de tempo, deve ser igual a zero.

$$\large \sum p = 0$$

Em outras palavras, a potência total fornecida ao circuito deve ser igual à potência total absorvida.


## Consumo de energia

>Energia é a capacidade de realizar trabalho, e é medida em joules ($\large J$).

A energia absorvida ou fornecida (convenção sinal passivo) por um elemento do instante $\large t_0$ ao instante $\large t$ é

$$\large w = \int_{t_0}^{t}p\ dt = \int_{t_0}^{t}vi\ dt = $$

As concessionárias de energia elétrica medem a energia em watts-hora ($\large Wh$), em que

$$\large 1 Wh = 3.600 J$$

---

### Exemplo

Uma fonte de energia com uma corrente constante de $\large 2A$ força a passagem dessa conrrente através de uma lâmpada por $\large 10s$. Se forem liberados $\large 2,3kJ$ na forma de energia luminosa e calorífica, calcule a queda de tensão na lâmpada.

<details>
<summary>Solução</summary>

A carga total é:

$$\large dq = i\ dt = 2A \cdot 10s = 20C$$

A queda de tensão é:

$$\large v = \frac{dw}{dq} = \frac{2,3\times 10^3J}{20C} = 115V$$

</details>

---

### Exemplo

Quanta energia uma lâmpada de $\large 100W$ consome em duas horas?

<details>
<summary>Solução</summary>

Como a potência da lâmpada é uma constante,

$$\large w = \int p\ dt = pt = 100W\cdot 2h = 200Wh$$

Isso é o mesmo que:

$$\large w = 200Wh \cdot 3.600\frac{J}{Wh} = 720\times 10^3 J = 720kJ$$

</details>

---

### Exemplo

Se uma concessionária de energia cobra $\large 30$ centavos por $\large kWh$ consumido, qual o valor cobrado referente a 5 lâmpadas fluorescentes de $\large 40W$ cada, mantidas acesas durante 30 dias? Se todas as lâmpadas forem substituídas por lâmpadas de led de $\large 10W$, qual será a economia mensal?

<details>
<summary>Solução</summary>

Como a potência das lâmpadas é constante, para 5 lâmpadas, temos que

$$\large w = 5pt = 5\cdot 40W\cdot 30\cdot 24h = 144kWh$$

O valor cobrado por essa energia será $\large (30centavos/kWh) \cdot 144kWh = 4.320 centavos = 43,2 reais$

Substituindo as lâmpadas por led, temos:

$$\large w = 5pt = 5\cdot 10W\cdot 30\cdot 24h = 36kWh$$

O valor cobrado por essa energia será $\large (30centavos/kWh) \cdot 36kWh = 1.080 centavos = 10,8 reais$

Portanto, a economia foi de $\large (43,2 - 10,8)reais = 32,4 reais$, que representa uma economia de

$$\large \frac{32,4}{43,2}\times 100\\% = 75\\% $$

</details>

---

## Elementos de Circuitos

Existem dois tipos de elementos encontrados nos circuitos elétricos: elementos _passivos_ e elementos _ativos_. Um elemento passivo não gera energia, porém, pode (ou não) armazenar energia. São o caso dos **resistores**, **capacitores** e **indutores**, por exemplo. Um elemento ativo é capaz de "gerar" energia em um circuito elétrico. É o caso das **fontes de tensão e de corrente**.

A rigor, nenhuma energia pode ser criada (pela lei da conservação da energia). Toda energia é transformada. Por exemplo, um gerador elétrico de uma usina hidrelétrico transforma a energia cinética (rotação motor) em energia elétrica. Uma bateria converte a energia química em energia elétrica. Em circuitos elétricos, consideramos tais elementos como geradores, ou fontes de energia.

Existem dois tipos de fontes: dependentes e independentes.

>Uma **fonte independente ideal** é um elemento ativo que fornece uma tensão ou corrente específica que é completamente independente de outros elementos do circuito.

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/77f91fe7-e480-4338-8286-74eea73702c3" />
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/ecc051a6-4a17-4406-944a-af5a000d54e7" />
</p>

>Uma **fonte dependente** (ou **controlada**) **ideal** é um elemento ativo no qual a quantidade de energia é controlada por outra tensão ou corrente.

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/4ceeff06-bc4b-44fa-a8c6-6782480aac04" />
</p>


Existem quatro tipos de fontes dependentes:

* Fonte de **tensão** controlada por **tensão**
* Fonte de **tensão** controlada por **corrente**
* Fonte de **corrente** controlada por **tensão**
* Fonte de **corrente** controlada por **corrente**

Ex: em cada circuito abaixo, a fonte da esquerda é uma fonte independente, e a da direita é uma dependente.

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/ab972ccd-b0f5-4cb6-a426-77bcdf5e59e4" />
</p>


# Leis básicas

## Lei de Ohm

A _Resistência_ é a propriedade dos materiais de resistir à passagem de corrente elétrica. Essa propriedade é representada pela letra $\large R$, e depende do comprimento do material, da área da seção transversal e da _resistividade_ do material, conforme a seguinte relação: 

$$\large R = \rho\frac{l}{A}$$

em que $\large \rho$ é a _resistividade do material_, $\large l$ é o comprimento e $\large A$ é a área da seção transversal.

<p align="center">
  <img height='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/318c730a-8210-4371-8067-7ef115096a96" />
</p>


Os valores da _resistividade_ de alguns materiais são mostrados na tabela abaixo:

<p align="center">
  <img height='500' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/31d929a9-90fe-4488-bc0c-e20849b7481f" />
</p>


O elemento de circuito utilizado para modelar a propriedade da _resistência_ é o **resistor**. Observe a simbologia. A letra $\large R$ representa o valor resistência do resistor, medida em $\large \Omega$.

<p align="center">
  <img width='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/61053714-2247-407f-8525-a00d61b85cdf" />
</p>


>A **Lei de Ohm** afirma que a tensão $\large v$ em um resistor é diretamente proporcional à corrente $\large i$ através dele, e a resistência $\large R$ é a constante de proporcionalidade.

Matematicamente, temos:

$$\large v = Ri$$

Porém, devemos também considerar o sentido que a corrente flui em relação à polaridade da queda de tensão no resistor:

<p align="center">
  <img width='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/b92c355d-4346-4d22-8cb3-a46cf36358dd" />
</p>




## Curto-circuito e Circuito aberto

Em análises de circuitos, quando dizemos que um elemento está em curto-cirucito, equivale dizer que a resistência e a tensão em seus terminais podem ser aproximados a zero. Nesse caso, a corrente nesse elemento será determinada pelo restante do circuito.

Quando dizemos que o elemento é um circuito aberto, equivale dizer que a corrente que passa por ele pode ser aproximada de zero, enquanto que a resistência pode ser aproximada de infinito. Nesse caso, a tensão nos terminais do elemento será determinada pelo restante do circuito.

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/834da3c2-46d1-4c3a-9e22-9f62b22a903a" />
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/293482c9-886e-4305-80c1-f6f91c2d4979" />
</p>

O comportamento de curto-circuito e circuito aberto pode ser modelado por uma chave interruptora ideal. Quando a chave está fechada (permitindo passagem de corrente), ela se comporta como um curto-circuito. Quando a chave está aberta (impedindo a passagem de corrente), ela se comporta como um circuito aberto.

<p align="center">
  <img width='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/4160df84-49ab-40cf-808f-3790569b99ec" />
</p>

## Potência com a Lei de Ohm

Vimos que a potência pode ser expressa como 

$$\large p = vi$$

Mas, pela Lei de Ohm,

$$\large v = Ri$$

$$\large i = \frac{v}{R}$$

temos outras possibilidades de representar a potência:

$$\large p = vi = Ri^2 = \frac{v²}{R}$$

---

### Exemplo 

Um ferro elétrico consome $\large 2A$ quando ligado a uma tensão de $\large 120V$. Determine a resistência interna dele.

<details>
<summary>Solução</summary>

Pela Lei de Ohm, temos que:

$$\large R = \frac{v}{i} = \frac{120V}{2A} = 60\Omega$$

</details>

---

### Exemplo

Para o circito abaixo, determine a corrente $\large i$ e a potência no resistor.

<p align="center">
  <img width='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/bc174c61-180a-44c9-8475-3d3fc759fc4f" />
</p>

<details>
<summary>Solução</summary>

Pela Lei de Ohm, temos que:

$$\large i = \frac{v}{R} = \frac{30V}{5k\Omega} = 6mA$$

Portanto, a potência no resistor é:

$$\large p = vi = 30V\cdot 6mA = 180mW$$

</details>

---

## Nós, ramos e laços

Uma vez que os elementos de um circuito elétrico podem ser interconectados
de diversas maneiras, precisamos compreender alguns conceitos básicos de
topologia de rede, que são os **nós**, **ramos** e os **laços**.


>**Ramo** representa um elemento único como fonte de tensão ou resistor.

> **Nó** é o ponto de conexão entre dois ou mais ramos.

>**Laço** é qualquer caminho fechado em um circuito.

Na figura abaixo, temos um circuito elétrico com 5 ramos e 3 nós ($\large a$, $\large b$ e $\large c$).

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/8c048745-36d9-4098-9455-51e33bb305a9" />
</p>

Observe que podemos formar no total, 6 caminhos fechados pelo circuito. Portanto, o número total de laços é 6. Porém, o circuito possui apenas 3 laços independentes. Diz-se que um laço é independente se ele contiver pelo menos um ramo que não faça parte de qualquer outro laço independente.

Outros dois conceitos importantes na topologia de circuitos são os coceitos de elementos em série e em paralelo.

>Dois ou mais elementos estão em **série** se eles compartilharem exclusivamente um único nó e, consequentemente, transportarem a mesma corrente.

>Dois ou mais elementos estão em **paralelo** se eles estiverem conectados aos mesmos dois nós e, consequentemente, tiverem a mesma tensão entre eles.

## Leis de Kirchhoff

>A **Lei de Kirchhoff para corrente (LKC)** diz que a soma algébrica de todas as correntes em qualquer nó é zero.

$$\large \sum_{n=1}^{N}i_n = 0$$

Isso implica que a soma de todas as correntes que entram em um nó é igual à soma de todas as correntes que saem desse nó.

---

### Exemplo

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/a8a074cd-bc4c-4547-94f6-387a63953946" />
</p>

$$\large i_1 + i_3 + i_4 = i_2 + i_5$$

$$\large i_1 -i_2 + i_3 + i_4 - i_5 = 0$$

---

>A **Lei de Kirchhoff para tensão (LKT)** diz que a soma algébrica de todas as tensões ao longo de qualquer caminho fechado (laço) é zero.

Isso implica que a soma de todas as quedas de tensões devem ser iguais à soma de todas as elevações de tensões em um caminho fechado.

---

### Exemplo

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/bf9dbd67-4860-4f80-915f-e8aa50277f26" />
</p>


$$\large v_1 + v_4 = v_2 + v_3 + v_5$$

$$\large v_1 - v_2 - v_3 + v_4 - v_5 = 0$$

---

### Exemplo

Determine todas as equações das correntes nos nós $\large a$, $\large b$, $\large c$ e $\large d$ no circuito abaixo.

obs: considere que, no centro do circuito, o cruzamento não é uma conexão elétrica, ou seja, $\large i_4$ entra no nó $\large c$, e $\large i_a$ sai do nó $\large d$. 

<p align="center">
  <img width='500' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/2fdb8908-746f-4a06-9d6d-8c95f8114750" />
</p>

<details>
<summary>Solução</summary>

* Nó $\large a$: $\large i_1 + i_4 - i_2 - i_5 = 0$
* Nó $\large b$: $\large i_2 + i_3 - i_1 - i_b -i_a = 0$
* Nó $\large c$: $\large i_b - i_3 - i_4 - i_c = 0$
* Nó $\large d$: $\large i_5 + i_a + i_c = 0$

</details>

---

### Exemplo

Determine todas as equações das tensões nos laços indicados ($\large a$, $\large b$, $\large c$ e $\large d$) no circuito abaixo.

<p align="center">
  <img width='500' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/cdd5fc5b-3102-436e-8730-da4cf4027bd9" />
</p>

<details>
<summary>Solução</summary>

* Laço $\large a$: $\large -v_1 + v_2 + v_4 - v_b - v_3 = 0$
* Laço $\large b$: $\large -v_a + v_3 + v_5 = 0$
* Laço $\large c$: $\large v_b - v_4 - v_c - v_6 - v_5 = 0$
* Laço $\large d$: $\large -v_a - v_1 + v_2 - v_c + v_7 - v_d = 0$

</details>

---

### Exemplo

Determine as tensões $\large v_1$ e $\large v_2$ no circuito.

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/7e4d17e4-2aa7-46be-be83-5d2d0390a390" />
</p>

<details>
<summary>Solução</summary>

Inicialmente, consideremos que uma corrente $\large i$ flua pelo laço, conforme mostra a figura seguinte.

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/145c42dd-5602-4bf2-a9b4-547f0e5c9b13" />
</p>

Pela Lei de Ohm, temos que 

$$\large v_1 = 2i \qquad\text{e}\qquad v_2 = -3i$$

Aplicando a LKT no laço, temos:

$$\large -20 + v_1 - v_2 = 0$$

$$\large -20 +2i +3i = 0$$

$$\large 5i = 20$$

$$\large i = 4A$$

Finalmente,

$$\large v_1 = 2i = 2\cdot 4 = 8V\qquad \text{3}\qquad v_2 = -3i = -3\cdot 4 = -12V$$

</details>

---

### Exemplo

Determine $\large v_0$ e $\large i$ no circuito.

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/8c9c8870-8479-444e-bc93-1262ffc29aca" />
</p>

<details>
<summary>Solução</summary>

Inicialmente, consideremos que uma corrente $\large i$ flua pelo laço, conforme mostra a figura seguinte. Observe que a corrente do laço trata-se da mesma corrente $\large i$.

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/27f7d6e5-efaf-4708-bb66-0d9e331eb8c6" />
</p>

Aplicando a LKT no laço, temos:

$$\large -12 + 4i + 2v_0 - 4 - v_0 = 0$$

$$\large -16 + 4i + v_0 = 0$$

Aplicando a Lei de Ohm no resistor de $6\Omega$ temos

$$\large v_0 = -6i$$

Substituindo na equação da malha, temos:

$$\large -16 + 4i - 6i = 0$$

$$\large -2i = 16$$

$$\large i = -8A$$

Assim, retornando à Lei de Ohm no resistor de $\large 6\Omega$, temos:

$$\large v_0 = -6i = -6\cdot (-8) = 48V$$

</details>

---

### Exemplo

Determine a corrente $\large i_0$ e a tensão $\large v_0$ no circuito.

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/fc731295-8820-4520-88c5-69b4427d21c6" />
</p>

<details>
<summary>Solução</summary>

Aplicando a LKC no nó $\large a$, obtemos:

$$\large 3 + 0,5i_0 = i_0$$

$$\large i_0 = 6A$$

Pela Lei de Ohm no resistor, temos:

$$\large v_0 = 4i_0 = 4\cdot 6 = 24A$$

</details>

---

### Exemplo

Determine as correntes e tensões no circuito.

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/d210c779-fe6c-4da1-88dd-2a0fe66951ea" />
</p>

<details>
<summary>Solução</summary>

Aplicando a Lei de Ohm nos resistores, temos:

$$\large v_1 = 8i_1\qquad v_2 = 3i_2\qquad v_3 = 6i_3$$

Aplicando a LKC no nó $a$, temos:

$$\large i_1 - i_2 - i_3 = 0$$

Agora, consideremos os seguintes laços:

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/fadb2988-89d8-4489-a4d3-eb0f25cfeed2" />
</p>

* Aplicando LKT no laço 1, temos:

$$\large -30 + v_1 + v_2 = 0$$

Expressando isso em termos das correntes (obtidas pela Lei de Ohm):

$$\large -30 + 8i_1 + 3i_2 = 0$$

Isolando-se $i_1$:

$$\large i_1 = \frac{30 - 3i_2}{8}$$

* Aplicando LKT no laço 2, temos:

$$\large -v_2 + v_3 = 0$$

$$\large v_3 = v_2$$

Observe que isso já era esperado, pois os resistores estão em paralelo.

Expressando isso em termos das corrrentes, temos:

$$\large 6i_3 = 3i_2$$

$$\large i_3 = \frac{i_2}{2}$$

Da LKC (nó $\large a$), temos:

$$\large i_1 - i_2 - i_3 = 0$$

$$\large \frac{30-3i_2}{8} - i_2 - \frac{i_2}{2} = 0$$

Resolvendo a equação, obtemos o valor de $\large i_2$:

$$\large i_2 = 2A$$

Com o valor de $\large i_2$, podemos tereminar o restante dos valores do circuito:

$$\large i_1 = 3A\quad i_3 = 1A\quad v_1 = 24V\quad v_2 = 6V\quad v_3 = 6V$$

</details>

---

## Resistores em série e divisão de tensão

>A **resistência equivalente** de qualquer número de resistores ligados em **série** é a soma das resistências individuais.

Matematicamente, para $\large N$ resistores em série, a resistência equivalente será:

$$\large R_{eq} = \sum_{n = 1}^{N}R_n = R_1 + R_2 + \ldots + R_N$$

---

<details>
<summary>Demonstração</summary>

Considerermos inicialmente um circuito com dois resistores em série conectados a uma fonte de tensão:

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/de0892b5-bb80-4ee3-8ff3-9b9a254beb10" />
</p>

Pela Lei de Ohm, temos que, para cada resistor,

$$\large v_1 = iR_1 \qquad v_2 = iR_2$$

Aplicando LKT no laço (sentido horário), temos:

$$\large -v + v_1 + v_2 = 0$$

$$\large v = v_1 + v_2$$

Combinando com a Lei de Ohm, temos:

$$\large v = iR_1 + iR_2 = i(R_1 + R_2)$$

que podemos reescrever como:

$$\large v = iR_{eq}$$

em que 

$$\large R_{eq} = R_1 + R_2$$

Extendendo-se esta análise para $\large N$ resistores, é possível demosntrar que 

$$\large R_{eq} = \sum_{n = 1}^{N}R_n = R_1 + R_2 + \ldots + R_N$$

</details>

---

Quando dois ou mais resistores estão conectados em série, ocorre entre eles uma divisão de tensão.

Por exemplo, considere dois resistores em série, conforme o circuito abaixo:

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/de0892b5-bb80-4ee3-8ff3-9b9a254beb10" />
</p>

As tensões em cada resistor são dadas por:

$$\large v_1 = v\frac{R_1}{R_1 + R_2} \qquad v_2 = v\frac{R_2}{R_1 + R_2}$$

Genericamente, para uma ligação em série de $\large n$ resistores, com uma tensão de entrada $\large v$, a tensão $\large v_j$ sobre o resistor $\large R_j$ será:

$$\large v_j = v\frac{R_j}{R_1 + R_2 + \ldots + R_n} = v\frac{R_j}{R_{eq}}$$

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/01241a03-b1ef-48da-9993-3ada5a94f222" />
</p>


## Resistores em paralelo e divisão de corrente


>O **inverso da resistência equivalente** de $\large N$ resistores conectados em **paralelo** é a soma dos inversos de cada resistência.

Matematicamente, para $\large N$ resistores em paralelo, a resistência equivalente será:

$$\large \frac{1}{R_{eq}} = \sum_{n=1}^{N}\frac{1}{R_n} = \frac{1}{R_1} + \frac{1}{R_2} + \ldots + \frac{1}{R_N}$$

* Para $\large 2$ resistores em paralelo:

$$\large R_{eq} = \frac{R_1 R_2}{R_1 + R_2}$$

* Para $\large N$ resistores $\large R$ **iguais** em paralelo:

$$\large R_{eq} = \frac{R}{N}$$

---

<details>
<summary>Demonstração</summary>

Considerermos inicialmente um circuito com dois resistores em paralelo conectados a uma fonte de tensão:

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/1fdcd265-1f8b-4eaa-abcc-84a29f143345" />
</p>

Pela Lei de Ohm, temos que,

$$\large v = i_1 R_1 = i_2 R_2$$

ou ainda,

$$\large i_1 = \frac{v}{R_1} \qquad i_2 = \frac{v}{R_2}$$

Aplicando LKC no nó $a$, temos:

$$\large i = i_1 + i_2$$

Combinando com a Lei de Ohm, temos:

$$\large i = \frac{v}{R_1} + \frac{v}{R_2} = v\left( \frac{1}{R_1} + \frac{1}{R_2}\right)$$

que podemos reescrever como:

$$\large i = \frac{v}{R_{eq}}$$

em que 

$$\large \frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2}$$

Extendendo-se esta análise para $\large N$ resistores, é possível demosntrar que 

$$\large \frac{1}{R_{eq}} = \sum_{n=1}^{N}\frac{1}{R_n} = \frac{1}{R_1} + \frac{1}{R_2} + \ldots + \frac{1}{R_N}$$

</details>

---

Quando dois ou mais resistores estão conectados em paralelo, ocorre entre eles uma divisão de corrente.

Por exemplo, considere dois resistores em paralelo, conforme o circuito abaixo:

<p align="center">
  <img width='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/1fdcd265-1f8b-4eaa-abcc-84a29f143345" />
</p>


As correntes em cada resistor são dadas por:

$$\large i_1 = i\frac{R_2}{R_1 + R_2} \qquad i_2 = i\frac{R_1}{R_1 + R_2}$$

Genericamente, para uma ligação em paralelo de $\large n$ resistores, com uma corrente de entrada $\large i$, a corrente $\large i_j$ sobre o resistor $\large R_j$ será:

$$\large i_j = i\frac{R_{eq}}{R_j}$$

<p align="center">
  <img width='600' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/5b16348b-002b-435b-a428-97602dbafeee" />
</p>

---

### Exemplo

Determine $\large R_{eq}$ para o circuito.

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/f5854f0e-2a9c-44ed-9dae-a692eb780d53" />
</p>


<details>
<summary>Solução</summary>

* Resistores de $\large 6\Omega$ e $3\Omega$ em paralelo:

$$\large 6\Omega || 3\Omega = \frac{6 \times 3}{6 + 3} = \frac{18}{9} = 2\Omega$$

* Resistores de $\large 1\Omega$ e $\large 5\Omega$ em série:

$$\large 1\Omega + 5\Omega = 6\Omega$$

Circuito equivalente:

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/a2236bc9-d920-4ca9-9113-52ceb2a968f0" />
</p>

* Resistores de $\large (2\Omega + 2\Omega)$ e $\large 6\Omega$ em paralelo:

$$\large 4\Omega||6\Omega = \frac{4 \times 6}{4 + 6} = \frac{24}{10} = 2,4\Omega$$

Circuito equivalente:

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/1e871fbc-6f26-4b17-bbd9-15c084d1a780" />
</p>

Assim, temos:

$$\large R_{eq} = 4\Omega + 2,4\Omega + 8\Omega = 14,4\Omega$$

</details>

---

### Exemplo

Determine $\large i_0$ e $v_0$ no circuito, e calcule a potência dissipada no resistor de $\large 3\Omega$.

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/c7345751-64d1-4cf2-9f2b-a34c03626025" />
</p>


<details>
<summary>Solução</summary>

* Resistores de $\large 6\Omega$ e $\large 3\Omega$ em paralelo:

$$\large 6\Omega || 3\Omega = \frac{6 \times 3}{6 + 3} = 2\Omega$$

Circuito equivalente:

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/d372cec3-df5b-4b0a-8edf-7206b4ecfff3" />
</p>

Pela Lei de Ohm, podemos determinar a corrente $\large i$:

$$\large i = \frac{12V}{(4+2)\Omega} = 2A$$

* Divisão de tensão ($\large v_0$):

$$\large v_0 = 12\frac{2}{2+4} = 4V$$

Agora que temos os valores de $\large v_0$ e de $\large i$, retornando ao circuito original, $\large i_0$ pode ser determinado de duas formas: pela Lei de Ohm no resistor de $\large 3\Omega$, ou pela divisão de correntes.

* Lei de Ohm:

$$\large i_0 = \frac{v_0}{3} = \frac{4}{3}A$$

* Divisão de correntes:

$$\large i_0 = i\frac{4}{2+4} = 2\frac{4}{6} = \frac{4}{3}A$$

* Potência dissipada no resistor de $\large 3\Omega$:

$$\large p = v_0 i_0 = 4\frac{4}{3} = 5,333W$$

</details>

---

### Exemplo

Determine a tensão $\large v_0$, a potência fornecida pela fonte de corrente e a potência absorvida por cada resistor do circuito.

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/589daf01-f3d3-4102-8da1-75821c40daae" />
</p>



<details>
<summary>Solução</summary>

Os resistores de $\large 6k\Omega$ e $\large 12k\Omega$ estão em série, formando um equivalente de $\large 6 + 12 = 18k\Omega$. Assim, podemos ter um circuito equivalente:

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/fe752ae8-e059-490b-a8e9-7d85e2a8d32f" />
</p>

Agora, aplicamos a divisão de corrente para determinar $\large i_1$ e $\large i_2$:

$$\large i_1 = i_0\frac{18}{9 + 18} = 30mA\frac{18}{9+18} = 20mA$$

$$\large i_2 = i_0\frac{9}{9 + 18} = 30mA\frac{18}{9+18} = 10mA$$

Assim, pela Lei de Ohm,

$$\large v_0 = 9k\Omega\cdot i_1 = 9k\Omega\cdot20mA = 180V$$

A potência fornecida pela fonte é:

$$\large p_0 = v_0 i_0 = 180V\cdot 30mA = 5,4W$$

A potência absorvida pelo resistor de $\large 12k\Omega$ é:

$$\large p = i_2^2\cdot 12k\Omega = (10mA)^2 \cdot 12k\Omega = 1,2W$$

A potência absorvida pelo resistor de $\large 6k\Omega$ é:

$$\large p = i_2^2\cdot 6k\Omega = (10mA)^2 \cdot 6k\Omega = 0,6W$$

A potência absorvida pelo resistor de $\large 9k\Omega$ é:

$$\large p = v_0 i_1 = 180V\cdot 20mA = 3,6W$$


</details>

---


## Transformações $\large Y-\Delta$ (estrela-triângulo)


Muitas vezes surgem situações na análise de circuitos em que os resistores não estão nem em paralelo nem em série. Porém, muitos desses circuitos podem ser simplificados usando-se redes equivalentes de três terminais, que correspondem à rede $\large Y$ (Estrela) e à rede $\large \Delta$ (Triângulo).

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/54f66644-890d-4feb-a690-9c1ed418ec08" /><br/>
  Rede $\large \Delta$ (triângulo ou $\large \Pi$)
</p>


<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/1359cdc2-5d5c-42d0-b45b-41ccad92c8ab" /><br/>
  Rede $\large Y$ (estrela ou $\large T$)
</p>


<p align="center">
  <img height='250' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/ec443663-427a-4c9c-9105-05286c9ea2cf" /><br/>
  Transformação $\large \Delta-Y$
</p>

$$\large R_1 = \frac{R_b R_c}{R_a + R_b + R_c}$$

$$\large R_2 = \frac{R_c R_a}{R_a + R_b + R_c}$$

$$\large R_3 = \frac{R_a R_b}{R_a + R_b + R_c}$$

$$\large R_a = \frac{R_1 R_2 + R_2 R_3 + R_3 R_1}{R_1}$$

$$\large R_b = \frac{R_1 R_2 + R_2 R_3 + R_3 R_1}{R_2}$$

$$\large R_c = \frac{R_1 R_2 + R_2 R_3 + R_3 R_1}{R_3}$$



---

### Exemplo

Determine a corrente elétrica fornecida pela fonte de tensão no circuito.

<p align="center">
  <img height='250' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/7fbbfefb-34c8-4e2a-b7b2-74cd4cd9cf85" />
</p>

<details>
<summary>Solução</summary>

O problema poderá ser resolvido depois de determinarmos a resistência equivalente nos terminais da fonte. Para isso, podemos substituir a rede em $\large \Delta$ superior, formado pelos resistores de $\large 100\Omega$, $\large 125\Omega$ e $\large 25\Omega$, em uma rede em $\large Y$:

<p align="center">
  <img height='250' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/107af2dd-e1b8-4464-9e78-a0c3b069233b" />
</p>

$$\large R_1 = \frac{100\times 125}{100 + 125 + 25} = 50\Omega$$

$$\large R_2 = \frac{125\times 25}{100 + 125 + 25} = 12,5\Omega$$

$$\large R_3 = \frac{100\times 25}{100 + 125 + 25} = 10\Omega$$

Assim, o circuito equivalente fica:

<p align="center">
  <img height='250' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/370b8c92-57d8-477f-b048-a4a5e6e8802c" />
</p>

Observe que $\large 10\Omega$ está em série com $\large 40\Omega$, formando $\large 50\Omega$. Também, $\large 12,5\Omega$ está em série com $\large 37,5\Omega$ formando $\large 50\Omega$. Assim, temos dois resistores de $\large 50\Omega$ em paralelo.

$$\large R_{eq} = 5\Omega + 50\Omega + \frac{50\Omega\cdot 50\Omega}{50\Omega + 50\Omega} = 80\Omega$$

Finalmente,

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/89c6225f-9075-42b2-b61f-4716f6f140d4" />
</p>

$$\large i = \frac{40V}{80\Omega} = 0,5A$$

</details>

---

