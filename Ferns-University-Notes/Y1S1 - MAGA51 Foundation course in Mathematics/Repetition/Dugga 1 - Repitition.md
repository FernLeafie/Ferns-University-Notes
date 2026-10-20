---
color: ""
---
#### 1

Let $A=\left\{  x \in \mathbb{R} | 1+\dfrac{x}{x-1}\geq \dfrac{9}{x^{2}-1}  \right\}$ and $B=\left\{  x\geq| \dfrac{1}{2x} \leq \dfrac{1}{x+3} \right\}$
Decide $A\cap B$

$$
\begin{align}
1+\dfrac{x}{x-1}\geq \dfrac{9}{x^{2}-1} \iff 1+\dfrac{x}{x+1}-\dfrac{9}{(x-1)(x+1)}\geq 0\iff \dfrac{(x^{2}-1)+(x^{2}+x)-9}{(x-1)(x+1)}\geq 0 \\
\dfrac{2x^{2}+x-10}{(x-1)(x+1)}\geq 0 \iff \dfrac{(x-2)\left( x+\dfrac{5}{2} \right)}{(x-1)(x+1)}\geq0
\end{align}
$$

|        $x$        |     | $-\dfrac{5}{2}$ |     | $-1$ |     | $1$ |     | $2$ |     |
| :---------------: | :-: | :-------------: | :-: | :--: | :-: | :-: | :-: | :-: | :-: |
|       $x-2$       |  -  |        -        |  -  |  -   |  -  |  -  |  -  | $0$ |  +  |
| $x+\dfrac{5}{2}$  |  -  |       $0$       |  +  |  +   |  +  |  +  |  +  |  +  |  +  |
|       $x-1$       |  -  |        -        |  -  |  -   |  -  | $0$ |  +  |  +  |  +  |
|       $x+1$       |  -  |        -        |  -  | $0$  |  +  |  +  |  +  |  +  |  +  |
| $\mathrm{L.H.S.}$ |  +  |       $0$       |  -  | N/A  |  +  | N/A |  -  | $0$ |  +  |
$A=\left( -\infty,-\dfrac{5}{2} \right]\cup(-1,1)\cup[2,\infty)$


$$
\begin{align}
 \dfrac{1}{2x} \leq \dfrac{1}{x+3}\iff  \dfrac{1}{2x}-\dfrac{1}{x+3} \leq 0 \iff \dfrac{(x+3)-2x}{2x(x+3)}\leq 0 \iff \dfrac{-x+3}{2x(x+3)}\leq 0
\end{align}
$$

| $x$               |     | $-3$ |     | $0$ |     | $3$ |     |
| ----------------- | --- | ---- | --- | --- | --- | --- | --- |
| $-x+3$            | +   | +    | +   | +   | +   | $0$ | -   |
| $2x$              | -   | -    | -   | $0$ | +   | +   | +   |
| $x+3$             | -   | $0$  | +   | +   | +   | +   | +   |
| $\mathrm{L.H.S.}$ | +   | N/A  | -   | N/A | +   | $0$ | -   |

$$
\begin{align}
B=[0,\infty)\cap((-3,0)\cup[3,\infty))=[3,\infty)
\end{align}
$$

$$
\begin{align}
A\cap B=\left( \left( -\infty,-\dfrac{5}{2} \right]\cup(-1,1)\cup[2,\infty )\right)\cap[3,\infty)=[3,\infty)
\end{align}
$$
#### 2
Decide the amount $M=\{ x \in [0,\pi]: 2\sin^{3}(2x)+\cos ^{2}(2x)+6\sin(2x)=4 \}$

$$
\begin{align}
2\sin^{3}(2x)+\cos ^{2}(2x)+6\sin(2x)=4\iff 2\sin^{3}(2x)+1-\sin ^{2}(2x)+6\sin(2x)=4 \\
[t=\sin 2x],2t^{3}+1-t^{2}+6t=6=4\iff 2t^{3}-t^{2}+6t+1=4\iff 2t^{3}-t^{2}+6t-3=0 \\
t^{2}(2t-1)+3(2t-1)=0\iff \underbrace{ (2t-1) }_{ =0 }\underbrace{ (t^{2}+3) }_{ \text{imaginary} }=0\iff 2t-1=0\iff 2t=1\iff t=\dfrac{1}{2} \\
\sin(2x)=\dfrac{1}{2}\iff \sin (2x)=\left\{ \begin{array}{lll}
\sin\left( \dfrac{\pi}{6}+2\pi n \right) \\
\sin\left( \pi-\dfrac{\pi}{6}+2\pi n \right)
\end{array} \right. \iff 2x=\left\{ \begin{array}{lll}
 \dfrac{\pi}{6}+2\pi n \\
 \pi-\dfrac{\pi}{6}+2\pi n
\end{array} \right.  \\
x=\left\{ \begin{array}{lll}
\dfrac{\pi}{12}+\pi n \\
\dfrac{\pi}{2} -\dfrac{\pi}{12}+\pi n
\end{array} \right.  \\
M=\left\{  \dfrac{\pi}{12},\dfrac{5\pi}{12}  \right\}
\end{align}
$$
#### 3
Decide the mid point and half axis for the ellipse $2x^{2}-4x+3y^{2}+12y+8=0$
$$
\begin{align}
2x^{2}-4x+3y^{2}+12y+8=0 \\
\text{Square completion of }x \\
2x^{2}-4x=2(x^{2}-2x+1-1)=2((x-1)^{2}-1)=2(x-1)^{2}-2 \\
\text{Square completion of }y \\
3y^{2}+12y=3(y^{2}+4y)=3(y^{2}+4y+4-4)=3((y^{2}+2)-4)=3(y^{2}+2)-12 \\
 \\
2x^{2}-4x+3y^{2}+12y+8=0\iff 2(x-1)^{2}-2+3(y^{2}+2)-12+8=0 \\
 2(x-1)^{2}+3(y^{2}+2)=6\iff \dfrac{2(x-1)^{2}}{6}+\dfrac{3(y^{2}+2)}{6}=1 \\
\dfrac{(x-1)^{2}}{3}+\dfrac{(y^{2}+2)}{2}=1\iff \dfrac{(x-1)^{2}}{\sqrt{ 3 }^{2}}+\dfrac{(y^{2}+2)}{\sqrt{ 2 }^{2}}=1
\end{align}
$$
Mid point $(1;-2)$, half axis $a=\sqrt{ 3 }$ and $b=\sqrt{ 2 }$
#### 4
Solve $e^{ \ln(x-1)+2\ln(x+1) }=4x^{2}-4$
$$
\begin{align}
e^{ \ln(x-1)+2\ln(x+1) }=4x^{2}-4\iff e^{ \ln(x-1)+\ln((x+1)^{2}) }=4x^{2}-4 \\
e^{ \ln((x+1)^{2}(x-1)) }=4x^{2}-4\iff (x+1)^{2}(x-1)=4x^{2}-4 \\
(x+1)^{2}(x-1)-4x^{2}+4=0\iff (x^{2}+2x+1)(x-1)-4x^{2}+4=0 \\
x^{3}+2x^{2}+1x-x^{2}-2x-1-4x^{2}+4=0\iff x^{3}-3x^{2}-x+3=0 \\
x^{2}(x-3)+(-1)(x-3)=0\iff (x-3)(x^{2}+(-1))=0\iff \underbrace{ (x-3) }_{ 0 }\underbrace{ (x^{2}-1) }_{ 0 }=0 \\
\left\{ \begin{array}{lll}
x_{1}=3 \\
x_{2}=-1 \\
x_{3}=1
\end{array} \right. 
\end{align}
$$
#### 10
$$
\begin{align}
\lim_{ x \to -\infty } \dfrac{1}{\sqrt{ 9x^{2}-x }+3x}=`` \dfrac{1}{\infty-\infty}"=\lim_{ x \to -\infty } \dfrac{1}{\dfrac{(9x^{2}-x)-(9x^{2})}{\sqrt{ 9x^{2}-x }+\sqrt{ 9x^{2} }}}=\lim_{ x \to -\infty } \dfrac{1}{\dfrac{-x}{\sqrt{ 9x^{2}-x }-3x}} \\
\lim_{ x \to -\infty } \dfrac{\sqrt{ 9x^{2}-x }-3x}{-x}=``\dfrac{\infty-\infty}{\infty} "=\lim_{ x \to -\infty } \dfrac{|3x|\sqrt{ 1-\dfrac{1}{9x} }-3x}{-x}=\lim_{ x \to -\infty } \dfrac{-3x\sqrt{ 1-\dfrac{1}{9x} }-3x}{-x} \\
\lim_{ x \to -\infty } \dfrac{3\cancel{ (-x) }\sqrt{ 1-\dfrac{1}{9x} }-3x}{\cancel{ -x }}=``3(\sqrt{ 1 }+1) "=6
\end{align}
$$
#### 11
Let $f(x)=\dfrac{\pi}{3}\arctan(3x)$ and $(f \circ g)(x)=\dfrac{3\pi}{2}x$, decide $g(x)$

$$
\begin{align}
(f \circ g)(x)=\dfrac{3\pi}{2}x=\dfrac{\pi}{3}\arctan(3g(x))\iff 
\end{align}
$$
#### 12
Solve the difference $\dfrac{1}{|2x-1|}\geq \dfrac{2}{|x+3|}$
$$
\begin{align}
\dfrac{1}{|2x-1|}\geq \dfrac{2}{|x+3|}\iff |x+3|\geq 2|2x-1|, x \neq \dfrac{1}{2},x\neq3 \\

\end{align}
$$

$$
\begin{align}
|x+3| = \left\{ \begin{array}{lll}
x+3, & x\geq-3\\
-(x+3), & x<-3
\end{array} \right.  \\
|2x-1| = \left\{ \begin{array}{lll}
2x-1, & x\geq \dfrac{1}{2}\\
-(2x-1), & x< \dfrac{1}{2}
\end{array} \right. 
\end{align}
$$
##### Case 1
$x<-3$
$$
\begin{align}
-(x+3)\geq 2(-(2x-1)) \\
-x-3\geq -4x+2 \\
3x\geq 5 \\
x\geq \dfrac{5}{3} \\
x \in \left[ \dfrac{5}{3},\infty \right) \cap (-\infty,-3) \\
x \in \varnothing
\end{align}
$$
##### Case 2
$-3\leq x< \dfrac{1}{2}$
$$
\begin{align}
-(x+3)\geq 2(-(2x-1)) \\
x+3\geq-4x+2 \\
5x\geq-1 \\
x\geq \dfrac{1}{5} \\
x \in\left[ -\dfrac{1}{5}, \infty\right]\cap\left[ -3, \dfrac{1}{2} \right) \\
x \in\left[ -\dfrac{1}{5}, \dfrac{1}{2} \right)
\end{align}
$$
##### Case 3
$x\geq \dfrac{1}{2}$

$$
\begin{align}
(x+3)\geq2(2x-1) \\
x+3\geq 4x-2 \\
-3x\geq -5 \\
x\leq \dfrac{5}{3} \\
x \in \left( -\infty, \dfrac{5}{3} \right] \cap \left[ \dfrac{1}{2},\infty \right) \\
x \in \left( \dfrac{1}{2}, \dfrac{5}{3} \right]
\end{align}
$$

Solution $x \in \left[-\dfrac{1}{2}, \dfrac{1}{2}\right)\cup\left( \dfrac{1}{2}, \dfrac{5}{3} \right]=\left[ -\dfrac{1}{2}, \dfrac{5}{3} \right]\setminus \left\{  \dfrac{1}{2}  \right\}$
#### 13
Let $f(x)=\ln(2x)$ and $g(x)=2\sin(\sqrt{ x })-1$
##### a)
Decide the domain for $f$ and $g$
$$
\begin{align}
2x>0 \\
x>0 \\
D_{f}=R_{+} \\
 \\
x\geq 0 \\
D_{g}=[0,\infty)
\end{align}
$$
##### b)
Decide $(g\circ f)(x)$, limit $D_{f}$ so that $(g \circ f)$ can be calculated, and decide $D_{(g\circ f)}$

$$
\begin{align}
(g\circ f)(x)=g(f(x))=g(\ln(2x))=2\sin(\sqrt{ \ln(2x) })-1 \\
\sqrt{  }: \ln(2x)\geq 0 \iff 2x \geq 1 \iff  x\geq \dfrac{1}{2} \\
D_{(g \circ f)}=\left[ \dfrac{1}{2} ,\infty\right) \\
D_{f \text{ new}}=\left[ \dfrac{1}{2} ,\infty\right)
\end{align}
$$
##### c)
Limit the domain of $g$ so it's inversible, and invert $g$
$$
\begin{align}
g(x)=y \iff 2\sin(\sqrt{ x })-1=y\iff 2\sin(\sqrt{ x })=y-1\iff \sin(\sqrt{ x })=\dfrac{y+1}{2} \\
\sqrt{ x } = \arcsin\left( \dfrac{y+1}{2} \right)\iff x=\arcsin ^{2}\left( \dfrac{y+1}{2} \right) \\
 \\
-1\leq \sin(\sqrt{ x })\leq 1 \iff -2\leq 2\sin(\sqrt{ x })\leq 2\iff -3\leq 2\sin(\sqrt{ x })-1\leq 1 \\
y \in [-3,1] \\
-3\leq y \leq 1 \\
-2\leq y+1\leq 2 \\
-1\leq \dfrac{y+1}{2}\leq 1 \\
\text{Yippie} \\
\text{But as arcsin is only defined for a limited interval} \\
\sin: \left[ -\dfrac{\pi}{2}, \dfrac{\pi}{2} \right]\to [-1,1] \\
\arcsin: [-1,1] \to \left[ -\dfrac{\pi}{2}, \dfrac{\pi}{2} \right] \\
\sqrt{ x } \in \left[ -\dfrac{\pi}{2}, \dfrac{\pi}{2} \right] \\
0\leq \sqrt{ x }\leq \dfrac{\pi}{2} \\
0\leq x \leq \dfrac{\pi^{2}}{4} \\
D_{g}=\left[ 0,\dfrac{\pi^{2}}{4} \right]
\end{align}
$$
#### 14
$$
\begin{align}
\lim_{ x \to -2^{-} } \dfrac{|x^{2}-4|}{x^{2}+x-2}=\lim_{ x \to -2^{-} } \dfrac{x^{2}-4}{(x+2)(x-1)}=\lim_{ x \to -2^{-} } \dfrac{(x-2)\cancel{ (x+2) }}{\cancel{ (x+2) }(x-1)}= `` \dfrac{-2-2}{-2-1}"=\dfrac{4}{3}
\end{align}
$$

Derived from [[Repetition]]