The trigonometric functions are clearly not inversible, as multiple $x$ correspond to a single $y$.
Thus, the domain of the inverse function must be limited
$$
\begin{align}
\sin:\left[ -\dfrac{\pi}{2},\dfrac{\pi}{2} \right]\to[-1,1] \\
\arcsin:[-1,1]\to\left[ -\dfrac{\pi}{2},\dfrac{\pi}{2} \right]
\end{align}
$$

$$
\begin{align}
f(x)=y \\
f^{-1}(y)=x
\end{align}
$$

$$
\begin{align}
f^{-1}(f(x))=x \\
f(f^{-1}(x))=x
\end{align}
$$

$$
\begin{align}
\ln (e^{ x })=x \\
e^{ \ln x }=x
\end{align}
$$
Arcus is Latin for angles, as arc functions take numbers and returns angles
$$
\begin{align}
\enclose{box}{\sin(\arcsin(x))=x} & | x \in [-1,1] \\
\enclose{box}{\arcsin(\sin(x))=x} & | x \in \left[ -\dfrac{\pi}{2},\dfrac{\pi}{2} \right]
\end{align}
$$

$$
\begin{align}
\arcsin(-x)=-\arcsin(x)
\end{align}
$$

### Cosine
$$
\begin{align}
\cos:[0,\pi]\to[-1,1] \\
\arccos:[-1,1]\to[0,\pi]
\end{align}
$$
These relationships can easily be gotten from a graph or a unit circle.
$$
\begin{align}
\enclose{box}{\cos(\arccos(x))=x} & | x \in [-1,1] \\
\enclose{box}{\arccos(\cos(x))=x} & | x \in [0,\pi]
\end{align}
$$

This can easily be visualised with the unit circle
$$
\begin{align}
\arccos(-x)=\pi-\arccos(x)
\end{align}
$$
### Cotan
Imagine the tan graph:
$$
\begin{align}
\tan:\left( -\dfrac{\pi}{2},\dfrac{\pi}{2} \right)\to \mathbb{R} \\
\arctan:\mathbb{R}\to\left( -\dfrac{\pi}{2},\dfrac{\pi}{2} \right)
\end{align}
$$

$$
\begin{align}
\enclose{box}{\tan(\arctan(x))=x} & | x \in \mathbb{R} \\
\enclose{box}{\arctan(\tan(x))=x} & | x \in \left( -\dfrac{\pi}{2},\dfrac{\pi}{2} \right)
\end{align}
$$



$$
\begin{align}
\cos(\arcsin(x))=\sqrt{ 1-x^{2} } \\
\sin(\arccos(x))=\sqrt{ 1-x^{2} }
\end{align}
$$
This is derived from the pythegorian identity
$$
\begin{align}
\cos ^{2}(\arcsin x)&=1-\sin ^{2}(\arcsin x) \\
&=1-(\sin (\arcsin x))^{2} \\
&=1-x^{2} \\
\cos(\arcsin x)&=\sqrt{ 1-x^{2} }
\end{align}
$$
(looking at the trigonometric circle, cos is just positive on the output range of arcsin, this only $+\sqrt{  }$ is kept)


Geometry say that
$$
\begin{align} \\
\sin(\arctan(x))=\dfrac{x}{\sqrt{ x^{2}+1 }}
\cos(\arctan(x))=\dfrac{1}{\sqrt{ x^{2}+1 }}
\end{align}
$$
### Examples
#### Example 1
Decide $\arcsin\left( \cos\left( \dfrac{5\pi}{3} \right) \right)$

$$
\begin{align}
\cos\left( \dfrac{5\pi}{3} \right)=\sin\left( \dfrac{\pi}{2}-\dfrac{5\pi}{3} \right)=\sin\left( \dfrac{3\pi}{6}-\dfrac{10\pi}{6} \right) \\
\sin\left( -\dfrac{7\pi}{6} \right)=-\sin\left( \dfrac{7\pi}{6} \right)=-\sin\left( \pi+\dfrac{\pi}{6} \right)=\sin\left( \dfrac{\pi}{6} \right) \\
 \\
\arcsin\left( \cos\left( \dfrac{5\pi}{3} \right) \right)=\arcsin\left( \sin\left( \dfrac{\pi}{6} \right) \right)=\dfrac{\pi}{6}
\end{align}
$$
#### Example 2
Decide $\cos\left( 2\arctan\left( \dfrac{1}{3} \right) \right)$

$$
\begin{align}
\cos\left( 2\arctan\left( \dfrac{1}{3} \right) \right)=1-2\sin ^{2}\left( \arctan\left( \dfrac{1}{3} \right) \right) \\
1-2\left( \dfrac{\dfrac{1}{3}}{\sqrt{ \left( \dfrac{1}{3} \right)^{2}+1 }} \right)^{2}=1-2\dfrac{\left( \dfrac{1}{3} \right)^{2}}{\left( \dfrac{1}{3} \right)^{2}+1} \\
1-2\dfrac{\dfrac{1}{9}}{\dfrac{1}{9}+1}=1-2 \dfrac{\dfrac{1}{9}}{\dfrac{10}{9}}=1-2\dfrac{1}{9}*\dfrac{9}{10}=1-\dfrac{2}{10}=\dfrac{4}{5}
\end{align}
$$
#### Example 3
Decide $\tan\left( \arcsin\left( -\dfrac{1}{4} \right) \right)$

$$
\begin{align}
\tan\left( \arcsin\left( -\dfrac{1}{4} \right) \right)=\dfrac{\sin\left( \arcsin\left( -\dfrac{1}{4} \right) \right)}{\cos\left( \arcsin\left( -\dfrac{1}{4} \right) \right)}=\dfrac{-\dfrac{1}{4}}{\sqrt{ 1-\sin ^{2}\left( \arcsin\left( -\dfrac{1}{4} \right) \right) }} \\
\dfrac{-\dfrac{1}{4}}{\sqrt{ 1-\left( -\dfrac{1}{4} \right)^{2} }}=\dfrac{-\dfrac{1}{4}}{\sqrt{ 1-\left( \dfrac{1}{16} \right) }}=\dfrac{-\dfrac{1}{4}}{\dfrac{\sqrt{ 15 }}{4}}=-\dfrac{1}{\sqrt{ 15 }}
\end{align}
$$
#### Example 4
a)
Decide the domain and range for $f(x)=-2\arccos\left( 1+\dfrac{1}{x} \right)+1$
range:
$\arccos:[-1,1]\to[0,\pi]$

$$
\begin{align}
0\leq \arccos\left( 1+\dfrac{1}{x} \right)\leq \pi \\
0\geq-2\arccos\left( 1+\dfrac{1}{x} \right)\geq-2\pi \\
1\geq-2\arccos\left( 1+\dfrac{1}{x} \right)+1\geq1-2\pi \\
V_{f}=[1-2\pi,1]
\end{align}
$$
domain:
$$
\begin{align}
-1\leq 1+\dfrac{1}{x}\leq 1 \cap x \neq 1 \\
\left\{ \begin{array}{lll}
1+\dfrac{1}{x}\leq1 \\
1+\dfrac{1}{x}\geq -1
\end{array} \right. =\left\{ \begin{array}{lll}
x \in(-\infty,0) \\
x \in \left(-\infty,-\dfrac{1}{2}\right] \cup(0,\infty)
\end{array} \right. =x=(-\infty,-1.2] \\
D_{f}=\left( -\infty,-\dfrac{1}{2} \right]
\end{align}
$$
b) 
Decide range and domain for $g(x)=\dfrac{1}{2x-1}$
domain:
$$
\begin{align}
D_{g}=\mathbb{R}\setminus \left\{  \dfrac{1}{2}  \right\} \\
D_{g}=\left\{  x \in \dfrac{\mathbb{R},x\neq_{1}}{2}  \right\} \\
D_{g}: x\neq \dfrac{1}{2}
\end{align}
$$
range:
$$
\begin{align}
V_{g}=\mathbb{R}\setminus \{ 0 \} \\
V_{g}: y\neq 0
\end{align}
$$
c)
Decide $(f\circ g)(x)$, the domain of $(f\circ g)$. Limit the domain of $g$ so that $( f\circ g)$ can be calculated
$$
\begin{align}
(f\circ  g)(x)=f(g(x))=-2\arccos\left( 1+\dfrac{1}{\dfrac{1}{2x-1}} \right)+1 \\
= -2\arccos(2x)+1, x\neq \dfrac{1}{2} \\
-1\leq2x\leq1 \\
-\dfrac{1}{2}\leq x \leq \dfrac{1}{2} \\
D_{f\circ g}=\left[ -\dfrac{1}{2}, \dfrac{1}{2} \right]\cap x\neq \dfrac{1}{2}=\left[ -\dfrac{1}{2}, \dfrac{1}{2} \right)=D_{g_{\text{limited}}}
\end{align}
$$
d)
Find the inverse of $f$
$$
\begin{align}
f(x)=y \\
-2\arccos\left( 1+\dfrac{1}{x} \right)+1=y \\
-2\arccos\left( 1+\dfrac{1}{x} \right)=y-1 \\
\arccos\left( 1+\dfrac{1}{x} \right)=\dfrac{y-1}{-2} \\
1+\dfrac{1}{x}=\cos\left( \dfrac{y-1}{-2} \right) \\
\dfrac{1}{x}=\cos\left( \dfrac{y-1}{-2} \right)-1 \\
x=\dfrac{1}{\cos\left( \dfrac{y-1}{-2} \right)-1}=f^{-1}(y)
\end{align}
$$


Derived from [[Lectures]]