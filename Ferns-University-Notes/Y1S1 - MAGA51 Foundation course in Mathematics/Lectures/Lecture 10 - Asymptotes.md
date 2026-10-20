---
color: ""
---
lost on windows
$$
\begin{align}
(a^{3}-b^{3})=(a-b)(a^{2}+ab+b^{2})
\end{align}
$$
$$
\begin{align}
\lim_{ x \to 0 } \dfrac{\sin x}{x}=1 \\
\lim_{ x \to a } \dfrac{\sin f(x)}{f(x)}=1\iff  x\to a,f(x)\to0 \\
\lim_{ x \to 0 } \dfrac{e^{ x }-1}{x}=1 \\
\lim_{ x \to a } \dfrac{e^{ f(x) }-1}{f(x)}=1\iff  x\to a,f(x)\to0 \\
\lim_{ x \to 0 } \dfrac{\ln(1+x)}{x}=1 \\
\lim_{ x \to a } \dfrac{\ln(1+f(x))}{f(x)}=1\iff  x\to a,f(x)\to0
\end{align}
$$
### Horizontal asymptotes
$$
\begin{align}
\lim_{ x \to \infty }f(x)=k, k\in \mathbb{R} \\
\lim_{ x \to -\infty }f(x)=k, k\in \mathbb{R}
\end{align}
$$
### Oblique asymptotes
Diagonal asymptotes where as the value of a function approaches infinity or negative infinity, resembles a linear function $f(x)=ax+b$, where the parameters can be decided through:
$$
\begin{align}
a=\lim_{ x \to \pm\infty }\dfrac{f(x)}{x} \\
b=\lim_{ x \to \pm\infty } (f(x)-ax) 
\end{align}
$$
If a function lacks horizontal asymptotes, it can have oblique asymptotes.
### Vertical asymptotes
## Exercises
#### 1
Decide the constants $a$ and $b$ so that the function $f$ has a limit in $x=-3$, expand the function so that it becomes continuous in $x=-3$.

$$
\begin{align}
f(x)=\left\{ \begin{array}{lll}
2a-\dfrac{x^{2}-9}{3-|x|},& x<-3 \\
\dfrac{12b\tan(x+3)}{9-x^{2}},&x>-3
\end{array} \right. 
\end{align}
$$
$$
\begin{align}
l_{l}=\lim_{ x \to -3^{-} } 2a-\dfrac{x^{2}-9}{3-|x|}=2a-\lim_{ x \to -3^{-} }\dfrac{x^{2}-9}{3+x}=2a-\lim_{ x \to -3^{-} }\dfrac{\cancel{ (x+3) }(x-3)}{\cancel{ (3+x) }}=2a-``-3-3 "=2a-6
\end{align}
$$
$$
\begin{align}
l_{r}=\lim_{ x \to -3^{+} }\dfrac{12b\tan(x+3)}{9-x^{2}}=12b \times\lim_{ x \to -3^{+} }\dfrac{\tan(x+3)}{9-x^{2}}=12b \times \lim_{ x \to -3^{+} } \dfrac{\tan(3+x)}{(3-x)(3+x)} \\
12b \times \lim_{ x \to -3^{+} } \dfrac{\tan(3+x)}{(3+x)} \dfrac{1}{(3-x)}=12b``1*\dfrac{1}{3-(-3)} "=\dfrac{12b}{6}=2b
\end{align}
$$
A limit exists in $-3$ when $l_{l}=l_{r}$
$$
\begin{align}
l_{l}=l_{r}\iff 2a-6=2b\iff a-3=b
\end{align}
$$
Let the expansion of $f$ be:
$$
\begin{align}
g(x)=\left\{ \begin{array}{lll}
2a-\dfrac{x^{2}-9}{3-|x|},& x<-3 \\
2a-6,& x=-3 \\
12(a-3)\dfrac{\tan(x+3)}{9-x^{2}},& x>-3
\end{array} \right. 
\end{align}
$$
#### 1 alt
Decide $a$ and $b$ so that $f$ is a continuous function
$$
\begin{align}
f(x)=\left\{ \begin{array}{lll}
\dfrac{\arctan(x^2-9)}{(27-x^3)},& x < 3 \\
ax+b,& x = 3 \\
\dfrac{e^{3a(x-3)}-1}{\ln((x-2)^2)},& x > 3
\end{array} \right. 
\end{align}
$$



Derived from [[Lectures]]