For $x^{2}+px+q=0$ we can only use the pq forumula as long as $p^{2}-4q\geq 0$
$$
x=-\dfrac{p}{2}\pm \sqrt{ \dfrac{p^{2}}{4}-q }\implies x=-\dfrac{p}{2}\pm \sqrt{ \left( \dfrac{p}{2} \right)^{2}-q }
$$
if $p^{2}-4q=0$ then the roots are identical
if $p^{2}-4q<0$ then the equiation has no real roots

$$
\begin{align}
\frac{P(x)}{Q(x)}=K(x)+\frac{r(x)}{Q(x)} \\
K(x)*Q(x)+R(x)=P(x)
\end{align}
$$

$$
\begin{align}
|x|=\left\{ \begin{array}{lll}
&x,&x\geq 0 \\
&-x,&x< 0
\end{array} \right.  \\
|x-3|=\left\{ \begin{array}{lll}
&x-3,&x\geq -3 \\
&-(x-3),&x< -3
\end{array} \right. 
\end{align}
$$
### Examples
$$
\begin{align}
(x+2)(x-3)<0
\end{align}
$$

|            | <-- | -2  | --- |  3  | --> |
| ---------- | :-: | :-: | :-: | :-: | :-: |
| (x+2)      |  -  |  0  |  +  |  +  |  +  |
| (x-3)      |  -  |  -  |  -  |  0  |  +  |
| (x+2)(x-3) |  +  |  0  |  -  |  0  |  +  |

$$
\begin{align}
-2<x<3 \\
(-2,3) \\
\{ x \in \mathbb{R},-2<x<3 \}
\end{align}
$$

$$
\begin{align}
x(x+2)(x-3)\geq 0
\end{align}
$$

|               |     | -2  |     |  0  |     |  3  |     |
| ------------- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| x             |  -  |  -  |  -  |  0  |  +  |  +  |  +  |
| $x+2$         |  -  |  0  |  +  |  +  |  +  |  +  |  +  |
| $x-3$         |  -  |  -  |  -  |  -  |  -  |  0  |  +  |
| $x(x+2)(x-3)$ |  -  |  0  |  +  |  0  |  -  |  0  |  +  |

$$
\begin{align}
[-2,0] \text{ or } [3,\infty) \\
\{ x \in \mathbb{R}, -2\leq x\leq0 \text{ or } 3\leq x \}
\end{align}
$$
---

$$
\begin{align}
|x-3|+x=5\implies \\
|x-3|=\left\{ \begin{array}{lll}
 & x-3, & x\geq 3 \\
 & 3-x, & x< 3
\end{array} \right.
\end{align}
$$
for $x\geq 3$
$$
x-3+x=5\implies
2x=8\implies x=4
$$
$x$ is correctly precent in the span

for $x<3$
$$
\begin{align}
3-x+x=5\implies 3=5
\end{align}
$$
no valid $x$ over $x<3$
answer: $x=4$
## Exercises
### Polynomial, rational expressions and polynomial division
2.1 a) c),  2.2 b) c);  2.3 a) b) c) h);  2.5 **a)** b) c) 
#### 2.1
a)
$$
\begin{align}
(x^{3}+1)(x^{3}-1)=x^{6}-1
\end{align}
$$
c)
$$
\begin{align}
(2x+1)(4x^{2}-2x+1)=8x^{3}-4x^{2}+2x+4x^{2}-2x+1=8x^{3}+1
\end{align}
$$
#### 2.2
b)
first degree
$$
\begin{align}
1+x^{2}-(1+x)^{2}=1+x^{2}-(1+2x+x^{2})=1+x^{2}-1-2x-x^{2}=-2x
\end{align}
$$
c)
third degree
$$
\begin{align}
(1+x)(1+x^{2})=1+x^{2}+x+x^{3}=x^{3}+x^{2}+x+1
\end{align}
$$
#### 2.3
a)
$$
\begin{align}
\dfrac{1}{x}-\dfrac{1}{x+1}=\dfrac{x+1}{x^{2}+x}-\dfrac{x}{x^{2}+x}=\dfrac{1}{x^{2}+x} 
\end{align}
$$
b)
$$
\begin{align}
\dfrac{1}{x+\dfrac{1}{x}}=\dfrac{1}{\dfrac{x}{1}+\dfrac{1}{x}}=\dfrac{1}{\dfrac{x^{2}}{x}+\dfrac{1}{x}}=\dfrac{1}{\dfrac{x^{2}+1}{x}}=\dfrac{1}{1}*\dfrac{x}{x^{2}+1}=\dfrac{x}{x^{2}+1}
\end{align}
$$
c)
$$
\begin{align}
\dfrac{\dfrac{x}{2}+\dfrac{2}{x}}{\dfrac{1}{x^{2}}+\dfrac{1}{4}}=\dfrac{\left( \dfrac{x^{2}}{2x}+\dfrac{4}{2x} \right)}{\dfrac{4}{4x^{2}}+\dfrac{x^{2}}{4x^{2}}}=\dfrac{\dfrac{x^{2}+4}{2x}}{\dfrac{4+x^{2}}{4x^{2}}}=\dfrac{x^{2}+4}{2x}*\dfrac{4x^{2}}{4+x^{2}}=\dfrac{4x^{2}}{2x}=2x
\end{align}
$$
h)
$$
\begin{align}
\dfrac{\dfrac{x-1}{x^{2}-4}+\dfrac{1}{x}}{\dfrac{1}{x^{2}-2x}+x}
\end{align}
$$
#### 2.5
a)
$$
\begin{align}
\require{enclose}
\begin{array}{rll}
   x^{3} -x^{2}\\[-3pt]
   x+2 \enclose{longdiv}{x^{4}-4x^{2}-2x+k}\kern-.2ex \\[-3pt]
      \underline{x^{4}+2x^{3}\phantom{\+0x+0}} \\[-3pt]
      \ -2x^{3}-4x^{2}\phantom{\ -0x+0} \\[-3pt]
      \underline{\ -2x^{3}-4x^{2}\phantom{\ -0x+0}} \\[-3pt]
      \ 6+k\\[-3pt]
  \end{array} \\ \\
6+k=0\implies k=-6
\end{align}
$$

$$
\begin{align}
\dfrac{x^{2}-3x+7}{x-2} \\ \\
\begin{array}{rll}
   x -1\\[-3pt]
   x-2 \enclose{longdiv}{x^{2}-3x+7}\kern-.2ex \\[-3pt]
      \underline{x^{2}+2x\phantom{\+0}} \\[-3pt]
      \ -x+7\phantom{} \\[-3pt]
      \underline{\ +x-2 \phantom{}} \\[-3pt]
      \ 5\\[-3pt]
  \end{array} \\ \\
\dfrac{x^{2}-3x+7}{x-2}=\dfrac{5}{x-2}+x-1
\end{align}
$$
b)
$$
\begin{align}
\dfrac{x^{4}}{x^{2}-1} \\ \\
\begin{array}{rll}
   x^{2}+1\\[-3pt]
   x^{2}-1 \enclose{longdiv}{x^{4}\ \phantom{+0x^{2}+0}}\kern-.2ex \\[-3pt]
      \underline{x^{4}-x^{2}\phantom{\ +0}} \\[-3pt]
      \ +x^{2}\phantom{\ +0} \\[-3pt]
      \underline{\ x^{2}-1 \phantom{}} \\[-3pt]
      \ 1\\[-3pt]
  \end{array} \\ \\
\dfrac{x^{4}}{x^{2}-1}=\dfrac{1}{x^{2}-1}+x+1
\end{align}
$$


### Equations and differences
2.6 a) h) i),  2.7 b) d),  2.8 b) d);  2.10 b),  2.11 a);  2.15 **a)** d);  2.16 a) c),  2.17 b),  2.18 **b)** c)
#### 2.6
a)
$$
\begin{align}
x^{2}+3x-10 \\
x=-1.5\pm \sqrt{ \dfrac{9}{4}+10 }\implies x=-1.5\pm \sqrt{ \dfrac{9+40}{4} }\implies x=-1.5\pm \dfrac{\sqrt{ 49}}{\sqrt{ 4}}\implies \\
x=-\dfrac{3}{2}\pm \dfrac{7}{2}\implies \left\{ \begin{array}{l}
x_{1}=2 \\
x_{2}=-5
\end{array} \right. 
\end{align}
$$
#### 2.15
a)
$$
\begin{align}
\sqrt{ x }-1=\sqrt{ x-9 }\implies (\sqrt{ x }-1)^{2}=x-9\implies x-2\sqrt{ x }+1=x-9\implies \\
-2\sqrt{ x }+1=-9\implies 10=2\sqrt{ x }\implies 5=\sqrt{ x }\implies x=25 \\
 \\
\sqrt{ 25 }-1=\sqrt{ 25-9 }\implies 4=\sqrt{ 16 }\implies 4=4 \\
\mathrm{L.H.S.}=\mathrm{R.H.S.}
\end{align}
$$
#### 2.18
b)
$$
\begin{align}
\frac{4x}{x+1}\leq x^{2}-2x\implies\frac{4x}{x+1}-(x^{2}-2x)\leq 0\implies \\
\frac{4x}{x+1}-(x^{2}-2x)\leq 0\implies \\
\dots \\
-\frac{x(x+2)(x-3)}{x+1}\leq 0\implies \frac{x(x+2)(x-3)}{x+1}\geq 0
\end{align}
$$

|                              | <-- | -2  | --- | -1  | --- | 0   | --- | 3   | --> |
| ---------------------------- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| $x$                          | -   | -   | -   | -   | -   | 0   | +   | +   | +   |
| $x+2$                        | -   | 0   | +   | +   | +   | +   | +   | +   | +   |
| $x-3$                        | -   | -   | -   | -   | -   | -   | -   | 0   | +   |
| $x(x+2)(x-3)$                | -   | 0   | +   | +   | +   | 0   | -   | 0   | +   |
| $x+1$                        | -   | -   | -   | 0   | +   | +   | +   | +   | +   |
| $\dfrac{x(x+2)(x-3)}{(x+1)}$ | +   | 0   | -   | N/A | +   | 0   | -   | 0   | +   |


$$
\begin{align}
\{ x \in \mathbb{Z}, x\leq -2\cup-1< x\leq 0\cup3\leq x \} \\
(-\infty,-2] \cup(-1,0]\cup[3,\infty)
\end{align}
$$
### Absolute amounts
2.19 e) f) g),  2.20 a) c) e),  2.22 a) **b)**,  2.23 a) 
#### 1.19
e)
$$
\begin{align}
\left| 3-(-2)^{2} \right| =\left| 3-2 \right| =\left| 1 \right| =1
\end{align}
$$
f)
$$
\begin{align}
|\pi -3|=\pi-3
\end{align}
$$
g)
$$
\begin{align}
|2-\pi|=-(2-\pi)=-2+\pi & =\pi-2
\end{align}
$$
2.20
a)
$$
\begin{align}
|x| = 2 \implies\\
\left\{ \begin{array}{lll}
x_{1}=-2 \\
x_{2}=2
\end{array} \right. 
\end{align}
$$
c)
$$
\begin{align}
|x+1|<2 \\
|x+1|=\left\{ \begin{array}{lll}
 & x+1, & x\geq -1 \\
 & -x-1, & x< -1
\end{array} \right.
\end{align}
$$
for $x\geq-1$
$$
\begin{align}
x+1<2 \\
x<1
\end{align}
$$
for $x<-1$
$$
\begin{align}
-x-1<2 \\
x+1>2 \\
x>1
\end{align}
$$
2.22
b)
$$
\begin{align}
|x-1|+|x-2|=3 \\
|x-1|=\left\{ \begin{array}{lll}
 & x-1, & x\geq 1 \\
 & 1-x, & x< 1
\end{array} \right. \\
|x-2|=\left\{ \begin{array}{lll}
 & x-2, & x\geq 2 \\
 & 2-x, & x< 2
\end{array} \right. \\
\end{align}
$$
answer is probably $x_{1}=3,x_{2}=0$ but not sure why
$x<1$
$$
\begin{align}
|x-1|+|x-2|=3 \\
(1-x)+(2-x)=3 \\
1-x+2-x=3 \\
3-x=3 \\
0=x
\end{align}
$$
$x$ correctly exists within the span

$1<x<2$
$$
\begin{align}
|x-1|+|x-2|=3 \\
(x-1)+(2-x)=3 \\
1=3
\end{align}
$$
not valid, no $x$ within the span
$2<x$
$$
\begin{align}
|x-1|+|x-2|=3 \\
(x-1)+(x-2)=3 \\
2x-3=3 \\
2x=6 \\
x=3
\end{align}
$$
$x$ correctly exists within the span

|     | <--   | 1   | --- | 2   | -->   |
| --- | ----- | --- | --- | --- | ----- |
|     | $x=0$ |     | N/A |     | $x=3$ |

