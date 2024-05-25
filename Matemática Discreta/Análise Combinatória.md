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

- Dessa forma, temos que a Permutação de P de tamanho $n$ é igual a:
$$
P_{n} = n!
$$
Exemplo: Seja um conjunto $A = \{ a,b,c \}$, as possíveis permutações desse conjunto são:
$$
abc, acb, bac, bca, cab, cba
$$
Como temos que $n = 3$, podemos conferir que $P_{3}=6$
