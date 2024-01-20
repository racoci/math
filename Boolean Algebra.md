
Elevating boolean algebra: 
$$
\begin{equation*}
\begin{array}{ c r c c c c }
S\ a\ P & \forall x: & S( x)\rightarrow P( x) & \Rightarrow  &  & S\land \neg P=\top \\
S\ e\ P & \neg \exists x: & S( x)\rightarrow P( x) & \Rightarrow  &  & S\land P=\top \\
S\ i\ P & \exists x: & S( x)\rightarrow P( x) & \Rightarrow  &  & S\land P\neq \top \\
S\ o\ P & \exists x: & S( x)\rightarrow \neg P( x) & \Rightarrow  &  & S\land \neg P\neq \top 
\end{array}
\end{equation*}
$$

Seja $\displaystyle f:\{\top ,\bot \}^{n}\rightarrow \{\top ,\bot \}^{n} =( x_{1} ,\cdots x_{n}) \mapsto ( y_{1} ,\cdots ,y_{m})$, $\displaystyle x_{\alpha } ,y_{\beta } \in \{\top ,\bot \} ,\ \alpha \in \{1,\cdots ,m\} ,\ \beta \in \{1,\cdots n\}$
Podemos escrever a função $\displaystyle f$ como $\displaystyle f_{1} ,\cdots f_{n}$ representando o valor de cada saída como uma função $\displaystyle f_{\beta } :\{\top ,\bot \}^{m}\rightarrow \{\top ,\bot \} =( x_{1} ,\cdots x_{m}) \mapsto y_{\beta } ,\forall \beta \in \{1,\cdots n\}$
Assim $\displaystyle y_{\beta } =f_{\beta }( x_{1} ,\cdots ,x_{n}) =\bigwedge _{\ell =0}^{2^{n}}\left( b_{\ell ,\beta } \leftrightarrow \bigvee _{\alpha =0}^{n}( a_{\ell ,\alpha } \leftrightarrow x_{\alpha })\right)$
Onde $\displaystyle a_{\ell ,\alpha }$ representa o valor verdade da entrada $\displaystyle x_{\alpha }$ na linha $\displaystyle \ell$ da tabela verdade. E $\displaystyle b_{\ell ,\beta } \overset{\text{def}}{=} f_{b}( a_{\ell ,1} ,\cdots ,a_{\ell ,n})$ é o valor verdade da saída $\displaystyle y_{\beta }$ na tabela verdade para a linha $\displaystyle \ell$
$$
\begin{equation*}
\begin{array}{ c c c c c|c c c c c }
x_{1} & \cdots  & x_{\alpha } & \cdots  & x_{n} & y_{1} & \cdots  & y_{\beta } & \cdots  & y_{m}\\
\hline
a_{1,1} & \cdots  & a_{1,\alpha } & \cdots  & a_{1,n} & b_{1,1} & \cdots  & b_{1,1} & \cdots  & b_{1,m}\\
\vdots  & \ddots  & \vdots  & \ddots  & \vdots  & \vdots  & \ddots  & \vdots  & \ddots  & \vdots \\
a_{\ell ,1} & \cdots  & a_{\ell ,\alpha } & \cdots  & a_{\ell ,n} & b_{\ell ,1} & \cdots  & b_{\ell ,\beta } & \cdots  & b_{\ell ,m}\\
\vdots  & \ddots  & \vdots  & \ddots  & \vdots  & \vdots  & \ddots  & \vdots  & \ddots  & \vdots \\
a_{2^{n} ,1} & \cdots  & a_{2^{n} \alpha } & \cdots  & a_{\ell ,n} & b_{2^{n} ,1} & \cdots  & b_{2^{n} ,\beta } & \cdots  & b_{2^{n} ,m}
\end{array}
\end{equation*}
$$

$$\displaystyle  \begin{array}{{>{\displaystyle}l}}
a\land b=\neg \left( a\rightarrow \neg b\right)\\
a\lor b=( \neg a)\rightarrow b\\
a\leftrightarrow b=( a\land b) \lor ( \neg a\land \neg b)
\end{array}$$


Essa noção de avaliar o valor de uma função por força bruta pode ser generalizado para qualquer função finita:
Sejam $\displaystyle A,B$ conjuntos de cardinalidade finita. Dada uma função $\displaystyle f:A\rightarrow B$. 
Se fizermos uma tabela com todas as possíveis entradas de $\displaystyle a\in A$ e o correspondente valor $\displaystyle f( a)$. Podemos definir $\displaystyle f( x) =\sum _{a\in A} \delta _{x}^{a} \cdot f( a) ,\forall f\in B^{A}$ onde 

$$\displaystyle \delta _{x}^{a} \overset{\text{def}}{=} \begin{cases}
1 & \text{se} \ x=a\\
0 & \text{se} \ x\neq a
\end{cases}$$ 

Essa noção de avaliar o valor de uma função por força bruta pode ser generalizado para qualquer função finita:

Sejam $\displaystyle A,B$ conjuntos de cardinalidade finita. Dada uma função $\displaystyle f:A\rightarrow B$. 

Se fizermos uma tabela com todas as possíveis entradas de $\displaystyle a\in A$ e o correspondente valor $\displaystyle f( a)$. Podemos definir $\displaystyle f( x) =\sum _{a\in A} \delta _{x}^{a} \cdot f( a) ,\forall f\in B^{A}$ onde $$\displaystyle \delta _{x}^{a} \eqdef \begin{cases}
1 & \text{se} \ x=a\\
0 & \text{se} \ x\neq a
\end{cases}$$ 


