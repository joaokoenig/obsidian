##### Definição: 
- Estudo do relacionamento de elementos de um mesmo conjunto. 
- Um subconjunto do produto cartesiano.

Um par ordenado $(a,b)$ é uma lista de objetos $a$ e $b$ em uma ordem estabelecida, sendo $a$ o primeiro e $b$ o segundo.

### Produto Cartesiano:
##### Definição:
- Se A e B são dois conjuntos não vazios, define-se o produto cartesiano $A\times B= \{ (a,b)| a \in A \text{ e }b \in B \}$
**Exemplo**: $A = \{ 1,2,3 \}$ e $B = \{ r,s \}$.

$A \times B = \{ (1,r), (1,s), (2,r), (2,s), (3,r), (3,s) \}$

_Sejam A e B conjuntos. Uma relação binária de A em B é um subconjunto de 
A x B._

- Uma relação binária de A em B é um conjunto R de pares onde o primeiro elemento vem de A e o segundo vem de B.
- Quando $(a,b) \in R$, diz-se que $a$ está relacionado com $b$ por R.
- Usamos a notação $aRb$ para denotar que $(a,b) \in R$.
- Usamos a notação $a\not Rb$ para denotar que $(a,b) \not\in R$.
- Também existem relações n-árias.

**Exemplo 1**: 

Considere o conjunto A com seus elementos sendo os alunos da UFSC e o conjunto B com seus elementos sendo os cursos ofertados pela universidade. Considere a relação R a relação com pares $(a,b)$, onde $a$ é um aluno matriculado e $b$ é um curso.

_Exemplos de pares em R:_

(Matheus, Engenharia Mecânica)
(Renata, Medicina)
(Alexandre, Ciências da Computação)
(José, Farmácia)

**Exemplo 2**:

Considere o conjunto A de todas as cidades do Brasil e o conjunto B sendo os 3 estados da região sul do país. $(a,b) \in R$ se a for uma cidade que está dentro de um dos 3 estados da região sul.

_Exemplos de pares em R:_
(Florianópolis, SC)
(Campo Mourão, Paraná)
(Canoas, Rio Grande do Sul)

**Exemplo 3**:
Seja $A=B=\{ 1,2,3,4,5 \}$. Define-se a relação R (menor do que) sobre A como:

$(a,b) \in R$ ou $aRb$ se $a<b$.

Nesse caso, temos que $R=\{ (1,2),(1,3),(1,4),(1,5),(2,3),(2,4),(2,5),(3,4),(3,5),(4,5) \}$.

Como $A=B$, podemos dizer que essa é uma relação de A em A.

**Exemplo 4**: 

Seja A o conjunto $\{ 1,2,3,4 \}$. Quais pares ordenados estão na relação $R = \{ (a,b) | a | b\}$? _lê-se "tal que a divide b"._

$R = \{ (1,1), (1,2), (1,3),(1,4),(2,2),(2,4),(3,3),(4,4) \}$.

##### Quantas relações podem ser construídas dentro de um conjunto de tamanho n? 

$2^{n^2}$

### Conjuntos Originados de Relações

Seja $R \subseteq A \times B$ uma relação de A em B. Definimos:

**Domínio**: Dom(R), o conjunto de elementos de A que estão relacionados com algum elemento em B.

**Contradomínio**: Ran(R), o conjunto de elementos de B que estão relacionados com algum elemento em A. 

**Exemplo**: 

Considere a relação R sobre $A = \{ 1,2,3,4,5 \}$ dada por $aRb$ se e somente se 
$a<b$. Descreva R, Dom(R) e Ran(R):

$R = \{ (1,2),(1,3),(1,4),(1,5),(2,3),(2,4),(2,5),(3,4),(3,5),(4,5) \}$.

$Dom(R)= \{1,2,3,4\}$.

$Ran(R)= \{2,3,4,5  \}$.

##### Definição: 
Seja $R \subseteq A \times B$ uma relação de A em B. O conjunto dos **R-relativos** de x é o conjunto de todos os elementos $y \in B$ que se relacionam com x em R. Chamamos esse conjunto de $R(x)$.

Ou seja, $R(x) = \{ y \in B | xRy \}$.

**Exemplo**: 

Seja $A=B=\{ a,b,c,d \}$ e seja $R= \{ (a,a),(a,b),(b,c),(c,a),(d,c),(c,b) \}$.

$R(a)=\{ a,b \}$.

$R(b) = \{ c \}$.

$R(c)= \{ a,b \}$.

$R(d)= \{ c \}$.

##### Definição:
Seja $R \subseteq A \times B$ uma relação de A em B e seja, $A_{1} \subseteq A$. O conjunto de **R-relativos de** $A_{1}$ é o conjunto de todos os elementos $y \in B$ que se relacionam em R com os elementos $x \in A_{1}$. Chamamos esse conjunto de $R(A_{1})$.

Ou seja, $R(A_{1})=\{ y \in B | xRy \text{ para algum }x \in A_{1} \}$.

obs: $R(A_{1})$ é a união dos conjuntos de $R(x)$ em que $x \in A_{1}$.

**Exemplo**:

Seja $A=B=\{ a,b,c,d \}$ e seja $R = \{ (a,a),(a,b),(b,c),(c,a), (d,c), (c,b) \}$.

Considere $A_{1}= \{ c,d \}$.

$R(c)=\{ a,b \}$

$R(d)= \{ c \}$.

$R(A_{1})=\{ a,b,c \}=R(c)\cup R(d)$.

##### Operações 

_Teorema:_ Seja $R$ uma relação sobre $A$ e seja $A_{1}$  e $A_{2}$ subconjuntos de $A$. Então:

1. Se $A_{1}\subseteq A_{2}$, então $R(A_{1})\subseteq R(A_{2})$.
2. $R(A_{1}\cup A_{2})=R(A_{1})\cup R(A_{2})$.
3. $R(A_{1} \cap A_{2})\subseteq R(A_{1} \cap R(A_{2}))$.

**Exemplo**: 

Seja $A = \{ 1,2,3 \}$, $B = \{ x,y,z,w,p,q \}$, $A_{1}=\{ 1,2 \}$, $A_{2}=\{ 2,3 \}$ e considere $R=\{ (1,x),(1,z),(2,w),(2,p),(2,q),(3,y) \}$.

$R(A_{1})=\{ x,z,w,p,q \}$.

$R(A_{2})= \{w, p,q,y \}$.

$R(2)= \{ w,p \}$.

$R(A_{1})\cup R(A_{2}))=B$.

$R(A_{1})\cap R(A_{2})=\{w, p,q \}$.

##### Representação com matrizes

**Exemplo**: 

Seja $A = \{ 1,2,3 \}$ e $B = \{ 1,2 \}$. Considere a relação de A em B com pares ordenados $(a,b)$, tal que $a \in A$, $b \in B$, e $a > b$.

$R = \{ (2,1), (3,1), (3,2) \}$.

Também podemos representar $R$ com a matriz:

$$M_{R} = 
\begin{bmatrix}
0&0 \\
1&0 \\
1&1
\end{bmatrix}
$$

**Exercício**:

Defina qual a relação da seguinte matriz:

$$ M =
\begin{bmatrix}
1 & 0 & 0 & 1 \\
0 & 1 & 1 & 0 \\
1 & 0 & 1 & 0
\end{bmatrix}
$$
Podemos definir essa relação $R$ como sendo: 

$R = \{ (a_{1},b_{1}),(a_{1},b_{4}),(a_{2},b_{2}),(a_{2},b_{3}),(a_{3},b_{1}),(a_{3},b_{3}) \}$

##### Operações com matrizes

- Considere $R_{1}$ e $R_{2}$ relações sobre o conjunto A representadas por matrizes $M_{R_{1}}$ e $M_{R_{2}}$.
- Operações de união e intersecção entre $R_{1}$ e $R_{2}$ podem ser representadas por operações booleanas nas matrizes correspondentes.
- $M_{R_{1}\cup R_{2}}= M_{R_{1}} \cup M_{R_{2}}$.
- $M_{R_{1}\cap R_{2}}= M_{R_{1}}\cap M_{R_{2}}$.

_As matrizes precisam ter a mesma ordem para realizar essas operações!_

**Exemplo**: 

Suponha que as relações $R_{1}$ e $R_{2}$ sobre um conjunto A sejam representadas pelas matrizes abaixo. Que matrizes representam $R_{1} \cup R_{2}$ e $R_{1}\cap R_{2}$?

$$
M_{R_{1}}= \begin{bmatrix}
1 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0
\end{bmatrix}
$$
$$
M_{R_{2}}= \begin{bmatrix}
1 & 0 & 1 \\
0 & 1 & 1 \\
1 & 0 & 0
\end{bmatrix}
$$
$$
M_{R_{1}\cup R_{2}}=
\begin{bmatrix}
1 & 0 & 1 \\
1 & 1 & 1 \\
1 & 1 & 0
\end{bmatrix}
$$
$$
M_{R_{1}\cap R_{2}}=\begin{bmatrix}
1 & 0 & 1 \\
0 & 0 & 0 \\
0 & 0 & 0
\end{bmatrix}
$$




