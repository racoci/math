  

# $\textcolor[rgb]{0.82,0.01,0.11}{\textbf{ME 323 D}}$

 
 $\textcolor{yellow}{ime.unicamp.br/\textasciitilde marinav/me323.html}$

   marinav@ime.unicamp.br

  
  
  

${\large \textcolor[rgb]{0.09,0.49,0.47}{\textbf{Probabilidade}}}$

  

Experimento aleatório: $\textcolor[rgb]{0.96,0.65,0.14}{\Omega} =\{\text{resultados} ,\ ...\}$

  
Ex: $\textcolor{lightgreen}{\underline{Moeda}}$$$\textcolor{lightgreen}{ }\textcolor{lightgreen}{\textcolor[rgb]{0.96,0.65,0.14}{\Omega } =\textcolor[rgb]{0.96,0.65,0.14}{\{}\text{Cara}\textcolor[rgb]{0.96,0.65,0.14}{,}\text{Coroa}\textcolor[rgb]{0.96,0.65,0.14}{\}}}$$

Se a moeda é honesta:

  

$$\textcolor[rgb]{0.96,0.65,0.14}{P\left(\text{Cara}\right)} = \textcolor[rgb]{0.96,0.65,0.14}{P\left(\text{Coroa}\right)} = \textcolor{yellow}{\cfrac{1}{2}}
$$


  
  
  

### $\textcolor[rgb]{0.09,0.49,0.47}{{\underline{\text{Princípio Básico de Contagem para 2 experimentos}}}}$

  

Primeiro experimento: $\displaystyle \textcolor{cyan}{n}\textcolor{cyan}{_{1}}$ resultados $\displaystyle P_{\textcolor{cyan}{1}} ,\ ...,\ P\textcolor{cyan}{_{n_{1}}}$ 
Segundo experimento: $\displaystyle \textcolor{lightgreen}{n}\textcolor{lightgreen}{_{2}}$ resultados  $\displaystyle S\textcolor{lightgreen}{_{1}} ,\ ...,\ S\textcolor{lightgreen}{_{n_{2}}}$
$\displaystyle \therefore$ O par $\displaystyle C\ =\left(\text{Primeiro} ,\text{Segundo}\right)$ tem os $\displaystyle \textcolor{cyan}{n}\textcolor{cyan}{_{1}} \cdotp \textcolor{lightgreen}{n}\textcolor{lightgreen}{_{2}}$ resultados: 
$$\displaystyle \textcolor{cyan}{n}\textcolor{cyan}{_{1}} \ \text{linhas}\overbrace{\begin{cases}

\begin{matrix}

( P_{\textcolor{cyan}{1}} ,S_{\textcolor{lightgreen}{1}}) & \cdots  & ( P_{1} ,S_{\textcolor{lightgreen}{n}\textcolor{lightgreen}{_{2}}})\\

\vdots  & \ddots  & \\

( P_{\textcolor{cyan}{n}\textcolor{cyan}{_{1}}} ,S_{\textcolor{lightgreen}{1}}) & \cdots  & ( P\textcolor{cyan}{_{\textcolor{cyan}{n}\textcolor{cyan}{_{1}}}} ,S_{\textcolor{lightgreen}{n}\textcolor{lightgreen}{_{2}}})

\end{matrix}

\end{cases}}^{\textcolor{lightgreen}{n}\textcolor{lightgreen}{_{2}}\textcolor{lightgreen}{\ }\text{colunas}}$$

  
  
  

O princípio básico da contagem é basicamente a cardinalidade do produto cartesiano $\displaystyle C=A\times B$, onde $\displaystyle A$ é o conjunto de resultados do primeiro experimento e $\displaystyle B$ é o conjunto de resusltados do segundo experimento.

  
  
  

## Princípio Básico de Contagem para n experimentos

  
Suponha que tenhamos uma lista de experimentos $\displaystyle E=[ e_{1} ,\cdots e_{m}]$

  

Seja $\displaystyle R$ o conjunto de todos os possíveis resultados. O conjunto de todos os possíveis resultados para um experimento específico pode ser pensado como uma função $\displaystyle r:E\rightarrow R$. 

Assim é possível definir o conjunto de todas as funções desse tipo $\displaystyle R^{E} := \left\{r:E\rightarrow R\right\}$. Queremos saber a cardinalidade de $\displaystyle R^{E}$. Cada $\displaystyle e_{k} \in E$ tem uma imagem $\displaystyle r( e_{k}) \subseteq R$. Seja $\displaystyle n_{k}$ a cardinalidade de $\displaystyle r( e_{k})$.

Vamos provar que $\displaystyle R^{E} =r( e_{1}) \times \cdots \times r( e_{m})$ e que portanto $\displaystyle \#\left( R^{E}\right) =\prod _{k=1}^{m} n_{k}$

Prova por indução.
#### Base

Se $\displaystyle m=1$, $\displaystyle E=[ e_{1}]$.
Assim $\displaystyle R=R^{E} =r( e_{1})$ portanto $\displaystyle \#\left( R^{E}\right) =\#( R) =\#( r( e_{1})) =n_{1} =\prod _{k=1}^{1} n_{k}$
Se $\displaystyle m=2$, $\displaystyle E=[ e_{1} ,e_{2}]$. Pelo princípio básico da contagem para 2 experimentos, $\displaystyle R^{E} =r( e_{1}) \times r( e_{2})$, assim $\displaystyle \#\left( R^{E}\right) =n_{1} \cdot n_{2}$

  

#### Passo

Suponha que tenhamos provado que:

$$R^{[ e_{1} ,\cdots ,e_{m-1}]} =r( e_{1}) \times \cdots \times r( e_{m-1})$$
e que portanto:
$$
\#\left( R^{[ e_{1} ,\cdots ,e_{m-1}]}\right) =\prod _{k=1}^{m-1} n_{k}{}
$$

Aplicando o princípio básico da contagem, considerando $\displaystyle A=R^{[ e_{1} ,\cdots ,e_{m-1}]}$ e $\displaystyle B=r( e_{m})$, teremos
$$

R^{E} =R^{[ e_{1} ,\cdots ,e_{m-1}]} \times r( e_{m}) =r( e_{1}) \times \cdots \times r( e_{m-1}) \times r( e_{m})

$$

Portanto, em termos de cardinalidade:
$$
\#\left( R^{E}\right) =\#\left( R^{[ e_{1} ,\cdots ,e_{m-1}]} \times r( e_{m})\right) =\#\left( R^{[ e_{1} ,\cdots ,e_{m-1}]}\right) \cdot \#( e_{m}) =\left(\prod _{k=1}^{m-1} n_{k}\right) \cdot n_{m} =\prod _{k=1}^{m} n_{k}
$$
Exemplo: Considere 4 experimentos:
$\displaystyle E_{1} :=$É o jogar de uma moeda
$\displaystyle E_{2} :=$É o jogar de um dado tetraédrico $\displaystyle D_{4}$
$\displaystyle E_{3} :=$É o jogar de um dado comum $\displaystyle D_{6}$
$\displaystyle E_{4} :=$É o jogar de um dado octaédrigo $\displaystyle D_{8}$
O primeiro experimento $\displaystyle E_{1}$ tem os resultados $\displaystyle R_{1,1} :=\text{Cara}$ e $\displaystyle R_{1,2} :=\text{Coroa}$, portanto $\displaystyle n_{1} =2$
O segundo experimento $\displaystyle E_{2}$ tem os resultados $\displaystyle 1,2,3,4$, portanto $\displaystyle n_{2} =4$
O terceiro experimento $\displaystyle E_{3}$ tem os resultados $\displaystyle 1,2,3,4,5,6$ portanto $\displaystyle n_{3} =6$
O quarto experimento $\displaystyle E_{4}$ tem os resultados $\displaystyle 1,2,3,4,5,6,7,8$ portanto $\displaystyle n_{4} =8$
Assim, o número de resultados combinados dos 4 experimentos é $\displaystyle 2\cdot 4\cdot 6\cdot 8$

## Permutações
$\displaystyle n$ objetos distintos, número de possibilidades de ordenar estes objetos:

  

### $\textcolor{yellow}{\text{Primeiro objeto}}$
Qualquer posição, $\displaystyle n$ possibilidades
### $\textcolor{yellow}{\text{Segundo Objeto}}$
Qualquer posição, menos a posição do primeiro. $\displaystyle n-1$ possibilidades
### $\textcolor{yellow}{\text{Último Objeto}}$ 
Só sobra uma posição.

  
Número total de permutações $n! =n\cdot \left( n-1\right)! =n\cdot \left( n-1\right) \cdots 2\cdot 1$

  

Outra forma é:

  

O número de permutações de $\displaystyle n$ elementos pode ser escrito como uma função de $\displaystyle n$. Digamos $\displaystyle f\left( n\right)$

  

O número de permutações de 1 único elemento é 1, porque só há uma permutação de 1 único elemento.

  

Assim, seja $\displaystyle f:\left\{1,\cdots \right\}\rightarrow \left\{1,\cdots \right\}$ a função que dê o número de permutações de $\displaystyle n$ elementos. Sabemos que $\displaystyle f\left( 1\right) =1$

  

Considere o problema geral como uma escolha da posição do primeiro elemento em conjunto com uma permutação das posições dos outros $\displaystyle n-1$ elementos. Assim, pelo princípio básico da contagem $\displaystyle f\left( n\right) =n\cdot f\left( n-1\right)$.

  

Sabemos que $\displaystyle f\left( n\right) =n!$ é a única função que respeita ambas as condições $\displaystyle f\left( n\right)$  

## $\textcolor[rgb]{0.09,0.49,0.47}{{\underline{Arranjos}}}$

  
Exemplo quantas formas há de ordenar $\displaystyle n$ objetos em $\displaystyle m$ posições, $\displaystyle 0< m< n$

Podemos pensar que há $\displaystyle n!$ formas de ordenar $\displaystyle n$ objetos em $\displaystyle n$ posições. Então podemos considerar que as $\displaystyle n-m$ últimas posições foram excluídas e devem ser desconsideradas da conta inicial. Então há $\displaystyle \cfrac{n!}{\left( n-m\right) !} =\cfrac{n\ \left( n-1\right)\left( n-2\right) \cdots \left( n-m+1\right)\cancel{\left( n-m\right) !}}{\cancel{\left( n-m\right)!}}$ formas de ordenar $\displaystyle n$ elementos em $\displaystyle m$ posições.


$$\displaystyle \binom{n}{m} =\cfrac{n!}{m!\ \left( n-m\right) !}$$

  
  
  

## $\textcolor[rgb]{0.09,0.49,0.47}{\underline{Coeficientes Binomiais}}$

  

Quais são os coeficientes da expansão $\displaystyle \left( x+y\right)^{n}$, $\displaystyle x,y\in {C}$, $\displaystyle n\in {N}$

Vamos um a um para ver se entendemos o padrão

### $n=0$
$$\displaystyle ( x+y)^{0} =1=x^{0} y^{0}$$
### $n=1$
$$\displaystyle ( x+y)^{1} =x+y=x^{0} y^{1} +x^{1} y^{0}$$
### $n=2$
$$\displaystyle \begin{aligned}
( x+y)^{2} & =( x+y)^{1}( x+y)\\
 & =\left( x^{0} y^{1} +x^{1} y^{0}\right)( y+x)\\
 & \begin{matrix}
= & ( x^{0} y^{1} & +\  & x^{1} y^{0} & ) &  & \cdot y\\
 &  & +( & x^{0} y^{1} & + & x^{1} y^{0}) & \cdot x
\end{matrix}\\
 & \begin{aligned}
= & x^{0} y^{2} & +x^{1} y^{1} & \\
 &  & +x^{1} y^{1} & +x^{2} y^{0}
\end{aligned}\\
 & =x^{0} y^{2} +2x^{1} y^{1} +x^{2} y^{0}\\
 & =y^{2} +2xy+x^{2}
\end{aligned}$$
### $n=3$

$$\displaystyle \begin{aligned}
( x+y)^{3} & =( x+y)^{2}( x+y)\\
 & =\left( x^{0} y^{2} +2x^{1} y^{1} +x^{2} y^{0}\right)( y+x)\\
 & \begin{matrix}
= & ( x^{0} y^{2} & + & 2x^{1} y^{1} & + & x^{2} y^{0}) &  &  & \cdot y\\
 &  &  & ( x^{0} y^{2} & + & 2x^{1} y^{1} & + & x^{2} y^{0}) & \cdot x
\end{matrix}\\
 & \begin{matrix}
= & x^{0} y^{3} & + & 2x^{1} y^{2} & + & 1x^{2} y^{1} &  & \\
 &  &  & 1x^{1} y^{2} & + & 2x^{2} y^{1} & + & x^{3} y^{0}
\end{matrix}\\
 & \begin{matrix}
= & x^{0} y^{3} & + & 3x^{1} y^{2} & + & 3x^{2} y^{1} & + & x^{3} y^{0}
\end{matrix}\\
 & =y^{3} +3xy^{2} +3x^{2} y+x^{3}\\
 & =y^{3} +x^{3} +3xy( x+y)
\end{aligned}$$
### $n=4$

$$\displaystyle \begin{aligned}
( x+y)^{4} & =( x+y)^{3}( x+y)\\
 & =\left( x^{0} y^{3} +3x^{1} y^{2} +3x^{2} y^{1} +x^{3} y^{0}\right)( y+x)\\
 & \begin{matrix}
= & ( x^{0} y^{3} & + & 3x^{1} y^{2} & + & 3x^{2} y^{1} & + & x^{3} y^{0}) &  &  & \cdot y\\
 &  & + & ( x^{0} y^{3} & + & 3x^{1} y^{2} & + & 3x^{2} y^{1} & + & x^{3} y^{0}) & \cdot x
\end{matrix}\\
 & \begin{matrix}
= & x^{0} y^{4} & + & 3x^{1} y^{3} & + & 3x^{2} y^{2} & + & x^{3} y^{1} &  & \\
 &  & + & x^{1} y^{3} & + & 3x^{2} y^{2} & + & 3x^{3} y^{1} & + & x^{4} y^{0}
\end{matrix}\\
 & \begin{matrix}
= & x^{0} y^{4} & + & 4x^{1} y^{3} & + & 6x^{2} y^{2} & + & 4x^{3} y^{1} & + & x^{4} y^{0}
\end{matrix}\\
 & =y^{4} +4xy^{3} +6x^{2} y^{2} +4x^{3} y+x^{4}\\
 & =y^{4} +x^{4} +4xy\left( y^{2} +x^{2}\right) +6x^{2} y^{2}
\end{aligned}$$
### For a Generic $n$
$$\displaystyle \begin{aligned}
( x+y)^{n+1} & =( x+y)^{n}( x+y)\\
 & =\left( c_{n,0} \ x^{0} y^{n} +c_{n,1} \ x^{1} y^{n-1} +\cdots +c_{n,k} \ x^{k} y^{n-k} +\cdots +c_{n,n} \ x^{n} y^{0}\right)( x+y)\\
 & \begin{array}{ c c r c c c c c r c c c c c c }
= & ( & c_{n,0} \ x^{0} y^{n} & + & c_{n,1} \ x^{1} y^{n-1} & + & \cdots  & + & c_{n,k} \ x^{k} y^{n-k} & \cdots  & + & c_{n,n} \ x^{n} y^{0} & ) &  & \cdot y\\
 &  & + & ( & c_{n,0} \ x^{0} y^{n} & + & \cdots  & + & c_{n,k-1} \ x^{k-1} y^{n-( k-1)} & \cdots  & + & c_{n,n-1} \ x^{n-1} y^{1} & + & c_{n,n} \ x^{n} y^{0}) & \cdot x
\end{array}\\
 & \begin{array}{ c c r c c c c c r c c c c c }
= & c_{n,0} \ x^{0} y^{n+1} & + & c_{n,1} \ x^{1} y^{n} & + & \cdots  & + & c_{n,k} \ x^{k} y^{n-k+1} & \cdots  & + & c_{n,n} \ x^{n} y^{1} &  &  & \\
 &  & + & c_{n,0} \ x^{1} y^{n} & + & \cdots  & + & c_{n,k-1} \ x^{k} y^{n-( k-1)} & \cdots  & + & c_{n,1} \ x^{n} y^{1} & + & c_{n,n} \ x^{n+1} y^{0} & 
\end{array}\\
 & \begin{array}{ c c r c c c c c r c c c c c c }
= & c_{n,0} \  & x^{0} y^{n+1} & + & \cdots  & + & ( c_{n,k} +c_{n,k-1}) & x^{k} y^{n-k+1} & \cdots  & + & ( c_{n,n} +c_{n,n-1}) \  & x^{n} y^{1} & + & c_{n,n} & x^{n+1} y^{0}\\
= & c_{n+1,0} \  & x^{0} y^{n+1} & + & \cdots  & + & c_{n+1,k} \  & x^{k} y^{n-k+1} & \cdots  & + & c_{n+1,n} & \ x^{n} y^{1} & + & c_{n+1,n+1} & x^{n+1} y^{0}
\end{array}
\end{aligned}$$


$$\displaystyle \begin{aligned}
( x+y)^{n+1} & =( x+y)^{n}( x+y)\\
 & \\
 & =\left( c_{n,0} \ x^{0} y^{n} +c_{n,1} \ x^{1} y^{n-1} +\cdots +c_{n,k} \ x^{k} y^{n-k} +\cdots +c_{n,n} \ x^{n} y^{0}\right)( x+y)\\
 & \\
 & \begin{aligned}
= &  & y\cdot ( & c_{n,0} \ x^{0} y^{n} & + & c_{n,1} \ x^{1} y^{n-1} & + & \cdots  & + & c_{n,k} \ x^{k} y^{n-k} & \cdots  & + & c_{n,n} \ x^{n} y^{0} &  &  & )\\
 & + & x\cdot ( &  &  & c_{n,0} \ x^{0} y^{n} & + & \cdots  & + & c_{n,k-1} \ x^{k-1} y^{n-( k-1)} & \cdots  & + & c_{n,n-1} \ x^{n-1} y^{1} & + & c_{n,n} \ x^{n} y^{0} & )
\end{aligned}\\
 & \\
 & \begin{aligned}
= & c_{n,0} \ x^{0} y^{n+1} & + & c_{n,1} \ x^{1} y^{n} & + & \cdots  & + & c_{n,k} \ x^{k} y^{n-k+1} & \cdots  & + & c_{n,n} \ x^{n} y^{1} &  &  & \\
 &  & + & c_{n,0} \ x^{1} y^{n} & + & \cdots  & + & c_{n,k-1} \ x^{k} y^{n-( k-1)} & \cdots  & + & c_{n,1} \ x^{n} y^{1} & + & c_{n,n} \ x^{n+1} y^{0} & 
\end{aligned}\\
 & \\
 & \begin{aligned}
= & c_{n,0} \  & x^{0} y^{n+1} & + & \cdots  & + & ( c_{n,k} +c_{n,k-1}) & x^{k} y^{n-k+1} & \cdots  & + & ( c_{n,n} +c_{n,n-1}) \  & x^{n} y^{1} & + & c_{n,n} & x^{n+1} y^{0}\\
= & c_{n+1,0} \  & x^{0} y^{n+1} & + & \cdots  & + & c_{n+1,k} \  & x^{k} y^{n-k+1} & \cdots  & + & c_{n+1,n} & \ x^{n} y^{1} & + & c_{n+1,n+1} & x^{n+1} y^{0}
\end{aligned}
\end{aligned}$$




| $n$ | Expansão | Coeficientes |
|---|----------|--------------|
| $0$ | $(x+y)^{0} = 1 = x^{0} y^{0}$ | $1$ |
| $1$ | $(x+y)^{1} = x+y = x^{0} y^{1} + x^{1} y^{0}$ | $1, 1$ |
| $2$ | $(x+y)^{2} = ... = y^{2} + 2xy + x^{2}$ | $1, 2, 1$ |
| $3$ | $(x+y)^{3} = ... = y^{3} + x^{3} + 3xy(x+y)$ | $1, 3, 3, 1$ |
| $4$ | $$$\displaystyle \begin{aligned}( x+y)^{4} & =( x+y)^{3}( x+y)\\ & =\left( x^{0} y^{3} +3+3x^{2} y^{1} +x^{3} y^{0}\right)( y+x)\\ & \begin{matrix}= & ( x^{0} y^{3} & + & 3x^{1} y^{2} & + & 3x^{2} y^{1} & + & x^{3} y^{0}) &  &  & \cdot y\\ &  & + & ( x^{0} y^{3} & + & 3x^{1} y^{2} & + & 3x^{2} y^{1} & + & x^{3} y^{0}) & \cdot x\end{matrix}\\ & \begin{matrix}= & x^{0} y^{4} & + & 3x^{1} y^{3} & + & 3x^{2} y^{2} & + & x^{3} y^{1} &  & \\ &  & + & x^{1} y^{3} & + & 3x^{2} y^{2} & + & 3x^{3} y^{1} & + & x^{4} y^{0}\end{matrix}\\ & \begin{matrix}= & x^{0} y^{4} & + & 4x^{1} y^{3} & + & 6x^{2} y^{2} & + & 4x^{3} y^{1} & + & x^{4} y^{0}\end{matrix}\\ & =y^{4} +4xy^{3} +6x^{2} y^{2} +4x^{3} y+x^{4}\\ & =y^{4} +x^{4} +4xy\left( y^{2} +x^{2}\right) +6x^{2} y^{2}\end{aligned}$$$ | $1, 4, 6, 4, 1$ || $\vdots$ | Seja $c_{n,k}$ o coeficiente de $x^{k}$ na expansão $(x+y)^{n}$ |  |


$$
\displaystyle
\begin{align}
(x+y)^{n+1} &= (x+y)^{n}(x+y) \\
&= (c_{n,0} x^{0} y^{n} + c_{n,1} x^{1} y^{n-1} + \cdots + c_{n,k} x^{k} y^{n-k} + \cdots + c_{n,n} x^{n} y^{0})(x+y) \\
&= c_{n,0} x^{0} y^{n+1} + (c_{n,1} + c_{n,0}) x^{1} y^{n} + \cdots + (c_{n,k} + c_{n,k-1}) x^{k} y^{n-k+1} + \cdots + c_{n,n} x^{n+1} y^{0} \\
&= c_{n+1,0} x^{0} y^{n+1} + c_{n+1,1} x^{1} y^{n} + \cdots + c_{n+1,k} x^{k} y^{n-k+1} + \cdots + c_{n+1,n+1} x^{n+1} y^{0}
\end{align}
$$

$$
\displaystyle
\begin{align}
c_{n+1,0} &= c_{n,0} \\
c_{n+1,1} &= c_{n,1} + c_{n,0} \\
&\vdots \\
c_{n+1,k} &= c_{n,k} + c_{n,k-1} \\
&\vdots \\
c_{n+1,n+1} &= c_{n,n}
\end{align}
$$


$$
c_{n+1,k} = c_{n,k} + c_{n,k-1}, \forall k \in \{0,...,n\}
$$

  
  

$\displaystyle c_{n,k} =\binom{n}{k} =\cfrac{n!}{k!\left( n-k\right) !}$


$\displaystyle \binom{n+1}{k} =\binom{n}{k} +\binom{n}{k-1}$

  

$\displaystyle \left[ S\right]_{\ell ,k} =\binom{\ell +k}{k} =\binom{\ell +k}{\ell }$


$$\displaystyle \left[\begin{matrix}

\binom{0}{0} & \binom{1}{1} & \binom{2}{2} & \binom{3}{3} & \binom{4}{4} & \cdots \\

\binom{1}{0} & \binom{2}{1} & \binom{3}{2} & \binom{4}{3} & \ddots  & \ddots \\

\binom{2}{0} & \binom{3}{1} & \binom{4}{2} & \ddots  & \ddots  & \ddots \\

\binom{3}{0} & \binom{4}{1} & \ddots  & \ddots  & \ddots  & \ddots \\

\binom{4}{0} & \ddots  & \ddots  & \ddots  & \ddots  & \ddots \\

\vdots  & \ddots  & \ddots  & \ddots  & \ddots  & \ddots

\end{matrix}\right] =\left[\begin{matrix}

1 & 1 & 1 & 1 & 1 & 1 & 1 & 1 & 1 & 1 & \cdots \\

1 & 2 & 3 & 4 & 5 & 6 & 7 & 8 & 9 & \ddots  & \ddots \\

1 & 3 & 6 & 10 & 15 & 21 & 28 & 36 & \ddots  & \ddots  & \ddots \\

1 & 4 & 10 & 20 & 35 & 46 & 74 & \ddots  & \ddots  & \ddots  & \ddots \\

1 & 5 & 15 & 35 & 70 & 116 & \ddots  & \ddots  & \ddots  & \ddots  & \ddots \\

1 & 6 & 21 & 46 & 116 & \ddots  & \ddots  & \ddots  & \ddots  & \ddots  & \ddots \\

1 & 7 & 28 & 74 & \ddots  & b & \ddots  & \ddots  & \ddots  & \ddots  & \ddots \\

  

1 & 8 & 36 & \ddots  & a & a+b & \ddots  & \ddots  & \ddots  & \ddots  & \ddots \\

1 & 9 & \ddots  & \ddots  & \ddots  & \ddots  & \ddots  & \ddots  & \ddots  & \ddots  & \ddots \\

\vdots  & \ddots  & \ddots  & \ddots  & \ddots  & \ddots  & \ddots  & \ddots  & \ddots  & \ddots  & \ddots

\end{matrix}\right]$$

  
  
  
$$
\displaystyle
\begin{aligned}
\left( x+y\right)^{\textcolor{lightgreen}{n}} 
&=\sum\limits _{\textcolor{cyan}{k} =0}^{\textcolor{lightgreen}{n}}\binom{\textcolor{lightgreen}{n}}{\textcolor{cyan}{k}} x^{\textcolor{cyan}{k}} y^{\textcolor{lightgreen}{n} -\textcolor{cyan}{k}}\\
&=\binom{\textcolor{lightgreen}{n}}{0} x^{0} y\textcolor{lightgreen}{^{n}} +\cdots +\binom{\textcolor{lightgreen}{n}}{\textcolor{cyan}{k}} x^{\textcolor{cyan}{k}} y^{\textcolor{lightgreen}{n} -\textcolor{cyan}{k}} +\cdots \binom{\textcolor{lightgreen}{n}}{0} x^{\textcolor{lightgreen}{n}} y^{0}\\
&=\sum\limits _{\textcolor{cyan}{k} =0}^{\left\lfloor \textcolor{lightgreen}{n} /2\right\rfloor } x^{\textcolor{cyan}{k}} y^{\textcolor{cyan}{k}}\binom{\textcolor{lightgreen}{n}}{\textcolor{cyan}{k}}\left( y^{\textcolor{lightgreen}{n} -2\textcolor{cyan}{k}}+x^{\textcolor{lightgreen}{n} -2\textcolor{cyan}{k}}\right)
\end{aligned}
$$

## Revisão de Propriedades do Somatório:

### Linearidade:

$$\begin{equation*}

\sum _{\textcolor{cyan}{k} =1}^{\textcolor{lightgreen}{n}}\left( ca_{\textcolor{cyan}{k}} +b_{\textcolor{cyan}{k}}\right) =c\sum _{\textcolor{cyan}{k} =1}^{\textcolor{lightgreen}{n}} a_{\textcolor{cyan}{k}} +\sum _{\textcolor{cyan}{k} =1}^{\textcolor{lightgreen}{n}} b_{\textcolor{cyan}{k}}

\end{equation*}
$$
### Permutação:

  
Seja $p: \{1, \cdots, n\} \rightarrow \{1, \cdots, n\}$ uma bijeção, com inversa $d: \{1, \cdots, n\} \rightarrow \{1, \cdots, n\}$

$$
\begin{equation*}

\sum _{\textcolor{cyan}{k} =d\left(\textcolor{cyan}{1}\right)}^{d\left(\textcolor{lightgreen}{n}\right)} a_{p\left(\textcolor{cyan}{k}\right)}

\end{equation*}
$$
  
  

## Coeficiente Multinomiais

 

De $\displaystyle \textcolor{lightgreen}{n}$ objetos queremos dividir esses $\displaystyle \textcolor{lightgreen}{n}$ objetos em $\displaystyle \textcolor{cyan}{m}$ grupos:
Descobrir os coeficientes da expansão $\displaystyle \left( x_{\textcolor{cyan}{1}} +\cdots +x\textcolor{cyan}{_{m}}\right)^{\textcolor{lightgreen}{n}}$

  
 

$$\displaystyle \begin{aligned}

\left(\sum _{\textcolor{cyan}{k} =1}^{\textcolor{cyan}{m}} x\textcolor{cyan}{_{k}}\right)^{\textcolor{lightgreen}{n}} & =\left( x\textcolor{cyan}{_{1}} +\sum _{\textcolor{cyan}{k} =\textcolor{cyan}{2}}^{\textcolor{cyan}{m}} x_{\textcolor{cyan}{k}}\right)^{\textcolor{lightgreen}{n}} =\sum _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} =0}^{\textcolor{lightgreen}{n}}\left(\binom{\textcolor{lightgreen}{n}}{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}}} \cdot x_{\textcolor{cyan}{1}}^{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}}}\left(\sum _{\textcolor{cyan}{k} =\textcolor{cyan}{2}}^{\textcolor{cyan}{m}} x_{\textcolor{cyan}{k}}\right)^{\textcolor{lightgreen}{n} -\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}}}\right)\\

 & =\sum _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} =0}^{\textcolor{lightgreen}{n}}\left(\binom{\textcolor{lightgreen}{n}}{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}}} \cdot x_{\textcolor{cyan}{1}}^{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}}}\right)\sum _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{2}} =0}^{\textcolor{lightgreen}{n} -\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}}}\left(\binom{\textcolor{lightgreen}{n} -\textcolor{lightgreen}{n}_{\textcolor{cyan}{1}}}{\textcolor{lightgreen}{n}\textcolor{cyan}{_{2}}} \cdot x_{\textcolor{cyan}{2}}^{\textcolor{lightgreen}{n}_{\textcolor{cyan}{2}}}\right) \cdots \sum _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} =0}^{\textcolor{lightgreen}{n} -\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} \cdots -\textcolor{lightgreen}{n}\textcolor{cyan}{_{m-1}}}\left(\binom{\textcolor{lightgreen}{n} -\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} \cdots -\textcolor{lightgreen}{n}\textcolor{cyan}{_{m-1}}}{\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}}} \cdot x_{\textcolor{cyan}{m}}^{\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}}}\right)\\

 & =\sum _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} =0}^{\textcolor{lightgreen}{n}}\sum _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{2}} =0}^{\textcolor{lightgreen}{n} -\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}}}\sum _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{3}} =0}^{\textcolor{lightgreen}{n} -\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} -\textcolor{lightgreen}{n}\textcolor{cyan}{_{2}}} \cdots \sum _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} =0}^{\textcolor{lightgreen}{n} -\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} \cdots -\textcolor{lightgreen}{n}\textcolor{cyan}{_{m-1}}}\left(\prod _{\textcolor[rgb]{0.82,0.01,0.11}{k} =1}^{\textcolor{cyan}{m}}\binom{\textcolor{lightgreen}{n}

  

-\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} -\cdots -\textcolor{lightgreen}{n}\textcolor{cyan}{_{k-1}}}{\textcolor{lightgreen}{n}\textcolor{cyan}{_{\textcolor[rgb]{0.82,0.01,0.11}{k}}}} \cdot x_{\textcolor[rgb]{0.82,0.01,0.11}{k}}^{\textcolor{lightgreen}{n}\textcolor[rgb]{0.82,0.01,0.11}{_{k}}}\right)\\

 & =\sum\limits _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} ,\cdots ,\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} \geq 0}^{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} +\cdots +\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} =\textcolor{lightgreen}{n}}\left(\prod _{\textcolor[rgb]{0.82,0.01,0.11}{k} =\textcolor[rgb]{0.82,0.01,0.11}{1}}^{\textcolor{cyan}{m}}\binom{\textcolor{lightgreen}{n} -\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} -\cdots -\textcolor{lightgreen}{n}\textcolor{cyan}{_{k-1}}}{\textcolor{lightgreen}{n}\textcolor{cyan}{_{\textcolor[rgb]{0.82,0.01,0.11}{k}}}} \cdot x_{\textcolor[rgb]{0.82,0.01,0.11}{k}}^{\textcolor{lightgreen}{n}\textcolor[rgb]{0.82,0.01,0.11}{_{k}}}\right)\\

 & =\sum\limits _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} ,\cdots ,\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} \geq 0}^{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} +\cdots +\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} =\textcolor{lightgreen}{n}}\left(\prod\limits _{\textcolor[rgb]{0.82,0.01,0.11}{k} =\textcolor[rgb]{0.82,0.01,0.11}{1}}^{\textcolor{cyan}{m}}\binom{\sum\nolimits _{\textcolor{yellow}{s} =\textcolor[rgb]{0.82,0.01,0.11}{k}}^{\textcolor{cyan}{m}} n_{\textcolor{yellow}{s}}}{\textcolor{lightgreen}{n}\textcolor{cyan}{_{\textcolor[rgb]{0.82,0.01,0.11}{k}}}} \cdot x_{\textcolor[rgb]{0.82,0.01,0.11}{k}}^{\textcolor{lightgreen}{n}\textcolor[rgb]{0.82,0.01,0.11}{_{k}}}\right)\\

 & =\sum\limits _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} ,\cdots ,\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} \geq 0}^{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} +\cdots +\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} =\textcolor{lightgreen}{n}}\left(\prod\limits _{\textcolor[rgb]{0.82,0.01,0.11}{k} =\textcolor[rgb]{0.82,0.01,0.11}{1}}^{\textcolor{cyan}{m}}\left(\cfrac{\left(\sum\limits _{\textcolor{yellow}{s} =\textcolor[rgb]{0.82,0.01,0.11}{k}}^{\textcolor{cyan}{m}} n_{\textcolor{yellow}{s}}\right) !}{\textcolor{lightgreen}{n}\textcolor{cyan}{_{\textcolor[rgb]{0.82,0.01,0.11}{k}}} !\left(\sum\limits _{\textcolor{yellow}{s} =\textcolor[rgb]{0.82,0.01,0.11}{k} +1}^{\textcolor{cyan}{m}} n_{\textcolor{yellow}{s}}\right) !}\right) \cdot x_{\textcolor[rgb]{0.82,0.01,0.11}{k}}^{\textcolor{lightgreen}{n}\textcolor[rgb]{0.82,0.01,0.11}{_{k}}}\right)\\

 & =\sum _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} ,\cdots ,\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} \geq 0}^{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} +\cdots +\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} =\textcolor{lightgreen}{n}}\left(\left(\prod\limits _{\textcolor[rgb]{0.82,0.01,0.11}{k} =\textcolor[rgb]{0.82,0.01,0.11}{1}}^{\textcolor{cyan}{m}}\cfrac{1}{\textcolor{lightgreen}{n}\textcolor{cyan}{_{\textcolor[rgb]{0.82,0.01,0.11}{k}}} !}\right)\left(\cfrac{\prod\limits _{\textcolor[rgb]{0.82,0.01,0.11}{k}

  

=\textcolor[rgb]{0.82,0.01,0.11}{1}}^{\textcolor{cyan}{m}}\left(\sum\limits _{\textcolor{yellow}{s} =\textcolor[rgb]{0.82,0.01,0.11}{k}}^{\textcolor{cyan}{m}} n_{\textcolor{yellow}{s}}\right) !}{\prod\limits _{\textcolor[rgb]{0.82,0.01,0.11}{k} =\textcolor[rgb]{0.82,0.01,0.11}{1}}^{\textcolor{cyan}{m}}\left(\sum\limits _{\textcolor{yellow}{s} =\textcolor[rgb]{0.82,0.01,0.11}{k} +1}^{\textcolor{cyan}{m}} n_{\textcolor{yellow}{s}}\right) !}\right) \cdot x_{\textcolor[rgb]{0.82,0.01,0.11}{k}}^{\textcolor{lightgreen}{n}\textcolor[rgb]{0.82,0.01,0.11}{_{k}}}\right)\\

 & =\sum _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} ,\cdots ,\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} \geq 0}^{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} +\cdots +\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} =\textcolor{lightgreen}{n}}\left(\left(\prod\limits _{\textcolor[rgb]{0.82,0.01,0.11}{k} =\textcolor[rgb]{0.82,0.01,0.11}{1}}^{\textcolor{cyan}{m}}\cfrac{1}{\textcolor{lightgreen}{n}\textcolor{cyan}{_{\textcolor[rgb]{0.82,0.01,0.11}{k}}} !}\right)\left(\sum\limits _{\textcolor{yellow}{s} =1}^{\textcolor{cyan}{m}} n_{\textcolor{yellow}{s}}\right) !\ \cancel{\cfrac{\prod\nolimits _{\textcolor[rgb]{0.82,0.01,0.11}{k} =\textcolor[rgb]{0.82,0.01,0.11}{1}}^{\textcolor{cyan}{m}}\left(\sum\limits _{\textcolor{yellow}{s} =\textcolor[rgb]{0.82,0.01,0.11}{k} +1}^{\textcolor{cyan}{m}} n_{\textcolor{yellow}{s}}\right) !}{\prod\limits _{\textcolor[rgb]{0.82,0.01,0.11}{k} =\textcolor[rgb]{0.82,0.01,0.11}{1}}^{\textcolor{cyan}{m}}\left(\sum\limits _{\textcolor{yellow}{s} =\textcolor[rgb]{0.82,0.01,0.11}{k} +1}^{\textcolor{cyan}{m}} n_{\textcolor{yellow}{s}}\right) !}} \cdot x_{\textcolor[rgb]{0.82,0.01,0.11}{k}}^{\textcolor{lightgreen}{n}\textcolor[rgb]{0.82,0.01,0.11}{_{k}}}\right)\\

 & =\sum _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} ,\cdots ,\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} \geq 0}^{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} +\cdots +\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} =\textcolor{lightgreen}{n}}\left(\prod\limits _{\textcolor[rgb]{0.82,0.01,0.11}{k} =\textcolor[rgb]{0.82,0.01,0.11}{1}}^{\textcolor{cyan}{m}}\cfrac{\textcolor{lightgreen}{n} !}{n\textcolor[rgb]{0.82,0.01,0.11}{_{k}} !}\right) \cdot x_{\textcolor[rgb]{0.82,0.01,0.11}{k}}^{\textcolor{lightgreen}{n}\textcolor[rgb]{0.82,0.01,0.11}{_{k}}}

\end{aligned}$$

O último passo pode ser justificado da seguinte forma
Imagine os termos $\displaystyle n_{k}$ em base 1. 
Cada soma será uma combinação dos $\displaystyle n+( m-1)$ símbolos $\displaystyle \{1,+\}$
$$\displaystyle 1_{1} +_{a} 1_{2} 1_{3} +_{b} 1_{4} 1_{5} 1_{6} +_{c}{} 1_{7}$$


Assim, temos $\displaystyle \binom{n+m-1}{m-1}$ manerias de escolher os $\displaystyle m-1$ símbolos $\displaystyle +$ entre os $\displaystyle n+m-1$ símbolos totais.

  
  
  

$$\displaystyle \left(\sum _{k=\textcolor{yellow}{1}}^{\textcolor{yellow}{m}} x_{\textcolor{yellow}{k}}\right)^{\textcolor{lightgreen}{n}} =\sum _{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} ,\cdots ,\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} \geq 0}^{\textcolor{lightgreen}{n}\textcolor{cyan}{_{1}} +\cdots +\textcolor{lightgreen}{n}\textcolor{cyan}{_{m}} =\textcolor{lightgreen}{n}}\left(\prod\limits _{\textcolor[rgb]{0.82,0.01,0.11}{k} =\textcolor[rgb]{0.82,0.01,0.11}{1}}^{\textcolor{cyan}{m}}\cfrac{\textcolor{lightgreen}{n} !}{n\textcolor[rgb]{0.82,0.01,0.11}{_{k}} !}\right) \cdot x_{\textcolor[rgb]{0.82,0.01,0.11}{k}}^{\textcolor{lightgreen}{n}\textcolor[rgb]{0.82,0.01,0.11}{_{k}}} =\sum _{\begin{matrix}

\textcolor[rgb]{0.82,0.01,0.11}{k} \in \{1,\cdots \textcolor{cyan}{m}\}\\

n_{\textcolor[rgb]{0.82,0.01,0.11}{k}} \in \{1,\cdots \textcolor{lightgreen}{n}\}\\

\sum _{\textcolor[rgb]{0.82,0.01,0.11}{k} =1}^{\textcolor{yellow}{m}} n\textcolor[rgb]{0.82,0.01,0.11}{_{\textcolor[rgb]{0.82,0.01,0.11}{k}}} =\textcolor{lightgreen}{n}

\end{matrix}}\left(\prod\limits _{\textcolor[rgb]{0.82,0.01,0.11}{k} =\textcolor[rgb]{0.82,0.01,0.11}{1}}^{\textcolor{cyan}{m}}\cfrac{\textcolor{lightgreen}{n} !}{n\textcolor[rgb]{0.82,0.01,0.11}{_{k}} !}\right) \cdot x_{\textcolor[rgb]{0.82,0.01,0.11}{k}}^{\textcolor{lightgreen}{n}\textcolor[rgb]{0.82,0.01,0.11}{_{k}}}$$

  
  
  

## Bayes Rule
  
$$\displaystyle  \begin{array}{{>{\displaystyle}l}}

{P}(\textcolor{cyan}{R} |\textcolor{yellow}{E}) := \cfrac{{P}(\textcolor{yellow}{E} ,\textcolor{cyan}{R})}{{P}(\textcolor{yellow}{E})} =\cfrac{{P}(\textcolor{yellow}{E} |\textcolor{cyan}{R}) \cdot P(\textcolor{cyan}{R})}{{P}(\textcolor{yellow}{E})} =\cfrac{{P}(\textcolor{yellow}{E} |\textcolor{cyan}{R}) \cdot P(\textcolor{cyan}{R})}{{P}(\textcolor{yellow}{E} |\textcolor{cyan}{R}) \cdot P(\textcolor{cyan}{R}) +{P}(\textcolor{yellow}{E} |\neg \textcolor{cyan}{R}) -{P}(\textcolor{yellow}{E} |\neg \textcolor{cyan}{R}) \cdot P(\textcolor{cyan}{R})}\\

=\cfrac{{P}(\textcolor{yellow}{E} ,\textcolor{cyan}{R})}{{P}(\textcolor{yellow}{E} ,\textcolor{cyan}{R}) +{P}(\textcolor{yellow}{E} ,\neg \textcolor{cyan}{R})} =\cfrac{1}{1+\cfrac{{P}(\textcolor{yellow}{E} ,\neg \textcolor{cyan}{R})}{{P}(\textcolor{yellow}{E} ,\textcolor{cyan}{R})}} =\cfrac{1}{1+\cfrac{{P}(\textcolor{yellow}{E} |\neg \textcolor{cyan}{R})}{{P}(\textcolor{yellow}{E} |\textcolor{cyan}{R})} \cdot \left(\cfrac{1}{{P}(\textcolor{cyan}{R})} -1\right)}\\

\\

\underbrace{{O}(\textcolor{lightgreen}{B} |\textcolor[rgb]{0.56,0.07,1}{A})}_{\cfrac{1}{\cfrac{1}{{P}(\textcolor{lightgreen}{B} |\textcolor[rgb]{0.56,0.07,1}{A})} -1}} =\cfrac{1}{\cfrac{{P}(\textcolor[rgb]{0.56,0.07,1}{A})}{{P}(\textcolor{pink}{A} |\textcolor{lightgreen}{B}) \cdotp {P}(\textcolor{lightgreen}{B})} -1} =\cfrac{1}{\cfrac{{P}(\textcolor{pink}{A} ,\textcolor{lightgreen}{B})

  

+{P}(\textcolor{pink}{A} ,\neg \textcolor{lightgreen}{B})}{{P}(\textcolor{pink}{A} ,\textcolor{lightgreen}{B})} -1} =\cfrac{{P}(\textcolor{pink}{A} ,\textcolor{lightgreen}{B})}{{P}(\textcolor{pink}{A} ,\neg \textcolor{lightgreen}{B})} =\underbrace{{L}(\textcolor{pink}{A} |\textcolor{lightgreen}{B})}_{\cfrac{{P}(\textcolor{pink}{A} |\textcolor{lightgreen}{B})}{{P}(\textcolor{pink}{A} |\neg \textcolor{lightgreen}{B})}} \cdot \underbrace{{O}(\textcolor{lightgreen}{B})}_{\cfrac{1}{\cfrac{1}{{P}(\textcolor{lightgreen}{B})} -1}}

\end{array}$$

  

$\displaystyle \underbrace{\log{O}(\textcolor{lightgreen}{B} |\textcolor[rgb]{0.56,0.07,1}{A})}_{\log{P}(\textcolor{lightgreen}{B} |\textcolor[rgb]{0.56,0.07,1}{A}) -\log{P} \neg (\textcolor{lightgreen}{B} |\textcolor[rgb]{0.56,0.07,1}{A})} =\log{P}(\textcolor{pink}{A} |\textcolor{lightgreen}{B}) -\log{P}(\textcolor{pink}{A} |\neg \textcolor{lightgreen}{B}) +\underbrace{\log{O}(\textcolor{lightgreen}{B})}_{\underbrace{\log{P}(\textcolor{lightgreen}{B}) -\log{P}(\textcolor{lightgreen}{\neg B})}_{-\log\left(\cfrac{1}{P(\textcolor{lightgreen}{B})} -1\right)}} =$

  

$\displaystyle {P}(\textcolor{lightgreen}{B} |\textcolor[rgb]{0.56,0.07,1}{A}) =\cfrac{1}{\cfrac{1}{{L}(\textcolor{pink}{A} |\textcolor{lightgreen}{B})}\left(\cfrac{1}{{P}(\textcolor{lightgreen}{B})} -1\right) +1}$

  
  
  

$$\displaystyle  \begin{array}{{>{\displaystyle}l}}

o( p) =\cfrac{1}{\cfrac{1}{p} -1} \Rightarrow \cfrac{1}{o} =\cfrac{1-p}{p} \Rightarrow o=\cfrac{p}{1-p}\\

\begin{matrix}

p=\sin^{2} \theta \\

o=\tan \theta

\end{matrix} \Rightarrow \begin{array}{ l }

p=\sin^{2}\arctan o\\

o=\tan\arcsin\sqrt{p}

\end{array} \Rightarrow \arcsin\sqrt{p} =\arctan o

\end{array}$$

  
  
  

$\displaystyle \tan \theta (\textcolor{lightgreen}{B} |\textcolor[rgb]{0.56,0.07,1}{A}) =\cfrac{\sin^{2} \theta (\textcolor{pink}{A} |\textcolor{lightgreen}{B})}{\sin^{2} \theta (\textcolor{pink}{A} |\neg \textcolor{lightgreen}{B})} \cdot \tan \theta (\textcolor{lightgreen}{B})$

  

## Probabilidade

  

[Probability spaces and random variables](https://www.youtube.com/watch?v=DqGUwoz4d4M\&ab\_channel=IntelligentSystemsLab)

  

Dado um (possivelmente incontável) conjunto de possíveis resultados $\displaystyle\textcolor{yellow}{\Omega}$, um evento $\displaystyle \textcolor{yellow}{\mathbb {E}} \subseteq \textcolor{yellow}{\Omega}$ é uma condição nos possíveis resultados. A $\sigma$-algebra de todos os possíveis eventos $\displaystyle \textcolor{yellow}{E}\subseteq 2^{\textcolor{yellow}{\Omega}}$ é tal que 

- $\displaystyle \{\} \in \textcolor{yellow}{E}$ (1)
- $\displaystyle \forall \textcolor{cyan}{A},\textcolor{lightgreen}{B}\in \textcolor{yellow}{E}:\textcolor{yellow}{\Omega} \backslash ( \textcolor{cyan}{A}\cap \textcolor{lightgreen}{B}) \in \textcolor{yellow}{E}$ (2)

Com $\displaystyle \textcolor{cyan}{A}=\textcolor{lightgreen}{B}=\{\}$ em (2) conclui-se que $\displaystyle\textcolor{yellow}{\Omega} \backslash (\{\} \cap \{\}) =\Omega \backslash \{\} =\Omega \in E$

Assim podemos deduzir que:
- $\forall \textcolor{cyan}{A}$, com $\textcolor{lightgreen}{B}=\textcolor{cyan}{A}$ em (2) conclui-se que $\textcolor{yellow}{\Omega} \backslash (\textcolor{cyan}{A}\cap \textcolor{cyan}{A}) =\textcolor{yellow}{\Omega} \backslash \textcolor{cyan}{A}\in \textcolor{yellow}{E}$ (3)
- $\forall \textcolor{cyan}{A}, \textcolor{lightgreen}{B}\in \textcolor{yellow}{E}$ de (3) $(\textcolor{yellow}{\Omega} \backslash \textcolor{cyan}{A}), (\textcolor{yellow}{\Omega} \backslash \textcolor{lightgreen}{B}) \in \textcolor{yellow}{E}$, de (2) $\textcolor{yellow}{\Omega} \backslash ((\textcolor{yellow}{\Omega} \backslash \textcolor{cyan}{A}) \cap (\textcolor{yellow}{\Omega} \backslash \textcolor{lightgreen}{B})) =(\textcolor{cyan}{A}\cup \textcolor{lightgreen}{B}) \in \textcolor{yellow}{E}$ (4)
- $\forall \textcolor{cyan}{A}, \textcolor{lightgreen}{B}\in \textcolor{yellow}{E}$ de (4) $(\textcolor{cyan}{A}\cup \textcolor{lightgreen}{B}) \in \textcolor{yellow}{E}$, de (3) $\textcolor{yellow}{\Omega} \backslash (\textcolor{cyan}{A}\cup \textcolor{lightgreen}{B}) \in \textcolor{yellow}{E}$ (5)
- $\forall \textcolor{cyan}{A}, \textcolor{lightgreen}{B}\in \textcolor{yellow}{E}$ de (3) $(\textcolor{yellow}{\Omega} \backslash \textcolor{cyan}{A}), (\textcolor{yellow}{\Omega} \backslash \textcolor{lightgreen}{B}) \in \textcolor{yellow}{E}$, de (5) $\textcolor{yellow}{\Omega} \backslash ((\textcolor{yellow}{\Omega} \backslash \textcolor{cyan}{A}) \cup (\textcolor{yellow}{\Omega} \backslash \textcolor{lightgreen}{B})) =(\textcolor{cyan}{A}\cap \textcolor{lightgreen}{B}) \in \textcolor{yellow}{E}$ (6)
- $\forall \textcolor{cyan}{A}, \textcolor{lightgreen}{B}\in \textcolor{yellow}{E}$ de (3) $(\textcolor{yellow}{\Omega} \backslash \textcolor{lightgreen}{B}) \in \textcolor{yellow}{E}$, de (6) $\textcolor{cyan}{A}\cap (\textcolor{yellow}{\Omega} \backslash \textcolor{lightgreen}{B}) =(\textcolor{cyan}{A}\backslash \textcolor{lightgreen}{B}) \in \textcolor{yellow}{E}$ (7)
- $\forall \textcolor{cyan}{A}, \textcolor{lightgreen}{B}\in \textcolor{yellow}{E}$ de (7) $(\textcolor{cyan}{A}\backslash \textcolor{lightgreen}{B}), (\textcolor{lightgreen}{B}\backslash \textcolor{cyan}{A}) \in \textcolor{yellow}{E}$, de (4) $(\textcolor{cyan}{A}\backslash \textcolor{lightgreen}{B}) \cup (\textcolor{lightgreen}{B}\backslash \textcolor{cyan}{A}) := \textcolor{cyan}{A} \underset{\cdot}{\cup} \textcolor{lightgreen}{B}\in \textcolor{yellow}{E}$ (8)


A probabilidade é definida como uma função $\displaystyle P:E\rightarrow [ 0,1]$ que mede os eventos de tal forma que

- $\displaystyle P(\textcolor{yellow}{\Omega} ) =1$ (A)
- $\displaystyle P((\textcolor{cyan}{A} \backslash \textcolor{lightgreen}{B}) \cup ( \textcolor{lightgreen}{B}\backslash \textcolor{cyan}{A})) =P( \textcolor{cyan}{A}\backslash \textcolor{lightgreen}{B}) +P( \textcolor{lightgreen}{B}\backslash \textcolor{cyan}{A})$ (B)

Com $\textcolor{cyan}{A}=\{\}\\ \text{ e } \textcolor{lightgreen}{B}=\textcolor{yellow}{\Omega}$ em (B), $\displaystyle P(\{\}) +P(\textcolor{yellow}{\Omega} ) =P((\{\} \backslash\textcolor{yellow}{\Omega} ) \cup (\textcolor{yellow}{\Omega} \backslash \{\})) =P(\{\} \cup\textcolor{yellow}{\Omega} ) =P(\textcolor{yellow}{\Omega} ) \Rightarrow P(\{\}) =0$ (C)

$$

\displaystyle \textcolor{cyan}{A}\subseteq \textcolor{lightgreen}{B}\Rightarrow \begin{array}{ r }
\textcolor{cyan}{A}\backslash \textcolor{lightgreen}{B}=\textcolor{cyan}{A}\\
\textcolor{cyan}{A}\cup ( \textcolor{lightgreen}{B}\backslash \textcolor{cyan}{A}) =\textcolor{lightgreen}{B}
\end{array} \Rightarrow P( \textcolor{lightgreen}{B}) =P\left(\overbrace{\underbrace{( \textcolor{cyan}{A}\backslash \textcolor{lightgreen}{B})}_{\textcolor{cyan}{A}} \cup ( \textcolor{lightgreen}{B}\backslash \textcolor{cyan}{A})}^{\textcolor{lightgreen}{B}}\right) =P( \textcolor{cyan}{A}) +P( \textcolor{lightgreen}{B}\backslash \textcolor{cyan}{A})
$$
$\displaystyle \therefore P( \textcolor{lightgreen}{B}\backslash \textcolor{cyan}{A}) =P( \textcolor{lightgreen}{B}) -P( \textcolor{cyan}{A})$ (D)

$\displaystyle \forall k\in \{1,\cdots ,n\}$ Seja $\displaystyle ( A_{k})$ uma família de mutuamente disjuntos ($\displaystyle \textcolor{cyan}{A_{k}} \cap \textcolor{lightgreen}{A_{\ell}} =\{\} \Leftrightarrow \textcolor{cyan}{A_{k}} \backslash \textcolor{lightgreen}{A_{\ell}} =\textcolor{cyan}{A_{k}}$)
Base: $\displaystyle P(( A_{1} \backslash A_{2}) \cup ( A_{2} \backslash A_{1})) =P( A_{1} \backslash A_{2}) +P( A_{2} \backslash A_{1}) =P( A_{1}) +P( A_{2})$
Hipótese de indução $\displaystyle P\left(\bigcup _{k=1}^{n-1} A_{k}\right) =\sum _{k=1}^{n-1} P( A_{k})$
$$\begin{aligned}

P\left(\bigcup _{k=1}^{n-1} A_{k} \cup A_{n}\right)
&=P\left(\bigcup _{k=1}^{n-1}( A_{k} \backslash A_{n}) \cup \bigcup _{k=1}^{n-1}( A_{n} \backslash A_{k})\right) \\
&=P\left(\left(\bigcup _{k=1}^{n-1} A_{k}\right) \backslash A_{n} \cup A_{n} \backslash \left(\bigcup _{k=1}^{n-1} A_{k}\right)\right)\\
&=P\left(\bigcup _{k=1}^{n-1} A_{k}\right) +P( A_{n}) \\
&=\sum _{k=1}^{n-1} P( A_{k}) +P( A_{n}) \\
&=\sum _{k=1}^{n} P( A_{k})
\end{aligned}$$
$\displaystyle \therefore P\left(\bigcup _{k=1}^{n} A_{k}\right) =\sum _{k=1}^{n} P( A_{k})$ (E)

  
  
  

Quaisquer conjuntos $\displaystyle A,B$ são tais que $\displaystyle A\backslash B,A\cap B,\ B\backslash A$ são mutuamente disjuntos, de (E)
$P( A\cup B) =P(( A\backslash B) \cup ( A\cap B) \cup ( B\backslash A)) =P( A\backslash B) +P( A\cap B) +P( B\backslash A)$
$P( A) +P( B) =P( A\backslash B) +P( A\cap B) +P( B\backslash A) +P( A\cap B) =P( A\cup B) +P( A\cap B)$ 
$\displaystyle \therefore P( A) +P( B) =P( A\cup B) +P( A\cap B)$ (F)

Para $\displaystyle n$ termos:
$$  \begin{aligned}
\displaystyle P\left(\bigcup _{k=1}^{n} A_{k}\right)
&=P\left(\bigcup_{k=1}^{n-1} A_{k} \cup A_{n}\right) \\
&=P\left(\bigcup_{k=1}^{n-1} A_{k}\right) +P( A_{n}) -P\left(\left(\bigcup _{k=1}^{n-1} A_{k}\right) \cap A_{n}\right)\\
&=\displaystyle\sum _{k=1}^{n-1}( -1)^{k}\sum _{k_{1} < \cdots < k_{k}} P\left(\bigcap _{\ell =1}^{n-1} A_{k_{\ell }}\right) +P( A_{n}) -P\left(\left(\bigcup _{k=1}^{n-1} A_{k}\right) \cap A_{n}\right)
\end{aligned}$$

For any binary relation $\displaystyle R$ defined on $\Omega$

A function $\displaystyle p:\Omega \rightarrow {R}$ is called a probability density function if $\displaystyle \forall A\in E$ $\displaystyle P( A) =\int _{A} \rho dP=\int _{A} \rho ( x) dP( x)$


For example, if $\displaystyle\textcolor{yellow}{\Omega} ={\mathbb{R}}^{4}$, and $\displaystyle \rho ( t,x,y,z)$ is the probability density function, so 
$$\displaystyle P\left(\begin{matrix}

T_{m} < t< T_{M}\\

X_{m} < x< X_{M}\\

Y_{m} < y< Y_{M}\\

Z_{m} < z< Z_{M}

\end{matrix}\right) =\int _{T_{m}}^{T_{M}}\int _{X_{m}}^{X_{M}}\int _{Y_{m}}^{Y_{M}}\int _{Z_{m}}^{Z_{M}} \rho ( t,x,y,z) \ dt\ dx\ dy\ dz$$

  
  
  
  
  
  
  

## Transformação de Variáveis Aleatórias

V.A. $\displaystyle X$ com densidade $\displaystyle \rho _{\textcolor{lightgreen}{X}}$ $\displaystyle \textcolor{cyan}{Y} =\textcolor{cyan}{p}(\textcolor{lightgreen}{X})$. Distribuição de $\displaystyle \textcolor{cyan}{Y}$?


$\displaystyle \textcolor{lightgreen}{X}$ é discreto $\displaystyle \Rightarrow$ Achar Valores $\displaystyle \textcolor{cyan}{p}(\textcolor{lightgreen}{x}) \Rightarrow {P}(\textcolor{cyan}{Y} =\textcolor{cyan}{y}) =\sum _{\textcolor{lightgreen}{x}_{k} ;\textcolor{lightgreen}{f}(\textcolor{lightgreen}{x}_{k}) =\textcolor{cyan}{y}}{P}(\textcolor{lightgreen}{x} =\textcolor{lightgreen}{x}_{i})$

  

### Teorema
Seja $\textcolor{lightgreen}{\displaystyle X}$ uma variável aleatória com densidade $\displaystyle \rho_\textcolor{lightgreen}{{X}}$, $\displaystyle \textcolor{cyan}{p}(\textcolor{lightgreen}{x})$ suave e bijetora (com inversa $\displaystyle \textcolor{lightgreen}{q}$), então podemos achar $\displaystyle \rho_\textcolor{cyan}{{Y}}$ de forma que $\displaystyle \textcolor{cyan}{Y} =\textcolor{cyan}{p}(\textcolor{lightgreen}{X})$


$$\begin{equation*}

\rho_\textcolor{cyan}{{Y}}(\textcolor{cyan}{y}) =
\begin{cases}
	\rho_\textcolor{lightgreen}{{X}}\left(
		\textcolor{lightgreen}{q}(\textcolor{cyan}{y})
	\right)\left|
		\cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right|  & ;\text{se} \ \exists \textcolor{lightgreen}{x} :\textcolor{cyan}{p}(\textcolor{lightgreen}{x}) =\textcolor{cyan}{y}\\

	0 & ;\text{caso contrário}

\end{cases}

\end{equation*}$$

#### Prova:
$$\displaystyle \begin{aligned}
\textcolor{cyan}{p}(\textcolor{lightgreen}{x}) \ \text{é decrescente} \ \Rightarrow \rho _{\textcolor{cyan}{Y}} & =\cfrac{d}{d\textcolor{cyan}{y}}\mathbb{P}(\textcolor{cyan}{Y} \leqslant \textcolor{cyan}{y})\\
 & =\cfrac{d}{d\textcolor{cyan}{y}}\mathbb{P}(\textcolor{cyan}{p}(\textcolor{lightgreen}{X}) \leqslant \textcolor{cyan}{y})\\
 & =\cfrac{d}{d\textcolor{cyan}{y}}\mathbb{P}(\textcolor{lightgreen}{X} \geqslant \textcolor{lightgreen}{q}(\textcolor{cyan}{y}))\\
 & =\cfrac{d}{d\textcolor{cyan}{y}}( 1-\mathbb{P}(\textcolor{lightgreen}{X} \leqslant \textcolor{lightgreen}{x})) \\
 & =\underbrace{\cfrac{d}{d\textcolor{cyan}{y}} 1}_{0} -\cfrac{d}{d\textcolor{cyan}{y}}\mathbb{P}(\textcolor{lightgreen}{X} \leqslant \textcolor{lightgreen}{x})\\
 & =-\cfrac{d}{d\textcolor{cyan}{y}}\mathbb{P}(\textcolor{lightgreen}{X} \leqslant \textcolor{lightgreen}{q}(\textcolor{cyan}{y}))\\
 & =-\underbrace{\cfrac{d}{d\textcolor{lightgreen}{q}(\textcolor{cyan}{y})}\mathbb{P}(\textcolor{lightgreen}{X} \leqslant \textcolor{lightgreen}{q}(\textcolor{cyan}{y}))}_{\rho _{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{q}(\textcolor{cyan}{y}))} \cdot \cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y})\\
 & =-\rho _{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{q}(\textcolor{cyan}{y}))\cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y})
\end{aligned}$$

$$\displaystyle \begin{aligned}
\textcolor{cyan}{p}(\textcolor{lightgreen}{x}) \ \text{é crescente} \ \Rightarrow \rho _{\textcolor{cyan}{Y}} & =\cfrac{d}{d\textcolor{cyan}{y}}\mathbb{P}(\textcolor{cyan}{Y} \leqslant \textcolor{cyan}{y})\\
 & =\cfrac{d}{d\textcolor{cyan}{y}}\mathbb{P}(\textcolor{cyan}{p}(\textcolor{lightgreen}{X}) \leqslant \textcolor{cyan}{y})\\
 & =\cfrac{d}{d\textcolor{cyan}{y}}\mathbb{P}(\textcolor{lightgreen}{X} \leqslant \textcolor{lightgreen}{q}(\textcolor{cyan}{y}))\\
 & =\cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y}) \cdot \underbrace{\cfrac{d}{d\textcolor{lightgreen}{q}(\textcolor{cyan}{y})}\mathbb{P}(\textcolor{lightgreen}{X} \leqslant \textcolor{lightgreen}{q}(\textcolor{cyan}{y}))}_{\rho _{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{q}(\textcolor{cyan}{y}))}\\
 & =\cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y}) \cdot \rho _{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{q}(\textcolor{cyan}{y}))
\end{aligned}$$

Se $\displaystyle \textcolor{cyan}{p}(\textcolor{lightgreen}{x}) \ \text{é decrescente}$, $\displaystyle \cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y}) < 0$.Então $\displaystyle \cfrac{\left| \cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y})\right| }{\cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y})} =-1$

Se $\displaystyle \textcolor{cyan}{p}(\textcolor{lightgreen}{x}) \ \text{é crescente}$, $\displaystyle \cfrac{\left| \cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y})\right| }{\cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y})} =1$

So, in general we can write $\displaystyle \rho _{\textcolor{cyan}{Y}} =\cfrac{\left| \cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y})\right| }{\bcancel{\cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y})}} \rho _{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{q}(\textcolor{cyan}{y}))\bcancel{\cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y})} =\left| \cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y})\right| \rho _{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{q}(\textcolor{cyan}{y}))$
$$\begin{equation*}
\textcolor{cyan}{\rho }\textcolor{cyan}{_{Y}}(\textcolor{cyan}{y}) =\begin{cases}
\rho _{\textcolor{lightgreen}{X}}\left(\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right)\left| \cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y})\right|  & ;\text{se} \ \exists \textcolor{lightgreen}{x} :\textcolor{cyan}{p}(\textcolor{lightgreen}{x}) =\textcolor{cyan}{y}\\
0 & ;\text{caso contrário}
\end{cases}
\end{equation*}$$




Dada uma variável aleatória $\textcolor{cyan}{X}$ com função característica $\varphi_{\textcolor{cyan}{X}}$, calcule a função característica $\varphi_{\textcolor{cyan}{Y}}$ tal que $\textcolor{cyan}{Y}=p\left(\textcolor{cyan}{X}\right)$ com inversa $q$, ou seja $\textcolor{cyan}{X} = q\left(\textcolor{cyan}{Y}\right)$

Para encontrar a função característica $\varphi_{\textcolor{cyan}{Y}}(t)$ de uma variável aleatória $\textcolor{cyan}{Y}=p(\textcolor{cyan}{X})$, onde $\textcolor{cyan}{X}$ é uma variável aleatória com função característica conhecida $\varphi_{\textcolor{cyan}{X}}(t)$ e $p$ é uma função tal que sua inversa é $q$, isto é, $\textcolor{cyan}{X} = q(\textcolor{cyan}{Y})$, podemos usar o conceito de transformação de variáveis em funções características.

A função característica de uma variável aleatória $\textcolor{cyan}{Y}$ é definida por:

$$
\varphi_{\textcolor{cyan}{Y}}(t) = \mathbb{E}\left[e^{it\textcolor{cyan}{Y}}\right]
$$

Substituindo $\textcolor{cyan}{Y}$ por $p(\textcolor{cyan}{X})$, temos:

$$
\varphi_{\textcolor{cyan}{Y}}(t) = \mathbb{E}\left[e^{itp(\textcolor{cyan}{X})}\right]
$$

Agora, se a transformação $p(\textcolor{cyan}{X})$ é tal que podemos expressar $\textcolor{cyan}{X}$ como $q(\textcolor{cyan}{Y})$, então podemos reescrever a expectativa em termos da distribuição de $\textcolor{cyan}{X}$. No entanto, a forma exata desta reescrita depende da natureza da função $p$ e de sua inversa $q$. 

Se $p$ for uma transformação linear, por exemplo, $p(\textcolor{cyan}{X}) = a\textcolor{cyan}{X} + b$, então a função característica pode ser encontrada mais diretamente. Mas para funções não lineares ou mais complexas, pode ser necessário usar métodos mais avançados, como integração ou até mesmo técnicas numéricas, dependendo da forma de $p$ e da distribuição de $\textcolor{cyan}{X}$. 

Portanto, sem informações específicas sobre a forma da função $p$ e da distribuição de $\textcolor{cyan}{X}$, não é possível fornecer uma fórmula exata para $\varphi_{\textcolor{cyan}{Y}}(t)$.



$\textcolor{lightgreen}{ X}$ com densidade $\displaystyle \textcolor{lightgreen}{\rho }\textcolor{lightgreen}{_{X}}$, $\displaystyle \textcolor{cyan}{p}(\textcolor{lightgreen}{x})$ suave e bijetora (com inversa $\displaystyle \textcolor{lightgreen}{q}$), então podemos achar $\displaystyle \textcolor{cyan}{\rho }\textcolor{cyan}{_{Y}}$ de forma que $\displaystyle \textcolor{cyan}{Y} =\textcolor{cyan}{p}(\textcolor{lightgreen}{X})$

  

$$\displaystyle \begin{aligned}

\textcolor{cyan}{p}(\textcolor{lightgreen}{x}) \ \text{é decrescente} \ \Rightarrow \rho _{\textcolor{cyan}{Y}} & =\cfrac{d}{d\textcolor{cyan}{y}}{P}(\textcolor{cyan}{Y} \leq \textcolor{cyan}{y})\\

 & =\cfrac{d}{d\textcolor{cyan}{y}}{P}(\textcolor{cyan}{p}(\textcolor{lightgreen}{X}) \leq \textcolor{cyan}{y})\\

 & =\cfrac{d}{d\textcolor{cyan}{y}}{P}\left(\textcolor{lightgreen}{X} \leq \textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right) =\cfrac{d}{d\textcolor{cyan}{y}}( 1-{P}(\textcolor{lightgreen}{X} \leq \textcolor{lightgreen}{x}))\\
 
 & =\underbrace{\cfrac{d}{d\textcolor{cyan}{y}}

  

1}_{0} -\cfrac{d}{d\textcolor{cyan}{y}}{P}(\textcolor{lightgreen}{X} \leq \textcolor{lightgreen}{x})\\

 & =-\cfrac{d}{d\textcolor{cyan}{y}}{P}\left(\textcolor{lightgreen}{X} \leq \textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right)\\

 & =-\underbrace{\cfrac{d}{d\textcolor{lightgreen}{q}(\textcolor{cyan}{y})}{P}\left(\textcolor{lightgreen}{X} \leq \textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right)}_{\rho _{\textcolor{lightgreen}{X}}\left(\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right)} \cdot \cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\\

 & =-\rho_\textcolor{lightgreen}{X}\left(
	 \textcolor{lightgreen}{q}(\textcolor{cyan}{y})
 \right)\cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y})
\end{aligned}$$

$$\displaystyle \begin{aligned}

\textcolor{cyan}{p}(\textcolor{lightgreen}{x}) \ \text{é crescente} \ \Rightarrow \rho _{\textcolor{cyan}{Y}} & =\cfrac{d}{d\textcolor{cyan}{y}}{P}(\textcolor{cyan}{Y} \leq \textcolor{cyan}{y})\\

 & =\cfrac{d}{d\textcolor{cyan}{y}}{P}(\textcolor{cyan}{p}(\textcolor{lightgreen}{X}) \leq \textcolor{cyan}{y})\\

 & =\cfrac{d}{d\textcolor{cyan}{y}}{P}\left(\textcolor{lightgreen}{X} \leq \textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right)\\

 & =\cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y}) \cdot \underbrace{\cfrac{d}{d\textcolor{lightgreen}{q}(\textcolor{cyan}{y})}{P}\left(\textcolor{lightgreen}{X} \leq \textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right)}_{\rho _{\textcolor{lightgreen}{X}}\left(\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right)}\\

 & =\cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y}) \cdot \textcolor{lightgreen}{\rho }\textcolor{lightgreen}{_{X}}\left(\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right)

\end{aligned}$$
Se $\displaystyle \textcolor{cyan}{p}(\textcolor{lightgreen}{x}) \ \text{é decrescente}$, $\displaystyle \cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y}) < 0$.
Então $\displaystyle \cfrac{\left| \cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right| }{\cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y})} =-1$

  

Se $\displaystyle \textcolor{cyan}{p}(\textcolor{lightgreen}{x}) \ \text{é crescente}$, $\displaystyle \cfrac{\left| \cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right| }{\cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y})} =1$

  

Então, no geral temos $\displaystyle \rho _{\textcolor{cyan}{Y}} =\cfrac{\left| \cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right| }{\bcancel{\cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y})}}\textcolor{lightgreen}{\rho }\textcolor{lightgreen}{_{X}}\left(\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right)\bcancel{\cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y})} =\left| \cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right| \textcolor{lightgreen}{\rho }\textcolor{lightgreen}{_{X}}\left(\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right)$

$$\begin{equation*}

\rho_\textcolor{cyan}{{Y}}(\textcolor{cyan}{y}) =
\begin{cases}
\rho_\textcolor{lightgreen}{{X}}\left(
	\textcolor{lightgreen}{q}(\textcolor{cyan}{y})
\right)\left|
	\cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right|  & ;\text{se} \ \exists \textcolor{lightgreen}{x} :\textcolor{cyan}{p}(\textcolor{lightgreen}{x}) =\textcolor{cyan}{y}\\

	0 & ;\text{caso contrário}

\end{cases}

\end{equation*}$$

  Claro, vamos reescrever os passos A a G no estilo solicitado:

**Ponto de Partida**:
   - Seja $\textcolor{lightgreen}{X}$ uma variável aleatória com função densidade $\rho_{\textcolor{lightgreen}{X}}$, e $\textcolor{cyan}{p}(\textcolor{lightgreen}{x})$ uma função suave e bijetora (com inversa $\textcolor{lightgreen}{q}$). Queremos achar $\rho_{\textcolor{cyan}{Y}}$ de forma que $\textcolor{cyan}{Y} = \textcolor{cyan}{p}(\textcolor{lightgreen}{X})$.

**Definição da Função Característica de $\textcolor{cyan}{Y}$**:
   - A função característica de $\textcolor{cyan}{Y}$ é definida por:
     $\varphi_{\textcolor{cyan}{Y}}(\textcolor{yellow}{t}) = \mathbb{E}\left[ e^{\textcolor{yellow}{t}\textcolor{cyan}{Y}\sqrt{-1}}\right]$
   - Em termos de integral, isso se traduz em:
     $\varphi_{\textcolor{cyan}{Y}}(\textcolor{yellow}{t}) = \int \rho_{\textcolor{cyan}{Y}}(\textcolor{magenta}{\omega}) e^{\textcolor{yellow}{t}\textcolor{magenta}{\omega}\sqrt{-1}} d\textcolor{magenta}{\omega}$

**Transformação de Variáveis**:
   - Usamos a transformação $\textcolor{cyan}{Y} = \textcolor{cyan}{p}(\textcolor{lightgreen}{X})$ e sua inversa $\textcolor{lightgreen}{X} = \textcolor{lightgreen}{q}(\textcolor{cyan}{Y})$ para transformar a variável na função densidade.

**Função Densidade de $\textcolor{cyan}{Y}$ em Termos de $\textcolor{lightgreen}{X}$**:
   - Se a transformação é bijetora, a densidade de $\textcolor{cyan}{Y}$ é:
 $$\rho_{\textcolor{cyan}{Y}}(\textcolor{cyan}{y}) = \rho_{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{q}(\textcolor{cyan}{y})) \left| \frac{d}{d\textcolor{cyan}{y}} \textcolor{lightgreen}{q}(\textcolor{cyan}{y}) \right|$$

**Expressão da Função Densidade de $\textcolor{lightgreen}{X}$ em Termos de $\varphi_{\textcolor{lightgreen}{X}}$**:
   - A função densidade de $\textcolor{lightgreen}{X}$ pode ser expressa usando a transformada de Fourier inversa da sua função característica:
$$\displaystyle \rho_{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{x}) = \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{-\textcolor{pink}{\tau}\textcolor{lightgreen}{x}\sqrt{-1}} \varphi_{\textcolor{lightgreen}{X}}(\textcolor{pink}{\tau}) d\textcolor{pink}{\tau}$$
   - Substituímos isso na expressão de $\varphi_{\textcolor{cyan}{Y}}(\textcolor{yellow}{t})$, obtendo:
$$\varphi_{\textcolor{cyan}{Y}}(\textcolor{yellow}{t}) = \int
\left(\displaystyle \rho_{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{q}(\textcolor{magenta}{\omega})) = \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{-\textcolor{pink}{\tau}\textcolor{lightgreen}{q}(\textcolor{magenta}{\omega})\sqrt{-1}} \varphi_{\textcolor{lightgreen}{X}}(\textcolor{pink}{\tau}) d\textcolor{pink}{\tau}\right)\left| \frac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{magenta}{\omega}) \right|e^{\textcolor{yellow}{t}\textcolor{magenta}{\omega}\sqrt{-1}} d\textcolor{magenta}{\omega}$$
   - Agora movemos tudo para a integral mais interna e trocar os limites de integração

$$\varphi_{\textcolor{cyan}{Y}}(\textcolor{yellow}{t}) = \cfrac{1}{2\pi} \int_{-\infty}^{\infty} \int_{-\infty}^{\infty}\varphi_{\textcolor{lightgreen}{X}}(\textcolor{pink}{\tau})\left| \frac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{magenta}{\omega}) \right| e^{\left(\textcolor{yellow}{t}\textcolor{magenta}{\omega}-\textcolor{pink}{\tau}\textcolor{lightgreen}{q}(\textcolor{magenta}{\omega})\right)\sqrt{-1}} d\textcolor{magenta}{\omega}d\textcolor{pink}{\tau}$$



**Substituição de Variáveis**:
   - Substituímos $\textcolor{lightgreen}{u} = \textcolor{lightgreen}{q}(\textcolor{pink}{\tau})$ e $\textcolor{pink}{\tau} = \textcolor{cyan}{p}(\textcolor{lightgreen}{u})$, com o diferencial $d\textcolor{pink}{\tau} = \frac{d\textcolor{cyan}{p}(\textcolor{lightgreen}{u})}{d\textcolor{lightgreen}{u}} d\textcolor{lightgreen}{u}$.
   - A expressão resultante é: $\varphi_{\textcolor{cyan}{Y}}(\textcolor{yellow}{t}) = \int_{-\infty}^{\infty} e^{i\textcolor{yellow}{t}\textcolor{cyan}{p}(\textcolor{lightgreen}{u})} \varphi_{\textcolor{lightgreen}{X}}(\textcolor{cyan}{p}(\textcolor{lightgreen}{u})) \left| \frac{d\textcolor{cyan}{p}(\textcolor{lightgreen}{u})}{d\textcolor{lightgreen}{u}} \right| d\textcolor{lightgreen}{u}$.

**G. Consideração da Função Delta de Dirac**:
   - Podemos considerar o uso da função delta de Dirac para simplificar a expressão, dependendo das propriedades de $\textcolor{cyan}{p}$ e $\textcolor{lightgreen}{q}$.

Este raciocínio destaca a complexidade da relação entre as funções características e densidades de variáveis aleatórias transformadas, especialmente em casos de transformações não lineares ou inversões.




































## Função Geratriz de Momentos

  

Sendo $\displaystyle X$ uma variável aleatória. A Função geratriz de momentos de $\displaystyle X$: $\displaystyle G_{X}( t) \ =\ Ee^{Xt}$

$$\displaystyle \rho _{Y}( g) =\rho _{X}$$

  

### Propriedades:
1. $\displaystyle G_X( 0) =Ee^{0\cdot X} =Ee⁰=E( 1) =1$
2. $\displaystyle X,Y\ \text{independentes} \ \Rightarrow G_{X+Y} =G_{X}( t) \cdot G_{Y}( t)$ porque
  $\displaystyle G_{X+Y}( t) =Ee^{t( X+Y)} =E\left[ e^{tX} e^{tY}\right] =Ee^{tX} \cdot Ee^{tY} =G_{X}( t) G_{Y}( t)$
3. $\displaystyle EX^{n} =\left(\left(\cfrac{d}{dt}\right)^{n} G\right)(0)$
  
  
  

### Função Característica

  

$$\displaystyle \Phi_{\textcolor{lightgreen}{X}}(\textcolor{yellow}{t}) 
=\mathbb{E} \left[e^{\textcolor{yellow}{t}\textcolor{lightgreen}{X}\sqrt{-1}} \right]

=\int \rho_{\textcolor{lightgreen}{X}}(\omega) \cdot e^{\textcolor{yellow}{t}\omega \sqrt{-1}} d\omega $$

  

### Propriedades
  

1. $\displaystyle \rho _{X+Y}( t) =\rho _{X}( t) \cdot \rho _{Y}( t)$
2. $\displaystyle \rho _{X}( -it) =G_{X}( t)$
3. $\displaystyle \rho _{X}( 0) =0$
4. $\displaystyle \rho _{X}( -t) =\overline{\rho _{X}( t)}$


$$\begin{align*}
\rho \textcolor{cyan}{_{\textcolor{cyan}{Y}}}(\textcolor{yellow}{t}) & =\mathbb{E}\left[ e^{\textcolor{yellow}{t}\textcolor{cyan}{Y}\sqrt{-1}}\right]\\
 & =\int \rho _{\textcolor{cyan}{Y}}(\textcolor{pink}{\omega }) \cdot e^{\textcolor{yellow}{t}\textcolor{pink}{\omega }\sqrt{-1}} d\textcolor{pink}{\omega }\\
 & =\int \rho _{\textcolor{cyan}{p}(\textcolor{lightgreen}{X})}(\textcolor{pink}{\omega }) \cdot e^{\textcolor{yellow}{t}\textcolor{pink}{\omega }\sqrt{-1}} d\textcolor{pink}{\omega }\\
 & =\int \rho _{\textcolor{cyan}{p}(\textcolor{lightgreen}{X})}(\textcolor{pink}{\omega }) \cdot e^{\textcolor{yellow}{t}\textcolor{pink}{\omega }\sqrt{-1}} d\textcolor{pink}{\omega }\\
 & =\int \rho _{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{q}(\textcolor{pink}{\omega })) e^{t\textcolor{pink}{\omega }\sqrt{-1}}\left| \cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{pink}{\omega })\right| d\textcolor{pink}{\omega }
\end{align*}$$



Para calcular a função característica da variável aleatória $\textcolor{cyan}{Y}$, que é uma função da variável aleatória $\textcolor{lightgreen}{X}$, você começou com a definição padrão da função característica e fez uma substituição utilizando a transformação da densidade de probabilidade sob uma mudança de variável. Vamos continuar o cálculo a partir de onde você parou:

Dada a fórmula da função característica $\upvarphi \textcolor{cyan}{_{\textcolor{cyan}{Y}}}(\textcolor{yellow}{t})$, já temos a expressão:

$$
\upvarphi \textcolor{cyan}{_{\textcolor{cyan}{Y}}}(\textcolor{yellow}{t}) = \int \rho _{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{q}(\textcolor{pink}{\omega })) e^{\textcolor{yellow}{t}\textcolor{pink}{\omega }\sqrt{-1}}\left| \cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{pink}{\omega })\right| d\textcolor{pink}{\omega }
$$

Agora, vamos integrar essa expressão, considerando que $\textcolor{lightgreen}{q}(\textcolor{pink}{\omega })$ é a inversa de $\textcolor{cyan}{p}(\textcolor{lightgreen}{x})$ e $\textcolor{magenta}{\omega} = \textcolor{cyan}{p}(\textcolor{lightgreen}{x}) = \textcolor{cyan}{y}$. Portanto, podemos substituir $\textcolor{magenta}{\omega}$ por $\textcolor{cyan}{y}$ e integrar em relação a $\textcolor{cyan}{y}$:

$$
\upvarphi \textcolor{cyan}{_{\textcolor{cyan}{Y}}}(\textcolor{yellow}{t}) = \int \rho _{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{q}(\textcolor{cyan}{y})) e^{\textcolor{yellow}{t}\textcolor{cyan}{p}(\textcolor{lightgreen}{x})\sqrt{-1}}\left| \cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y})\right| d\textcolor{cyan}{y}
$$

Agora, substituindo $\rho _{\textcolor{cyan}{Y}}(\textcolor{cyan}{y})$ pela expressão que você forneceu, temos:

$$
\upvarphi \textcolor{cyan}{_{\textcolor{cyan}{Y}}}(\textcolor{yellow}{t}) = \int_{-\infty}^{\infty} \rho _{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{q}(\textcolor{cyan}{y})) e^{\textcolor{yellow}{t}\textcolor{cyan}{y}\sqrt{-1}}\left| \cfrac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y})\right| d\textcolor{cyan}{y}
$$

Esta é a expressão final da função característica da variável $\textcolor{cyan}{Y}$ em termos da densidade de probabilidade de $\textcolor{lightgreen}{X}$ e da transformação bijetora $\textcolor{cyan}{p}$. Essa fórmula é válida para qualquer função bijetora suave $\textcolor{cyan}{p}$ e sua inversa $\textcolor{lightgreen}{q}$, desde que as condições necessárias para a existência e unicidade da inversa sejam satisfeitas.

Para aplicar a transformada de Fourier à função de densidade de probabilidade (FDP) $\rho_{\textcolor{cyan}{Y}}(\textcolor{cyan}{y})$ da variável transformada $\textcolor{cyan}{Y}$, usaremos a definição padrão da transformada de Fourier. A função característica, que é a transformada de Fourier da FDP, é dada por:

$$
\Phi_{\textcolor{cyan}{Y}}(\textcolor{yellow}{t}) = \int_{-\infty}^{\infty} e^{\textcolor{yellow}{t}\textcolor{cyan}{y}\sqrt{-1}} \rho_{\textcolor{cyan}{Y}}(\textcolor{cyan}{y}) d\textcolor{cyan}{y}.
$$

Substituindo a expressão de $\rho_{\textcolor{cyan}{Y}}(\textcolor{cyan}{y})$ na integral, temos:

$$
\Phi_{\textcolor{cyan}{Y}}(\textcolor{yellow}{t}) = \int_{-\infty}^{\infty} e^{\textcolor{yellow}{t}\textcolor{cyan}{y}\sqrt{-1}} 
\begin{cases}
	\rho_{\textcolor{lightgreen}{X}}\left(\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right)\left|\cfrac{d}{d\textcolor{cyan}{y}}\textcolor{lightgreen}{q}(\textcolor{cyan}{y})\right| & ;\text{se} \ \exists \textcolor{lightgreen}{x} :\textcolor{cyan}{p}(\textcolor{lightgreen}{x}) =\textcolor{cyan}{y},\\
	0 & ;\text{caso contrário}
\end{cases}
d\textcolor{cyan}{y}.
$$

Essa expressão pode ser simplificada ao observar que a integral de um produto de uma função complexa exponencial com zero é zero. Portanto, a integral só precisa ser avaliada sobre o intervalo onde $\textcolor{lightgreen}{x}$ existe tal que $\textcolor{cyan}{p}(\textcolor{lightgreen}{x}) = \textcolor{cyan}{y}$. A expressão simplificada é:

A expressão da função característica $\Phi_{\textcolor{cyan}{Y}}(\textcolor{yellow}{t})$ da variável aleatória $\textcolor{cyan}{Y}$, em termos da transformada de Fourier da sua função densidade de probabilidade $\rho_{\textcolor{cyan}{Y}}(\textcolor{cyan}{y})$, é dada por:

$$\displaystyle
\Phi_{\textcolor{cyan}{Y}}(\textcolor{yellow}{t}) = \int_{-\infty}^{\infty} e^{\textcolor{yellow}{t}\textcolor{cyan}{y}\sqrt{-1}} \rho_{\textcolor{lightgreen}{X}}(\textcolor{lightgreen}{q}(\textcolor{cyan}{y})) \left| \frac{d\textcolor{lightgreen}{q}}{d\textcolor{cyan}{y}}(\textcolor{cyan}{y}) \right| d\textcolor{cyan}{y}.
$$

Esta integral representa a função característica de $\textcolor{cyan}{Y}$, que é uma transformação da variável aleatória $\textcolor{lightgreen}{X}$ através da função bijetora $\textcolor{cyan}{p}$, com $\textcolor{lightgreen}{q}$ sendo sua inversa. A solução exata desta integral dependerá das funções específicas $\rho_{\textcolor{lightgreen}{X}}$ e $\textcolor{lightgreen}{q}$.

