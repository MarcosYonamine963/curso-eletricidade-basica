# Aula 03

# Capacitores e indutores

## Capacitores

Um capacitor é formado por duas placas condutores separadas por um material dielétrico (isolante). A principal função de um capacitor é armazenar energia em seu campo elétrico.

Quando uma fonte de tensão $\large v$ é aplicada ao capacitor, a fonte deposita uma carga positiva $\large q$ sobre uma placa e uma carga negativa $\large -q$ na outra. A quantidade de carga $\large q$ armazenada é diretamente proporcional à tensão $\large v$ aplicada, de modo que:


$$\large q = Cv$$

em que $\large C$ é chamada de _capacitância_, medida em farad ($\large F$), em homenagem ao físico inglês Michael Faraday.

A quantidade de carga armazenada também depende das dimensões físicas do capacitor, além do material do dielétrico. Assim, a capaciância de duas placas paralelas pode ser dada por:

$$\large C = \frac{\epsilon A}{d}$$

em que $\large \epsilon$ é a permissividade elétrica do material dielétrico, $\large A$ é a área de cada placa condutora, e $\large d$ é a distância que separa as duas placas.

A figura seguinte mostra a simbologia de um capacitor.

<p align="center">
  <img width='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/569c6747-6c59-46c8-8ecb-ce8c124a8d96" />
</p>

A corrente que passa pelo capacitor é definida pela derivada da carga armazenada. Ou seja, sabendo que $\large q = Cv$, temos:

$$\large i = C\frac{dv}{dt}$$

Isolando-se a tensão e integrando a equação, temos:

$$\large v(t) = \frac{1}{C}\int_{-\infty}^{t}i(\tau)d\tau$$

ou ainda,

$$\large v(t) = \frac{1}{C}\int_{t_0}^{t}i(\tau)d\tau + v(t_0)$$

onde $\large v(t_0) = q(t_0)/C$ é a tensão no capacitor no instante $\large t_0$. Isso mostra que a tensão do capacitor depende do histórico da corrente.

A energia armmazenada no capacitor é dada por:

$$\large w = \frac{1}{2}Cv^2$$

ou ainda,

$$\large w = \frac{q^2}{2C}$$

### Propriedades

* Um capacitor é um circuito aberto em CC.

* A tensão no capacitor não pode variar abruptamente.

## Capacitores em série e em paralelo

## Indutores

## Indutores em série e em paralelo


# Sinais variantes no tempo

## Valor médio e eficaz (RMS)

## Potência média e eficaz (RMS)

# Dispositivos semicondutores

## Condutores

## Semicondutores

## Cristais de silício

## Dopagem de um semicondutor

## Junção PN

## Polarização direta

## Polarização reversa

## Ruptura

# Diodo

## Diodo ideal e aproximações

## Retas de carga

## Retificador de meia onda

## Transformador

## Retificador de onda completa com _tap_ central

## Retificador de onda completa em ponte

## Filtro de entrada com indutor

## Filtro de entrada com capacitor

## Ripple

## Circuitos ceifadores e limitadores

## Circuitos grampeadores

## Circuitos multiplicadores de tensão

# Diodo Zener

## Regulador zener

## Regulador zener com carga

## Retas de carga do diodo zener

# LED

# Diodo Schottky

# Varactor


# Transistores de junção bipolar

## Transistor não polarizado

## Transistor polarizado

## Correntes no transistor

## Ganho de corrente

## Conexão Emissor Comum

## Curva de base do Emissor Comum

## Curva de coletor do Emissor Comum

## Reta de carga do Emissor Comum

## Ponto quiescente (Q)

## Transistor como chave

## Polarização do Emissor

## Polarização da Base

## Polarização por divisor de tensão (PDT)

## PDT bem projetado

## Reta de carga e ponto Q para o PDT

## Polarização do emissor com fonte dupla


## Polarização por realimentação do emissor

## Polarização por realimentação do coletor-emissor

## Transistores PNP


# Resumo (Transistores)










