### Generalised Integrals
#### Calculation of Area Between Curves
$$
\begin{align}
A=\int_{a}^{b} (f(x)-g(x)) \, dx 
\end{align}
$$
To prevent getting a negative area if we accidentally reverse the order of the functions, we can take the absolute value of the expression.
$$
\begin{align}
A=\left| \int_{a}^{b} (f(x)-g(x)) \, dx \right| 
\end{align}
$$
![[6 - Applications of Integrals 2026-11-25 08.25.30.excalidraw]]
#### Volume for Rotation Bodies
Rotation around the ${}x{}$-axis
$$
\begin{align}
V=\int_{a}^{b} \pi(f(x))^{2} \, dx 
\end{align}
$$
Rotation around the ${}y{}$-axis
$$
\begin{align}
V=\int_{a}^{b} 2\pi xf(x) \, dx 
\end{align}
$$
#### Arc Length
We can approximate the curve as if it is made up of infinitely many short angled segments, a bit like how the integral works.
![[6 - Applications of Integrals 2026-11-25 08.32.19.excalidraw]]
Using the Pythagorean theorem ${}\Delta x^{2}+\Delta y^{2}=\Delta s^{2}{}$
$$
\begin{align}
\Delta s \approx \sqrt{ (\Delta x)^{2}+(\Delta y)^{2} }=\sqrt{ (\Delta x)^{2}\left( 1+\left( \dfrac{\Delta y}{\Delta x} \right)^{2} \right) } \\
=\sqrt{ 1+\left( \dfrac{\Delta y}{\Delta x} \right)^{2} }\Delta x \\
{ \Delta x \to 0 } \text{ gives } ds=\sqrt{ 1+(f'(x))^{2} } \,dx \\
s=\int_{a}^{b}  \, ds =\int_{a}^{b} \sqrt{ 1+(f'(x))^{2} } \, dx  \\
s = \int_{a}^{b} \sqrt{ 1+(f'(x))^{2} } \, dx 
\end{align}
$$
### Example
Calculate the length of the curve ${}y=\sqrt{ 4-x^{2} }{}$ for ${}-2 \leqslant x\leqslant 1{}$
#### Solution
$$
\begin{align}
y=\sqrt{ 4-x^{2} }=f(x)=(4-x^{2})^{1/2} \\
f'(x)=\dfrac{1}{2}(4-x^{2})^{-1/2}(-2x) \\
= -x(4-x^{2})^{-1/2} = -\dfrac{x}{\sqrt{ 4-x^{2} }} \\
 \\
s=\int_{-2}^{1} \sqrt{ 1+\left( -\dfrac{x}{\sqrt{ 4-x^{2} }} \right)^{2} } \, dx  \\
=\int_{-2}^{1} \sqrt{ 1+\dfrac{x^{2}}{ 4-x^{2} } } \, dx  \\
=\int_{-2}^{1} \sqrt{ \dfrac{4-x^{2}}{4-x^{2}}+\dfrac{x^{2}}{ 4-x^{2} } } \, dx  \\
=\int_{-2}^{1} \sqrt{ \dfrac{4}{ 4-x^{2} } } \, dx  \\
=\int_{-2}^{1}  \dfrac{2}{ \sqrt{4-x^{2}} } \, dx  \\
=2\int_{-2}^{1}  \dfrac{1}{ \sqrt{4-x^{2}} } \, dx  \\
\text{Remember: } \int \dfrac{1}{\sqrt{ 1-x^{2} }} \, dx =\arcsin(x)+C \\
\int \dfrac{1}{ \sqrt{4-x^{2}} } \, dx \\
=\int \dfrac{1}{ \sqrt{4\left( 1-\dfrac{x^{2}}{4} \right)} } \, dx =\int \dfrac{1}{\sqrt{ 4 }}\times \dfrac{1}{\sqrt{ 1-\dfrac{x^{2}}{4} }} \, dx  \\
=\int \dfrac{1}{2}\times \dfrac{1}{\sqrt{ 1-\left( \dfrac{x}{2} \right)^{2} }} \, dx = \dfrac{1}{2}\int \dfrac{1}{\sqrt{ 1-\left( \dfrac{x}{2} \right)^{2} }} \, dx  \\
=\left[ \begin{array}{c}
t=\dfrac{x}{2} \\
\sqrt{ 1-t^{2} }=\sqrt{ 1-\left( \dfrac{x}{^{2}} \right)^{2} } \\
dt=\dfrac{1}{2}dx
\end{array} \right] = \int \dfrac{1}{\sqrt{ 1-t^{2} }} \, dt \\
= \arcsin(t)+C = \arcsin\left( \dfrac{x}{2} \right) +C \\
s=2\int_{-2}^{1} \dfrac{1}{\sqrt{ 4-x^{2} }} \, dx =2\left[ \arcsin\left( \dfrac{x}{2} \right) \right]_{-2}^{1} \\
=2\arcsin\left( \dfrac{1}{2} \right)-2\arcsin(-1) \\
=2 \dfrac{\pi}{6}-2 \left( -\dfrac{\pi}{2} \right) =\dfrac{\pi}{3}+\pi =\dfrac{4\pi}{3}
\end{align}
$$
Alternatively, we could interpret the exercise a little differently.
$$
\begin{align}
y=\sqrt{ 4-x^{2} } \\
y^{2}=4-x^{2} \\
x^{2}+y^{2}=4
\end{align}
$$
This is a circle, so the arc of a curve is an arc segment.
![[6 - Applications of Integrals 2026-11-25 08.56.56.excalidraw]]
$$
\begin{align}
s=r\times \theta \implies s=2\times \dfrac{2\pi}{3}=\dfrac{4\pi}{3}
\end{align}
$$