##### Operação mod
**Definição**: 
- Para $a$ inteiro e $n$ inteiro positivo, $a \text{ mod }n$ é o resto da divisão de $a$ por $n$.
- Ou seja, $a \text{ mod } n$ é o inteiro $r$ em que $a=qn+r$, em que $0\leq r<n$.
**Exemplo**:
$17 \text{ mod }5=2$
$-133 \text{ mod }9 =2$
$2001 \text{ mod }101=82$

##### Congruência
- O inteiro $a$ é congruente a $b \text{ mod }n$ se $a \text{ mod }n = b \text{ mod }n$.
- notação $a\equiv b\text{ mod }n$.
**Exemplo**:
$24\equiv 9 \text{ mod }5$
$17 \equiv 5 \text{ mod }6$
$-11 \equiv 17 \text{ mod }7$
- Se $a$ e $b$ são inteiros e $n$ é um inteiro positivo, então $a$ é congruente a $b \text{ mod }n$ se e somente se  $n|(a-b)$.
**Exemplo**:
$24\equiv 9 \text{ mod } 5$ pois $24-9=5\times 3$.
$17 \equiv 5 \text{ mod }6$ pois $17-5=6\times 2$.
##### Operações Aritméticas Modulares
- Podemos definir operações aritméticas de adição e multiplicação.
- Elas funcionam exatamente como nos inteiros, a única diferença é que o resultado é reduzido módulo $n$.
**Exemplo**:
$11+13$ em $\mathbb{Z}_{16}$.
$11+13=24$, depois reduzimos $24 \text{ mod }16$, onde iremos obter $24\text{ mod }16 = 8$.
Portando, $11+13$ em $\mathbb{Z}_{16}$ é igual a $8$.

##### Propriedades da Aritmética Modular
- $(a+b) \text{ mod }n=[(a\text{ mod }n)+(b\text{ mod }n)]\text{ mod }n$
- $(a-b) \text{ mod }n=[(a\text{ mod }n)-b\text{ mod }n)]\text{ mod }n$
- $(a\times b) \text{ mod }n=[(a\text{ mod }n)\times b\text{ mod }n)]\text{ mod }n$
##### Inversa Aditiva
**Definição**:
Seja $a \in\mathbb{Z}_{n}$. A inversa aditiva de $a$ módulo $n$ é um número inteiro $b \in \mathbb{Z}_{n}$ tal que $a+b\equiv 0\text{ mod }n$.
**Exemplo**:
- a inversa aditiva de $3$ em $\mathbb{Z}_{7}$ é igual a $4$.
- a inversa aditiva de $3$ em $\mathbb{Z}_{10}$ é igual a 7.
- a inversa aditiva de $2$ em $\mathbb{Z}_{3}$ é igual a 1.
##### Inversa Multiplicativa
