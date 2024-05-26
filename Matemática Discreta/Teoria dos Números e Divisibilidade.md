- A teoria dos números é um ramo da matemática que estuda as propriedades dos números.
	- Em particular, estamos interessados nos números inteiros.
- A teoria dos números é a base para entendermos o funcionamento da criptografia que conhecemos hoje.
### Noções Elementares
- Divisibilidade, divisores comuns, números primos e fatoração.

##### Divisibilidade
**Definição**: 
- Se $a \text{ e } b$ são números inteiros e com $a \neq 0$, dizemos que $a \text{ divide }b$ (a | b) se existe um número inteiro $c$ tal que $b = ac$.
- Quando $a \text{ divide }b$ dizemos que a é um divisor de b.
- A notação $a \mid b$ indica que a é um divisor de b.
- A notação $a \nmid b$ indica que a não é um divisor de b.
**Exemplos**:

$\frac{12}{3}$? 

**Resposta**: Sim, pois existe um número inteiro c tal que $3 \times c = 12$, e $c = 4$.

$\frac{11}{3}$?

**Resposta**: Não, pois não existe um número inteiro c tal que $3 \times c = 11$.

_E se a divisão de a/b não resultar em número inteiro?_

##### Teorema da divisão
Sejam $a,n \in \mathbb{Z}$:
$$
a = q \times n + r
$$
em que $0\leq r<n$.

- Existe um único par de inteiros que satisfaz essa condição.
- O inteiro q é chamado de _quociente_ e o inteiro r é _resto_.
- $q = a \text{ div } n$
- $r = a\text{ mod }n$
- $n|a$ se e somente se $a \text{ mod } n = 0$

> Todo inteiro b tem divisores triviais 1 e b.
> Divisores diferentes de 1 e b são chamados de fatores (ou divisores não triviais).

**Exemplo**: os divisores de 24 = $\{ 1,2,3,4,6,8,12,24 \}$.

> Divisores Triviais: 1 e 24.
> Divisores Não triviais(fatores): 2, 3, 4, 6, 8, 12.

