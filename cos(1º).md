[cos(1º)](https://www.youtube.com/watch?v=KG7MyVhhZ9k&ab_channel=FlammableMaths))


$$\displaystyle \cos n\theta +i\sin n\theta =e^{i\theta n} =\left( e^{i\theta }\right)^{n} =(\cos \theta +i\sin \theta )^{n} =\sum _{k=0}^{n}\binom{n}{k} i^{k}\sin^{k} \theta \cos^{n-k} \theta $$

We can write $\displaystyle x=\cos \theta$ and $\displaystyle y=\sin \theta$ to take less space: 



$$\displaystyle \begin{aligned}
( x+iy)^{2n} & =\sum _{k=0}^{2n}\binom{2n}{k} i^{k} x^{2n-k} y^{k} & \\
 & =\sum _{k=0}^{n}\binom{2n}{2k} i^{2k} x^{2n-2k} y^{2k} +\sum _{k=0}^{n} i^{1+2k}\binom{2n}{2k+1} i^{2k+1} x^{2n-2k-1} y^{2k+1} & \\
 & =\sum _{k=0}^{n}( -1)^{k}\binom{2n}{2k} x^{2( n-k)} y^{2k} +i\sum _{k=0}^{n}( -1)^{k}\binom{2n}{2k+1} x^{2( n-k) -1} y^{2k+1} & \\
\sin 2n\theta  & =\sum _{k=0}^{n}( -1)^{k}\binom{2n}{2k+1} x^{2( n-k) -1} y^{2k+1} & \\
\cos 2n\theta  & =\sum _{k=0}^{n}( -1)^{k}\binom{2n}{2k}\left( x^{2}\right)^{n-k}\left( 1-x^{2}\right)^{k} & \\
 & =\sum _{k=0}^{n}( -1)^{k}\binom{2n}{2k}\left( x^{2}\right)^{n-k}\sum _{\ell =0}^{k}\binom{k}{\ell }( -1)^{k-\ell }\left( x^{2}\right)^{k-\ell } & \\
 & =\sum _{\ell =0}^{n}( -1)^{-\ell }\left( x^{2}\right)^{n-\ell }\underbrace{\sum _{k=\ell }^{n}\binom{2n}{2k}\binom{k}{\ell }}_{a_{\ell }} & \\
 & =\sum _{\ell =0}^{n} a_{\ell }( -1)^{-\ell }\left( x^{2}\right)^{n-\ell } =\sum _{s=0}^{n} a_{n-s}( -1)^{-( n-s)}\left( x^{2}\right)^{n-( n-s)} & [ s=n-\ell ]\\
 & =\sum _{s=0}^{n}( -1)^{( s-n)}\left( x^{2}\right)^{s}\left(\sum _{k=n-s}^{n}\binom{2n}{2k}\binom{k}{n-s}\right) & \\
 & =\sum _{s=0}^{n}( -1)^{( s-n)}\left( x^{2}\right)^{s}\left(\underbrace{\sum _{t=0}^{s}\binom{2n}{2( t+n-s)}\binom{t+n-s}{n-s}}_{b_{s}}\right) & [ t+n-s=k]\\
 & =-( -1)^{( n)} b_{0} +\sum _{s=1}^{n}( -1)^{( s-n)}\left( x^{2}\right)^{s}\left(\underbrace{\sum _{t=0}^{s}\binom{2n}{2( t+n-s)}\binom{t+n-s}{n-s}}_{b_{s}}\right) & \\
0 & =-\left(\cos 2n\theta +( -1)^{( n)} b_{0}\right) +\sum _{s=1}^{n}( -1)^{( s-n)} b_{s}\left( x^{2}\right)^{s} & \\
0 & =-\left(\cos 2n\theta +( -1)^{( n)} b_{0}\right) +\sum _{s=1}^{n}( -1)^{( s-n)} b_{s}\left( x^{2}\right)^{s} & 
\end{aligned}$$




$\displaystyle ( x+iy)^{7} =x^{7} +7ix^{6} y-21x^{5} y^{2} -35ix^{4} y^{3} +35x^{3} y^{4} +21ix^{2} y^{5} -7xy^{6} -iy^{7}$

$$\displaystyle \begin{array}{ c l }
\cos 7\theta  & =x^{7} -21x^{5} y^{2} +35x^{3} y^{4} -7xy^{6}\\
 & =x^{7} -21x^{5}\left( 1-x^{2}\right) +35x^{3}\left( 1-x^{2}\right)^{2} -7x\left( 1-x^{2}\right)^{3}\\
 & =x^{7} -21x^{5}\left( 1-x^{2}\right) +35x^{3}\left( 1-x^{2}\right)^{2} -7x\left( 1-x^{2}\right)^{3}\\
 & =x\left( x^{6} -21x^{4}\left( 1-x^{2}\right) +35x^{2}\left( 1-x^{2}\right)^{2} -7\left( 1-x^{2}\right)^{3}\right)\\
 & =x\left( x^{6} -7\left( 3x^{4}\left( 1-x^{2}\right) +5x^{2}\left( 1-x^{2}\right)^{2} -\left( 1-x^{2}\right)^{3}\right)\right)
\end{array}$$

For $\displaystyle n\ =\ 4m$ and take $\displaystyle t=y^{2}$

$$\displaystyle \begin{aligned}
\cos( 4m\theta ) & =\sum _{k=0}^{\lfloor n/4\rfloor }\left(\binom{4m}{4k}( 1-t)^{2k} t^{2( m-k)} -\binom{n}{4k+2}( 1-t)^{2k+1} t^{( 2( m-k) -1))}\right)\\
 & =\sum _{k=0}^{\lfloor n/4\rfloor }\left(\sum _{\ell =0}^{2k}( -1)^{\ell }\cfrac{( 4m) !}{( 4k) !( 4( m-k)) !}\cfrac{( 2k) !}{\ell !( 2k-\ell ) !} t^{2m-\ell }\right)\\
 & +\sum _{k=0}^{\lfloor n/4\rfloor }\left(\sum _{\ell =0}^{2k+1}( -1)^{\ell +1}\cfrac{( 4m) !}{( 2( 2k+1)) !( 2( 2m-2k-1)) !}\cfrac{( 2k+1) !}{\ell !( 2k+1-\ell ) !} t^{2m-\ell }\right)\\
 & \sum _{k=0}^{m}\sum _{\ell =0}^{2k}( -1)^{\ell }\left(\cfrac{( 4m) !( 2k) !}{( 4k) !( 4( m-k)) !\ell !( 2k-\ell ) !} -\cfrac{( 4m) !( 2k+1) !}{( 2( 2k+1)) !( 2( 2m-2k-1)) !\ell !( 2k+1-\ell ) !}\right) t^{2m-\ell }\\
 & +\cfrac{( 4m) !}{( 2( 2k+1)) !( 2( 2m-2k-1)) !} t^{2( m-k) -1}
\end{aligned}$$



$$\displaystyle  \begin{array}{{>{\displaystyle}l}}
\cfrac{( 4m) !( 2k) !}{( 4k) !( 4( m-k)) !\ell !( 2k-\ell ) !} -\cfrac{( 4m) !( 2k+1) !}{( 2( 2k+1)) !( 2( 2m-2k-1)) !\ell !( 2k+1-\ell ) !}\\
=\cfrac{( 4m) !( 2k) !}{( 4k) !\ell !( 2k-\ell ) !(( 4( m-k) -2)) !}\left(\cfrac{1}{( 4( m-k))( 4( m-k) -1)} -\cfrac{( 2k+1)}{( 4k+2)( 4k+1)( 2k+1-\ell )}\right)\\
=\cfrac{( 4m) !( 2k) !}{( 4k) !\ell !( 2k-\ell ) !(( 4( m-k) -2)) !}\left(\cfrac{2( 4k+1)( 2k+1)( 2k+1-\ell ) -4( 2k+1)( m-k)( 4( m-k) -1)}{( 4( m-k))( 4( m-k) -1)( 4k+2)( 4k+1)( 2k+1-\ell )}\right)\\
=\cfrac{( 4m) !( 2k) !}{( 4k) !\ell !( 2k-\ell ) !(( 4( m-k) -2)) !}\left(\cfrac{( 4k+1)( 2k+1-\ell ) +2\left( m-k-4( m-k)^{2}\right)}{4( m-k)( 4k+1)( 2k+1-\ell )( 4( m-k) -1)}\right)
\end{array}$



$\displaystyle \binom{4m}{4k+2} =\cfrac{( 4m) !}{( 4k+2) !( 4m-4k-2) !} =\cfrac{( 4m-4k-2)( 4m-4k-1)}{( 4k+2)( 4k+1)}\cfrac{4m!}{( 4k) !( 4m-4k) !}$

$\displaystyle \begin{aligned}
\cos( 4m\theta ) & =\sum _{k=0}^{\lfloor n/4\rfloor }\left(\binom{4m}{4k}( 1-t)^{2k} t^{2( m-k)} -\cfrac{( 4m-4k-2)( 4m-4k-1)}{( 4k+2)( 4k+1)}\cfrac{( 1-t)}{t}\binom{4m}{4k}( 1-t)^{2k} t^{2( m-k)}\right)\\
 & =\sum _{k=0}^{\lfloor n/4\rfloor }\binom{4m}{4k}( 1-t)^{2k} t^{2( m-k)}\left( 1-\cfrac{( 4m-4k-2)( 4m-4k-1)}{( 4k+2)( 4k+1)}\cfrac{1-t}{t}\right)
\end{aligned}$$

Then, if we split the real and imaginary parts we get

$\displaystyle \cos n\theta =$



If we break imaginary and real components we get



$$\begin{array}{{>{\displaystyle}l}}
\displaystyle  \cos n\theta =\sum _{k=0}^{\lfloor n/2\rfloor }\binom{n}{2k} i^{2k}\sin^{2k} \theta \cos^{n-2k} \theta =\sum _{k=0}^{\lfloor n/2\rfloor }( -1)^{k}\binom{n}{2k}\sin^{2k} \theta \cos^{n-2k} \theta \\

\displaystyle  \sin n\theta =\sum _{k=0}^{\lfloor n/2\rfloor }\binom{n}{2k+1} i^{2k}\sin^{2k+1} \theta \cos^{n-2k-1} \theta =\sum _{k=0}^{\lfloor n/2\rfloor }( -1)^{k}\binom{n}{2k+1}\sin^{2k+1} \theta \cos^{n-2k-1} \theta 
\end{array}$$



We know that $\displaystyle \sin^{2}( \theta ) =\left( 1-\cos^{2} \theta \right)$ so $\displaystyle \sin^{2k}( \theta ) =\left( 1-\cos^{2k} \theta \right)$

Then the formula for cossines becomes

$\displaystyle \cos n\theta =\sum _{k=0}^{\lfloor n/2\rfloor }( -1)^{k}\binom{n}{2k}\left( 1-\cos^{2k} \theta \right)\cos^{n-2k} \theta $

Let's call $\displaystyle x=\cos \theta $ and $\displaystyle y=\cos n\theta $

$\displaystyle y=\sum _{k=0}^{\lfloor n/2\rfloor }( -1)^{k}\binom{n}{2k}\left( 1-x^{2k}\right) x^{n-2k}$

Let's see how this looks for some examples of $\displaystyle n$

$\displaystyle n=3$

$\displaystyle y=-3\left( 1-x^{2}\right) x$