Constructing curves
1. Decide the functions domain
2. Find possible symmetry, odd or even
3. Find possible asymptotes
	1. Vertical asymptotes
	2. Horizontal asymptotes
	3. Slanted/oblique asymptotes
4. Study the derivative

## Examples
### 1.
Let ${}f(x)=\dfrac{\sqrt{ x^{2}-1 }-1}{|x|-2}{}$
#### a)
find the domain for ${}f{}$
Due to the division

$$
\begin{align}
|x|-2\neq 0\implies|x|\neq 2\implies x\neq\pm 2
\end{align}
$$
Due to root

$$
\begin{align}
x^{2}-1\geq 0\iff (x-1)(x+1)\geq 0
\end{align}
$$

| ${}x{}$               |         | ${}-1{}$ |         | ${}1{}$ |         |
| --------------------- | ------- | -------- | ------- | ------- | ------- |
| ${}x-1{}$             | ${}-{}$ | ${}-{}$  | ${}-{}$ | ${}0{}$ | ${}+{}$ |
| ${}x+1{}$             | ${}-{}$ | ${}0{}$  | ${}+{}$ | ${}+{}$ | ${}+{}$ |
| ${}\mathrm{L.H.S.}{}$ | ${}+{}$ | ${}0{}$  | ${}-{}$ | ${}0{}$ | ${}+{}$ |
${}x \in(-\infty,-1]\cup[1,\infty){}$#
${}D_{f}=(-\infty,-2)\cup(-2,-1]\cup [1,2)\cup(2,\infty){}$
#### b)
Find all asymptotes for ${}f{}$
##### Vertical Asymptotes
${}\pm 2 \not\in D_{f}\implies x=\pm 2{}$ candidates for vertical asymptotes
###### Negative Two

$$
\begin{align}
l_{l}=\lim_{ x \to -2^{-} } f(x)=\ `` \dfrac{\sqrt{ 3 }-1}{+0} "=\infty \\
l_{r}=\lim_{ x \to -2^{+} } f(x)=\ `` \dfrac{\sqrt{ 3 }-1}{-0} "=-\infty 
\end{align}
$$
###### Positive Two

$$
\begin{align}
l_{l}=\lim_{ x \to 2^{-} } f(x)=\ `` \dfrac{\sqrt{ 3 }-1}{-0} "=-\infty \\
l_{r}=\lim_{ x \to 2^{+} } f(x)=\ `` \dfrac{\sqrt{ 3 }-1}{+0} "=\infty 
\end{align}
$$
##### Horizontal Asymptotes

$$
\begin{align}
\lim_{ x \to \infty } f(x)=\lim_{ x \to \infty } \dfrac{\sqrt{ x^{2}-1 }-1}{|x|-2}=\lim_{ x \to \infty } \dfrac{\sqrt{ x^{2}-1 }-1}{x-2} =`` \dfrac{\infty}{\infty} "=[\text{get the fastest growing function}] \\
\lim_{ x \to \infty } \dfrac{\cancelto{ \cancel{ x } }{ |x| }\left( \sqrt{ 1-\dfrac{1}{x^{2}} }-\dfrac{1}{x} \right)}{\cancel{ x }\left( 1-\dfrac{2}{x} \right)}=`` \dfrac{\sqrt{ 1-0 }-0}{1-0} "=1
\end{align}
$$

$$
\begin{align}
\lim_{ x \to -\infty } f(x)=\lim_{ x \to -\infty } \dfrac{\cancelto{ \cancel{ -x } }{ |x| }\left( \sqrt{ 1-\dfrac{1}{x^{2}} }-\dfrac{1}{|x|} \right)}{\cancel{ -x }\left( 1+\dfrac{2}{x} \right)}=\ `` \dfrac{\sqrt{ 1-0 }-0}{1+0} "1
\end{align}
$$
##### Oblique Asymptotes
Nope, since both directions are already accounted for as horizontal asymptotes
### 2
Analyse ${}f(x)=\dfrac{x^{3}-x^{2}+1}{x^{2}-1}{}$
#### Step 1
Domain and intersections with ${}x{}$ and ${}y{}$ axis

$$
\begin{align}
x^{2}-1\neq 0\iff x^{2}\neq 1\iff x\neq\pm 1 \\
D_{f}=\mathbb{R}\setminus \{ \pm 1 \}
\end{align}
$$

$$
\begin{align}
\cap O_{y}:f(0)=\dfrac{1}{-1}=-1 \implies A=(0,-1) \in G_{f} \\
\cap O_{x}: y=0 \implies f(x)=0 \implies x^{3}-x^{2}+1=0\implies x\approx -0.75
\end{align}
$$
#### Step 2
Asymptotes
${}x=\pm 1{}$ are candidates for vertical asymptotes
##### Vertical Asymptotes
###### Negative 1
$$
\begin{align}
l_{l}=\lim_{ x \to -1^{-} } f(x)=\ `` \dfrac{-1\cancel{ -1+1 }}{+0} "=-\infty \\
l_{r}=\lim_{ x \to -1^{+} } f(x)=\ `` \dfrac{-1\cancel{ -1+1 }}{-0} "=\infty \\
\end{align}
$$
###### Positive 1
$$
\begin{align}
l_{l}=\lim_{ x \to 1^{-} } f(x)=\ `` \dfrac{1\cancel{ -1+1 }}{-0} "=-\infty \\
l_{r}=\lim_{ x \to 1^{+} } f(x)=\ `` \dfrac{1\cancel{ -1+1 }}{+0} "=\infty \\
\end{align}
$$
#### Horizontal Asymptotes

$$
\begin{align}
\lim_{ x \to \infty } \dfrac{x^{3}-x^{2}+1}{x^{2}-1}=\ `` \dfrac{\infty}{\infty} " \overset{\text{L'H}}{=}\lim_{ x \to \infty } \dfrac{3x^{2}-2x}{2x}=\lim_{ x \to \infty } \dfrac{\cancel{ x }(3x-2)}{2\cancel{ x }}=\infty \\
\implies \text{There are no horizontal asymptotes} \\
\text{In the same way} \lim_{ x \to -\infty } f(x)=-\infty 
\end{align}
$$
#### Oblique Asymptotes
##### General Method
Let ${}y=ax+b{}$ be our asymptote

$$
\begin{align}
a=\lim_{ x \to \infty } \dfrac{f(x)}{x}=\lim_{ x \to \infty } \dfrac{\dfrac{x^{3}-x^{2}+1}{x^{2}-1}}{x}= \lim_{ x \to \infty } \dfrac{x^{3}-x^{2}+1}{x^{3}-x}=\ `` \dfrac{\infty}{\infty} " \\
\overset{\text{L'H}}{=}\lim_{ x \to \infty } \dfrac{3x^{2}-2x}{3x^{2}-1}\overset{\text{L'H}}{=}\lim_{ x \to \infty } \dfrac{6x-2}{6x}=\overset{\text{L'H}}{=}\lim_{ x \to \infty } \dfrac{6}{6}=1
\end{align}
$$

$$
\begin{align}
b=\lim_{ x \to \infty } (f(x)-ax)=\lim_{ x \to \infty } \left( \dfrac{x^{3}-x^{2}+1}{x^{2}-1} -x\right)=-1
\end{align}
$$
Oblique asymptote: ${}y=x-1{}$
##### Division Specific Method
For rational functions of the form ${}\dfrac{P(x)}{Q(x)}{}$, where ${}\text{Degree }P(x)=\text{Degree }Q(x)+1{}$

$$
f(x)=\dfrac{P(x)}{Q(x)}=\overbrace{ T(x) }^{ \text{1st degree} }+\dfrac{\overbrace{ R(x) }^{ \text{Degree }Q>\text{Degree} R }}{Q(x)}
$$
The oblique asymptote then becomes ${}y=T(x){}$

$$
\dfrac{x^{3}-x^{2}+1}{x^{2}-1}=(x-1)+\dfrac{x}{x^{2}-1}
$$
Oblique asymptote: ${}y=x-1{}$
#### Step 3
Derivative

$$
\begin{align}
f'(x)=\dfrac{(3x^{2}-2x)(x^{2}-1)-(x^{3}-x^{2}+1)2x}{(x^{2}-1)^{2}}=\dfrac{3x^{4}-3x^{2}\cancel{ -2x^{3} }\cancel{ +2x }-2x^{4}\cancel{ +2x^{3} }\cancel{ -2x }}{(x^{2}-1)^{2}} \\
\dfrac{x^{4}-3x^{2}}{(x^{2}-1)^{2}}=\dfrac{x^{2}(x^{2}-3)}{(x^{2}-1)^{2}}=\dfrac{x^{2}(x-\sqrt{ 3 })(x+\sqrt{ 4 })}{(x+1)^{2}(x-1)^{2}}
\end{align}
$$
Stationary: ${}f'(x)=0\implies x_{1}=0,x_{2}=\sqrt{ 3 },x_{3}=-\sqrt{ 3 }{}$
Singular: None ${}D_{f}=D_{f'}{}$


|      ${}x{}$       |                | ${}-\sqrt{ 3 }{}$ |                | ${}-1{}$ |                | ${}0{}$  |                | ${}1{}$ |                | ${}\sqrt{ 3 }{}$ |                |
| :----------------: | :------------: | :---------------: | :------------: | :------: | :------------: | :------: | :------------: | :-----: | :------------: | :--------------: | :------------: |
|    ${}x^{2}{}$     |    ${}+{}$     |      ${}+{}$      |    ${}+{}$     | ${}+{}$  |    ${}+{}$     | ${}0{}$  |    ${}+{}$     | ${}+{}$ |    ${}+{}$     |     ${}+{}$      |    ${}+{}$     |
| ${}x-\sqrt{ 3 }{}$ |    ${}-{}$     |      ${}-{}$      |    ${}-{}$     | ${}-{}$  |    ${}-{}$     | ${}-{}$  |    ${}-{}$     | ${}-{}$ |    ${}-{}$     |     ${}0{}$      |    ${}+{}$     |
| ${}x+\sqrt{ 3 }{}$ |    ${}-{}$     |      ${}0{}$      |    ${}+{}$     | ${}+{}$  |    ${}+{}$     | ${}+{}$  |    ${}+{}$     | ${}+{}$ |    ${}+{}$     |     ${}+{}$      |    ${}+{}$     |
|  ${}(x-1)^{2}{}$   |    ${}+{}$     |      ${}+{}$      |    ${}+{}$     | ${}+{}$  |    ${}+{}$     | ${}+{}$  |    ${}+{}$     | ${}0{}$ |    ${}+{}$     |     ${}+{}$      |    ${}+{}$     |
|  ${}(x+1)^{2}{}$   |    ${}+{}$     |      ${}+{}$      |    ${}+{}$     | ${}0{}$  |    ${}+{}$     | ${}+{}$  |    ${}+{}$     | ${}+{}$ |    ${}+{}$     |     ${}+{}$      |    ${}+{}$     |
|      ${}f'{}$      |    ${}+{}$     |      ${}0{}$      |    ${}-{}$     |   N/A    |    ${}-{}$     | ${}0{}$  |    ${}-{}$     |   N/A   |    ${}-{}$     |     ${}0{}$      |    ${}+{}$     |
|      ${}f{}$       | ${}\nearrow{}$ |                   | ${}\searrow{}$ |          | ${}\searrow{}$ | ${}-1{}$ | ${}\searrow{}$ |         | ${}\searrow{}$ |                  | ${}\nearrow{}$ |
|                    |                |   local<br>max    |                |          |                | terrass  |                |         |                |   local<br>min   |                |
