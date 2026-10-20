Blah blah, physics is applied mathematics, or connecting maths to reality

A function has a derivative in point $x_{0}$ if one can construct a non vertical tangent line in the coordinate point $(x_{0},f(x_{0}))$
the tangent lines angle coefficient is $f'(x_{0})$

The definition of derivative
$$
\begin{align}
f'(x_{0})=\lim_{ h \to 0 } \dfrac{f(x_{0}+h)-f(x_{0})}{h}
\end{align}
$$
The linear equation for the tangent line can be gotten through the single point formula
$$
\begin{align}
(y-y_{0})=k(x-x_{0})
\end{align}
$$
And as the angle $k$ is the same for the tangent as the derivative $f'(x_{0})$ the formula can become
$$
\begin{align}
(y-y_{0})=f'(x_{0})(x-x_{0})
\end{align}
$$

The normal line is a line that cuts the graph in a point $90\degree$ offset from the tangent, to get the slope, $k_{t}*k_{n}=-1$ as that's the relationship between the slope of two lines intersecting in a right angle. $k_{n}=-\dfrac{1}{k_{t}}$
Thus the equation for a normal becomes:
$$
\begin{align}
y-y_{1}=-\dfrac{1}{k_{t}}(x-x_{0})
\end{align}
$$


$$
\begin{align}
y-y_{0}=dy \\
x-x_{0}=dx \\
(y-y_{0})=f'(x_{0})(x-x_{0}) \\
dy=f'(x_{0})dx \\
\dfrac{dy}{dx}=f'(x_{0})
\end{align}
$$

$$
\begin{align}
y=f(x): \text{explicit function} \\
f(x,y)=0 : \text{implicit function}
\end{align}
$$
Implicit functions are functions where $y$ is to deeply ingrained in the function that it cant be broken out
## Exercises
#### 1
Decide $f'(x)$ where $f(x)=\sin ^{2}\left( \dfrac{x+1}{x-1} \right)$

$$
\begin{align}
f(x)=\sin ^{2}\left( \dfrac{x+1}{x-1} \right)=\left( \sin\left(\dfrac{x+1}{x-1} \right) \right)^{2} \\
 \\
(x^{2})'=2x \\
((f(x))^{2})'=2f(x)*f'(x) \\f'(x)g(x)-f(x)g'(x)
\text{division formula: } \left( \dfrac{f(x)}{g(x)} \right)'=\dfrac{f'(x)g(x)-f(x)g'(x)}{g^{2}(x)} \\
 \\
\left( \left( \sin\left(\dfrac{x+1}{x-1} \right) \right)^{2} \right)'=2\sin\left( \dfrac{x+1}{x-1} \right)*\left( \sin\left( \dfrac{x+1}{x-1} \right) \right)'= \\
2\sin\left( \dfrac{x+1}{x-1} \right)*\cos\left( \dfrac{x+1}{x-1} \right)*\left( \dfrac{x+1}{x-1} \right)'= \\
2\sin\left( \dfrac{x+1}{x-1} \right)*\cos\left( \dfrac{x+1}{x-1} \right)*\dfrac{1(x-1)-(x+1)1}{(x-2)^{2}} \\
\sin\left( \dfrac{2(x+1)}{x-1} \right)\dfrac{-2}{(x-1)^{2}}
\end{align}
$$
#### 4
Decide the equation for the for the tangent and normal line to the curve $f(x)=\dfrac{\cos(2x)}{x^{2}-x}$ in the point $\left( \dfrac{\pi}{4},0 \right)$

$$
\begin{align}
f\left( \dfrac{\pi}{4} \right)=\dfrac{\cos\left( \dfrac{\pi}{2} \right)}{\left( \dfrac{\pi}{4} \right)^{2}-\dfrac{\pi}{4}}=\dfrac{0}{\left( \dfrac{\pi}{4} \right)^{2}-\dfrac{\pi}{4}}=0 \\
\text{The formula falls on the graph, yippie :3} \\
t:y-0=f'\left( \dfrac{\pi}{4} \right)\left( x-\dfrac{\pi}{4} \right) \\
n:y-0=-\dfrac{1}{f'\left( \dfrac{\pi}{4} \right)}\left( x-\dfrac{\pi}{4} \right) \\
 \\
f'(x)=\ ? \\
f'\left( \dfrac{\pi}{4} \right)=k_{t} \\
 \\
 \left( \dfrac{f(x)}{g(x)} \right)'=\dfrac{f'(x)g(x)-f(x)g'()}{g^{2}(x)} \\
u=u(x) \\
(\cos(u)))'=-\sin(u)*u' \\
 \\
f'(x)=\dfrac{-\sin(2x)*2*(x^{2}-x)-\cos(2x)(2x-1)}{(x^{2}-x)^{2}} \\
f'\left( \dfrac{\pi}{4} \right)=\dfrac{-\sin\left( \dfrac{2\pi}{4} \right)*2*\left( \left( \dfrac{\pi}{4}^{2} \right)-\dfrac{\pi}{4} \right)-\cos\left( \dfrac{2\pi}{4} \right)\left( \dfrac{2\pi}{4}-1 \right)}{\left( \left( \dfrac{\pi}{4} \right)^{2}-\dfrac{\pi}{4} \right)^{2}}= \\
\dfrac{-2\left( \dfrac{\pi^{2}}{16} \right)-\dfrac{\pi}{4}}{\left( \dfrac{\pi^{2}}{16}-\dfrac{\pi}{4} \right)^{2}}=\dfrac{-2}{\dfrac{\pi^{2}}{16}-\dfrac{\pi}{4}}=\dfrac{-32}{\pi^{2}-4\pi}=k_{t} \\
 \\
l: y=-\dfrac{32}{\pi^{2}-4\pi}\left( x-\dfrac{\pi}{4} \right) \\
n: y=\dfrac{\pi^{2}-4\pi}{32}\left( x-\dfrac{\pi}{4} \right)
\end{align}
$$
#### 6
Show that the curves $y=x^{2}$ and $y=\dfrac{1}{\sqrt{ x }}$ meet each other in a right angle, motivate the answer using algebra
$$
\begin{align}
\left\{ \begin{array}{lll}
y=x^{2} \\
y=\dfrac{1}{\sqrt{ x }}
\end{array} \right. \iff x^{2}=\dfrac{1}{\sqrt{ x }}\iff x^{2}\sqrt{ x }=1\iff x^{4}x=1\iff x^{5}=1\iff x=1 \\
1^{2}=1 \\
\text{They intersect in }(1,1) \\
 \\
k_{x^{2}}=(x^{2})'=2x, y'(1)=2=k_{1} \\
k_{\frac{1}{\sqrt{ x }}}=y'=\left( \dfrac{1}{\sqrt{ x }} \right)'=(x^{-1/2})'=-\dfrac{1}{2}x^{-1/2-1},y'(1)=-\dfrac{1}{2}=k_{2} \\
k_{1}*k_{2}=2*\left( -\dfrac{1}{2} \right)=-1
\end{align}
$$
They intersect, and their tangents meet in a right angle