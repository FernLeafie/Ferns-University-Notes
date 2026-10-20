$$
\begin{align}
\lim_{ x \to \infty } \dfrac{x}{x+1}=" \dfrac{\infty}{\infty}"=\lim_{ x \to \infty } \dfrac{\cancel{ x } 1}{\cancel{ x }\left( 1+\dfrac{1}{x} \right)}=" \dfrac{1}{1+0}"=1
\end{align}
$$

$$
\begin{align}
\text{constant}<\log_{a}x<\{ x^{a},0<a<1 \}<\{ x^{a},1<a<\infty \}<\{ a^{x},a>1 \}
\end{align}
$$

| $\infty+C=\infty$                      | $-\infty+C=-\infty$      |
| -------------------------------------- | ------------------------ |
| $\infty+\infty=\infty$                 | $-\infty-\infty=-\infty$ |
| $\infty*\infty=-\infty*-\infty=\infty$ | $\infty*-\infty=\infty$  |
|                                        |                          |


$$
\begin{align}
\lim_{ x \to a } \dfrac{\sin(f(x))}{f(x)}=1, \iff  f(x)\to0\text{ when }x\to a \\
\lim_{ x \to 0 } \dfrac{\tan(f(x))}{f(x)}=1 \\
\lim_{ x \to 0 } \dfrac{\arcsin(f(x))}{f(x)}=1 \\
\lim_{ x \to 0 } \dfrac{\arctan(f(x))}{f(x)}=1
\end{align}
$$

proof for additional forms
$$
\begin{align}
\lim_{ x \to 0 } \dfrac{\tan x}{x}=\lim_{ x \to 0 } \dfrac{\dfrac{\sin(x)}{\cos (x)}}{1}=\lim_{ x \to 0 } \dfrac{\sin(x)}{1} \dfrac{1}{\cos(x)}=`` 1*\dfrac{1}{1}"=1 \\
\lim_{ x \to 0 } \dfrac{x}{\sin (x)}=1\iff \lim_{ x \to 0 } \dfrac{\sin(x)}{x}=1\iff \lim_{ x \to 0 } \left( \dfrac{\sin(x)}{x} \right)^{-1}=1^{-1}\iff \lim_{ x \to 0 }  \dfrac{x}{\sin(x)}=\dfrac{1}{1}=1
\end{align}
$$

$$
\begin{align}
\lim_{ x \to \pm\infty } \left( 1+\dfrac{1}{x} \right)^{x}=e \\
\lim_{ x \to \pm a } \left( 1+\dfrac{1}{f(x)} \right)^{f(x)}=e \iff f(x)\to \pm \infty \text{ when }x\to a
\end{align}
$$

$$
\begin{align}
\underbrace{ \sqrt{ A } }_{ a }\pm \underbrace{ \sqrt{ B } }_{ b }=\dfrac{a^{2}-b^{2}}{a\mp b}=\dfrac{A-B}{\sqrt{ A }\mp \sqrt{ B }}
\end{align}
$$
For a limit in a point to exist, the result when aproaching from below and above must be equal
## Examples
#### a

$$
\begin{align}
\lim_{ x \to \infty } \dfrac{x^{2}-1}{x^{3}-1}=\lim_{ x \to \infty } \dfrac{\cancel{ x^{3} }\left( \dfrac{1}{x}-\dfrac{1}{x^{3}} \right)}{\cancel{ x^{3} }\left( 1-\dfrac{1}{x^{3}} \right)}=" \dfrac{0-0}{1-\infty}"=" \dfrac{0}{-\infty} "=-0
\end{align}
$$

$$
\begin{align}
\lim_{ x \to \infty } \dfrac{x^{2}-1}{x^{3}-1}=\lim_{ x \to \infty } \dfrac{\cancel{ x^{2} }\left( 1-\dfrac{1}{x^{2}} \right)}{\cancel{ x^{3} }\left( 1-\dfrac{1}{x^{3}} \right)} =" \dfrac{1-0}{\infty(1-0)}"=0
\end{align}
$$
#### b
since $x=1$ results in $0$ then $x-1$ should be a root
$$
\begin{align}
\lim_{ x \to 1 } \dfrac{x^{2}-1}{x^{3}-1}=" \dfrac{0}{0}"=\lim_{ x \to 1 } \dfrac{\cancel{ (x-1) }(x+1)}{\cancel{ (x-1) }(x^{2}+x+1)}=" \dfrac{1+1}{1+1+1}"=\dfrac{2}{3}
\end{align}
$$
#### c

$$
\begin{align}
\lim_{ x \to \infty } \dfrac{x^{3}e^{ x }+2 e^{ 2x }\ln x-x}{x^{3}e^{2x}-\sin x}="\dfrac{\infty-\infty}{\infty}"=\dfrac{\cancel{ e^{2x} }\left( \dfrac{x^{3}}{e^{ x }}+2\ln x-\dfrac{x}{e^{ 2x }}\right)}{\cancel{ e^{ 2x } }\left( x^{3}-\dfrac{\sin x}{e^{ 2x }} \right)}=`` \dfrac{0+\infty-0}{\infty-0} "= \\
\dfrac{\cancel{ x^{3} }\left( \dfrac{1}{e^{ x }}+\dfrac{2\ln x}{x^{3}}-\dfrac{1}{x^{2}e^{ 2x }} \right)}{\cancel{ x^{3} }\left( 1-\dfrac{\sin x}{x^{3}e^{ 2x }} \right)}=`` \dfrac{0}{1-0} "=0
\end{align}
$$
#### d

$$
\begin{align}
\lim_{ x \to \infty } \dfrac{1}{\sqrt{ 4x^{2}+x }-2x}=`` \dfrac{1}{\infty-\infty} "=\lim_{ x \to \infty } \dfrac{1}{\sqrt{ 4x^{2}+x}-\sqrt{ 4x^{2} }}=\lim_{ x \to \infty } \dfrac{1}{\dfrac{4x^{2}+x-4x^{2}}{\sqrt{ 4x^{2}+x }+2x}} \\
\lim_{ x \to \infty } \dfrac{1}{\dfrac{x}{\sqrt{ 4x^{2}+x }+2x}}=\lim_{ x \to \infty } \dfrac{\sqrt{ 4x^{2}+x }+2x}{x}=`` \dfrac{\infty}{\infty}"=\lim_{ x \to \infty }\dfrac{2\cancel{ x }\left( \sqrt{1+ \dfrac{1}{4x} }+1 \right)}{\cancel{ x }} \\
`` \dfrac{2(1+1)}{1}"=4
\end{align}
$$
#### e

$$
\begin{align}
\lim_{ x \to \pi } \dfrac{\sin(x)}{\pi-x}=`` \dfrac{0}{0}"=\lim_{ x \to \pi } \dfrac{\sin(\pi-x)}{\pi-x}=1 \iff f(x)=\pi-x\to0,x\to \pi
\end{align}
$$
#### f

$$
\begin{align}
\lim_{ x \to 1^{+} } \arctan\left( \dfrac{x^{2}}{x-1} \right)=`` \arctan\left( \dfrac{1}{+0} \right) "=`` \arctan(+\infty)"=\dfrac{\pi}{2}
\end{align}
$$
#### g

$$
\begin{align}
\lim_{ x \to 2^{+} } \dfrac{\sqrt{ 4-4x+x^{2} }}{x-2}=`` \dfrac{0}{0}"= \lim_{ x \to 2^{+} } \dfrac{\sqrt{ (x-2)^{2} }}{x-2}=\lim_{ x \to 2^{+} } \dfrac{ |x-2| }{x-2}=\lim_{ x \to 2^{+} }  \dfrac{x-2}{x-2}=1
\end{align}
$$
#### h

$$
\begin{align}
\lim_{ x \to 9 } \dfrac{\sqrt{ x }-3}{81-x^{2}}=`` \dfrac{0}{0} "=[ \text{substitute } t=\sqrt{ x }]=\lim_{ t \to 3 } \dfrac{y-3}{81-t^{4}}=\lim_{ t \to 3 } \dfrac{\cancel{ t-3 }}{(\cancel{ 3-t })(t+3)(9+t^{2})}=`` \dfrac{1}{(-1)(6)(18)} "=-\dfrac{1}{108} \\
 \\
\lim_{ x \to 9 } \dfrac{\sqrt{ x }-3}{81-x^{2}}=`` \dfrac{0}{0} "=\lim_{ x \to 9 } \dfrac{\sqrt{ x }-3}{(9-x)(9+x)}=\lim_{ x \to 9 } \dfrac{\sqrt{ x }-3}{(\sqrt{ x }-3)(\sqrt{ x }+3)(9+x)}=`` \dfrac{1}{(-1)(6)(18)}"=-\dfrac{1}{108}
\end{align}
$$
#### i

$$
\begin{align}
\lim_{ x \to \infty } \dfrac{\ln(5x^{2})}{\ln(6x^{3})}=`` \dfrac{\infty}{\infty}"= \lim_{ x \to \infty } \dfrac{\ln(5)+2\ln(x)}{\ln(6)+3\ln(x)}= `` \dfrac{\infty}{\infty}" =\lim_{ x \to \infty } \dfrac{\cancel{ \ln(x) }\left( \dfrac{\ln(5)}{\ln(x)}+2 \right)}{\cancel{ \ln(x) }\left( \dfrac{\ln(6)}{\ln(x)}+3 \right)}=`` \dfrac{0+2}{0+3}"=\dfrac{2}{3}
\end{align}
$$
#### j

$$
\begin{align}
\lim_{ x \to \infty } \dfrac{\sin(x)}{\sqrt{ x }}=`` \dfrac{k}{\infty} ",k \in[-1,1]=\infty
\end{align}
$$
or using squeeze theorem
$$
\begin{align}
\lim_{ x \to \infty } \dfrac{\sin(x)}{\sqrt{ x }} \\
-1\leq\sin(x)\leq1 \\
-\dfrac{1}{\sqrt{ x }}\leq \dfrac{\sin(x)}{\sqrt{ x }}\leq \dfrac{1}{\sqrt{ x }} | \lim_{ x \to \infty } \\
0\leq \lim_{ x \to \infty } \dfrac{\sin(x)}{\sqrt{ x }}\leq 0 \iff \lim_{ x \to \infty } \dfrac{\sin(x)}{\sqrt{ x }}=0 
\end{align}
$$

$$
\begin{align}
\lim_{ x \to 0 } \dfrac{\sin(x)}{\sqrt{ x }}=`` \dfrac{0}{0} " =\lim_{ x \to 0 } \dfrac{\sin(x)}{x} * \dfrac{x}{\sqrt{ x }}=\lim_{ x \to 0 } \dfrac{\sin(x)}{x} \dfrac{\sqrt{ x }}{1}=`` 1 * \dfrac{0}{1}"=0
\end{align}
$$
#### k

$$
\begin{align}
\lim_{ x \to \infty } \left( 1+\dfrac{1}{2x} \right)^{-x}=`` \underbrace{ 1^{-\infty} }_{ \text{almost }1 }"=\lim_{ x \to \infty } \left( \left( 1+\dfrac{1}{2x} \right)^{2x} \right)^{-1/2}=e^{-1/2}=\dfrac{1}{\sqrt{ e }}
\end{align}
$$

Derived from [[Lectures]]