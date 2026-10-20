#### 1.
Let the set $A = \left\{  x \in\mathbb{R} | \dfrac{x}{x^{2}-4}\leq \dfrac{1}{x-1}  \right\}$ and $B=\{ x \in \mathbb{R}|\sqrt{ x+1 }\geq x-1 \}$ and calculate $A\cap B$

$$
\begin{align}
\dfrac{x}{x^{2}-4}\leq \dfrac{1}{x-1}\iff \dfrac{x}{(x-2)(x+2)}-\dfrac{1}{x-1}\leq 0\iff \dfrac{x(x-1)-1(x-2)(x+2)}{(x-2)(x+2)(x-1)}\leq 0 \iff  \\
\dfrac{(x^{2}-x)-(x^{2}-4)}{(x-2)(x+2)(x-1)}\leq 0\implies \dfrac{-x+4}{(x-2)(x+2)(x-1)}\leq 0
\end{align}
$$

|         x         | <-- | -2  | --- |  1  | --- |  2  | --- |  4  | --> |
| :---------------: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|      $-x+4$       |  +  |  +  |  +  |  +  |  +  |  +  |  +  |  0  |  -  |
|       $x-2$       |  -  |  -  |  -  |  -  |  -  |  0  |  +  |  +  |  +  |
|       $x+2$       |  -  |  0  |  +  |  +  |  +  |  +  |  +  |  +  |  +  |
|       $x-1$       |  -  |  -  |  -  |  0  |  +  |  +  |  +  |  +  |  +  |
| $\mathrm{L.H.S.}$ |  -  | \|  |  +  | \|  |  -  | \|  |  +  |  0  |  -  |
$x \in\underbrace{ (-\infty,-2)\cup(1,2)\cup[4,\infty) }_{ A= }$


For root differances we're unsure how sides with $x$ behave, since it might be negative, so we must attempt both cases
$$
\begin{align}
\sqrt{ x+1 } \geq x-1
\end{align}
$$
##### Case 1
$x-1\geq0\iff x\geq 1$
$$
\begin{align}
\sqrt{ x+1 }\geq x-1 \quad | \quad ()^{2} \\
x+1\geq (x-1)^{2} \\
x+1\geq x^{2}-2x+1 \\
0\geq x^{2}-3x \\
0\geq x(x-3)
\end{align}
$$

|         x         |  1  | --- |  3  | --> |
| :---------------: | :-: | :-: | :-: | :-: |
|        $x$        |  +  |  +  |  +  |  +  |
|       $x-3$       |  -  |  -  |  0  |  +  |
| $\mathrm{R.H.S.}$ |  -  |  -  |  0  |  +  |
$x \in[1,3]$
##### Case 2
$x-1<0\iff x< 1$
$$
\begin{align}
\underbrace{ \sqrt{ x+1 } }_{ \geq0 }\geq \underbrace{ x-1 }_{ <0 }
\end{align}
$$
$x-1$ is always less than $0$ since we require x to be less than one, which makes it always less than the L.H.S as square roots are always positive
However we require $x \in \mathbb{R}$, so the contents of the root cant be negative, so $x\geq-1$
thus for case 2, $x \in[-1,1)$

for the full answer we need the union between the two $x$'s
$B=[-1,1)\cup[1,3]=[-1,3]$

$A\cap B=((-\infty,-2)\cup(1,2)\cup[4,\infty))\cap[-1,3]=(1,2)$
#### 2.
Solve the inequality $|2 x-3|+|x-1|≥x+3$
$$
\begin{align}
|2 x-3|+|x-1|≥x+3 \\
|2 x-3|+|x-1|-x-3≥0
\end{align}
$$

This step is important to explain for some reason, or you risk loosing points
$$
\begin{align}
|2x-3|=\left\{ \begin{array}{lll}
2x-3, & \text{if }x\geq \dfrac{3}{2} \\
3-2x, & \text{if }x< \dfrac{3}{2}
\end{array} \right.  \\
|x-1|=\left\{ \begin{array}{lll}
x-1, & \text{if } x\geq1 \\
1-x, & \text{if } x<1
\end{array} \right. 
\end{align}
$$
Now we need cases for each combination of the cases the absolute values end up in

<--case 1--1--case 2--3/2--case 3-->
##### Case 1
$x<1$
$$
\begin{align}
3-2x+1-x\geq x+3 \\
-4x\geq-1 \\
x\leq \dfrac{1}{4}
\end{align}
$$
$x \in\left( -\infty, \dfrac{1}{4} \right]$
$x$ falls within the cases' span
##### Case 2
$1\leq x < \dfrac{3}{2}$

$$
\begin{align}
3-2x+x-1 \geq x+3 \\
-2x\geq 1 \\
x\leq-\dfrac{1}{2}
\end{align}
$$
$x \in \left( -\infty, -\dfrac{1}{2} \right]$
$x$ falls outside the cases' span
$x \in \varnothing$
##### Case 3
$x\geq \dfrac{3}{2}$

$$
\begin{align}
2x-3+x-1\geq x+3 \\
2x\geq7 \\
x\geq \dfrac{7}{2}
\end{align}
$$
$x \in\left[ \dfrac{7}{2},\infty \right)$
$x$ falls fully within the case's span
##### Result
$x \in\left( -\infty, \dfrac{1}{4} \right]\cup\left[ \dfrac{7}{2}, \infty \right)$
#### 3.
let $P:x^{2}>9$ and $Q:x<-3$
a) Is P necessary for Q
$P\implies Q$
$x^{2}>9\implies x<-3$ 
yes???
b) Is Q necessary for Q
$Q\implies P$
$x<-3\implies x^{2}>9$ 
no, because $x>3$ also results in this
c) Is P required for Q
$P\impliedby Q$
no, as $x>3$ is also required for this
d) is Q required for P
$Q\impliedby P$
yes
#### 4.
a)
$x^{3}=-y^{3}\iff x=-y$
the asumption is made that $x$ and $y$ are both real numbers,
so logically, statement $P$ should have the same amount of outcomes as $Q$


#### Example 2.
a)
$A:\exists x: (x<1\implies x^{2}>1)$
no, negative numbers under -1 disprove this
b)

Derived from [[Lectures]]