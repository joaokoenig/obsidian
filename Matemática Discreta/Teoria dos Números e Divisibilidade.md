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

##### Números Primos
**Definição**:
- um número é dito primo quando é maior do que 1 e seus divisores são 1 e eles mesmo.
- um inteiro é $a>1$ é chamado de composto se a não for primo.

>Existem infinitos números primos.

\- Euclides, O Livro dos Elementos, 1782.
##### Propriedades dos divisores comuns
Teorema:

Sejam $a,b,c$ inteiros, com $a\neq 0$, então:
1. se $a\mid b$ e $a \mid c$ , então $a\mid(b+c)$.
2. se $a\mid b$, então $a \mid b\times c$ para todos os inteiros c.
3. se $a \mid b$ e $b \mid c$, então $a \mid c$.

Teorema:

Sejam $a,b,d,x,y$ números inteiros com $d\neq 0$. Então se $d\mid a$ e $d \mid b$ então
$d \mid (a\times x + b\times y)$.

---

### MDC - Máximo Divisor Comum
**Definição**:
Sejam a e b números inteiros. Dizemos que o inteiro $d$ é o máximo divisor comum de $a$ e $b$ se:
1. $d$ é um divisor comum de $a$ e de $b$.
2. se $e$ também é um divisor comum de $a$ e $b$, então $e \leq d$.
O máximo divisor comum é denotado mdc$(a,b)$. Esse valor é único para $a$ e $b$.

##### Propriedades do MDC
- Se $a$ e $b$ não forem nulos $1\leq mdc(a,b)\leq min(\left|a\right|, \left|b\right|)$
- $mdc(a,b) = mdc(b,a)$
- $mdc(a,b)= mdc(-a,b)$
- $mdc(a,b)= mdc(\left|a\right|,\left|b\right|)$
- $mdc(a,0) = \left|a\right|$
- $mdc(a, ka)= \left|a\right|, \forall k\in\mathbb{Z}$
##### Como calcular o mdc?
Na escola aprendemos a técnica de cálculo de mdc que consiste em:
- Fatorar os números em seus fatores primos
	- $24 = 2^{3}\times_{3}$ e $30 = 2\times{3}\times{5}$
- Identificar os fatores primos em comum e seus menores expoentes
	- os fatores primos comuns são 2 e 3 e os menores expoentes são 1 para 2 e 1 para 3
- Calcular o mdc:
	- $mdc(24,30)= 2^1\times 3^1= 6$

_Essa técnica da escola funciona para números pequenos no qual já conhecemos a fatoração prima. Se esse não for o caso, existem técnicas mais eficientes._

##### Primos entre si
**Definição**:
- dois inteiros $a$ e $b$  são ditos primos entre si quando o se o seu único divisor comum é o 1, ou seja, se o seu $mdc$ é igual a 1.
**Exemplo**:
- os divisores de $8 = (1,2,4,8)$
- os divisores de $15 = (1,3,5,15)$
- o $mdc(8,15)=1$, portanto, 15 e 8 são primos entre si
##### Fatoração única
**Teorema**:
- Para todo primo $p$ e $\forall a,b \in \mathbb{Z}$: se $p\mid ab$, então $p\mid a$ ou $p\mid b$ ou ambos
**Exemplo**:
- 5 é primo, $a = 4$ e $b=10$
- Divisores de $4=(1,2,4)$
- Divisores de $5 = (1,5)$
- Divisores de $10=(1,2,5,10)$
Repare que $5\mid 4\times 10$.
Pelo teorema, sabemos que $5\mid 4$ ou $5 \mid 10$.
Sabemos que nesse caso, $5 \mid 10$.
**Teorema**:
- 