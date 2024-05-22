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

**Solução**:

Cada elétron tem carga igual a $e^- = -1,602\times 10^{-19}C$. Portanto, $4.600$ elétrons terão $4.600 \times (-1,602\times 10^{-19}C) = -7,369\times 10^{-16}C$


### Exemplo 2

A carga total entrando em um terminal é dada por $q = 5t\ sen(4\pi t)mC$. Calcule a corrente no instante $t = 0,5s$.

**Solução**:

$$i = \frac{dq}{dt} = \frac{d}{dt}(5t\ sen(4\pi t))mC/s = 5sen(4\pi t) + 20\pi t\ cos(4\pi t) mA$$

Para $t = 0,5s$:

$$i = 5 sen(2\pi) + 10\pi cos(2\pi) = 0 + 10\pi = 31,42mA$$

### Exemplo 3

Determine a carga total que entra em um terminal entre os instantes $t = 1s$ e $t = 2s$ se a corrente que  passa pelo terminal é $i = (3t^2 - t)A$.

**Solução**:

$$Q = \int_{t=1}^{2}i\ dt = \int_{1}^{2}(3t^2 -t)dt = \left(t^3 - \frac{t^2}{2} \right) \Bigg|_{1}^{2} = (8 - 2) - \left( 1 - \frac{1}{2}\right) = 5,5C$$


## Tensão

## Potência e energia

## Elementos de circuito
