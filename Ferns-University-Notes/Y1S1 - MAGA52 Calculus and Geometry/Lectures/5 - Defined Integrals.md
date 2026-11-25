After this lecture, there's a recorded lecture covering area and volume.
### Problem
![[5 - Defined Integrals 2026-11-20 08.20.27.excalidraw]]
${}y=f(x)>0{}$
The area above the ${}x{}$-axis, below ${}y=f(x){}$, between ${}x=a{}$ and ${}x=b{}$.
Does the area exist?
An area under a graph can be approximated with a multitude of rectangles aligned to the graph.
![[5 - Defined Integrals 2026-11-20 08.32.03.excalidraw]]
If the span is divided in ${}n{}$ segments, then the width of one column is ${}\dfrac{b-a}{n}=\Delta x{}$.
The area of one column comes out to the function value, in this case ${}x_{k}{}$, times the width, ${}\Delta A=f(x_{k})\Delta x{}$.
So an approximation of the area comes out to:
$$
\begin{align}
\text{sought area}\approx \sum_{k=1}^{n} f(x_{k})\Delta x 
\end{align}
$$
This is called the Riemann sum.
The more rectangles we use, the higher ${}n{}$, the smaller ${}\Delta x{}$, the better approximation.
If we use an infinite number of rectangles, or infinity narrow rectangles, the approximation should logically be exact.
$$
\begin{align}
\text{Sought area} = \lim_{ \Delta x \to 0 } \sum f(x_{k})\Delta x
\end{align}
$$
This is the limit of the Riemann sum, or the Riemann integral, also called the defined integral.
The limit exists for "kind" functions (continuous functions). It can also be written as:
$$
\begin{align}
\int_{a}^{b} f(x) \, dx 
\end{align}
$$
The defined integral, where ${}a{}$ is the start of the span, and ${}b{}$ is the end of the span.
It's pronounced "The integral from $a$ to $b$ of ${}f(x){}$", ${}a{}$ and ${}b{}$ are called **limits**.

If ${}f(x)>0,a<x<b{}$. Then the formula ${}\int_{a}^{b} f(x) \, dx{}$ gives the area of the area between the graph and the ${}x{}$-axis, between ${}x=a{}$ and ${}x=b{}$
### Two Integrals
$$
\begin{align}
\int f(x) \, dx  & =\text{undefined integral} \\
 & =\text{primitive function} \\
 & = \text{anti derivative} \\
 & = \text{the function } F(x)+C \\
 & \text{so that }F'(x)=f(x)
\end{align}
$$
$$
\begin{align}
\int_{a}^{b} f(x) \, dx  & =\text{defined integral} \\
 & =\text{a number}
\end{align}
$$
So a defined integral, is an undefined integral with limits. Now how do they correlate?
**The fundamental theorem of calculus**
Says that:
$$
\begin{align}
\int_{a}^{b} f(x) \, dx =F(b)-F(a)
\end{align}
$$
So we can express the limit of a Riemann sum as the relation of the primitive functions of the limits.
We can write ${}F(b)-F(a){}$ a little differently with this notation, as it comes up a lot:
$$
\begin{align}
F(b)-F(a)=[F(x)]_{a}^{b}
\end{align}
$$
### Example
Calculate the area under ${}y=x^{2}{}$ above the ${}x{}$-axis between ${}x=1{}$ and ${}x=2{}$.
#### Solution
$$
\begin{align}
\int_{1}^{2} x^{2} \, dx =\left[ \dfrac{x^{3}}{3} \right]_{1}^{2}=\dfrac{2^{3}}{3}-\dfrac{1^{3}}{3}=\dfrac{8}{3}-\dfrac{1}{3}=\dfrac{7}{3}
\end{align}
$$
We've now essentially done really complicated Riemann sum limits, with relatively simple maths, thanks to the fundamental theorem of calculus.
We don't have to include ${}C{}$, as the ${}+C{}$ of ${}F(b){}$ is taken out by the ${}C{}$ of ${}-F(a){}$, as it's the same primitive function, and thus the same ${}C{}$.

### Useful Notation
$$
\begin{align}
\Delta A=f(x_{k})\Delta x \\
\Delta x\to 0 \\
dA =f(x)\,dx \\
A=\int_{a}^{b}  \, dA =\int_{a}^{b} f(x) \, dx 
\end{align}
$$
$$
\begin{align}
\Delta V=\pi f(x_{k})^{2}\Delta x \\
dV=\pi f(x)^{2}\,dx \\
V=\int_{a}^{b}  \, dV =\int_{a}^{b} \pi f(x)^{2} \, dx =\pi\int_{a}^{b} f(x)^{2} \, dx 
\end{align}
$$
What happens if ${}f(x){}$ passes through the ${}x{}$-axis, or switches signs.

Good question, gotta experiment with that, seems like the area under the ${}x{}$-axis, turns out negative, so if you want the full area, without it nullifying, you might have to take ${}\text{positive area}-\text{negative area}{}$

### Properties
$$
\begin{align}
\int_{a}^{b} (f(x)\pm g(x)) \, dx =\int_{a}^{b} f(x) \, dx \pm \int_{a}^{b} g(x) \, dx  \\
\int_{a}^{b} kf(x) \, dx =k\int_{a}^{b} f(x) \, dx  \\
\text{if }a<x_{0}<b \text{ then} \\
\int_{a}^{b} f(x) \, dx =\int_{a}^{x_{0}} f(x) \, dx +\int_{x_{0}}^{b} f(x) \, dx 
\end{align}
$$
The last one gets pretty obvious when we draw a graph.
$$
\begin{align}
\int_{b}^{a} f(x) \, dx =-\int_{a}^{b} f(x) \, dx 
\end{align}
$$
This is called the orientation of integration.
$$
\begin{align}
\text{if } f(x)\leqslant g(x) \text{ then} \\
\int_{a}^{b} f(x) \, dx \leqslant \int_{a}^{b} g(x) \, dx  
\end{align}
$$
### Example
Calculate ${}\int_{0}^{\pi/3} \tan(x) \, dx{}$
#### Solution 1
$$
\begin{align}
\int_{0}^{\pi/3} \tan(x) \, dx = F\left( \dfrac{\pi}{3} \right)-F(0) \\
\text{where } F(x)=\int \tan(x) \, dx 
\end{align}
$$
We calculate the undefined integrals first, and then insert the limits
$$
\begin{align}
\int \tan(x) \, dx =\int \dfrac{\sin(x)}{\cos(x)} \, dx =\int \sin(x)\times \dfrac{1}{\cos(x)} \, dx = \\
\left[ \begin{array}{ccc}
t=\cos(x) \\
\dfrac{1}{t}=\cos(x) \\
\dfrac{dt}{dx}=-\sin(x)\iff-dt=\sin(x)dx
\end{array} \right] =\int \dfrac{1}{t}(-1) \, dt=-\int \dfrac{1}{t} \, dt =-\ln|t|+C= \\
-\ln|\cos(x)|+C 
\end{align}
$$
$$
\begin{align}
\int_{0}^{\pi/3} \tan(x) \, dx = [-\ln|\cos(x)|]_{0}^{\pi/3}= \\
=-\ln| \dfrac{1}{2}|-(-\ln|1|)=-\ln \left( \dfrac{1}{2}\right)=\ln(2)
\end{align}
$$
#### Solution 2
$$
\begin{align}
\int_{0}^{\pi/3} \tan(x) \, dx =\int_{0}^{\pi/3} \dfrac{\sin(x)}{\cos(x)} \, dx =\left[ \begin{array}{ccc}
t=\cos(x) \\
-dt=\sin(x)dx \\
x=0\implies t=\cos(0)=1 \\
x=\dfrac{\pi}{3}\implies \cos\left( \dfrac{\pi}{3} \right)=\dfrac{1}{2}
\end{array} \right] = \\
\int_{1}^{1/2} \dfrac{1}{t} \, dt =\int_{1/2}^{1} \dfrac{1}{t} \, dt =[\ln|t|]_{1 /2}^{1}=\ln 1-\ln\left( \dfrac{1}{2} \right)=\ln (2)
\end{align}
$$
The benefits of solution 2 is that we don't have to translate back to ${}x{}$, at the cost of having to translate the limits.