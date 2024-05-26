- Técnicas de contagem que são estudas desde o século 17 com foco em jogos de azar.
- Hoje são extremamente importantes para a computação sendo muito utilizado em análise de algoritmos e determinação de recursos para executar um algoritmo.


### Permutações
==Ordem importa!

##### Princípio Fundamental da Contagem:
**Problema**: Quantos bolos diferentes podemos fazer tento 4 opções de massa e 3 opções de recheio?
**Resposta**: $4 \times 3 = 12$

- O Princípio Fundamental da Contagem (Princípio da Multiplicação) é um dos princípios mais básicos da contagem.
**Problema**: Quantas placas diferentes podemos ter se uma placa deve conter uma sequência de 4 letras seguidos por 3 números?
**Resposta**: Total de letras no alfabeto = 26, total de algarismos diferentes = 10 (0...9).

$$
26 \times 26 \times 26 \times 26 \times 10 \times 10 \times 10 = 456,976,000
$$

**Problema**: Quantas strings binárias de diferentes de tamanho 7 podemos formar? 
**Resposta**: $2 \times 2 \times 2 \times 2 \times 2 \times 2 \times 2 = 2⁷ = 128$

**Problema**: De quantas maneiras diferentes podemos ordenar 5 alunos diferentes em uma fila? 
**Resposta**: $5 \times 4 \times 3 \times 2 \times 1 = 5! = 120$
##### Permutações de tamanho n
- Dessa forma, temos que a Permutação de P de tamanho $n$ é igual a:
$$
P_{n} = n!
$$
**Exemplo**: Seja um conjunto $A = \{ a,b,c \}$, as possíveis permutações desse conjunto são:
$$
abc, acb, bac, bca, cab, cba
$$
Como temos que $n = 3$, podemos conferir que $P_{3}= 3! = 6$.
##### Permutações de tamanho r
- Para um inteiro positivo $n$ e um inteiro positivo $r$ com $1\leq r\leq n$, temos que:
$$
_{n}P_{r}= \frac{n!}{(n-r)!}
$$
**Exemplo**: Seja um conjunto $A = \{ a,b,c \}$, as possíveis permutações de tamanho 2 são:
$$
_{3}P_{2}= \frac{3!}{(3-2)!} = \frac{3!}{1!} = 6
$$
Tendo assim os subconjuntos: $ab, ac, ba, bc, ca, cb$.
##### Permutações de tamanho r com repetição de elementos
- Se pudermos repetir os elementos, temos : $n^r$

**Exemplo**:  Seja um conjunto $A= \{ a,b,c \}$, e podendo repetir os elementos, quantas permutações de tamanho 2 podemos fazer? 

$$
n^r = 3^2 = 9
$$
e o resultado dessas permutações será:  aa, ab, ac, ba, bb, bc, ca, cb, cc.

##### Permutações com repetições limitadas
- Vamos analisar um exemplo que torna a visualização desse caso mais claro:
**Exemplo**: Quantas permutações distinguíveis existem com as letras da palavra ==BANANA==?
**Respota**: 
 Se rotularmos as letras que contém repetição, teremos que: 
BANANA = $B A_{1} N_{1} A_{2} N_{2} A_{3}$ = 6 letras = $P_{6}$ = 6! = 720 permutações.

Todavia, algumas dessas permutações são idênticas sem os rótulos das letras, como por exemplo: $A_{1}A_{2}A_{3}N_{1}N_{2}B$ é idêntico a $A_{2}A_{1}A_{3}N_{2}N_{1}B$.

Como $N_{1}N_{2}$ e $N_{2}N_{1}$ geram palavras indistinguíveis, tirando os rótulos, temos que $\frac{720}{2} = 360$  palavras distinguíveis.

De modo similar, essas 360 permutações podem ser agrupadas em grupos de 3!, já que o A se repete em 3! ($A_{1}A_{2}A_{3}$).

$\frac{360}{6} = 60$, sendo assim, 60 é o número de permutações distinguíveis que podemos fazer com a palavra BANANA.

Podemos concluir então que o número de permutações distintas que podem ser formadas com uma coleção $n$ de objetos em que:

- o primeiro objeto aparace $K_{1}$ vezes.
- o segundo objeto aparece $K_{2}$ vezes.
- ... 
é dado por $$
\frac{n!}{k_{1}!k_{2}!\dots k_{t}}
$$
onde $k_{1}+ k_{2} + k_{3}\dots k_{t}=n$.

### Combinações 
==Ordem não importa!

**Exemplo**: Quantos grupos de 3 alunos podem ser formados a partir de um grupo de 4 alunos? 

_note que a ordem dos alunos no grupo não importa. Queremos saber quantos subconjuntos de 3 elementos podemos formar a partir de um conjunto de 4 elementos._

**Resposta**: $G = \{ a,b,c,d \}$ 
$S_{1}= \{ a,b,c \}$
$S_{2} = \{ a,b,d \}$
$S_{3}= \{ a, d,c\}$
$S_{4} = \{ b,c,d \}$

- Uma **r-combinação** de elementos de um conjunto S é uma seleção não ordenada de r elementos a partir de S. 
- Uma combinação de S tomado r a r. 
- Ou seja, um subconjunto de S com r elementos.
**Exemplo**: Seja $S = \{ a,b,c,d\}$, uma  3-combinação de S seria = $\{ a,b,c\}$.

- O número de **r-combinações** de um conjunto de n elementos distintos é representado por C(n,r) ou  $_{n}C_{r}$  ou  $\binom{n}{r}$ (coeficiente binomial).
##### **Teorema**:
- O número de r-combinações de um conjunto com n elementos distintos, em que $n$ é um número inteirio não negativo e $r$ é um número inteiro em que $0\leq r\leq n$, é:
$$
C(n,r) = \frac{n!}{r!(n-r)!}
$$
