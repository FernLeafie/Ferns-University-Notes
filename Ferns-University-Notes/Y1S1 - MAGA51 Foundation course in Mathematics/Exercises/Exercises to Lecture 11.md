## Examples
#### 1
##### a)
Use the derivatives definition to describe $f'(x)$ where $f(x)=\sqrt{ x^{2}+x }$


$$
\begin{align}
\lim_{ h \to 0 } \dfrac{f(x+h)-f(x)}{h}=\lim_{ h \to 0 } \dfrac{\sqrt{ (x+h)^{2}+x+h }-\sqrt{ x^{2}+x }}{h} \\
\lim_{ h \to 0 } \dfrac{\dfrac{(x+h)^{2}+x+h-(x^{2}+x)}{\sqrt{ (x+h)^{2}+x+h }+\sqrt{ x^{2}+x }}}{h}=\lim_{ h \to 0 } \dfrac{x^{2}+2xh+h^{2}+x+h-x^{2}-x}{h(\sqrt{ (x+h)^{2}+x+h}+\sqrt{ x^{2}+x })} \\
\lim_{ h \to 0 } \dfrac{2x\cancel{ h }+h^{\cancel{ 2 }}+h}{\cancel{ h }(\sqrt{ (x+h)^{2}+x+h}+\sqrt{ x^{2}+x })}=``\dfrac{2x+1}{\sqrt{ x^{2}+x }+\sqrt{ x^{2}+x }} "=\dfrac{2x+1}{2\sqrt{ x^{2}+x }} \\
f'(x)=\dfrac{2x+1}{2\sqrt{ x^{2}+x }}
\end{align}
$$
##### b)
Decide the equation for the tangent and normal line for the function in $p=(1,\sqrt{ 2 })$

$$
\begin{align}
f(1)=\sqrt{ 2 } \\
\text{The point is on the line :3} \\
k_{t}=f'(1)=\dfrac{2+1}{2\sqrt{ 1+1 }}=\dfrac{3}{2\sqrt{ 2 }} \\
t:y-\sqrt{ 2 }=\dfrac{3}{2\sqrt{ 2 }}(x-1) \\
n:y-\sqrt{ 2 }=-\dfrac{2\sqrt{ 2 }}{3}(x-1)
\end{align}
$$
#### 2.
Decide the equation for the tangent line for the curve $f(x)=\dfrac{\sin(2x)}{x^{2}+x}$ in the point $\left( \dfrac{\pi}{2},0 \right)$

$$
\begin{align}
D_{f}=\mathbb{R}\setminus \{ -1,0 \} \\
\\
u(x)=\sin2x \\
u'(x)=\cos(2x) (2x)'=2\cos(2x) \\
v(x)=x^{2}+x \\
v'(x)=v'(x)=2x+1 \\
f'(x)=\dfrac{u'(x)v(x)-u(x)v'(x)}{v(x)^{2}}= \\
\dfrac{2\cos(2x)(x^{2}+x)-\sin(2x)(2x+1)}{(x^{2}+x)^{2}} \\
f'\left( \dfrac{\pi}{2} \right)=\dfrac{2\cos\left(2 \dfrac{\pi}{2} \right)\left( \left( \dfrac{\pi}{2} \right)^{2}+\dfrac{\pi}{2} \right)-\sin\left( 2\dfrac{\pi}{2} \right)\left( 2 \dfrac{\pi}{2}+1 \right)}{\left( \left( \dfrac{\pi}{2} \right)^{2}+\dfrac{\pi}{2} \right)^{2}}= \\
-\dfrac{2\left( \left( \dfrac{\pi}{2} \right)^{2}+\dfrac{\pi}{2} \right)}{\left( \left( \dfrac{\pi}{2} \right)^{2}+\dfrac{\pi}{2} \right)^{2}}=-\dfrac{2}{\dfrac{\pi^{2}}{4}+\dfrac{\pi}{2}}=-\dfrac{2}{\dfrac{\pi^{2}+2\pi}{4}}=-\dfrac{8}{\pi^{2}+2\pi}=-\dfrac{8}{\pi(\pi+2)} \\
 \\
t: y-0 = -\dfrac{8}{\pi(\pi+2)}\left( x-\dfrac{\pi}{2} \right)
\end{align}
$$
#### 3.
Decide the coordinates to the points on the curve $y=\dfrac{x+1}{x+2}$, in which the tangent line is parallel to the line $y=4x$
$$
\begin{align}
D_{f}=\mathbb{R}\setminus \{ -2 \}\\
f'(x)=\left( \dfrac{x+1}{x+2} \right)'=\dfrac{(x+1)'(x+2)-(x+1)(x+2)'}{(x+2)^{2}}=\dfrac{(x+1)-(x+2)}{(x+2)^{2}}=\dfrac{x+1-x-2}{(x+2)^{2}}= \\
\dfrac{-1}{(x+2)^{2}}=-\dfrac{1}{x^{2}+4x+4} \\
g(x)=(4x)'=4 \\
 \\
\left\{ \begin{array}{lll}
k_{t}=\dfrac{1}{(x+2)^{2}} \\
k_{t}=4
\end{array} \right. \iff \dfrac{1}{(x+2)^{2}}=4\iff 4(x+2)^{2}=1 \iff (x+2)^{2}=\dfrac{1}{4} \iff \\
x+2=\pm\dfrac{1}{2} \iff x=\pm \dfrac{1}{2}-2 \iff \left\{ \begin{array}{lll}
x_{1}=+\dfrac{1}{2}-2=-\dfrac{3}{2} \\
x_{2}=-\dfrac{1}{2}-2=-\dfrac{5}{2}
\end{array} \right.  \\
f\left( -\dfrac{3}{2} \right)=\dfrac{-\dfrac{3}{2}+1}{-\dfrac{3}{2}+2}=\dfrac{-\dfrac{1}{2}}{\dfrac{1}{2}}=-1 \\
f\left( -\dfrac{5}{2} \right)=\dfrac{-\dfrac{5}{2}+1}{-\dfrac{5}{2}+2}=\dfrac{-\dfrac{3}{2}}{-\dfrac{1}{2}}=3 \\
\left( -\dfrac{3}{2},-1 \right),\left( -\dfrac{5}{2},3 \right)
\end{align}
$$



