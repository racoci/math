
```glsl
vec2 mapping(vec2 z) {
  for (int i=0; i<64; i++) {
    // f(z) = z^5 -z -1
    vec2 c = cpow(z, vec2(5.0,0.0)) - z - vec2(1.0,0.0);
    // f'(z) = 5 * z^4 - 1
    vec2 b = cmul(vec2(5.0,0.0), cpow(z, vec2(4.0,0.0))) - vec2(1.0,0.0);
    // 2a = 5 * 4 * z^3
    vec2 aTimes2 = cmul(vec2(4.0*5.0,0.0), cpow(z, vec2(3.0,0.0)));
    vec2 delta = cpow(b, vec2(2.,0.) - cmul(vec2(2.0,0.0), cmul(aTimes2,f)));
    z = z + cdiv(-b+cpow(delta, vec2 (.5,0.)), aTimes2 );
  }
  return z;
}
```


Let $\displaystyle f:\mathbb{C}\rightarrow \mathbb{C}$ be a holomorphic function, we can expand $\displaystyle f( z)$ arround $\displaystyle f( z_{0})$ as 

$\displaystyle f( z) =\sum _{k=0}^{\infty }\cfrac{1}{k!}\cfrac{d^{k} f}{dz^{k}}( z_{0}) \ ( z-z_{0})^{k}$

$$\displaystyle  \begin{array}{{>{\displaystyle}l}}
f( z) =f( z_{0}) +f'( z_{0})( z-z_{0}) =f( z_{0}) +f'( z_{0}) z-f'( z_{0}) z_{0}\\
\Rightarrow z=\cfrac{f( z) -f( z_{0})}{f'( z_{0})} +z_{0}
\end{array}$$

$$\displaystyle  \begin{array}{{>{\displaystyle}l}}
ax^{2} +bx+c\Rightarrow x=\cfrac{-b\pm \sqrt{b^{2} -4ac}}{2a} =\left(\cfrac{-b}{2a}\right) \pm \sqrt{\cfrac{b^{2} -4ac}{4a^{2}}} =\left(\cfrac{-b}{2a}\right) \pm \sqrt{\left(\cfrac{-b}{2a}\right)^{2} -\cfrac{c}{a}}\\
x^{2} +2p+q\Rightarrow x=-p\pm \sqrt{p^{2} -q}\\
\end{array}$$

$$\begin{equation*}
\begin{array}{ c l }
0=f(z) & \approx f(z_{n} )+f'(z_{n} )(z-z_{n} )+\cfrac{1}{2} f''(z_{n} )(z-z_{n} )^{2}\\
 & \approx \cfrac{1}{2} f''(z_{n} )z^{2} +( f'(z_{n} )-f''(z_{n} )z_{n}) z+\left( f(z_{n} )+\cfrac{1}{2} f''(z_{n} )z_{n}^{2} -f'(z_{n} )z_{n}\right)\\
 & \approx z^{2} +2\left(\cfrac{f'(z_{n} )}{f''(z_{n} )} -\cfrac{f''(z_{n} )z_{n}}{f''(z_{n} )}\right) z+\left(\cfrac{2f(z_{n} )}{f''(z_{n} )} -\cfrac{2f'(z_{n} )z_{n}}{f''(z_{n} )} +z_{n}^{2}\right)
\end{array}
\end{equation*}$$
$$
\begin{equation*}
z_{n+1} =\cfrac{f'(z_{n} )}{f''(z_{n} )} -\cfrac{f''(z_{n} )z_{n}}{f''(z_{n} )} \pm \sqrt{\left(\cfrac{f'(z_{n} )}{f''(z_{n} )} -\cfrac{f''(z_{n} )z_{n}}{f''(z_{n} )}\right)^{2} -\cfrac{2f(z_{n} )}{f''(z_{n} )} +\cfrac{2f'(z_{n} )z_{n}}{f''(z_{n} )} -z_{n}^{2}}
\end{equation*}
$$


$$\displaystyle  \begin{array}{{>{\displaystyle}l}}
f( z) =f( z_{0}) +f'( z_{0})( z-z_{0}) +\cfrac{1}{2} f''( z_{0})( z-z_{0})^{2}\\
z=z_{0} +\cfrac{-f'( z_{0}) \pm \sqrt{f'( z_{0})^{2} -2f''( z_{0}) f( z_{0})}}{f''( z_{0})}
\end{array}$$



$\displaystyle {\displaystyle \frac{d}{dx}\left[\prod _{i=1}^{k} f_{i} (x)\right] =\sum _{i=1}^{k}\left(\left(\frac{d}{dx} f_{i} (x)\right)\prod _{j=1,j\neq i}^{k} f_{j} (x)\right) =\left(\prod _{i=1}^{k} f_{i} (x)\right)\left(\sum _{i=1}^{k}\frac{f'_{i} (x)}{f_{i} (x)}\right) .\frac{d}{dx}\left[\prod _{i=1}^{k} f_{i} (x)\right] =\sum _{i=1}^{k}\left(\left(\frac{d}{dx} f_{i} (x)\right)\prod _{j=1,j\neq i}^{k} f_{j} (x)\right) =\left(\prod _{i=1}^{k} f_{i} (x)\right)\left(\sum _{i=1}^{k}\frac{f'_{i} (x)}{f_{i} (x)}\right) .}$

$$\displaystyle  \begin{array}{{>{\displaystyle}l}}
f( z) =\prod _{k=1}^{n}( z-z_{k})\\
f'( z) ={\displaystyle f( z)\sum _{k=1}^{n}\frac{1}{z-z_{k}}}\\
f''( z) =f'( z){\displaystyle \sum _{k=1}^{n}\frac{1}{z-z_{k}} +f( z)\sum _{k=1}^{n} -\left(\frac{1}{z-z_{k}}\right)^{2}} ={\displaystyle f( z)\left(\left(\sum _{k=1}^{n}\frac{1}{z-z_{k}}\right)^{2} -\sum _{k=1}^{n}\left(\frac{1}{z-z_{k}}\right)^{2}\right)}\\
={\displaystyle f( z)\left(\sum _{k=1}^{n}\frac{1}{z-z_{k}}\sum _{k'=1}^{n}\frac{1}{z-z_{k'}} -\sum _{k=1}^{n}\left(\frac{1}{z-z_{k}}\right)^{2}\right)}\\
={\displaystyle f( z)\left(\sum _{k=1}^{n}\frac{1}{z-z_{k}}\left(\sum _{k'=1}^{n}\frac{1}{z-z_{k'}}\right) -\left(\frac{1}{z-z_{k}}\right)^{2}\right)} ={\displaystyle f( z)\left(\sum _{k=1}^{n}\frac{1}{z-z_{k}}\left(\left(\sum _{k'=1}^{n}\frac{1}{z-z_{k'}}\right) -\left(\frac{1}{z-z_{k}}\right)\right)\right)}\\
f''( z) ={\displaystyle f( z)\left(\left(\sum _{k=1}^{n}\frac{1}{z-z_{k}}\right)^{3} -\sum _{k=1}^{n}\frac{1}{z-z_{k}}\sum _{k=1}^{n}\left(\frac{1}{z-z_{k}}\right)^{2}\right) +2f( z)\left(\sum _{k=1}^{n}\left(\frac{1}{z-z_{k}}\right)^{3} -\sum _{k=1}^{n}\frac{1}{z-z_{k}}\sum _{k=1}^{n}\left(\frac{1}{z-z_{k}}\right)^{2}\right)}
\end{array}$$

