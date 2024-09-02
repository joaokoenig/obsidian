
##### Definições Iniciais

**Álgebra**: ramo da matemática que estuda a manipulação formal de equações, operações matemáticas, polinômios e estruturas algébricas. 

**Algebra elementar**: Não é boa para lidar com circuitos digitais, umas vez que as variáveis nos circuitos tem valores *binários* e não valores reais.

**Álgebra Booleana**: Variáveis só podem assumir *dois valores diferentes*.

**Três operações básicas**:
- AND 
- OR 
- NOT

>Em nosso mundo digital, essas operações são contruídas com *portas lógicas* que são construídas com *transistores*.


##### Porta OR

 $A \vee B$
 $A$ or $B$
$A +B$

|  A  |  B  |  S  |
| :-: | :-: | :-: |
|  0  |  0  |  0  |
|  0  |  1  |  1  |
|  1  |  0  |  1  |
|  1  |  1  |  1  |
**Entradas**: A e B
**Saída**: S


##### Porta AND

$A \land B$
$A$ and $B$
$A \cdot B$


|  A  |  B  |  S  |
| :-: | :-: | :-: |
|  0  |  0  |  0  |
|  0  |  1  |  0  |
|  1  |  0  |  0  |
|  1  |  1  |  1  |
**Entradas**: A e B 
**Saída**: S

##### Porta NOT 

not $A$
$\neg A$
$\bar{A}$


|  A  |  S  |
| :-: | :-: |
|  0  |  1  |
|  1  |  0  |
**Entrada**: A
**Saída**: S

##### Porta NAND 

$S = \overline{A\cdot B}$


| A   | B   | S   |
| --- | --- | --- |
| 0   | 0   | 1   |
| 0   | 1   | 1   |
| 1   | 0   | 1   |
| 1   | 1   | 0   |
**Entradas**: A e B
**Saída**: S

##### Porta NOR

$S = \overline{A+B}$


| A   | B   | S   |
| --- | --- | --- |
| 0   | 0   | 1   |
| 0   | 1   | 0   |
| 1   | 0   | 0   |
| 1   | 1   | 0   |


**Execício 2.1 Aula**:

![[exercicio2.1.png]]

| $\neg A$ |  B  |  C  | $\neg A\cdot B$ | $B\cdot C$ |  S  |
| :------: | :-: | :-: | :-------------: | :--------: | :-: |
|    1     |  0  |  0  |        0        |     0      |  0  |
|    1     |  0  |  1  |        0        |     0      |  0  |
|    1     |  1  |  0  |        1        |     0      |  1  |
|    1     |  1  |  1  |        1        |     1      |  1  |
|    0     |  0  |  0  |        0        |     0      |  0  |
|    0     |  0  |  1  |        0        |     0      |  0  |
|    0     |  1  |  0  |        0        |     0      |  0  |
|    0     |  1  |  1  |        0        |     1      |  1  |
