## Generalised Integrals
Generalised integrals are integrals that have a limit which tend towards infinity on one or the other side, or towards an undefined point of the function. But mostly because they tend towards infinity in the upper limit
$$
\begin{align}
\int_{a}^{\infty} f(x) \, dx =\lim_{ R \to \infty } \int_{a}^{R} f(x) \, dx 
\end{align}
$$
If this limit *exists*, and is *finite*. We call the generalised integral *convergent*, otherwise we call the integral *divergent*.
### Example
Decide if the generalised integral ${}\int_{1}^{\infty} \frac{1}{1+x^{2}} \, dx{}$ is convergent or divergent.
#### Solution
$$
\begin{align}
\int_{1}^{R} \dfrac{1}{1+x^{2}} \, dx =[\arctan(x)]_{1}^{R}=\arctan(R)-\arctan(1) \\
=\arctan(R)-\dfrac{\pi}{4} \\
\int_{1}^{\infty} \dfrac{1}{1+x^{2}} \, dx =\lim_{ R \to \infty } \int_{1}^{R} \dfrac{1}{1+x^{2}} \, dx  \\
=\lim_{ R \to \infty } \left( \arctan(R)-\dfrac{\pi}{4} \right)=(\lim_{ R \to \infty } \arctan(R))-\dfrac{\pi}{4} \\
=\dfrac{\pi}{2}-\dfrac{\pi}{4}=\dfrac{\pi}{4}
\end{align}
$$
The integral is convergent and has the value ${}\dfrac{\pi}{4}{}$.
### Example
Decide if the generalised integral ${}\int_{2}^{\infty} \frac{1}{x} \, dx{}$, is convergent or divergent.
#### Solution
$$
\begin{align}
\int_{2}^{\infty} \dfrac{1}{x} \, dx =\lim_{ R \to \infty } \int_{2}^{R} \dfrac{1}{x} \, dx  \\
=\lim_{ R \to \infty } [\ln|x|]_{2}^{R}=\lim_{ R \to \infty } (\ln(R)-\ln(2)) \\
=(\lim_{ R \to \infty } \ln(R))-\ln(2)=\infty
\end{align}
$$
The integral is divergent.

### Logic
${}\int_{a}^{\infty} f(x) \, dx{}$ is convergent if ${}\lim_{ R \to \infty }\int_{a}^{R} f(x) \, dx{}$ exists, *and* is finite.
${}\int_{a}^{\infty} f(x) \, dx{}$ is divergent if ${}\lim_{ R \to \infty }\int_{a}^{R} f(x) \, dx{}$ doesn't exists, *or* isn't finite.
or expressed with logical operators
${}\int_{a}^{\infty} f(x) \, dx{}$ is convergent if ${}\exists\lim_{ R \to \infty }\int_{a}^{R} f(x) \, dx \land \lim_{ R \to \infty }\int_{a}^{R} f(x) \, dx \in \mathbb{R}{}$ .
${}\int_{a}^{\infty} f(x) \, dx{}$ is divergent if ${}\nexists\lim_{ R \to \infty }\int_{a}^{R} f(x) \, dx \lor \lim_{ R \to \infty }\int_{a}^{R} f(x) \, dx \not\in \mathbb{R}{}$ .

### P-Integral
The integral:
$$
\begin{align}
\int_{1}^{\infty} \dfrac{1}{x^{p}} \, dx , &  &  p>0
\end{align}
$$
$$
\begin{align}
\int_{1}^{\infty} \dfrac{1}{x^{p}} \, dx =\begin{cases}
\text{Convergent if} &  p>1 \\ \\
\text{Divergent if} &  p\leq 1 
\end{cases}
\end{align}
$$
$$
\begin{align}
\int_{1}^{\infty} \dfrac{1}{x^{2}} \, dx < \infty  & (\text{convergent}) \\
\int_{1}^{\infty} \dfrac{1}{x^{1}} \, dx = \infty  & (\text{divergent}) \\
\end{align}
$$
#### Proving p>1
$$
\begin{align}
\int_{1}^{\infty} \dfrac{1}{x^{P}} \, dx =\lim_{ R \to \infty } \int_{1}^{R} x^{-P} \, dx  \\
= \lim_{ R \to \infty } \left[ \dfrac{x^{-p+1}}{-p+1} \right]_{1}^{R} \\
= \left( \lim_{ R \to \infty } \dfrac{R^{-p+1}}{-p+1} \right)-\dfrac{1}{-p+1} \\
\lim_{ R \to \infty } R^{\alpha}= \begin{cases}
0 \text{ if } \alpha < 0 \\
\infty \text{ if } \alpha > 0
\end{cases}
\end{align}
$$
So the graph is convergent if ${}-p+1<0\iff p>1{}$
