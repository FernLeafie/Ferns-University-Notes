## Examples
$f:A\to B$ $g:C\to D$
$$
h(x)=(g\circ f)=g(f(x))
$$

$$
\begin{align}

\end{align}
$$
Let $f(x)=\ln(x-1)$ and $g(x)=\sqrt{ x }$
a) decide the domain($D(x)$) and range ($V(x)$) of $f$ and $g$
$$
\begin{align}
D_{f} = (1,\infty) \\
V_{f} = \mathbb{R} \\
D_{g}= [0,\infty) \mid  D_{g}= \{ x\geq0 \} \mid D_{g}: x\geq0 \mid D_{g} = \mathbb{R}_{+} \cup \{ 0 \} \\
V_{g} = [0,\infty)
\end{align}
$$
b)
Decide the domain and range of $h(x)=(g\circ f)(x)$ 

$$
\begin{align}
V_{f} \not\subset D_{g}
\end{align}
$$

$$
\begin{align}
g(f(x))=\sqrt{ \ln(x-1) }
\end{align}
$$

$$
\begin{align}
D_{h} = [2,\infty)
\end{align}
$$
Since $x>0$ due to $\ln$ needing positive values, and since the $\sqrt{  }$ requires postive values, $\ln(x-1)\geq 0 \iff x-1\geq e^{ 0 }=1 \iff x\geq 2$, and $(1,\infty)\cap[2,\infty)=[2,\infty)$

Let $f(x)=2\sin x$ and $g(x)=\sqrt{ 1-x^{2} }$
a) find the domain of $f$ and $g$
$$
\begin{align}
D_{f} = \mathbb{R} \\
V_{f} = [-2,2] \\
D_{g} = [-1,1] \\
V_{f} = [0,1]
\end{align}
$$
b) limit the domain so that $(g\circ f)$ is possible, decide $(g\circ f)(x)$ and the domain
$$
\begin{align}
(g \circ f)(x)=\sqrt{ 1-(2\sin x)^{2} }=\sqrt{ 1-4\sin ^{2}x }
\end{align}
$$

$$
\begin{align}
1-4\sin ^{2} x\geq 0 \\
(1-2\sin x)(1+2\sin x) \geq 0 \\
\sin x=t, t\in[-1,1] \\
(1-2t)(1+2t) \geq 0 \\
\end{align}
$$

|        $t$        | $-1$ | $-\dfrac{1}{2}$ |     | $\dfrac{1}{2}$ | $1$ |
| :---------------: | :--: | :-------------: | :-: | :------------: | :-: |
|      $1-2t$       |  +   |        +        |  +  |       0        |  -  |
|      $1+2t$       |  -   |        0        |  +  |       +        |  +  |
| $\mathrm{L.H.S.}$ |  -   |        0        |  +  |       0        |  -  |

$$
\begin{align}
-\dfrac{1}{2} \leq \sin x\leq \dfrac{1}{2} \\
\end{align}
$$

$$
\begin{align}
x \in\left[ -\dfrac{\pi}{6}+2\pi n,\dfrac{\pi}{6}+2\pi n \right] \cup \left[ \dfrac{5\pi}{6}+2\pi n,\dfrac{7\pi}{6}+2\pi n \right]=\left[ -\dfrac{\pi}{6}+\pi n,\dfrac{\pi}{6}+\pi n \right]
\end{align}
$$

$$
\begin{align}
D_{(g\circ f)}=\left[ -\dfrac{\pi}{6}+\pi n,\dfrac{\pi}{6}+\pi n \right]
\end{align}
$$

Derived from [[Lectures]]