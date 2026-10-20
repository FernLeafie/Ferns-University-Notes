First degree equations are usually not full lines, but part, or parts of a line, limited by the domain

$$
\begin{align}
k=\dfrac{y_{2}-y_{1}}{x_{2}-x_{1}}=\dfrac{\Delta y}{\Delta x}=\tan \theta \\
y-y_{1}=k(x-x_{1}) \\
y-y_{1}=\dfrac{y_{2}-y_{1}}{x_{2}-x_{1}}(x-x_{1})
\end{align}
$$
the first degree equation based on a single point and angle, or two points without angle

if $P(a)=0$ then $a$ is a root of $P$, but $a$ is also a solution to the polynomial division $P(a)=0$

The factor theorem states that if $a$ is a root of $P$, then:
$$
\begin{align}
P(x)=(x-a)*Q(x)
\end{align}
$$

Theorem
for polynomials larger than the second degree, we can find one root $\dfrac{p}{q}$

## Lecture 4.5
a function must yield one output from one input, but one output may be achieved through several inputs.
If a function yields multiple outputs for an input, it's not a function
The domain or definition amount, is the values for which you can calculate the function, limited by the rules of maths.
For example, $y=\dfrac{1}{x}$ is defined as all $\mathbb{R}$ except $0$.
Codomain or target amount is the amount of possible outputs you can achieve, it is less important than the domain

## Discussion
#### 1.
$$
\begin{align}
\left\{ \begin{array}{lll}
y=x^{3}+4 \\
y=x^{2}+4x
\end{array} \right. \iff x^{3}+4=x^{2}+4x\iff x^{3}-x^{2}-4x+4=0
\end{align}
$$
Since all coefficients are integers, the function should have at least one real root in the form $\alpha=\dfrac{p}{q}$ where $p|a_{0}$ and $q|a_{n}$, so $p|4\iff p \in \{ \pm 1,\pm 2, \pm 4 \}$, and $q|1 \iff q \in \{ \pm 1 \}$ and $\alpha \in \{ \pm 1,\pm 2, \pm 4 \}$


$$
\begin{align}
& \alpha = -1 \implies -1-1+4+4\neq0 \\
& \alpha=1\implies 1-1-4+4=0
\end{align}
$$
$\alpha =1$ is a root!
long division time, the rest has to be 0 for the root to be true
$$
\begin{align}
\dfrac{x^{3}-x^{2}-4x+4}{x-1}=x^{2}-4
\end{align}
$$

$$
\begin{align}
x^{3}-x^{2}-4x+4=0\iff (x-1)(x^{2}-4)=0\iff \left\{ \begin{array}{lll}
x_{1}=1 \\
x_{2}=-2 \\
x_{3}=2
\end{array} \right. 
\end{align}
$$
we now know that intersections occur at all these $x$ so we can use the original equations to find all the coordinates of them
$$
\begin{align}
x_{1}=1\iff y=1+4=5  \\
x_{2}=-2\iff y=-8+4=-4 \\
x_{3}=2 \iff y=8+4=12
\end{align}
$$
answer: $(1,5),(-2,-4),(2,12)$

Attempt twoooo
$$
\begin{align}
x^{3}-x^{2}-4x+4=0\iff x^{2}(x-1)-4(x-1)=0\iff (x-1)(x^{2}-4)
\end{align}
$$
wow t hat was simple
#### 2.
Find the area of the inscribed rectangle in the ellipse $\dfrac{x^{2}}{4}+y^{2}=1$
$$
\begin{align}
\dfrac{x^{2}}{4}+y^{2}=1\iff \dfrac{x^{2}-0}{2^{2}}+\dfrac{y^{2}-0}{1^{2}}
\end{align}
$$
$M=(0,0)$ $a=2$ $b=1$
for this we need to find the point where $x=y$, as that is one corner and length of a half side

$$
\begin{align}
\dfrac{x^{2}}{4}+y^{2}=1\implies\dfrac{x^{2}}{4}+x^{2}=1\iff x^{2}+4x^{2}=4\iff 5x^{2}=4\iff x^{2}=\dfrac{4}{5}\iff x=\dfrac{2}{\sqrt{ 5 }}
\end{align}
$$
area of the square should then be $(2x)^{2}=\left( 2 \dfrac{2}{\sqrt{ 5 }} \right)^{2}=\dfrac{16}{5}$
#### 3.
decide all real roots for $P(x)=x^{5}+3x^{4}+x^{3}+3x^{2}-2x-6$
$$
\begin{align}
P(x)=x^{5}+3x^{4}+x^{3}+3x^{2}-2x-6=0\iff x^{4}(x+3)+x^{2}(x+3)-2(x+3)=0 \\
(x+3)(x^{4}+x^{2}-2)=0
\end{align}
$$
or
$\alpha \in \{ \pm 1 \pm 2 \pm 3 \pm 6 \}$

$$
\begin{align}
\alpha = 1 \implies P(\alpha)=0 \\
\alpha = -1 \implies P(\alpha)=0
\end{align}
$$

$$
\begin{align}
\dfrac{x^{5}+3x^{4}+x^{3}+3x^{2}-2x-6}{(x-1)(x+1)}=\dfrac{x^{5}+3x^{4}+x^{3}+3x^{2}-2x-6}{x^{2}-1}=x^{3}+3x^{2}+2x+6
\end{align}
$$


$$
\begin{align}
P(x)=(x-1)(x+1)(x+3)(x^{2}+2)
\end{align}
$$
so the real roots are $\left\{ \begin{array}{lll}x_{1}=1 \\  x_{2}=-1 \\  x_{3}=-3\end{array} \right.$
#### 4.
find the global minimum and max for the function $f(x)=\cos ^{2}x+7\cos x+7$
substitution!
$\cos(x)=t\in[-1,1]$

$$
\begin{align}
g(t)=t^{2}+7t+7
\end{align}
$$
square complete it to find minimum and max
$$
\begin{align}
g(t)=\left( t^{2}+2*\dfrac{7}{2}t+\left( \dfrac{7}{2} \right)^{2} \right)-\left( \dfrac{7}{2} \right)^{2}+7 \\
\left( t+\dfrac{7}{2} \right)^{2}-\dfrac{49-28}{4}=\left( t+\dfrac{7}{2} \right)^{2}-\dfrac{21}{4}
\end{align}
$$

$$
\begin{align}
&-1\leq x\leq1 &|+\dfrac{7}{2} \\
&\dfrac{5}{2}\leq x \leq \dfrac{9}{2} &|()^{2} \\
\end{align}
$$
Solve the equation $z^{4}-z^{3}+4z^{2}+3z+5=0$ if $z=1+2i$ is a solution
we know that $\bar{z}=1-2i$ is also a solution
$$
\begin{align}
(z-(1+2i))(z-(1-2i))=(z^{2}-z(1-2i)-z(1+2i)+(1+2i)(1-2i)) \\
(z^{2}-z((1-2i)+(1+2i))+(1+4))=(z^{2}-2z+5)
\end{align}
$$
too lazy to write long division again
$$
\begin{align}
\dfrac{z^{4}-z^{3}+4z^{2}+3z+5}{z^{2}-2z+5}=z^{2}+z+1
\end{align}
$$
quadratic formula that bitch!
$$
\begin{align}
z_{3,4}=-\dfrac{1}{2}\pm \sqrt{ \dfrac{1}{4}-1 }=-\dfrac{1}{2}\pm \sqrt{ -\dfrac{3}{4} }=-\dfrac{1}{2}\pm \dfrac{\sqrt{ 3 }}{2}i
\end{align}
$$
## Lecture 5

$$
\begin{align}
f\underbrace{ :A }_{ \text{Defined in A} }\underbrace{ \to B }_{ With values in B } \\
A \text{ is the domain} \\
B \text{ is the codomain}
\end{align}
$$
for polynomials $D(f)=\mathbb{R}$

 functions:
$$
\begin{align}
f:D(f)\to V(f)
\end{align}
$$
If you have a function where exponents are added, e.g. $e^{2x}+e^{-1}$, find a common value and substitute
## Discussion
#### 1?
a)
when undoing a logarithm we must check that the contents of the logarithm is positive
$$
\begin{align}
\ln\left( \dfrac{x^{3}-x^{2}-3x+5}{x+1} \right)=0\iff \dfrac{x^{3}-x^{2}-3x+5}{x+1} =e^{0}=1 \\
x^{3}-x^{2}-3x+5 =x+1\iff x^{3}-x^{2}-4x+1 =0
\end{align}
$$
b)
$$
\begin{align}
4^{1-2x}+3*4^{-x}-1=0\iff 4 \dfrac{1}{(4^{x})^{2}}+3\left( \dfrac{1}{4^{x}} \right)
\end{align}
$$
c)
solve $e^{ \ln(x-1)+2\ln(x+1) }=x^{2}+x-2$
method 1
$$
\begin{align}
e^{ \ln(x-1)+2\ln(x+1) }=x^{2}+x-2\iff \ln(e^{ \ln(x-1)+2\ln(x+1) })=\ln(x^{2}+x-2) \\
\ln(x-1)+2\ln(x+1)=\ln(x^{2}+x-2) \iff \ln(x-1)+\ln(x+1)^{2}=\ln(x^{2}+x-2) \\
\ln(x-1)(x+1)^{2}=\ln(x^{2}+x-2)\iff (x-1)(x+1)^{2}=x^{2}+x-2
\end{align}
$$
method 2

$$
\begin{align}
e^{ \ln(x-1)+2\ln(x+1) }=x^{2}+x-2\iff e^{ \ln(x-1)+\ln(x+1)^{2} }=x^{2}+x-2 \\
 e^{ \ln(x-1)(x+1)^{2} }=x^{2}+x-2 \iff (x-1)(x+1)^{2}=x^{2}+x-2
\end{align}
$$
method 3

$$
\begin{align}
e^{ \ln(x-1)+2\ln(x+1) }=x^{2}+x-2\iff e^{ \ln(x-1)}*e^{ 2\ln(x+1) }=x^{2}+x-2 \\
 e^{ \ln(x-1)}*e^{ \ln(x+1)^{2}}=x^{2}+x-2\iff  (x-1)*(x+1)^{2}=x^{2}+x-2
\end{align}
$$


$$
\begin{align}
(x-1)(x+1)^{2}=x^{2}+x-2
\end{align}
$$
short method (factorise the other side as opposed to writing out the third degree polynomial)
$$
x^{2}+x-1=0\iff \left\{ \begin{array}{lll}
x_{1}=1 \\
x_{2}=-2
\end{array} \right. 
$$
don't simplify away any solutions!
$$
\begin{align}
(x-1)(x+1)^{2}=x^{2}+x-2 \iff (x-1)(x+1)^{2}=(x-1)(x+2) \\
(x-1)(x+1)^{2}-(x-1)(x+2)=0\iff (x-1)((x+1)^{2}-(x+2))=0
\end{align}
$$
All solutions are false as they are under 1, and they need to be over to yield positive logarithms
$$
\begin{align}
x \in \varnothing
\end{align}
$$
Derived from [[Lectures]]
