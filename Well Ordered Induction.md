Todo conjunto de números naturais contém um menor elemento:
$$\begin{equation*}
\begin{matrix}
S\subseteq \mathbb{N} & \exists ( m\in S) :\forall ( n\in S) :\left( n\neq m\rightarrow m< n\right)\\
S\neq \emptyset  & 
\end{matrix}
\end{equation*}$$
Provar que:

$$\begin{equation*}
\begin{array}{ l }
P( 1)\\
P( n)\rightarrow P( n+1) ,\forall n\geq 1\\
\hline
\therefore P( n) ,\forall n\geq 1
\end{array}
\end{equation*}$$

$$\begin{equation*}
\left( P( 1) \land \left( P( n)\rightarrow P( n+1) ,\ \forall n\geq 1\right)\right)\rightarrow ( P( n) ,\ \forall n\geq 1)
\end{equation*}$$

$$\begin{aligned}
\neg \left(\left( P( 1) \land \left( P( n)\rightarrow P( n+1) ,\ \forall n\geq 1\right)\right)\rightarrow ( P( n) ,\ \forall n\geq 1)\right)\\
\neg ( P( n) ,\ \forall n\geq 1)\\
P( 1)\\
\left( P( n)\rightarrow P( n+1) ,\ \forall n\geq 1\right)
\end{aligned}$$


Assuma para contradição que $\displaystyle \exists ( n\geq 1) :\neg P( n)$ e construa $\displaystyle S:=\{n|\neg P( n) ,\ n\geq 1\}$

Pelo axioma da boa ordenação, $\displaystyle \exists ( k\in S) :\ \forall ( n\in S) :\left( n\neq m\rightarrow m< n\right)$, ou seja, $\displaystyle k$ é o menor elemento de $\displaystyle S$, i.e. $\displaystyle k=\min S$. Como $\displaystyle P( 1)$, $\displaystyle 1\notin S$, então $\displaystyle k=\min S >1$

Se $\displaystyle P( k-1)$ fosse falso, $\displaystyle k-1\in S$ e $\displaystyle k-1\ < k=\min S$, o que seria absurdo, portanto $\displaystyle k-1\notin S$

De outra forma,
$$\begin{equation*}
k-1\ < k=\min S\Longrightarrow k-1\notin S\Longrightarrow P( k-1)
\end{equation*}$$
Usando o passo para $\displaystyle n=k-1$, temos $\displaystyle P( k-1)\rightarrow P( k)$

Pela construção de $\displaystyle S$, $\displaystyle P( k) \Longrightarrow k\notin S$, o que contradiz $\displaystyle k=\min S$


Para demonstrar a equivalência entre o princípio da boa ordenação, o princípio da indução fraca e o princípio da indução forte, precisamos mostrar que cada um deles implica nos outros dois. Vamos usar as seguintes notações:



- PBO: Princípio da boa ordenação, que afirma que todo subconjunto não vazio de números naturais possui um elemento mínimo.

- PIF: Princípio da indução forte, que afirma que se uma propriedade P(n) vale para n = 0 e se para todo n natural, P(k) vale para todo k ≤ n implica que P(n+1) vale, então P(n) vale para todo n natural.

- PIM: Princípio da indução fraca ou simples, que afirma que se uma propriedade P(n) vale para n = 0 e se para todo n natural, P(n) implica que P(n+1) vale, então P(n) vale para todo n natural.



Vamos mostrar as seguintes implicações:



- PBO ⇒ PIF

- PIF ⇒ PIM

- PIM ⇒ PBO



 

Suponha que:

	PBO seja verdadeiro;

	P(0) seja verdadeiro;

	Para todo n natural, 

		P(k) seja verdadeiro para todo k ≤ n implique que P(n+1) seja verdadeiro. 

Queremos mostrar que P(n) é verdadeiro para todo n natural. 

Para isso, vamos usar um argumento por contradição. 

Suponha que exista algum n natural tal que P(n) seja falso. 

Então, o conjunto $\displaystyle S\ =\ \{n\ \in \mathbb{N} \ |\ \neg P( n)\}$ é não vazio. 

Mas pelo PBO, $\displaystyle S$ tem um elemento mínimo, digamos $\displaystyle m$. 

Então P(m) é falso e m > 0, pois P(0) é verdadeiro por hipótese. 

Mas se m > 0, então existe um k natural tal que m = k + 1. Logo, ¬P(k+1) é verdadeiro e k ∈ A. 

Mas isso contradiz o fato de que m é o mínimo de A, pois k < m.

Portanto, não existe nenhum n natural tal que ¬P(n) seja verdadeiro, ou seja, P(n) é verdadeiro para todo n natural.



PIF ⇒ PIM: Suponha que PIF seja verdadeiro e que P(0) seja verdadeiro e que para todo n natural, P(n) implique que P(n+1) seja verdadeiro. Queremos mostrar que P(n) é verdadeiro para todo n natural. Para isso, vamos usar o próprio PIF. Seja Q(n) a propriedade "P(k) é verdadeiro para todo k ≤ n". Então Q(0) é verdadeiro, pois P(0) é verdadeiro por hipótese. Além disso, se Q(n) é verdadeiro para algum n natural, então Q(n+1) também é verdadeiro, pois Q(n) implica que P(n) é verdadeiro e P(n) implica que P(n+1) é verdadeiro por hipótese. Logo, pelo PIF, Q(n) é verdadeiro para todo n natural. Mas Q(n) implica que P(n) é verdadeiro para todo n natural. Portanto, P(n) é verdadeiro para todo n natural.



PIM ⇒ PBO: Suponha que PIM seja verdadeiro e que A seja um subconjunto não vazio de números naturais. Queremos mostrar que A tem um elemento mínimo. Para isso, vamos usar um argumento por contradição. Suponha que A não tenha um elemento mínimo. Então, para todo n natural, existe um k ∈ A tal que k < n. Seja B = \{n ∈ N | ∃k ∈ A (k < n)\}. Então B = N, pois para todo n natural existe um k ∈ A tal que k < n por hipótese. Seja C = \{n ∈ N | ∀k ∈ A (k ≥ n)\}. Então C = ∅, pois se existisse algum n ∈ C, então n seria o mínimo de A, o que contradiz a hipótese de que A não tem mínimo. Seja D = \{n ∈ N | n ∉ B\}. Então D = C, pois n ∈ B se e somente se n ∉ C. Seja P(n) a propriedade "n ∈ D". Então P(0) é falso, pois 0 ∈ B, já que A é não vazio. Além disso, se P(n) é falso para algum n natural, então P(n+1) também é falso, pois se n+1 ∈ D, então n+1 ∉ B, o que implica que não existe k ∈ A tal que k < n+1, o que implica que n+1 é o mínimo de A, o que contradiz a hipótese de que A não tem mínimo. Logo, pelo PIM, P(n) é falso para todo n natural. Mas isso implica que D = ∅, ou seja, C = ∅, o que contradiz o fato de que C = N \textbackslash \ B. Portanto, A tem que ter um elemento mínimo.



Assim, mostramos que PBO, PIF e PIM são equivalentes.