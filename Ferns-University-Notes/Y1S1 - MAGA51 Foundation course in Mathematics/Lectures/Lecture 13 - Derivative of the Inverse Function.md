The formula for the derivative of the inverse function, useful when it's difficult or impossible to find the inverse function to derive, but values for it is known.
$$
\begin{align}
f(f^{-1}(x))=x \\
\dfrac{d}{dx} f(f^{-1}(x))=\dfrac{d}{dx}x \\
f'(f^{-1}(x))(f^{-1}(x))'=1 \\
 \\
(f^{-1}(x))'=\dfrac{1}{f'(f^{-1}(x))}
\end{align}
$$
Logarithmic derivation, when the amount of products get annoying, you can do the logarithm of both sides, to simplify things, or when you have exponents of exponents.
$$
\begin{align}
(f(x)^{g(x)})'\neq g(x) f(x)^{g(x)-1}f'(x) \\
 \\
a=e^{ \ln a } \iff a^{b}=e^{ b\ln a } \\
(f(x)^{g(x)})' \iff (e^{ g(x)\ln f(x) })' \\
 \\
(f(x)^{g(x)})'=(h(x))' \\
h(x)=f(x)^{g(x)} \\
\ln(h(x))=g(x)*\ln(f(x)) | \dfrac{d}{dx} \\
\dfrac{1}{h(x)}h'(x)=g'(x) \ln(f(x))+ g(x) \dfrac{1}{f(x)} f'(x) \\
h'(x)=f(x)^{g(x)}(g'(x) \ln(f(x))+ g(x) \dfrac{1}{f(x)} f'(x))
\end{align}
$$
$$
\begin{align}
(\arcsin x)'=\dfrac{1}{\sqrt{ 1-x^{2} }} \\
(\arccos x)'=-\dfrac{1}{\sqrt{ 1-x^{2} }} \\
(\arctan x)'= \dfrac{1}{1+x^{2}}
\end{align}
$$

$$
\begin{align}
(\ln x)'=\dfrac{1}{x}
\end{align}
$$
### Examples
####  4
Decide the tangent line to the curve $y=y(x)$ that fulfils the equation $\arcsin(x^{2}y^{2})-\ln(4x^{2}+y^{2})+\arctan 2(x+y)=\dfrac{\pi}{4}$  in the point $\left( \dfrac{1}{2},0 \right)$
Check if $\left( \dfrac{1}{2},0 \right) \in G_{y}$
$$
\begin{align}
\arcsin\left( \dfrac{1}{2}^{2}0^{2} \right)-\ln\left( 4 \dfrac{1}{4}+0 \right)+\arctan 2\left( \dfrac{1}{2}+0 \right)=\dfrac{\pi}{4} \\
0-0+\dfrac{\pi}{4}=\dfrac{\pi}{4}
\end{align}
$$
it is, now derivation $\dfrac{d}{dx}$

$$
\begin{align}
\dfrac{d}{dx}\underbrace{ (\arcsin(x^{2}y^{2})) }_{ T_{1} }-\dfrac{d}{dx}\underbrace{ (\ln(4x^{2}+y^{2})) }_{ T_{2} }+\dfrac{d}{dx}\underbrace{ (\arctan 2(x+y)) }_{ T_{3} }=0 \\
T_{1}=(\arcsin(x^{2}y^{2}))' = \dfrac{1}{\sqrt{ 1-(x^{2}y^{2})^{2} }}(x^{2}y^{2})'=\dfrac{1}{\sqrt{ 1-x^{4}y^{4} }}(2xy^{2}+x^{2}2yy')= \\
\dfrac{2xy^{2}+x^{2}2yy'}{\sqrt{ 1-x^{4}y^{4} }} \\
T_{2}=(\ln(4x^{2}+y^{2}))'=\dfrac{1}{4x^{2}+y^{2}}(4x^{2}+y^{2})'=\dfrac{1}{4x^{2}+y^{2}}(8x+2yy')=\dfrac{8x+2yy'}{4x^{2}+y^{2}} \\
T_{3}=(\arctan(2(x+y)))'=\dfrac{1}{1+4(x+y)^{2}}(2(x+y))'=\dfrac{1}{1+4(x+y)^{2}}2(1+y') \\
\dfrac{2xy^{2}+x^{2}2yy'}{\sqrt{ 1-x^{4}y^{4} }}-\dfrac{8x+2yy'}{4x^{2}+y^{2}}+\dfrac{1}{1+4(x+y)^{2}}2(1+y')=0 \\
x=\dfrac{1}{2} \\
y\left( \dfrac{1}{2} \right)=0 \\
y'\left( \dfrac{1}{2} \right)=k \\
\dfrac{0+0}{\sqrt{ 1-0 }}-\dfrac{4+0}{4 \dfrac{1}{4}+0}+\dfrac{2+2k}{1+4\left( \dfrac{1}{2}+0 \right)^{2}}=0 \iff 0-4+\dfrac{2+2k}{2}=0\iff -4+1+k=0 \\
k=3 \\
t: y=3\left( x-\dfrac{1}{2} \right)
\end{align}
$$
#### 2
##### a)
for an invertible  function $f$, $f(-3)=5$ and $f'(-3)=-2$, decide $(f^{-1})'(5)$, that being the derivative of the inverse function in 5, answer exact
$$
\begin{align}
(f^{-1})'(5)=\dfrac{1}{f'(f^{-1}(5))}=\dfrac{1}{f'(-3)}=\dfrac{1}{-2}=-\dfrac{1}{2}
\end{align}
$$
Decide $(f^{-1})'(2)$ for $f(x)=x^{3}-4x^{2}-4x+3$
$$
\begin{align}
f(x)=x^{3}-4x^{2}-4x+3 \\
f'(x)=3x^{2}-8x-4 \\
(f^{-1})'(2)=\dfrac{1}{f'(\underbrace{ f^{-1}(2) }_{ x_{0} })}=\dfrac{1}{3x_{0}^{2}-8x_{0}-4} \\
f(x)=2 \iff x^{3}-4x^{2}-4x+3=2\iff x^{3}-4x^{2}-4x+1=0 \\
(x^{3}+1)-4x(x+1)=0 \\
(x+1)(x^{2}-x+1)-4x(x+1)=0 \iff (\underbrace{ x+1 }_{ x=-1 })\left( \underbrace{ x^{2}_--5x+1 }_{ x_{1,2}=\frac{5}{2}\pm \sqrt{ \frac{25}{4}-1 } } \right)=0 \\
\nexists f^{-1}(2)
\end{align}
$$
if $f(x)=2$ doesn't have any solutions $\implies \nexists f^{-1}(2)$
if $f(x)=2$ has one solution $\implies\text{Ok}$
if $f(x)=2$ has many solutions $\implies \nexists f^{-1}(2)$
ie if there are many solutions, the function is non invertible

#### 5
Decide $(f^{-1})'(3)$ when $f(x)=x^{3}-2x^{2}+4x-5$
$$
\begin{align}
f(x)=x^{3}-2x^{2}+4x-5 \\
f'(x)=3x^{2}-4x+4 \\
 \\
f(x)=3\iff x^{3}-2x^{2}+4x-5=3\iff x^{3}-2x^{2}+4x-8=0 \\
x^{2}(x-2)+4(x-2)=0\iff (\underbrace{ x-2 }_{ x=2 })(\underbrace{ x^{2}+4 }_{ \in \mathbb{C} })=0 \\
\exists f^{-1}(3) \\
 \\
(f^{-1})'(3)=\dfrac{1}{f'(f^{-1}(3))}=\dfrac{1}{f'(2)}=\dfrac{1}{3*2^{2}-4*2+4}=\dfrac{1}{12-8+4}= \enclose{box}{\dfrac{1}{8}}
\end{align}
$$
#### 3
Decide $f'\left( \dfrac{\pi}{4} \right)$ when $f(x)=(\sin 2x)^{\sqrt{ x }}$
$$
\begin{align}
f(x)=(\sin 2x)^{\sqrt{ x }} \\
\ln(f(x))=\sqrt{ x }\ln(\sin 2x) \\
\dfrac{1}{f(x)}f'(x)=\dfrac{1}{2\sqrt{ x }}\ln(\sin 2x)+\sqrt{ x } \dfrac{1}{\sin(2x)} \cos(2x)2 \\
f'(x)=\sin 2x^{\sqrt{ x }}\left( \dfrac{1}{2\sqrt{ x }}\ln(\sin 2x) +2\sqrt{ x } \dfrac{\cos(2x)}{\sin(2x)} \right) \\
f'\left( \dfrac{\pi}{4} \right)=\left( \sin \dfrac{\pi}{2} \right)^{\sqrt{ \pi/4 }}\left( \dfrac{1}{2\sqrt{ \dfrac{\pi}{4} }}\underbrace{ \ln(\underbrace{ \sin(2x) }_{ 1 }) }_{ 0 } +\underbrace{ 2\sqrt{ \dfrac{\pi}{4}  }\dfrac{\cos\left( \dfrac{\pi}{2} \right)}{\sin \left( \dfrac{\pi}{2} \right)} }_{ 0 }\right)=1(0+0)=0
\end{align}
$$