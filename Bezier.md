$$\displaystyle b_{0}[ a_{0}]( t) =a_{0}$$

$$\displaystyle b_{1}[ a_{0} ,a_{1}]( t) =b_{0}[ a_{0}]( t) \cdot ( 1-t) +b_{0}[ a_{1}]( t) \cdot t=a_{0} \cdot ( 1-t) +a_{1} \cdot t$$

$$\displaystyle  \begin{aligned}
b_{2}[ a_{0} ,a_{1} ,a_{2}]( t) =b_{1}[ a_{0} ,a_{1}]( t) \cdot ( 1-t) +b_{1}[ a_{1} ,a_{2}]( t) \cdot t\\
=( 1-t)(( 1-t) a_{0} +t\cdot a_{1}) +( 1-t)(( 1-t) a_{1} +t\cdot a_{2})\\
=( 1-t)^{2} a_{0} +( 1-t) a_{1} +( 1-t) t\cdot a_{2}
\end{aligned}$$

$$\displaystyle  \begin{aligned}
y( t) =b_{3}[ a_{0} ,a_{1} ,a_{2} ,a_{3}]( t) =b_{2}[ a_{0} ,a_{1}]( t) \cdot ( 1-t) +b_{2}[ a_{1} ,a_{2}]( t) \cdot t\\
=( 1-t)^{3} a_{0} +( 1-t)^{2}( 2-t) a_{1} +( 1-t)^{2}( 1+t) \cdot a_{2} +( 1-t)^{2} t\cdot a_{3}\\
=( 1-t)^{3} a_{0} +( 1-t)^{2}(( 2-t) a_{1} +( t+1) \cdot a_{2}) +( 1-t)^{2} t\cdot a_{3}\\
=p_{0}( t) \cdot a_{0} +p_{1}( t) \cdot a_{1} +p_{2}( t) \cdot a_{2} +p_{3}( t) \cdot a_{3}\\
=\sum _{k=0}^{3} p_{k}( t) a_{k}
\end{aligned}$$

$$\displaystyle  \begin{aligned}
y'( t) =-3( 1-t)^{2} \cdot a_{0} +\left( -2( 1-t)( 2-t) -( 1-t)^{2}\right) \cdot a_{1} +\left(( 1-t)^{2} -( 1-t)( 1+t)\right) \cdot a_{2} +\left( -2( 1-t) t+( 1-t)^{2}\right) \cdot a_{3}\\
=-3( 1-t)^{2} \cdot a_{0} \ +( 1-t)( -5+t) \cdot a_{1} \ +( 1-t)( -2t) \cdot a_{2} \ +( 1-t)( 1-3t) \cdot a_{3}\\
=p'_{0}( t) \cdot a_{0} +p'_{1}( t) \cdot a_{1} +p'_{2}( t) \cdot a_{2} +p'_{3}( t) \cdot a_{3}\\
=\sum _{k=0}^{3} p'_{k}( t) a_{k}
\end{aligned}$$

If $\displaystyle a_{k}$ has $\displaystyle D$ components $\displaystyle ( a_{k,1} ,...a_{k,D})$

$$\displaystyle -3( 1-t)^{2} \cdot a_{0} \ +( 1-t)( -5+t) \cdot a_{1} \ +( 1-t)( -2t) \cdot a_{2} \ +( 1-t)( 1-3t) \cdot a_{3}$$

$$ $$
Closed form solution to the length of a cubic bezier curve

$$\begin{aligned}
\int _{a_{0}}^{a} db_{3} &=\int _{0}^{\tau }\sqrt{\sum _{d=0}^{D}\left(\sum _{k=0}^{3} a_{kd} \cdot p'_{k}( t)\right)^{2}} dt\\
&=\int _{0}^{\tau }\sqrt{\sum _{d=0}^{D}\sum _{k=0}^{3}\sum _{k'=0}^{3} a_{kd} a_{k'd} \cdot p'_{k}( t) \cdot p'_{k'}( t)} dt
\end{aligned}$$

Let $\displaystyle c_{l,\prescript{}{}{} k,k'}$ be the coeficient of $\displaystyle t^{l}$ of the polinomial $\displaystyle p'_{k}( t) \cdot p'_{k'}( t)$

$$\displaystyle  \begin{aligned}
&=\int _{0}^{\tau }\sqrt{\sum _{k=0}^{3}\sum _{k'=0}^{3}\left(\sum _{d=0}^{D} a_{kd} \cdot a_{k'd}\right)\left( c_{0,k,k'} +c_{1,\prescript{}{}{} k,k'} \cdot t+c_{2,\prescript{}{}{} k,k'} \cdot t^{2}\right)} dt\\
&=\int _{0}^{\tau }\sqrt{\sum _{k=0}^{3}\sum _{k'=0}^{3}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right)( c_{0,k,k'}) +\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right)( c_{1,\prescript{}{}{} k,k'} \cdot t) +\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right)\left( c_{2,\prescript{}{}{} k,k'} \cdot t^{2}\right)} dt\\
&=\int _{0}^{\tau }\sqrt{\sum _{k=0}^{3}\sum _{k'=0}^{3}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right) c_{0,k,k'} +\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right)( c_{1,\prescript{}{}{} k,k'}) \cdot t+\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right)( c_{2,\prescript{}{}{} k,k'}) \cdot t^{2}} dt
\end{aligned}$$

Let's call $$\displaystyle C_{l} =\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right)( c_{l,\prescript{}{}{} k,k'})$$

$$\displaystyle =\int _{0}^{\tau }\sqrt{C_{0} +C_{1} t+C_{2} t^{2}} dt$$

$$\displaystyle  \begin{aligned}
=\cfrac{1}{8C_{2}^{2}}\left(\sqrt{C_{2}}\left( 4C_{0} C_{2} -C_{1}^{2}\right)\left[\operatorname{\ln}\left(\frac{2C_{2} t+C_{1}}{\sqrt{4C_{0} C_{2} -C_{1}^{2}}} +\sqrt{\left(\frac{2C_{2} t+C_{1}}{\sqrt{4C_{0} C_{2} -C_{1}^{2}}}\right)^{2} +1}\right)\right]_{0}^{\tau } +\left[\left( 4C_{2}^{2} \tau +2C_{1} C_{2}\right)\sqrt{C_{2} t^{2} +C_{1} t+C_{0}}\right]_{0}^{\tau } +2C_{1} C_{2}\sqrt{C_{0}}\right)\\
=\cfrac{1}{8C_{2}^{2}}\left(\sqrt{C_{2}}\left( 4C_{0} C_{2} -C_{1}^{2}\right)\left[\operatorname{arsinh}\left(\frac{2C_{2} t+C_{1}}{\sqrt{4C_{0} C_{2} -C_{1}^{2}}}\right)\right]_{0}^{\tau } +\left[\left( 4C_{2}^{2} t+2C_{1} C_{2}\right)\sqrt{C_{2} t^{2} +C_{1} t+C_{0}}\right]_{0}^{\tau } +2C_{1} C_{2}\sqrt{C_{0}}\right)\\
=\cfrac{1}{8C_{2}^{2}}\left(\sqrt{C_{2}}\left( 4C_{0} C_{2} -C_{1}^{2}\right)\left(\operatorname{arsinh}\left(\frac{2C_{2} \tau +C_{1}}{\sqrt{4C_{0} C_{2} -C_{1}^{2}}}\right) -\operatorname{arsinh}\left(\frac{C_{1}}{\sqrt{4C_{0} C_{2} -C_{1}^{2}}}\right)\right) +\left( 4C_{2}^{2} \tau +2C_{1} C_{2}\right)\sqrt{C_{2} \tau ^{2} +C_{1} \tau +C_{0}} +2C_{1} C_{2}\sqrt{C_{0}}\right)\\
=\dfrac{\sqrt{C_{2}}\left( 4C_{0} C_{2} -C_{1}^{2}\right)\operatorname{arsinh}\left(\frac{2C_{2} t+C_{1}}{\sqrt{4C_{0} C_{2} -C_{1}^{2}}}\right) +\left( 4C_{2}^{2} \tau +2C_{1} C_{2}\right)\sqrt{C_{2} t^{2} +C_{1} t+C_{0}}}{8C_{2}^{2}} -\dfrac{\sqrt{C_{2}}\left( 4C_{0} C_{2} -C_{1}^{2}\right)\operatorname{arsinh}\left(\frac{C_{1}}{\sqrt{4C_{0} C_{2} -C_{1}^{2}}}\right) +2\sqrt{C_{0}} C_{1} C_{2}}{8C_{2}^{2}}\\
=\dfrac{\sqrt{C_{2}}\left( 4C_{0} C_{2} -C_{1}^{2}\right)\operatorname{arsinh}\left(\frac{2C_{2} +C_{1}}{\sqrt{4C_{0} C_{2} -C_{1}^{2}}}\right) +\sqrt{C_{2} +C_{1} +C_{0}}\left( 4C_{2}^{2} +2C_{1} C_{2}\right)}{8C_{2}^{2}} -\dfrac{\sqrt{C_{2}}\left( 4C_{0} C_{2} -C_{1}^{2}\right)\operatorname{arsinh}\left(\frac{C_{1}}{\sqrt{4C_{0} C_{2} -C_{1}^{2}}}\right) +2\sqrt{C_{0}} C_{1} C_{2}}{8C_{2}^{2}}
\end{aligned}$$



$$\displaystyle \operatorname{\ln}\left( A\left( 1+\sqrt{1+\cfrac{1}{A^{2}}}\right)\right)$$







...

$$\displaystyle  \begin{aligned}
\int _{a_{0}}^{a_{3}} db_{3} =\int _{0}^{1}\sqrt{\sum _{d=0}^{D}\cfrac{d}{dt}( b_{3d}[ a_{0d} ,a_{1d} ,a_{2d} ,a_{3d}]( t))^{2}} dt\\
=\int _{0}^{1}\sqrt{\sum _{d=0}^{D}\left(\cfrac{d}{dt} p_{0}( t) \cdot a_{0d} +\cfrac{d}{dt} p_{1}( t) \cdot a_{1d} +\cfrac{d}{dt} p_{2}( t) \cdot a_{2d} +\cfrac{d}{dt} p_{3}( t) \cdot a_{3d}\right)^{2}} dt\\
=\int _{0}^{1}\sqrt{\sum _{d=0}^{D}\left(\sum _{k=0}^{n}\cfrac{d}{dt} p_{k}( t) \cdot a_{kd}{}\right)^{2}} dt\\
=\int _{0}^{1}\sqrt{\sum _{d=0}^{D}\sum _{k=0}^{n}\sum _{k'=0}^{n}{}\cfrac{d}{dt} p_{k}( t) \cdot \cfrac{d}{dt} p_{k'}( t) a_{kd} a_{k'd}} dt\\
=\int _{0}^{1}\sqrt{\sum _{k=0}^{n}\sum _{k'=0}^{n}\cfrac{d}{dt} p_{k}( t) \cdot \cfrac{d}{dt} p_{k'}( t)\sum _{d=0}^{D} a_{kd} a_{k'd}} dt\\
=\int _{0}^{1}\sqrt{\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right) p_{k} '( t) p_{k'} '( t)} dt\\
=\int _{0}^{1}\sqrt{x( t)} dt=\int _{0}^{1}\lim _{n\rightarrow \infty } S_{n} \ dt
\end{aligned}$$

Let $$\displaystyle c_{l,\prescript{}{}{} k,k'}$$ be the coeficient of $$\displaystyle t^{l}$$ of the polinomial $$\displaystyle p'_{k'}( t) \cdot p'_{k}( t)$$

$$\displaystyle  \begin{aligned}
\int _{0}^{1}\sqrt{\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right)\left( c_{0,k,k'} +c_{1,\prescript{}{}{} k,k'} \cdot t+c_{2,\prescript{}{}{} k,k'} \cdot t^{2}\right)} dt\\
=\int _{0}^{1}\sqrt{\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right)( c_{0,k,k'}) +\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right)( c_{1,\prescript{}{}{} k,k'} \cdot t) +\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right)\left( c_{2,\prescript{}{}{} k,k'} \cdot t^{2}\right)} dt\\
=\int _{0}^{1}\sqrt{\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right) c_{0,k,k'} +\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right)( c_{1,\prescript{}{}{} k,k'}) \cdot t+\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right)( c_{2,\prescript{}{}{} k,k'}) \cdot t^{2}} dt
\end{aligned}$$

Let's call $$\displaystyle C_{l} =\sum _{k=0}^{n}\sum _{k'=0}^{n}\left(\sum _{d=0}^{D} \cdot a_{kd} \cdot a_{k'd}\right)( c_{l,\prescript{}{}{} k,k'})$$

$$\displaystyle  \begin{aligned}
\int _{a_{0}}^{a_{3}} db_{3} =\int _{0}^{1}\sqrt{C_{0} +C_{1} t+C_{2} t^{2}} dt\\
=\int _{0}^{1}\sum _{k=0}^{\infty }\left(\cfrac{1}{k!}\prod _{l=0}^{k-1}\left(\cfrac{1}{2} -l\right)( C_{0} +x_{0})^{1/2-k}\left( C_{1} t+C_{2} t^{2} -x_{0}\right)^{k}\right) dt\\
=\sum _{k=0}^{\infty }\cfrac{1}{k!}\prod _{l=0}^{k-1}\left(\cfrac{1}{2} -l\right)( C_{0} +x_{0})^{1/2-k}\int _{0}^{1}\left( C_{1} t+C_{2} t^{2} -x_{0}\right)^{k} dt\\
=\sum _{k=0}^{\infty }\cfrac{1}{k!}\prod _{l=0}^{k-1}\left(\cfrac{1}{2} -l\right)( C_{0} +x_{0})^{1/2-k}\int _{0}^{1}\left( C_{1} t+C_{2} t^{2} -x_{0}\right)^{k} dt\\
=\sum _{k=0}^{\infty }\cfrac{1}{k!}\prod _{l=0}^{k-1}\left(\cfrac{1}{2} -l\right)( C_{0} +x_{0})^{1/2-k}\int _{0}^{1}\sum _{k_{0} ,k_{1} ,k_{2}  >0}^{k_{0} +k_{1} +k_{2} =k}\cfrac{( k_{0} +k_{1} +k_{2}) !}{k_{0} !k_{1} !k_{2} !}( -x_{0})^{k_{0}}( C_{1} t)^{k_{1}}\left( C_{2} t^{2}\right)^{k_{2}} dt\\
=\sum _{k=0}^{\infty }\cfrac{1}{k!}\prod _{l=0}^{k-1}\left(\cfrac{1}{2} -l\right)( C_{0} +x_{0})^{1/2-k}\sum _{k_{0} ,k_{1} ,k_{2}  >0}^{k_{0} +k_{1} +k_{2} =k}\cfrac{( k_{0} +k_{1} +k_{2}) !}{k_{0} !k_{1} !k_{2} !}( -x_{0})^{k_{0}} C_{1}^{k_{1}} C_{2}^{k_{2}}\int _{0}^{1} t^{k_{1} +2k_{2}} dt\\
=\sum _{k=0}^{\infty }\cfrac{1}{k!}\prod _{l=0}^{k-1}\left(\cfrac{1}{2} -l\right)( C_{0} +x_{0})^{1/2-k}\sum _{k_{0} ,k_{1} ,k_{2}  >0}^{k_{0} +k_{1} +k_{2} =k}\cfrac{( k_{0} +k_{1} +k_{2}) !}{k_{0} !k_{1} !k_{2} !}\cfrac{( -x_{0})^{k_{0}} C_{1}^{k_{1}} C_{2}^{k_{2}}}{k_{1} +2k_{2} +1}
\end{aligned}$$



$$\displaystyle  \begin{aligned}
\int _{a_{0}}^{a_{3}} db_{3} =\int _{0}^{1}\sqrt{C_{2} t^{2} +C_{1} t+C_{0}} dt
&=\int _{0}^{1}\sqrt{C_{2} t^{2} +C_{1} t+\left(\cfrac{C_{1}}{2C_{2}}\right)^{2} +C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}} dt\\
&=\int _{0}^{1}\sqrt{\left( C_{2} t+\cfrac{C_{1}}{2C_{2}}\right)^{2} +\left( C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}\right)} dt\\
&=\left( C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}\right)^{2}\int _{0}^{1}\sqrt{\left(\left(\cfrac{C_{2}}{C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}} t+\cfrac{\cfrac{C_{1}}{2C_{2}}}{C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}}\right)^{2} +1\right)} dt\\
&=C\int _{0}^{1}\sqrt{\left(( At+B)^{2} +1\right)} dt\\
\text{replace }\tan x=At+B\ ;\sec^{2}( x) dx=Adt\\
&=\cfrac{C}{A}\int _{\atan( B)}^{\atan( A+B)}\sqrt{\left((\tan x)^{2} +1\right)}\sec^{2} x\ dx\\
&=\cfrac{C}{A}\int _{\atan( B)}^{\atan( A+B)}\sec^{3}( x) dx\\
&=\cfrac{C}{A}\cfrac{1}{2}\left[\tan x\sqrt{\left((\tan x)^{2} +1\right)} -\ln\left(\cfrac{1-\tan\cfrac{x}{2}}{1+\tan\cfrac{x}{2}}\right)\right]_{\atan B}^{\atan( A+B)}\\
&=\cfrac{\left( C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}\right)^{3}}{C_{2}}\cfrac{1}{2}\left[\tan x\sqrt{\left((\tan x)^{2} +1\right)} -\ln\left(\cfrac{1-\tan\cfrac{x}{2}}{1+\tan\cfrac{x}{2}}\right)\right]_{\atan\cfrac{\cfrac{C_{1}}{2C_{2}}}{C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}}}^{\atan\left(\cfrac{C_{2} +\cfrac{C_{1}}{2C_{2}}}{C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}}\right)}\\
&=\cfrac{\left( C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}\right)^{3}}{C_{2}}\cfrac{1}{2}(\left[\tan x\sqrt{\left((\tan x)^{2} +1\right)}\right]_{\atan\cfrac{\cfrac{C_{1}}{2C_{2}}}{C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}}}^{\atan\cfrac{C_{2} +\cfrac{C_{1}}{2C_{2}}}{C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}}} -\ln\left(\cfrac{1-\tan\left(\cfrac{1}{2}\atan\cfrac{C_{2} +\cfrac{C_{1}}{2C_{2}}}{C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}}\right)}{1+\tan\left(\cfrac{1}{2}\atan\cfrac{C_{2} +\cfrac{C_{1}}{2C_{2}}}{C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}}\right)}\cfrac{1+\tan\left(\cfrac{1}{2}\atan\cfrac{\cfrac{C_{1}}{2C_{2}}}{C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}}\right)}{1-\tan\left(\cfrac{1}{2}\atan\cfrac{\cfrac{C_{1}}{2C_{2}}}{C_{0} -\left(\cfrac{C_{1}}{2C_{2}}\right)^{2}}\right)}\right)
\end{aligned}$$

$$\displaystyle y=\tan\left(\cfrac{1}{2}\arctan x\right) \Rightarrow \atan y=\cfrac{1}{2}\atan x$$





$$\displaystyle f( x) =\sqrt{C_{0} +x}$$ arround $$\displaystyle x_{0}$$
$$\displaystyle  \begin{aligned}
\left( \partial _{x}^{0} f\right)( x_{0}) &=( C_{0} +x_{0})^{1/2}\\
\left( \partial _{x}^{1} f\right)( x_{0}) &=( 1/2)( C_{0} +x_{0})^{1/2-1}\\
\left( \partial _{x}^{2} f\right)( x_{0}) &=( 1/2)( 1/2-1)( C_{0} +x_{0})^{1/2-2}\\
\left( \partial _{x}^{k} f\right)( x_{0}) &=\prod _{l=0}^{k-1}\left(\cfrac{1}{2} -l\right)( C_{0} +x_{0})^{1/2-k}
\end{aligned}$$









$$\displaystyle  \begin{aligned}
\left( \partial _{t}^{0} f\right)( t) &=\left( C_{0} +C_{1} t+C_{2} t^{2}\right)^{\cfrac{1}{2}}\\
\left( \partial _{t}^{1} f\right)( t) &=\left(\cfrac{1}{2}\right)\left( C_{0} +C_{1} t+C_{2} t^{2}\right)^{\cfrac{1}{2} -1}( C_{1} +2C_{2} t)\\
\left( \partial _{t}^{2} f\right)( t) &=\left(\cfrac{1}{2}\right)\left(\cfrac{1}{2} -1\right)\left( C_{0} +C_{1} t+C_{2} t^{2}\right)^{\cfrac{1}{2} -2}( C_{1} +2C_{2} t) +C_{2}\left( C_{0} +C_{1} t+C_{2} t^{2}\right)^{\cfrac{1}{2} -1}\\
\left( \partial _{t}^{3} f\right)( t) &=\left(\cfrac{1}{2}\right)\left(\cfrac{1}{2} -1\right)\left(\cfrac{1}{2} -2\right)\left( C_{0} +C_{1} t+C_{2} t^{2}\right)^{\cfrac{1}{2} -3}( C_{1} +2C_{2} t) +\left(\cfrac{1}{2}\right)\left(\cfrac{1}{2} -1\right)\left( C_{0} +C_{1} t+C_{2} t^{2}\right)^{\cfrac{1}{2} -2}( 2C_{2}) +C_{2}\left(\cfrac{1}{2} -1\right)\left( C_{0} +C_{1} t+C_{2} t^{2}\right)^{\cfrac{1}{2} -2}( C_{1} +2C_{2} t)
\end{aligned}$$

For $$\displaystyle f( x) =\sqrt{x+c}$$

$$\displaystyle  \begin{aligned}
f^{( 1)}( x) =\cfrac{1}{2}( x+c)^{\cfrac{1}{2} -1}\\
f^{( 2)}( x) =\cfrac{1}{2}\left(\cfrac{1}{2} -1\right)( x+c)^{\cfrac{1}{2} -2}\\
f^{( 3)}( x) =\cfrac{1}{2}\left(\cfrac{1}{2} -1\right)\left(\cfrac{1}{2} -2\right)( x+c)^{\cfrac{1}{2} -3}\\
f^{( k)}( x) =\prod _{l=0}^{k-1}\left(\cfrac{1}{2} -l\right)( x+c)^{\cfrac{1}{2} -k}
\end{aligned}$$









Substituting 

$$\displaystyle S( t) =\sqrt{x( t)} \Rightarrow S( t)^{2} -x( t) =0$$ can be approximated succesivelly with newton's method, considering

 $$\displaystyle  \begin{aligned}
f( S) =S^{2} -x( t) =0\Rightarrow \\
S_{n+1} =S( t)_{n} -\cfrac{f( S_{n})}{f'( S_{n})} =S_{n} -\cfrac{S_{n}^{2} -x( t)}{2S_{n}} =\cfrac{2S_{n}^{2} -S_{n}^{2} +x( t)}{2S_{n}} =\cfrac{S_{n}^{2} +x( t)}{2S_{n}} =\cfrac{1}{2}\left(\cfrac{S_{n}^{2} +x( t)}{S_{n}}\right)
\end{aligned}$$

$$\displaystyle  \begin{aligned}
S'=\cfrac{1}{x} \Rightarrow \cfrac{1}{S'} -x=0\\
\Rightarrow S'_{k+1} =S'_{n} -\cfrac{S^{\prime -1}_{k} -x}{-S^{\prime -2}_{k}} =S_{n} +\cfrac{S^{\prime 2}_{k}}{S^{\prime 2}_{k}}\cfrac{S^{\prime -1}_{k} -x}{S^{\prime -2}_{k}} =S'_{n} +\cfrac{S^{\prime 2}_{k}}{S^{\prime 2}_{k}}\cfrac{S^{\prime -1}_{k} -x}{S^{\prime -2}_{k}} =S'_{k} +S'_{k} -xS^{\prime 2}_{k} =S'_{k}( 2-xS'_{k}) =2S'_{k} -xS^{\prime 2}_{k}
\end{aligned}$$

Replacing ...

$$\displaystyle  \begin{aligned}
\sqrt{x( t)} =\lim _{n\rightarrow \infty } S_{n} \ \text{where} \ \\
S_{n+1} =\cfrac{1}{S_{n}}\cfrac{1}{2}\left( S_{n}^{2} +x( t)\right) =\cfrac{1}{\cfrac{1}{S_{n-1}}\cfrac{1}{2}\left(( S_{n-1})^{2} +x( t)\right)}\cfrac{1}{2}\left(\left(\cfrac{1}{S_{n-1}}\cfrac{1}{2}\left(( S_{n-1})^{2} +x( t)\right)\right)^{2} +x( t)\right)\\
=\cfrac{1}{\cfrac{1}{S_{n-1}}\left(( S_{n-1})^{2} +x( t)\right)}\left(\cfrac{1}{( S_{n-1})^{2}}\left(\left(\cfrac{1}{2}\right)^{2}( S_{n-1})^{4} +\left(\cfrac{1}{2}\right)^{2} 2( S_{n-1})^{2} x( t) +\left(\cfrac{1}{2}\right)^{2} x^{2}( t)\right) +x( t)\right)\\
=\cfrac{1}{( S_{n-1})\left(( S_{n-1})^{2} +x( t)\right)}\left(\cfrac{1}{4}( S_{n-1})^{4} +\cfrac{1}{2}\left(( S_{n-1})^{2} +1\right) x( t) +\cfrac{1}{4} x^{2}( t)\right)
\end{aligned}$$

A somation formula $$\displaystyle S=\sum _{n=0}^{\infty } f( x,n)$$ can be recursivelly though of as

 $$\displaystyle S=\lim _{n\rightarrow \infty } S_{n} \ \text{where} \ S_{0} =f( x,0) \ \text{and} \ S_{n+1} =S_{n} +f( x,n) =S_{n} +f( x,n)$$

With newton's method any differentiable function inverse $$\displaystyle g^{-1}( y) =x$$ can be though of as $$\displaystyle f( x) =g( x) -y=0$$

Then $$\displaystyle x=\lim _{n\rightarrow \infty } x_{n}$$ where $$\displaystyle x_{n+1} =x_{n} -\cfrac{f( x_{n}) -y}{f'( x_{n})}$$. If we replace $$\displaystyle f'( x_{n})$$ by a secant $$\displaystyle \cfrac{f( x_{n}) -f( x_{n-1})}{x_{n} -x_{n-1}}$$

Improving a little bit on secant method, expanding $$\displaystyle k$$ terms of taylor series around $$\displaystyle x_{n}$$ we have:

$$\displaystyle f( x) =f( x_{n}) +( \partial _{x} f)( x_{n})( x-x_{n}) +\cfrac{1}{2}\left( \partial _{x}^{2} f\right)( x_{n})( x-x_{n})^{2} +\cfrac{1}{6}\left( \partial _{x}^{3} f\right)( x_{n})( x-x_{n})^{3} +\cfrac{1}{24}\left( \partial _{x}^{4} f\right)( x_{n})( x-x_{n})^{4} +...+\cfrac{1}{k!}\left( \partial _{x}^{k+1} f\right)( x_{n})( x-x_{n})^{k+1}$$

$$\displaystyle f( x) =f( x_{n}) +( \partial _{x} f)( x_{n})( x-x_{n}) +\cfrac{1}{2}\left( \partial _{x}^{2} f\right)( x_{n})( x-x_{n})^{2} +\cfrac{1}{6}\left( \partial _{x}^{3} f\right)( x_{n})( x-x_{n})^{3} +\cfrac{1}{24}\left( \partial _{x}^{4} f\right)( x_{n})( x-x_{n})^{4} +O\left(( x-x_{n})^{5}\right)$$

In general

$$\displaystyle  \begin{aligned}
\sum _{k}^{K}\left(\sum _{l}^{L} a_{k}{}_{l}\right)^{2}\\
=\sum _{k}^{K}\left(\sum _{l}^{L}\left(\sum _{l}^{L} a_{k}{}_{l}\right) a_{k}{}_{l}\right)\\
=\sum _{k}^{K}\left(\sum _{l'}^{L}\left(\sum _{l}^{L} a_{k}{}_{l}\right) a_{k}{}_{l'}\right)\\
=\sum _{k}^{K}\left(\sum _{l,l'}^{L} a_{k}{}_{l} a_{k}{}_{l'}\right)
\end{aligned}$$



$$\displaystyle b_{n+1}[ a_{0} ,...,a_{n} ,a_{n+1}]( t) =b_{n}[ a_{0} ,a_{n}]( t) \cdot t+b_{n-1}[ a_{1} ,a_{n+1}]( t) \cdot ( 1-t)$$

$$\displaystyle \partial _{t}^{k} b_{n+1}[ a_{0} ,...,a_{n} ,a_{n+1}]( t) =\partial _{t}^{k} b_{n}[ a_{0} ,a_{n}]( t) -\partial _{t}^{k} b_{n-1}[ a_{1} ,a_{n+1}]( 1-t)$$

$$\displaystyle b_{1}[ a_{0} ,a_{1}]( t) =( 1-t) a_{0} +t\cdot a_{1}$$

$$\displaystyle \partial _{t}^{k} b_{1}[ a_{0} ,a_{1}]( t) =a_{1} -a_{0}$$

$$\displaystyle  \begin{aligned}
b_{2}[ a_{0} ,a_{1} ,a_{2}]( t) =b_{1}[ b_{1}[ a_{0} ,a_{1}]( t) ,b_{1}[ a_{1} ,a_{2}]( t)]( t)\\
=( 1-t) \cdotp b_{1}[ a_{0} ,a_{1}]( t) +t\cdotp b_{1}[ a_{1} ,a_{2}]( t)\\
=( 1-t) \cdotp (( 1-t) \cdot a_{0} +t\cdot a_{1}) +t\cdotp (( 1-t) \cdot a_{1} +t\cdot a_{2})
\end{aligned}$$

$$\displaystyle \partial _{t}^{k} b_{2}[ a_{0} ,a_{1} ,a_{2}]( t) =( 1-t) \cdotp b_{1}[ a_{0} ,a_{1}]( t) +t\cdotp b_{1}[ a_{1} ,a_{2}]( t)$$

$$\displaystyle  \begin{aligned}
y=b_{3}[ a_{0} ,a_{1} ,a_{2} ,a_{3}]( t)\\
=t\cdot ( t\cdot a_{0} +( 1-t) \cdot a_{1}) +( 1-t) \cdot ( t\cdot a_{1} +( 1-t) \cdot a_{2}) +t\cdot ( t\cdot a_{1} +( 1-t) \cdot a_{2}) +( 1-t) \cdot ( t\cdot a_{2} +( 1-t) \cdot a_{3})
\end{aligned}$$

$$\displaystyle b_{n}[ a_{0} ,...,a_{n}]( t) =( 1-t) \cdot b_{n-1}[ a_{0} ,a_{n-1}]( t) +t\cdot b_{n-1}[ a_{1} ,a_{n}]( t)$$

$$\displaystyle \partial _{t}^{k} b_{n}[ a_{0} ,...,a_{n}]( t) =$$