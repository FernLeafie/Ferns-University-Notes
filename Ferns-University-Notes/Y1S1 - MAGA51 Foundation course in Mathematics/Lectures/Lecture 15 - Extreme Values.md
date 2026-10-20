There are three candidates to max and minimum values
- Stationary points ${}f'(a)=0{}$
- Singular points ${}\nexists f'(a){}$
- End points of the functions domain or interval 

- ${}f''(x)\geq 0{}$ for an interval ${}l\implies f{}$ is convex in ${}l{}$
- ${}f''(x)\leq 0{}$ for an interval ${}l\implies f{}$ is concave in ${}l{}$
Inflection point is when a function goes from convex to concave or vise versa
it's the point where the angle of the graph goes from increasing, to decreasing, or the reverse
## Examples
### 1.
Decide if possible the largest and smallest value for 
#### a)
${}f(x)=3x^{1/3}-x,x \in[-8,8]{}$

$$
\begin{align}
f(x)=3x^{1/3}-x \\
f'(x)=x^{-2/3}-1=\dfrac{1}{x^{2/3}}-\dfrac{x^{2/3}}{x^{2/3}}=\dfrac{1-x^{2/3}}{x^{2/3}} \\
f'(x)=0\iff \dfrac{1-x^{2/3}}{x^{2/3}}=0\implies 1-x^{2/3}\iff x^{2/3}=1\iff x^{2}=1 \iff x=\pm 1 \in[-8,8]
\end{align}
$$
Singular points require ${}\exists f(a), \nexists f'(a){}$

$$
\begin{align}
D_{f}=[-8,8] \\
D_{f'}=[-8,8] \setminus \{ 0 \}
\end{align}
$$
${}0{}$ is a singular point, ${}f(0)=0{}$
There are two end points, ${}x=-8{}$ and ${}x=8{}$


|  ${}x{}$   | ${}-8{}$ | ${}\longleftrightarrow{}$ | ${}-1{}$ | ${}\longleftrightarrow{}$ | ${}0{}$ | ${}\longleftrightarrow{}$ | ${}1{}$ | ${}\longleftrightarrow{}$ | ${}8{}$  |
| :--------: | :------: | :-----------------------: | :------: | :-----------------------: | :-----: | :-----------------------: | :-----: | :-----------------------: | :------: |
| ${}f(x){}$ | ${}2{}$  |      ${}\searrow{}$       |    -2    |      ${}\nearrow{}$       | ${}0{}$ |      ${}\nearrow{}$       | ${}2{}$ |      ${}\searrow{}$       | ${}-2{}$ |
|            |   max    |                           |   min    |                           |         |                           |   max   |                           |   min    |
#### b
${}f(x)=\dfrac{x^{2}}{\sqrt{ 9-x^{2} }}{}$
Find domain
${}D_{\div}=9-x^{2}\neq 0\iff x^{2}\neq 9\iff x\neq\pm 3{}$
${}D_{\sqrt{}}=9-x^{2}\geq 0\iff(3-x)(3+x)\geq 0{}$

|        ${}x{}$        |         | ${}-3{}$ |         | ${}3{}$ |         |
| :-------------------: | :-----: | :------: | :-----: | :-----: | :-----: |
|       ${}3-x{}$       | ${}+{}$ | ${}+{}$  | ${}+{}$ | ${}0{}$ | ${}-{}$ |
|       ${}3+x{}$       | ${}-{}$ | ${}0{}$  | ${}+{}$ | ${}+{}$ | ${}+{}$ |
| ${}\mathrm{L.H.S.}{}$ | ${}-{}$ | ${}0{}$  | ${}+{}$ | ${}0{}$ | ${}-{}$ |
${}D_{\sqrt{  }}=[-3,3]{}$
${}D_{f}=[-3,3]\setminus \{ -3,3 \}=(-3,3){}$
This implies a lack of end points
Find ${}f'(x){}$

$$
\begin{align}
f(x)=\dfrac{x^{2}}{\sqrt{ 9-x^{2} }} \\
f'(x)=\dfrac{2x\sqrt{ 9-x^{2} }-x^{2}\left( -\dfrac{x}{\sqrt{ 9-x^{2} }} \right)}{9-x^{2}}=\dfrac{\dfrac{2x(9-x^{2})+x^{3}}{\sqrt{ 9-x^{2} }}}{9-x^{2}} \\
=\dfrac{18x-x^{3}}{(9-x^{2})\sqrt{ 9-x^{2} }}
\end{align}
$$
Find stationary points

$$
\begin{align}
f'(x)=0\implies 18x-x^{3}=0 \iff x(18-x)=0 \\
\iff \left\{ \begin{array}{ll}
x_{1}=0, & x_{1}\in(-3,3) \\
x_{2}=\sqrt{ 18 }=3\sqrt{ 2 }, & x_{2}\notin(-3,3) \\
x_{3}=-\sqrt{ 18 }=-3\sqrt{ 2 }, & x_{3}\notin(-3,3)
\end{array} \right. 
\end{align}
$$
Find singular points
${}D_{f}=D_{f'}=(-3,3)\implies\text{no singularities}{}$


|   ${}x{}$   | ${}(-3{}$ |                | ${}0{}$ |                | ${}3){}$ |
| :---------: | :-------: | :------------: | :-----: | :------------: | :------: |
| ${}f'(x){}$ |  ${}-{}$  |    ${}-{}$     | ${}0{}$ |    ${}+{}$     | ${}+{}$  |
| ${}f(x){}$  |           | ${}\searrow{}$ | ${}0{}$ | ${}\nearrow{}$ |          |
|             |           |                |   min   |                |          |
#### c
${}f(x)=\dfrac{2x}{\sqrt{ x^{2}+4 }}{}$
##### Step 1 definition
${}D_{f}=\mathbb{R}{}$, so no end points
##### Step 2 find derivative

$$
\begin{align}
f(x)=\dfrac{2x}{\sqrt{ x^{2}+4 }} \\
f'(x)=\dfrac{2\sqrt{ x^{2}+4 }-(2x) \dfrac{1}{\cancel{ 2 }x\sqrt{ x^{2}+4 }} \cancel{ 2 }x}{(x^{2}+4)} \\
\dfrac{2x^{2}+8-2x^{2}}{\sqrt{ x^{2}+4 }(x^{2}+4)}=\dfrac{8}{\sqrt{ x^{2}+4 }(x^{2}+4)}
\end{align}
$$
##### Step 3 stationary points
${}f'(x)=0\implies 8=0 \implies \nexists f'(x)=0{}$
##### Step 4 singular points
${}D_{f'}=D_{f}=\mathbb{R}\implies\text{no stationary points}{}$

Answer: no max or minimum values
### 2.
Study the function ${}f(x)=\dfrac{x^{2}}{9-x^{2}}{}$ (eventual extreme or terass points)
#### Step 1 find the domain

$$
\begin{align}
D_{f}=\{ 9-x^{2} \neq 0 \}=\{ 9\neq x^{2} \}=\{ \pm3\neq x \}=\mathbb{R}\setminus \{ \pm 3 \}
\end{align}
$$
#### Step 2, odd/even/none?
${}f(-x)=\dfrac{(-x)^{3}}{9-(-x)^{2}}=-\underbrace{ \dfrac{3x^{3}}{9-x^{2}} }_{ f(x) }=-f(x)\implies f\text{ is odd}{}$
#### Step 3 asymptotes
we skip this lol
#### Step 4 first derivative

$$
\begin{align}
f'(x)=\left( \dfrac{x^{3}}{9-x^{2}} \right)'=\dfrac{3x^{2}(9-x^{2})-x^{3}(-2x)}{(9-x^{2})^{2}}=\dfrac{27x^{2}-3x^{4}+2x^{4}}{(9-x^{2})^{2}}=\dfrac{27x^{2}-x^{4}}{(9-x^{2})^{2}} \\
=\dfrac{x^{2}(27-x^{2})}{(9-x^{2})^{2}}=\dfrac{x^{2}(3\sqrt{ 3} -x)(3\sqrt{ 3 }+x)}{(3-x)^{2}(3+x)^{2}}= \\
f'(x)=0\iff x^{2}(3\sqrt{ 3} -x)(3\sqrt{ 3 }+x)=0 \\
\left\{ \begin{array}{lll}
x_{1}=0 \\
x_{2}=3\sqrt{3} \\
x_{3}=-3\sqrt{ 3 }
\end{array} \right. 
\end{align}
$$
${}D_{f}=D_{f'}=\mathbb{R}\setminus \{ \pm 3 \}{}$

#### Step ?? table

|   ${}x{}$   |                |      ${}-3\sqrt{ 3 }{}$      |                | ${}-3{}$ |                | ${}0{}$ |                | ${}3{}$ |                |       ${}3\sqrt{ 3 }{}$       |                |
| :---------: | :------------: | :--------------------------: | :------------: | :------: | :------------: | :-----: | :------------: | :-----: | :------------: | :---------------------------: | :------------: |
| ${}f'(x){}$ |    ${}-{}$     |           ${}0{}$            |    ${}+{}$     |   N/A    |    ${}+{}$     | ${}0{}$ |    ${}+{}$     |   N/A   |    ${}+{}$     |            ${}0{}$            |    ${}-{}$     |
| ${}f(x){}$  | ${}\searrow{}$ | ${}\dfrac{9\sqrt{ 3 }}{3}{}$ | ${}\nearrow{}$ |          | ${}\nearrow{}$ |    0    | ${}\nearrow{}$ |         | ${}\nearrow{}$ | ${}-\dfrac{9\sqrt{ 3 }}{2}{}$ | ${}\searrow{}$ |
|             |                |           loc min            |                |          |                |  terr   |                |         |                |            loc max            |                |
