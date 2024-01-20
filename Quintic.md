$\displaystyle x^{2} +c_{1} x+c_{0} =\left( x+\cfrac{c_{1}}{2} +\sqrt{\left(\cfrac{c_{1}}{2}\right)^{2} -c_{0}}\right)\left( x+\cfrac{c_{1}}{2} -\sqrt{\left(\cfrac{c_{1}}{2}\right)^{2} -c_{0}}\right)$



$\displaystyle \begin{aligned}
0 & =x^{n+1} +\alpha _{n} x^{n} +\cdots +\alpha _{2} x^{2} +\alpha _{1} x+\alpha _{0} =( x-t)\left( x^{n} +\beta _{n-1} x^{n-1} +\cdots +\beta _{1} x+\beta _{0}\right)\\
 & =x^{n+1} +( \beta _{n-1} -t) x^{n} +( \beta _{n-2} -\beta _{n-1} t) x^{n-1} +\cdots +( \beta _{0} -\beta _{1} t) x-\beta _{0} t\\
 & \begin{aligned}
\alpha _{n} & =\beta _{n-1} -t\\
\alpha _{n-1} & =\beta _{n-2} -\beta _{n-1} t\\
 & \vdots \\
\alpha _{1} & =\beta _{0} -\beta _{1} t\\
\alpha _{0} = & -\beta _{0} t
\end{aligned} \Rightarrow \begin{aligned}
\alpha _{n} +t & =\beta _{n-1}\\
\alpha _{n-1} +t\beta _{n-1}{} & =\beta _{n-2}\\
 & \vdots \\
\alpha _{1} +\beta _{1} t & =\beta _{0}\\
\alpha _{0} +\beta _{0} t= & 0
\end{aligned} \Rightarrow \begin{aligned}
\alpha _{n} +t & =\beta _{n-1}\\
\alpha _{n-1} +\alpha _{n} t+t^{2}{} & =\beta _{n-2}\\
 & \vdots \\
\alpha _{1} +\alpha _{2} t+\cdots +\alpha _{n} +t^{n} & =\beta _{0}\\
\alpha _{0} +\beta _{0} t= & 0
\end{aligned}
\end{aligned}$



For example, for $\displaystyle n=4$

$\displaystyle  \begin{array}{{>{\displaystyle}l}}
0=x^{5} +\alpha _{4} x^{4} +\alpha _{3} x^{3} +\alpha _{2} x^{2} +\alpha _{1} x+\alpha _{0} =( x-t)\left( x^{4} +\beta _{3} x^{3} +\beta _{2} x^{2} +\beta _{1} x+\beta _{0}\right)\\
=x^{5} +( \beta _{3} -t) x^{4} +( \beta _{2} -t\beta _{3}) x^{3} +( \beta _{1} -t\beta _{2}) x^{2} +( \beta _{0} -t\beta _{1}) x-t\beta _{0}\\
\begin{aligned}
\alpha _{4} & =\beta _{3} -t\\
\alpha _{3} & =\beta _{2} -t\beta _{3}\\
\alpha _{2} & =\beta _{1} -t\beta _{2}\\
\alpha _{1} & =\beta _{0} -t\beta _{1}\\
\alpha _{0} & =-t\beta _{0}
\end{aligned} \Rightarrow \begin{aligned}
\alpha _{4} +t & =\beta _{3}\\
\alpha _{3} +\beta _{3} t & =\beta _{2}\\
\alpha _{2} +\beta _{2} t & =\beta _{1}\\
\alpha _{1} +\beta _{1} t & =\beta _{0}\\
\alpha _{0} +\beta _{0} t & =0
\end{aligned} \Rightarrow \begin{aligned}
\alpha _{4} +t & =\beta _{3}\\
\alpha _{3} +\alpha _{4} t+t^{2} & =\beta _{2}\\
\alpha _{2} +\alpha _{3} t+\beta _{3} t^{2} & =\beta _{1}\\
\alpha _{1} +\alpha _{2} t+\beta _{2} t^{2} & =\beta _{0}\\
\alpha _{0} +\alpha _{1} t+\beta _{1} t^{2} & =0
\end{aligned} \Rightarrow \begin{aligned}
\alpha _{4} -\beta _{3} +t & =0\\
\alpha _{3} -\beta _{2} +\alpha _{4} t+t^{2} & =0\\
\alpha _{2} -\beta _{1} +\alpha _{3} t+\beta _{3} t^{2} & =0\\
\alpha _{1} -\beta _{0} +\alpha _{2} t+\beta _{2} t^{2} & =0\\
\alpha _{0} +\alpha _{1} t+\beta _{1} t^{2} & =0
\end{aligned}\\
\Rightarrow \begin{aligned}
t & =\beta _{3} -\alpha _{4}\\
t & =\cfrac{\alpha _{4}}{2} \pm \sqrt{\left(\cfrac{\alpha _{4}}{2}\right)^{2} -\alpha _{3} +\beta _{2}}\\
t & =\cfrac{\alpha _{3}}{2\beta _{3}} \pm \sqrt{\left(\cfrac{\alpha _{3}}{2\beta _{3}}\right)^{2} +\cfrac{\beta _{1} -\alpha _{2}}{4\beta _{3}^{2}}}\\
t & =\cfrac{\alpha _{2}}{2\beta _{2}} \pm \sqrt{\left(\cfrac{\alpha _{2}}{2\beta _{2}}\right)^{2} -\cfrac{\alpha _{1} -\beta _{0}}{4\beta _{2}^{2}}}\\
t & =\cfrac{\alpha _{1}}{2\beta _{1}} \pm \sqrt{\left(\cfrac{\alpha _{1}}{2\beta _{1}}\right)^{2} -\cfrac{\alpha _{0}}{4\beta _{1}^{2}}}
\end{aligned}
\end{array}$



$\displaystyle ( a+b)^{n} =\sum _{k=0}^{n}\begin{pmatrix}
n\\
k
\end{pmatrix} a^{k} b^{n-k} =\sum _{\alpha +\beta =n} S_{\alpha ,\beta } a^{\alpha } b^{\beta }$

$\displaystyle \left(\sum _{k=0}^{n} x_{k}\right) =\sum _{k=\sum _{t=0}^{k} k_{t}}\begin{pmatrix}
n\\
k
\end{pmatrix}$

$\displaystyle  \begin{array}{{>{\displaystyle}l}}
\sqrt{a^{2} +b^{2}}\left(\cos \theta +\sqrt{-1}\sin \theta \right)\sqrt{c^{2} +d^{2}}\left(\cos \phi +\sqrt{-1}\sin \phi \right)\\
=\sqrt{a^{2} +b^{2}}\sqrt{c^{2} +d^{2}}\left(\cos \theta +\sqrt{-1}\sin \theta \right)\textcolor[rgb]{0.29,0.56,0.89}{\left(}\textcolor[rgb]{0.29,0.56,0.89}{\cos}\textcolor[rgb]{0.29,0.56,0.89}{\phi +}\textcolor[rgb]{0.29,0.56,0.89}{\sqrt{-1}}\textcolor[rgb]{0.29,0.56,0.89}{\sin}\textcolor[rgb]{0.29,0.56,0.89}{\phi }\textcolor[rgb]{0.29,0.56,0.89}{\right)}\\
=\sqrt{a^{2} +b^{2}}\sqrt{c^{2} +d^{2}}\left(\cos \theta \textcolor[rgb]{0.29,0.56,0.89}{\left(}\textcolor[rgb]{0.29,0.56,0.89}{\cos}\textcolor[rgb]{0.29,0.56,0.89}{\phi +}\textcolor[rgb]{0.29,0.56,0.89}{\sqrt{-1}}\textcolor[rgb]{0.29,0.56,0.89}{\sin}\textcolor[rgb]{0.29,0.56,0.89}{\phi }\textcolor[rgb]{0.29,0.56,0.89}{\right)} +\sqrt{-1}\sin \theta \textcolor[rgb]{0.29,0.56,0.89}{\left(}\textcolor[rgb]{0.29,0.56,0.89}{\cos}\textcolor[rgb]{0.29,0.56,0.89}{\phi +}\textcolor[rgb]{0.29,0.56,0.89}{\sqrt{-1}}\textcolor[rgb]{0.29,0.56,0.89}{\sin}\textcolor[rgb]{0.29,0.56,0.89}{\phi }\textcolor[rgb]{0.29,0.56,0.89}{\right)}\right)
\end{array}$

$\displaystyle  \begin{array}{{>{\displaystyle}l}}
=\sqrt{a^{2} +b^{2}}\sqrt{c^{2} +d^{2}}\left(\cos \phi \cos \theta +\sqrt{-1}\sin \phi \cos \theta +\sqrt{-1}\sin \theta \cos \phi +\sqrt{-1}\sin \theta \sqrt{-1}\sin \phi \right)\\
=\sqrt{a^{2} +b^{2}}\sqrt{c^{2} +d^{2}}\left(\cos \phi \cos \theta -\sin \theta \sin \phi +\sqrt{-1}(\sin \phi \cos \theta +\sin \theta \cos \phi )\right)\\
=\sqrt{a^{2} +b^{2}}\sqrt{c^{2} +d^{2}}\left(\cos( \phi +\theta ) +\sqrt{-1}\sin( \phi +\theta )\right)
\end{array}$

$\displaystyle \left(\cos \theta +\sqrt{-1}\sin \theta \right)^{2} =\left(\cos \theta +\sqrt{-1}\sin \theta \right)\left(\cos \theta +\sqrt{-1}\sin \theta \right) =\left(\cos 2\theta +\sqrt{-1}\sin 2\theta \right)$

$\displaystyle \left(\cos \theta +\sqrt{-1}\sin \theta \right)^{n} =\left(\cos n\theta +\sqrt{-1}\sin n\theta \right)$

$\displaystyle \left(\cos \theta +\sin \theta \sqrt{-1}\right)^{n} =\cos n\theta +\sqrt{-1}\sin n\theta =\sum _{k=0}^{n}( -1)^{k/2}\begin{pmatrix}
n\\
k
\end{pmatrix}\cos^{n-k} \theta \cdotp \sin^{k} \theta $



$$\displaystyle  \begin{array}{{>{\displaystyle}l}}
\cos 5\theta +\sqrt{-1}\sin 5\theta =\sum _{k=0}^{5}( -1)^{k/2}\begin{pmatrix}
5\\
k
\end{pmatrix}\cos^{5-k} \theta \cdotp \sin^{k} \theta \\
=( -1)^{0/2}\begin{pmatrix}
5\\
k
\end{pmatrix}\cos^{5-0} \theta \cdotp \sin^{0} \theta \\
+( -1)^{1/2}\begin{pmatrix}
5\\
k
\end{pmatrix}\cos^{5-1} \theta \cdotp \sin^{1} \theta \\
+( -1)^{2/2}\begin{pmatrix}
5\\
k
\end{pmatrix}\cos^{5-2} \theta \cdotp \sin^{2} \theta \\
+( -1)^{3/2}\begin{pmatrix}
5\\
k
\end{pmatrix}\cos^{5-3} \theta \cdotp \sin^{3} \theta \\
+( -1)^{4/2}\begin{pmatrix}
5\\
k
\end{pmatrix}\cos^{5-4} \theta \cdotp \sin^{4} \theta \\
+( -1)^{5/2}\begin{pmatrix}
5\\
k
\end{pmatrix}\cos^{5-5} \theta \cdotp \sin^{5} \theta \\
=\cos^{5} \theta \\
+( -1)^{1/2} 5\cos^{4} \theta \cdotp \sin \theta \\
-10\cos^{5-2} \theta \cdotp \sin^{2} \theta \\
-1( -1)^{1/2} 10\cos^{2} \theta \cdotp \sin^{3} \theta \\
+5\cos \theta \cdotp \sin^{4} \theta \\
+( -1)^{1/2}\sin^{5} \theta +5\cos \theta \cdotp \sin^{4} \theta \\
=\cos^{5} \theta -10\cos^{5-2} \theta \cdotp \sin^{2} \theta \\
+\left( 5\cos^{4} \theta \cdotp \sin \theta -10\cos^{2} \theta \cdotp \sin^{3} \theta +\sin^{5} \theta \right)\sqrt{-1}\\
=\cos 5\theta +\sqrt{-1}\sin 5\theta \\
\\
$$
$$
\begin{pmatrix}
\cos^{5} \theta -10\cos^{3} \theta \cdotp \sin^{2} \theta  & = & \cos 5\theta \\
5\cos^{4} \theta \cdotp \sin \theta -10\cos^{2} \theta \cdotp \sin^{3} \theta +\sin^{5} \theta  & = & \sin 5\theta 
\end{pmatrix}
\end{array}$$



$$\displaystyle  \begin{array}{{>{\displaystyle}l}}
( x-x_{\textcolor[rgb]{0.82,0.01,0.11}{1}})( x-x_{\textcolor[rgb]{0.55,0.34,0.16}{2}})( x-x_{\textcolor[rgb]{0.25,0.46,0.02}{3}})( x-x_{\textcolor[rgb]{0.29,0.56,0.89}{4}})( x-x_{\textcolor[rgb]{0.56,0.07,1}{5}}) =x^{5}\\
-( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.56,0.07,1}{5}}) \cdot x^{4}\\
+( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} +x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.56,0.07,1}{5}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.56,0.07,1}{5}} +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.56,0.07,1}{5}} +x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}}) \cdot x^{3}\\
-( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.56,0.07,1}{5}} +x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.56,0.07,1}{5}} +x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.56,0.07,1}{5}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}} +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}}) \ x^{2}\\
+( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.56,0.07,1}{5}} +x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}} +x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}}) \cdot x\\
-x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}}\\
=x^{5}\\
-( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.56,0.07,1}{5}}) \cdot x^{4}\\
+( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} +( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}}) x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}}) x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +x_{\textcolor[rgb]{0.29,0.56,0.89}{4}}) x_{\textcolor[rgb]{0.56,0.07,1}{5}}) \cdot x^{3}\\
-( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} +( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}}) x_{\textcolor[rgb]{0.25,0.46,0.02}{3}}) x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} +( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}}) x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}}) x_{\textcolor[rgb]{0.29,0.56,0.89}{4}}) x_{\textcolor[rgb]{0.56,0.07,1}{5}}) \cdot x^{2}\\
+( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} +( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}}) x_{\textcolor[rgb]{0.25,0.46,0.02}{3}}) x_{\textcolor[rgb]{0.29,0.56,0.89}{4}}) x_{\textcolor[rgb]{0.56,0.07,1}{5}}) \cdot x\\
-x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}}\\
=x^{5}\\
-( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.56,0.07,1}{5}}) \cdot x^{4}\\
+( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}}( x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.56,0.07,1}{5}}) +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}}( x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.56,0.07,1}{5}}) +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}}( x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.56,0.07,1}{5}}) +x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}}) \cdot x^{3}\\
-( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}}( x_{\textcolor[rgb]{0.55,0.34,0.16}{2}}( x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} +x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.56,0.07,1}{5}}) +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}}( x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.56,0.07,1}{5}}) +x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}}) +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}}( x_{\textcolor[rgb]{0.25,0.46,0.02}{3}}( x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.56,0.07,1}{5}}) +x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}}) +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}}) \ \cdot x^{2}\\
+( x_{\textcolor[rgb]{0.82,0.01,0.11}{1}}( x_{\textcolor[rgb]{0.55,0.34,0.16}{2}}( x_{\textcolor[rgb]{0.25,0.46,0.02}{3}}( x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} +x_{\textcolor[rgb]{0.56,0.07,1}{5}}) +x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}}) +x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}}) +x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}}) \cdot x\\
-x_{\textcolor[rgb]{0.82,0.01,0.11}{1}} x_{\textcolor[rgb]{0.55,0.34,0.16}{2}} x_{\textcolor[rgb]{0.25,0.46,0.02}{3}} x_{\textcolor[rgb]{0.29,0.56,0.89}{4}} x_{\textcolor[rgb]{0.56,0.07,1}{5}} \ 
\end{array}$$

$$\displaystyle \begin{bmatrix}
a_{\textcolor[rgb]{0.82,0.01,0.11}{1}}\\
a_{\textcolor[rgb]{0.55,0.34,0.16}{2}}\\
a_{\textcolor[rgb]{0.25,0.46,0.02}{3}}\\
a_{\textcolor[rgb]{0.29,0.56,0.89}{4}}\\
a_{\textcolor[rgb]{0.56,0.07,1}{5}}
\end{bmatrix} =\begin{bmatrix}
 &  &  &  & \\
 &  &  &  & \\
 &  &  &  & \\
 &  &  &  & \\
 &  &  &  & 
\end{bmatrix}\begin{bmatrix}
x_{\textcolor[rgb]{0.82,0.01,0.11}{1}}\\
x_{\textcolor[rgb]{0.55,0.34,0.16}{2}}\\
x_{\textcolor[rgb]{0.25,0.46,0.02}{3}}\\
x_{\textcolor[rgb]{0.29,0.56,0.89}{4}}\\
x_{\textcolor[rgb]{0.56,0.07,1}{5}}
\end{bmatrix}$$

$$\begin{align*}
\prod _{k=1}^{n}( x-x_{k}) & =\sum _{k=0}^{n} x^{n-k}( -1)^{k}\sum _{s_{1} =1}^{n-k+1} x_{s_{1}}\left(\sum _{s_{2} =s_{1}}^{n} x_{s_{2}}\left(\sum _{s_{3} =s_{2}}^{n} x_{s_{3}}( \dotsc )\right)\right)\\
 & =\sum _{k=0}^{n} x^{n-k}( -1)^{k}\sum _{s_{1} =1}^{n-k+1} x_{s_{1}}\left(\sum _{s_{2} =1}^{n} x_{s_{2}} 1_{s_{2} \geqslant s_{1}}\left(\sum _{s_{3} =1}^{n} x_{s_{3}} 1_{s_{3} \geqslant s_{2}}( \dotsc )\right)\right)\\
 & =\sum _{k=0}^{n} x^{n-k}( -1)^{k}\sum _{s_{1} =1}^{n-k+1}\sum _{s_{2} =1}^{n}\sum _{s_{3} =1}^{n} ...\prod _{t=1}^{k} x_{s_{t}} 1_{s_{t+1} \geqslant s_{t}}\\
 & =\sum _{k=0}^{n} x^{n-k}( -1)^{k}\sum _{s_{1} =1}^{n-k+1}\sum _{s_{2} ,s_{3} ,...s_{k} =1}^{n}\prod _{t=1}^{k} x_{s_{t}} 1_{s_{t+1} \geqslant s_{t}}\\
 & =\sum _{k=0}^{n} x^{n-k}( -1)^{k}\sum _{s=1}^{c_{n,k}}\prod _{t=1}^{k}( x_{n_{t,s,k}})
\end{align*}$$

Multi-binomial theorem

$$\displaystyle \prod _{k=1}^{n}( a_{k} +b_{k})^{m_{k}} =\sum _{n_{k} \leqslant m_{k}}^{\forall k\leqslant n}\prod _{k=1}^{n}\begin{pmatrix}
m_{k}\\
n_{k}
\end{pmatrix} a_{k}^{n_{k}} b_{k}^{m_{k} -n_{k}}$$



No nosso caso:

$$\displaystyle  \begin{array}{{>{\displaystyle}l}}
m_{k} =1,\ \\
a_{k} =x;\\
b_{k} =( -x_{k})
\end{array}$$

Substituindo:

$$\displaystyle \prod _{k=1}^{n}( x-x_{k}) =\sum _{n_{k} \leqslant 1}^{\forall k\leqslant n}\prod _{d=1}^{n}\begin{pmatrix}
1\\
n_{k}
\end{pmatrix} x^{n_{k}}( -x_{k})^{1-n_{k}} =$$

$\displaystyle  \begin{array}{{>{\displaystyle}l}}
n_{t,s,1} =s;\\
n_{t,( c_{n,t}) ,k} =t;\\
n_{t,s,k+1} =\begin{cases}
n_{t,s,k} & \text{se} \ s=1\\
 & 
\end{cases}\\
n_{t,s,n} =t;\\
\\
n_{t,s,n-1} =n_{t,s,n}
\end{array}$

$\displaystyle c_{n,k} =\begin{pmatrix}
n\\
k
\end{pmatrix}$

$\displaystyle  \begin{array}{{>{\displaystyle}l}}
c_{n,0} =c_{n,n} =c_{0,k} =1;\ \\
c_{n+1,k+1} =c_{n,k} +c_{n,k+1} ;\\
\sum _{k=0}^{n} c_{n,k} =2^{n}
\end{array}$

$\displaystyle c_{n+1,k+1} =c_{n,k} +c_{n,k+1} =\begin{cases}
\textcolor[rgb]{0.29,0.56,0.89}{c}\textcolor[rgb]{0.29,0.56,0.89}{_{n-1,k-1}} +\textcolor[rgb]{0.31,0.89,0.76}{c}\textcolor[rgb]{0.31,0.89,0.76}{_{n-1,k}} +\textcolor[rgb]{0.25,0.46,0.02}{c}\textcolor[rgb]{0.25,0.46,0.02}{_{n,k+1}} =\begin{cases}
\textcolor[rgb]{0.29,0.56,0.89}{c}\textcolor[rgb]{0.29,0.56,0.89}{_{n-2,k-2}}\textcolor[rgb]{0.29,0.56,0.89}{+c}\textcolor[rgb]{0.29,0.56,0.89}{_{n-2,k-1}} +c_{n-1,k} +c_{n,k+1}\\
c_{n-1,k-1} +\textcolor[rgb]{0.31,0.89,0.76}{c}\textcolor[rgb]{0.31,0.89,0.76}{_{n-2,k-1}}\textcolor[rgb]{0.31,0.89,0.76}{+c}\textcolor[rgb]{0.31,0.89,0.76}{_{n-2,k}} +c_{n,k+1}\\
c_{n-1,k-1} +c_{n-1,k} +\textcolor[rgb]{0.25,0.46,0.02}{c}\textcolor[rgb]{0.25,0.46,0.02}{_{n-1,k}}\textcolor[rgb]{0.25,0.46,0.02}{+c}\textcolor[rgb]{0.25,0.46,0.02}{_{n-1,k+1}}
\end{cases}\\
\textcolor[rgb]{0.29,0.56,0.89}{c}\textcolor[rgb]{0.29,0.56,0.89}{_{n,k}} +\textcolor[rgb]{0.31,0.89,0.76}{c}\textcolor[rgb]{0.31,0.89,0.76}{_{n-1,k}} +\textcolor[rgb]{0.25,0.46,0.02}{c}\textcolor[rgb]{0.25,0.46,0.02}{_{n-1,k}} =\begin{cases}
\textcolor[rgb]{0.29,0.56,0.89}{c}\textcolor[rgb]{0.29,0.56,0.89}{_{n,k}}\textcolor[rgb]{0.29,0.56,0.89}{+c}\textcolor[rgb]{0.29,0.56,0.89}{_{n-1,k}} +c_{n-1,k} +c_{n-1,k}\\
c_{n,k} +\textcolor[rgb]{0.31,0.89,0.76}{c}\textcolor[rgb]{0.31,0.89,0.76}{_{n-1,k}}\textcolor[rgb]{0.31,0.89,0.76}{+c}\textcolor[rgb]{0.31,0.89,0.76}{_{n-2,k}} +c_{n-1,k}\\
c_{n,k} +c_{n-1,k} +\textcolor[rgb]{0.25,0.46,0.02}{c}\textcolor[rgb]{0.25,0.46,0.02}{_{n-1,k}}\textcolor[rgb]{0.25,0.46,0.02}{+c}\textcolor[rgb]{0.25,0.46,0.02}{_{n-2,k}}
\end{cases}
\end{cases}$









Multi-variable polynomials:

$\displaystyle P( x_{1} ,x_{2} ,...,x_{n}) =\sum _{k=0}^{2^{n}} \alpha _{k}\prod _{t=0}^{n} x_{t}^{k_{t}}$ where $\displaystyle k_{t} =\left\lfloor k/2^{t}\right\rfloor -2\left\lfloor k/2^{t+1}\right\rfloor $ is the t-th digit of k in base 2

Example:

$\displaystyle P(\textcolor[rgb]{0.25,0.46,0.02}{x} ,\textcolor[rgb]{0.82,0.01,0.11}{y}) =\alpha _{0} +\alpha _{1}\textcolor[rgb]{0.25,0.46,0.02}{x} +\alpha _{2}\textcolor[rgb]{0.82,0.01,0.11}{y} +\alpha _{3}\textcolor[rgb]{0.25,0.46,0.02}{x}\textcolor[rgb]{0.82,0.01,0.11}{y} =\alpha _{0} +\alpha _{1}\textcolor[rgb]{0.25,0.46,0.02}{x} +( \alpha _{2} +\alpha _{3}\textcolor[rgb]{0.25,0.46,0.02}{x})\textcolor[rgb]{0.82,0.01,0.11}{y}$

In this case, if we have a factorization it'll be of the form $\displaystyle ( c_{\textcolor[rgb]{0.25,0.46,0.02}{x}} +s_{\textcolor[rgb]{0.25,0.46,0.02}{x}}\textcolor[rgb]{0.25,0.46,0.02}{x})( c\textcolor[rgb]{0.82,0.01,0.11}{_{y}} +s_{\textcolor[rgb]{0.82,0.01,0.11}{y}}\textcolor[rgb]{0.82,0.01,0.11}{y})$ because

$\displaystyle ( c_{\textcolor[rgb]{0.25,0.46,0.02}{x}} +s_{\textcolor[rgb]{0.25,0.46,0.02}{x}}\textcolor[rgb]{0.25,0.46,0.02}{x})( c\textcolor[rgb]{0.82,0.01,0.11}{_{y}} +s_{\textcolor[rgb]{0.82,0.01,0.11}{y}}\textcolor[rgb]{0.82,0.01,0.11}{y}) =( c_{\textcolor[rgb]{0.25,0.46,0.02}{x}} +s_{\textcolor[rgb]{0.25,0.46,0.02}{x}}\textcolor[rgb]{0.25,0.46,0.02}{x}) c\textcolor[rgb]{0.82,0.01,0.11}{_{y}} +( c_{\textcolor[rgb]{0.25,0.46,0.02}{x}} +s_{\textcolor[rgb]{0.25,0.46,0.02}{x}}\textcolor[rgb]{0.25,0.46,0.02}{x}) s_{\textcolor[rgb]{0.82,0.01,0.11}{y}}\textcolor[rgb]{0.82,0.01,0.11}{y} =c_{\textcolor[rgb]{0.25,0.46,0.02}{x}} c\textcolor[rgb]{0.82,0.01,0.11}{_{y}} +\textcolor[rgb]{0.25,0.46,0.02}{x} +c_{\textcolor[rgb]{0.25,0.46,0.02}{x}} s_{\textcolor[rgb]{0.82,0.01,0.11}{y}}\textcolor[rgb]{0.82,0.01,0.11}{y} +s_{\textcolor[rgb]{0.25,0.46,0.02}{x}} s_{\textcolor[rgb]{0.82,0.01,0.11}{y}}\textcolor[rgb]{0.25,0.46,0.02}{x}\textcolor[rgb]{0.82,0.01,0.11}{y}$, so we have four equations and four variables:

$\displaystyle \begin{matrix}
\alpha _{0} =c_{\textcolor[rgb]{0.25,0.46,0.02}{x}} c\textcolor[rgb]{0.82,0.01,0.11}{_{y}}\\
\alpha _{1} =s_{\textcolor[rgb]{0.25,0.46,0.02}{x}} c\textcolor[rgb]{0.82,0.01,0.11}{_{y}}\\
\alpha _{2} =c_{\textcolor[rgb]{0.25,0.46,0.02}{x}} s_{\textcolor[rgb]{0.82,0.01,0.11}{y}}\\
\alpha _{3} =s_{\textcolor[rgb]{0.25,0.46,0.02}{x}} s_{\textcolor[rgb]{0.82,0.01,0.11}{y}}
\end{matrix} \Rightarrow \begin{matrix}
\ln \alpha _{0} =\ln c_{\textcolor[rgb]{0.25,0.46,0.02}{x}} +\ln c\textcolor[rgb]{0.82,0.01,0.11}{_{y}}\\
\ln \alpha _{1} =\ln s_{\textcolor[rgb]{0.25,0.46,0.02}{x}} +\ln c\textcolor[rgb]{0.82,0.01,0.11}{_{y}}\\
\ln \alpha _{2} =\ln c_{\textcolor[rgb]{0.25,0.46,0.02}{x}} +\ln s_{\textcolor[rgb]{0.82,0.01,0.11}{y}}\\
\ln \alpha _{3} =\ln s_{\textcolor[rgb]{0.25,0.46,0.02}{x}} +\ln s_{\textcolor[rgb]{0.82,0.01,0.11}{y}}
\end{matrix} \Rightarrow \begin{bmatrix}
\ln \alpha _{0}\\
\ln \alpha _{1}\\
\ln \alpha _{2}\\
\ln \alpha _{3}
\end{bmatrix} =\begin{bmatrix}
1 &  & 1 & \\
 & 1 & 1 & \\
1 &  &  & 1\\
 & 1 &  & 1
\end{bmatrix}\begin{bmatrix}
\ln c_{\textcolor[rgb]{0.25,0.46,0.02}{x}}\\
\ln s_{\textcolor[rgb]{0.25,0.46,0.02}{x}}\\
\ln c\textcolor[rgb]{0.82,0.01,0.11}{_{y}}\\
\ln s_{\textcolor[rgb]{0.82,0.01,0.11}{y}}
\end{bmatrix}$

If we consider this a simple system:

x = c - w and y = d - w and z = b - d + w and a = b + c - d

$\displaystyle \begin{bmatrix}
1 &  & 1 & \\
 & 1 & 1 & \\
1 &  &  & 1\\
 & 1 &  & 1
\end{bmatrix}\begin{bmatrix}
x\\
y\\
z\\
w
\end{bmatrix} =\begin{bmatrix}
a\\
b\\
c\\
d
\end{bmatrix} \Rightarrow \begin{bmatrix}
1 & - &  & \\
 & 1 & 1 & \\
 &  & 1 & -\\
 &  &  & 
\end{bmatrix}\begin{bmatrix}
x\\
y\\
z\\
w
\end{bmatrix} =\begin{bmatrix}
a-b\\
b\\
b-d\\
b+c-a-d
\end{bmatrix} \Rightarrow \begin{bmatrix}
x\\
y\\
z\\
d
\end{bmatrix} =\begin{bmatrix}
c-w\\
d-w\\
b-d+w\\
b+c-a
\end{bmatrix}$

$\displaystyle \cfrac{\alpha _{0}}{\alpha _{1}} =\cfrac{\alpha _{2}}{\alpha _{3}}$



So if we chose $\displaystyle \ln s_{\textcolor[rgb]{0.82,0.01,0.11}{y}} =\ln \alpha _{3}$, we have $\displaystyle \begin{bmatrix}
\ln c_{\textcolor[rgb]{0.25,0.46,0.02}{x}}\\
\ln s_{\textcolor[rgb]{0.25,0.46,0.02}{x}}\\
\ln c\textcolor[rgb]{0.82,0.01,0.11}{_{y}}
\end{bmatrix} =\begin{bmatrix}
\ln \alpha _{0}\\
\ln \alpha _{1}\\
\ln \alpha _{2}
\end{bmatrix} \Rightarrow \begin{bmatrix}
c_{\textcolor[rgb]{0.25,0.46,0.02}{x}}\\
s_{\textcolor[rgb]{0.25,0.46,0.02}{x}}\\
c\textcolor[rgb]{0.82,0.01,0.11}{_{y}}\\
s_{\textcolor[rgb]{0.82,0.01,0.11}{y}}
\end{bmatrix} =\begin{bmatrix}
\alpha _{0}\\
\alpha _{1}\\
\alpha _{2}\\
\alpha _{3}
\end{bmatrix} +2\pi \begin{bmatrix}
k_{0}\\
k_{1}\\
k_{2}\\
k_{3}
\end{bmatrix}\sqrt{-1}$

Let's consider $\displaystyle P\left( x,x^{2}\right) =\alpha _{0} +\alpha _{1} x+\alpha _{2} x^{2} +\alpha _{3} x^{3} =( c_{\textcolor[rgb]{0.25,0.46,0.02}{x}} +s_{\textcolor[rgb]{0.25,0.46,0.02}{x}} x)\left( c\textcolor[rgb]{0.82,0.01,0.11}{_{y}} +s_{\textcolor[rgb]{0.82,0.01,0.11}{y}} x^{2}\right)$

Let's check $\displaystyle x=-\cfrac{\alpha _{0} +2\pi k_{0}\sqrt{-1}}{\alpha _{1} +2\pi k_{1}\sqrt{-1}}$ is a solution, but first let's put this in polar form:

$\displaystyle x=-\sqrt{\cfrac{\alpha _{0}^{2} +( 2\pi k_{0})^{2}}{\alpha _{1}^{2} +( 2\pi k_{1})^{2}}} e^{\arctan()\sqrt{-1}}$

$\displaystyle \alpha _{0} +\alpha _{1} x+\alpha _{2} x^{2} +\alpha _{3} x^{3}$



$\displaystyle P( x_{1} ,x_{2} ,...,x_{n}) =\sum _{k=0}^{2^{n}} \alpha _{k}\prod _{t=0}^{n} x_{t}^{k_{t}}$ where $\displaystyle k_{t} =\left\lfloor k/2^{t}\right\rfloor -2\left\lfloor k/2^{t+1}\right\rfloor $ is the t-th digit of k in base 2

$\displaystyle \prod _{t=0}^{n}\left( a_{t} +\sum _{k=0}^{n} a_{kt}\right) =\sum $



$\displaystyle  \begin{array}{{>{\displaystyle}l}}
( z-a_{0})\left(( z-a_{1})^{2} +b_{1}^{2}\right)\left(( z-a_{2})^{2} +b_{2}^{2}\right) =\left(( z-a_{0})( z-a_{1})^{2} +( z-a_{0}) b_{1}^{2}\right)\left(( z-a_{2})^{2} +b_{2}^{2}\right)\\
=( z-a_{0})( z-a_{1})^{2}\left(( z-a_{2})^{2} +b_{2}^{2}\right) +( z-a_{0}) b_{1}^{2}\left(( z-a_{2})^{2} +b_{2}^{2}\right)\\
=( z-a_{0})( z-a_{1})^{2}( z-a_{2})^{2} +( z-a_{0})( z-a_{1})^{2} b_{2}^{2} +( z-a_{0}) b_{1}^{2}( z-a_{2})^{2} +( z-a_{0}) b_{1}^{2} b_{2}^{2}\\
=( z-a_{0})( z-a_{1})( z-a_{1})( z-a_{2})( z-a_{2})\\
+b_{2}^{2}( z-a_{0})( z-a_{1})( z-a_{1})\\
+b_{1}^{2}( z-a_{0})( z-a_{2})( z-a_{2})\\
+zb_{1}^{2} b_{2}^{2} -a_{0} b_{1}^{2} b_{2}^{2}\\
=z^{5} -a_{2} z^{4} -a_{2} z^{4} +a_{2}^{2} z^{3} -a_{1} z^{4} +a_{1} a_{2} z^{3} +a_{1} a_{2} z^{3} -a_{1} a_{2}^{2} z^{2}\\
-\left(\left( a_{1} z^{4} -a_{1} a_{2} z^{3} -a_{1} a_{2} z^{3} +a_{1} a_{2}^{2} z^{2}\right) -\left( a_{1}^{2} z^{2}( z-a_{2}) -a_{1}^{2} a_{2} z( z-a_{2})\right)( z-a_{2})\right)\\
-( a_{0} z-a_{0} a_{1})( z-a_{1})( z-a_{2})( z-a_{2})\\
+b_{2}^{2}( z-a_{0})( z-a_{1})( z-a_{1})\\
+b_{1}^{2}( z-a_{0})( z-a_{2})( z-a_{2})\\
+zb_{1}^{2} b_{2}^{2} -a_{0} b_{1}^{2} b_{2}^{2}
\end{array}$



