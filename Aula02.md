# Aula 02

# Métodos de análise

## Análise nodal

Na análise nodal, estamos interessados em encontrar as tensões nos nós. Para isso, precisamos definir um nó de referência, que costumamos chamá-lo de GND (Ground), Comum, Terra, Chassi, ou simplesmente $\large 0V$. A figura a seguir mostra algumas simbologias comuns para o nó de referência.

<p align="center">
  <img width='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/7e784925-e186-4985-8f89-7564dc9da579" />
</p>

Para gerar uma equação de tensões de um nó, precisamos expressar a corrente que sai do nó, em termos das tensões nodais. Para isso, usamos a Lei de Ohm:

>Em um resistor, a corrente flui de um potencial mais elevado para um potencial mais baixo.


Podemos expressar esse princípio como

$$\large i = \frac{v_{maior} - v_{menor}}{R}$$

em que $\large v_{maior}$ será a tensão nodal no nó que estamos analisando, $\large v_{menor}$ será a tensão no nó seguinte, e $\large R$ será a resistência entre os nós.

---

### Exemplo

Considere o seguinte circuito.

<p align="center">
  <img height='200' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/15ff1571-2838-41a8-a329-c300798b313b" />
</p>

Para o nó 1, imaginamos três correntes saindo dele, e aplicamos a Lei de Ohm:

$$\large \frac{v_1 - 10}{1} + \frac{v_1-v_2}{2} + \frac{v_1}{5} = 0$$


Para o nó 2, imaginamos três correntes saindo dele, porém, observe que a corrente de $\large 2A$ está entrando. Portanto, esta corrente será negativa na equação:

$$\large \frac{v_2 - v_1}{2} + \frac{v_2}{10} - 2 = 0$$

Temos portanto, um sistema com duas equações independentes, e duas variáveis, que pode ser resolvido, obtendo-se

$$\large v_1 = \frac{100}{11} = 9,09V$$

$$\large v_2 = \frac{120}{11} = 10,91V$$

Conhecidas as tensões de nó, todas as correntes de ramo podem ser calculadas.

---


No exemplo anterior, vimos que existe uma fonte de tensão. No caso apresentado, a fonte está conectada entre o nó de referência e outro nó a ser analisado. Nesse caso, a tensão no nó a ser analizado será igual à tensão da fonte (respeitando a polaridade). No caso de a fonte estar conectada em dois nós que não são de referência, aplicaremos o conceito de **supernó**, e utilizaremos a LKC e a LKT para determinar as tensões nodais.

>Um **supernó** é formado envolvendo-se uma fonte de tensão (dependente ou independente) conectada entre dois nós que não são de referência e quaisquer elementos conectados em paralelo com ele.



---

### Exemplo

Observe que no circuito temos três tensões nodais a serem determinadas: $\large v_1$, $\large v_2$, e $\large v_3$. Além disso, consideramos um supernó envolvendo a fonte de tensão de $\large 5V$.

<p align="center">
  <img height='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/4d25ef4c-3bab-4ca7-a7f0-e6f68981175d" />
</p>

A LKC no supernó ficará:

$$\large i_1 + i_4 = i_2 + i_3$$

ou então,

$$\large \frac{v_1 - v_2}{2} + \frac{v_1 - v_3}{4} = \frac{v_2}{8} + \frac{v_3}{6}$$


Para aplicar a LKT no supernó, consideramos o seguinte laço:

<p align="center">
  <img height='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/3cb17fcc-6b7a-4a86-8133-12401d75e2d5" />
</p>

$$\large -v_2 + 5 + v_3 = 0$$

Finalmente, observamos que, devido à fonte de $10V$, 

$$\large v_1 = 10V$$

Assim, temos 3 equações independentes com 3 variáveis, sendo possível encontrar a solução.

---

### Exemplo

Determine as tensões nodais no circuito.

<p align="center">
  <img height='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/3252aaa9-1f25-47ba-b689-a7a3cf9d56ba" />
</p>

<details>
<summary>Solução</summary>

Inicialmente, aplicaremos a LKC nos dois supernós, considerando as seguintes correntes:

<p align="center">
  <img height='400' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/22fc6d8b-21c9-440d-98a4-92e92bbce436" />
</p>

* Supernó $1-2$:

$$\large i_3 + 10 = i_1 + i_2$$

Em termos das tensões nodais:

$$\large \frac{v_3 - v_2}{6} + 10 = \frac{v_1 - v_4}{3} + \frac{v_1}{2}$$

Reorganizando,

$$\large 5v_1 + v_2 - v_3 - 2v_4 = 60$$

* Supernó $3-4$:

$$\large i_1 = i_3 + i_4 + i_5$$

Em termos das tensões nodais:

$$\large \frac{v_1 - v_4}{3} = \frac{v_3 - v_2}{6} + \frac{v_4}{1} + \frac{v_3}{4}$$

Reorganizando,

$$\large 4v_1 + 2v_2 - 5v_3 - 16v_4 = 0$$


Para aplicarmos a LKT, consideremos os seguintes laços:

<p align="center">
  <img height='300' src="https://github.com/MarcosYonamine963/curso-eletricidade-basica/assets/92953755/8bb32126-b557-4b3e-9aab-72ac0dc69468" />
</p>

* Laço 1:

$$\large -v_1 + 20 + v_2 = 0$$

$$\large v_1 - v_2 = 20$$

* Laço 2:

$$\large -v_3 + 3v_x + v_4 = 0$$

Porém, $v_x = v_1 - v_4$, de modo que:

$$\large 3v_1 - v_3 - 2v_4 = 0$$

* Laço 3:

$$\large v_x - 3v_x + (v_3 - v_2) - 20 = 0$$

Como $v_x = v_1 - v_4$, temos:

$$\large -2v_1 - v_2 + v_3 + 2v_4 = 20$$


Temos, portanto, cinco equações para quatro variáveis.


Resolvendo-se as equações (dica: use a regra de cramer), tem-se que 

$$\large v_1 = 26,67V$$

$$\large v_2 = 6,667V$$

$$\large v_3 = 173,33V$$

$$\large v_4 = -46,67V$$


</details>

---


## Análise de malhas

$$\large olair$$

## Análises nodal e de malhas por inspeção

## Análise nodal _versus_ análise de malhas

# Teoremas de circuitos

## Propriedade da linearidade

## Superposição

## Transformação de fontes

## Teorema de Thévenin

## Teorema de Norton

## Dedução dos teoremas de Thévenin e de Norton

## Máxima transferência de potência

