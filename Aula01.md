# Aula 01 - Conceitos Básicos

## Introdução

Nesta aula serão apresentados os conceitos básicos de....

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

## Elementos de circuito
