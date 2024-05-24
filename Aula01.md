# Aula 01

Nesta aula serão apresentados os conceitos básicos de carga e corrente, tensão, potência e energia, além de algumas leis básicas, fundamentais para a análise de circuitos elétricos.

# Conceitos básicos


## Carga e corrente

>**Carga** é uma propriedade elétrica das partículas atômicas que compõem a matéria, medida em coulombs ($C$).

O conceito de carga elétrica é o princípio fundamental para explicar todos os fenômenos elétricos. A carga é a quantidade mais elementar de um circuito elétrico.

A carga $e^-$ de um elétron é negativa, e tem uma magnitude de $1,602\times 10^{-19}C$:

$$e^- = -1,602\times 10^{-19}C$$

>**Corrente elétrica** é o fluxo de carga por unidade de tempo, medido em ampères ($A$).

Matematicamente, a relação entre a corrente $i$, a carga $q$ e o tempo $t$ é:

$$i \triangleq \frac{dq}{dt}$$

onde a corrente é medida em ampères ($A$) e 1 ampère = 1 coulomb/segundo.

A carga transferida entre o instante $t_0$ e o instante $t$ é obtida integrando ambos os lados da equação anterior:

$$Q \triangleq \int_{t_0}^{t}i\ dt$$

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


### Exemplo 1

Qual é a quantidade de carga representada por $4.600$ elétrons?


<details>
<summary>Solução</summary>

Cada elétron tem carga igual a $e^- = -1,602\times 10^{-19}C$. Portanto, $4.600$ elétrons terão $4.600 \times (-1,602\times 10^{-19}C) = -7,369\times 10^{-16}C$

</details>


### Exemplo 2

A carga total entrando em um terminal é dada por $q = 5t\ sen(4\pi t)mC$. Calcule a corrente no instante $t = 0,5s$.


<details>
<summary>Solução</summary>
  
$$i = \frac{dq}{dt} = \frac{d}{dt}(5t\ sen(4\pi t))mC/s = 5sen(4\pi t) + 20\pi t\ cos(4\pi t) mA$$

Para $t = 0,5s$:

$$i = 5 sen(2\pi) + 10\pi cos(2\pi) = 0 + 10\pi = 31,42mA$$

</details>

### Exemplo 3

Determine a carga total que entra em um terminal entre os instantes $t = 1s$ e $t = 2s$ se a corrente que  passa pelo terminal é $i = (3t^2 - t)A$.


<details>
<summary>Solução</summary>

$$Q = \int_{t=1}^{2}i\ dt = \int_{1}^{2}(3t^2 -t)dt = \left(t^3 - \frac{t^2}{2} \right) \Bigg|_{1}^{2} = (8 - 2) - \left( 1 - \frac{1}{2}\right) = 5,5C$$

</details>

## Tensão

Para deslocar um elétron em um condutor a um determinado sentido, é necessária uma força eletromotriz (FEM). Essa força também é conhecida como _tensão elétrica_ ou _diferença de potencial_. 

>A tensão $v_{ab}$ entre dois pontos $a$ e $b$ em um circuito elétrico é a energia necessária para deslocar uma carga unitária de $a$ para $b$. A tensão é medida em volts ($V$).

$$v_{ab} \triangleq \frac{dw}{dq}$$

em que $w$ é a energia em joules ($J$).

<p align="center">
  <img height='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/825fac87-6163-499f-96ea-1ad868142d48" />
</p>

Observe a polaridade na representação da tensão. Podemos dizer que o ponto $a$ se encontra a um potencial de $v_{ab}$ volts mais alto que o ponto $b$. Podemos dizer ainda que, de $a$ para $b$ houve uma queda de tensão no valor de $v_{ab}$.

Segue que, em geral, uma queda de tensão de $a$ para $b$ é equivalente a uma elevação de tensão de $b$ para $a$:

$$v_{ab} = -v_{ba}$$

## Potência e energia

>**Potência** é a velocidade com que se consome ou se absorve energia, medida em watts ($W$).

Matematicamente, escrevemos como:

$$p \triangleq \frac{dw}{dt}$$

em que $w$ é a energia em joules ($J$), $t$ é o tempo em segundos ($s$) e $p$ é a potência em watts ($W$).

Da equação anterior, temos ainda que:

$$p = \frac{dw}{dt} = \frac{dw}{dq}\cdot\frac{dq}{dt} = v\cdot i$$

$$p = v\cdot i$$

O sentido da corrente e a polaridade da tensão desempenham um papel fundamental na determinação do sinal da potência em um elemento. 

Pela _convenção de sinal passivo_, quando a corrente entra pela polaridade positiva da tensão, a potência nesse elemento será positiva ($p = +vi$). Quando a corrente entra pela polaridade negativa da tensão, a potência nesse elemento será negativa ($p = -vi$). 

Quando a potência é positiva, dizemos que o elemento está absorvendo (consumindo) energia. Quando a potência é negativa, o elemento está liberando (fornecendo) energia ao circuito.

<p align="center">
  <img height='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/e62a6a6d-07e3-40a1-babe-46aff57ce820" />
</p>

>A _lei da conservação da energia_ diz que a soma algébrica da potência em um circuito, a qualquer instante de tempo, deve ser igual a zero.

$$\sum p = 0$$

Em outras palavras, a potência total fornecida ao circuito deve ser igual à potência total absorvida.


## Consumo de energia

>Energia é a capacidade de realizar trabalho, e é medida em joules ($J$).

A energia absorvida ou fornecida (convenção sinal passivo) por um elemento do instante $t_0$ ao instante $t$ é

$$w = \int_{t_0}^{t}p\ dt = \int_{t_0}^{t}vi\ dt = $$

As concessionárias de energia elétrica medem a energia em watts-hora ($Wh$), em que

$$1 Wh = 3.600 J$$

### Exemplo 4

Uma fonte de energia com uma corrente constante de $2A$ força a passagem dessa conrrente através de uma lâmpada por $10s$. Se forem liberados $2,3kJ$ na forma de energia luminosa e calorífica, calcule a queda de tensão na lâmpada.

<details>
<summary>Solução</summary>


A carga total é:

$$dq = i\ dt = 2A \cdot 10s = 20C$$

A queda de tensão é:

$$v = \frac{dw}{dq} = \frac{2,3\times 10^3J}{20C} = 115V$$


</details>


### Exemplo 5

Quanta energia uma lâmpada de 100W consome em duas horas?

<details>
<summary>Solução</summary>

Como a potência da lâmpada é uma constante,

$$w = \int p\ dt = pt = 100W\cdot 2h = 200Wh$$

Isso é o mesmo que:

$$w = 200Wh \cdot 3.600\frac{J}{Wh} = 720\times 10^3 J = 720kJ$$


</details>


### Exemplo 6

Se uma concessionária de energia cobra $30$ centavos por $kWh$ consumido, qual o valor cobrado referente a 5 lâmpadas fluorescentes de $40W$ cada, mantidas acesas durante 30 dias? Se todas as lâmpadas forem substituídas por lâmpadas de led de 10W, qual será a economia mensal?

<details>
<summary>Solução</summary>

Como a potência das lâmpadas é constante, para 5 lâmpadas, temos que

$$w = 5pt = 5\cdot 40W\cdot 30\cdot 24h = 144kWh$$

O valor cobrado por essa energia será $(30centavos/kWh) \cdot 144kWh = 4.320 centavos = 43,2 reais$

Substituindo as lâmpadas por led, temos:

$$w = 5pt = 5\cdot 10W\cdot 30\cdot 24h = 36kWh$$

O valor cobrado por essa energia será $(30centavos/kWh) \cdot 36kWh = 1.080 centavos = 10,8 reais$

Portanto, a economia foi de $(43,2 - 10,8)reais = 32,4 reais$, que representa uma economia de

$$\frac{32,4}{43,2}\times 100\\% = 75\\% $$


</details>




## Elementos de Circuitos

Existem dois tipos de elementos encontrados nos circuitos elétricos: elementos _passivos_ e elementos _ativos_. Um elemento passivo não gera energia, porém, pode (ou não) armazenar energia. São o caso dos **resistores**, **capacitores** e **indutores**, por exemplo. Um elemento ativo é capaz de "gerar" energia em um circuito elétrico. É o caso das **fontes de tenão e de corrente**.

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

## Nós, ramos e laços

## Leis de Kirchhoff

## Resistores em série e divisão de tensão

## Resistores em paralelo e divisão de corrente

## Transformações $Y-\Delta$ (estrela-triângulo)






