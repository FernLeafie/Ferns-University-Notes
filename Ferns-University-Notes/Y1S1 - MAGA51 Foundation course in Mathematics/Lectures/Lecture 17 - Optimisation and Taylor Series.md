Taylor polynomial:
$$
f(a)+f'(a)(x-a)+f''(a)\dfrac{(x-a)^{2}}{2!}+\dots+f^{(n)}(a) \dfrac{(x-a)^{n}}{n!}+\underbrace{ R_{n+1}(x) }_{ \text{Rest} }
$$
MacLaurin: if ${}a=0{}$:
$$
f(x)=f(0)+f'(0)*x+f''(0)\dfrac{x^{2}}{2!}+\dots
$$


$$
\begin{align}
f(x)=y_{n}(x)+O(x^{n+1}) \\
O(x^{n+1}) = Kx^{n+1}
\end{align}
$$
## Examples
Problem:
A storage tank consists of a flipped cone, tipped by a half sphere, the cone, and the sphere have a radius of ${}r{}$, and a height of ${}h{}$. The tank should store a total of ${}30\pi \pu{ m^{3} }{}$.
Material costs
- Cones mantel area: ${}60 \pu{ kr/m^{2} }{}$
- Spheres area: ${}70\pu{ kr/m^{2} }{}$

${}r=\text{radius in metre}{}$
${}h=\text{height in metre}{}$
${}A_{\text{cone mantle}}=\pi r\sqrt{ r^{2}+h^{2} }{}$
${}A_{\text{sphere}}=4\pi r^{2}\iff A_{\text{half sphere}}=2\pi r^{2}{}$
${}V_{\text{cone}}=\dfrac{\pi r^{2}h}{3}{}$
${}V_{\text{sphere}}=\dfrac{4}{3}\pi r^{3}\iff V_{\text{half sphere}}=\dfrac{2}{3}\pi r^{3}{}$


$$
\begin{align}
\dfrac{2}{3}\pi r^{3}+\dfrac{\pi r^{2}h}{3}=30\pi \\
\iff \dfrac{2}{3}r^{3}+\dfrac{r^{2}h}{3}=30 \iff 2r^{3}+r^{2}h=90\iff h=\dfrac{90-2r^{3}}{r^{2}} \iff h=\dfrac{90}{r^{2}}-2r
\end{align}
$$
${}h>0{}$
${}\dfrac{90}{r^{2}}-2r>0\iff 90-2r^{3}>0\iff 45-r^{3}>0\iff -r>-\sqrt[3]{ 45 } \iff r<\sqrt[3]{ 45 }{}$
${}C_{\text{cone}}=60\pi r\sqrt{ r^{2}+h^{2} }{}$
${}C_{\text{half sphere}}=70*2\pi r^{2}{}$
${}C_{tot}=60\pi r\sqrt{ r^{2}+h^{2} }+70*2\pi r^{2}{}$
${}C_{tot}(r)=60\pi r\sqrt{ r^{2}+\left( \dfrac{90}{r^{2}}-2r \right)^{2} }+70*2\pi r^{2}{}$
${}C'(3)=0{}$

## Exercises
### 1

$$
\begin{align}
\lim_{ x \to 0 } \dfrac{\sin(3x)-3\ln(1+2x)}{4e^{2x}-8x^{2}-4x-4}=\ `` \dfrac{0}{0} "
\end{align}
$$
since the one statement already polynomial is of the second degree, all the others should be estimated of at least the second degree
$$
\begin{align}
\sin(3x)=3x+O(x^{3}) \\
\ln(1+2x)=2x+O(x^{2}) \\
e^{ 2x }=1+2x+\dfrac{(2x)^{2}}{2!}+O(x^{3})=1+2x+2x^{2}+O(x^{3})
\end{align}
$$

$$
\begin{align}
\lim_{ x \to 0 } \dfrac{(3x+O(x^{3}))-3(2x+O(x^{2}))}{4(1+2x+2x^{2}+O(x^{3}))-8x^{2}-4x-4}= \\
\lim_{ x \to 0 } \dfrac{3x+O(x^{3})-6x-3O(x^{2})}{\cancel{ 4+ }8x\cancel{ +8x^{2} }+4O(x^{3}))\cancel{ -8x^{2} }-4x\cancel{ -4 }} \\
\lim_{ x \to 0 } \dfrac{-3x+O(x^{3})-O(x^{2})}{4x+O(x^{3})} =\ `` \dfrac{0}{0} " \\
\lim_{ x \to 0 } \dfrac{\cancel{ x }(-3+O(x^{2})-O(x))}{\cancel{ x }(4+O(x^{2}))}=\ `` \dfrac{-3+0-0}{4+0} "=-\dfrac{3}{4}
\end{align}
$$
Now the same shit but with L'Hôpital.

$$
\begin{align}
\lim_{ x \to 0 } \dfrac{\sin(3x)-3\ln(1+2x)}{4e^{2x}-8x^{2}-4x-4}=\ `` \dfrac{0}{0} "\ \overset{\text{L'H}}{=}\dfrac{\cos(3x)3-3 \dfrac{1}{1+2x}2}{4 e^{ 2x }2-16x-4}=\ `` \dfrac{3-3\dfrac{1}{1}2}{4*1*2-0-4} "\ =\ `` \dfrac{3-6}{8-4} "\ =-\dfrac{3}{3}
\end{align}
$$
### 2

$$
\begin{align}
\lim_{ x \to 0 } \dfrac{2 e^{ 3x^{2} } -2\cos(4x)}{\arctan(4x^{2})}
\end{align}
$$

$$
\begin{align}
e^{ 3x^{2} }=1+3x^{2}+O((x^{2})^{2})=1+3x^{2}+O(x^{4}) \\
\cos(4x)=1-\dfrac{(4x)^{2}}{2!}+O((4x^{2})^{2})=1-8x^{2}+O(x^{4}) \\
\arctan(4x^{2})=4x^{2}+O((x^{2})^{3})=4x^{2}+O(x^{6})
\end{align}
$$

$$
\begin{align}
\lim_{ x \to 0 } \dfrac{2 e^{ 3x^{2} } -2\cos(4x)}{\arctan(4x^{2})}=\lim_{ x \to 0 } \dfrac{2(1+3x^{2}+O(x^{4}))-2(1-8x^{2}+O(x^{4}))}{4x^{2}+O(x^{6})} \\
\lim_{ x \to 0 } \dfrac{22x^{2}+O(x^{4})}{4x^{2}+O(x^{6})}=\lim_{ x \to 0 } \dfrac{x^{2}(22+O(x^{2}))}{x^{2}(4+O(x^{4}))}=\ `` \dfrac{22+0}{4+0} " \ =\dfrac{11}{2}
\end{align}
$$
### 3
You have a wooden ball from which you're supposed to cut a cylinder of as large a volume as possible. How many percent of the ball will you have to cut away.


$$
\begin{align}
r=\text{cyl radius} \\
R=\text{spheres radius} \\
h=\text{cyl height} \\
V_{\text{cyl}}=\text{cyl volume} \\
V_{\text{sphere}}=\text{sphere volume}
\end{align}
$$
![[Lecture 17 - Optimisation and Taylor Series 2026-10-28 11.45.10.excalidraw]]

$$
\begin{align}
V_{cyl}=\pi r^{2}h \\
\dfrac{h}{2}^{2}+r^{2}=R^{2} \\
V_{\text{cyl}}(h)=\pi h\left( R^{2}-\dfrac{h^{2}}{4} \right)=\pi R^{2}-\dfrac{\pi}{4}h^{3} \\
V'_{\text{cyl}}(h)=\pi R^{2}-\dfrac{\pi}{4}3h^{2}=0 \implies h^{2}=\dfrac{\pi R^{2}}{\dfrac{3\pi}{4}}=\dfrac{4R^{2}}{4}\iff h=\dfrac{2R}{\sqrt{ 3 }} \\
V_{\text{cyl max}}=\pi \dfrac{2R}{\sqrt{ 3 }}\left( R^{2}-\dfrac{R^{2}}{3} \right)=\dfrac{2\pi}{\sqrt{ 3 }}R \dfrac{2R^{2}}{3}=\dfrac{4\pi R^{3}}{3\sqrt{ 3 }} \\
V_{\text{sphere}}=\dfrac{4\pi R^{3}}{3} \\
\dfrac{V_{\text{cyl max}}}{V_{\text{cyl}}}=\dfrac{1}{\sqrt{ 3 }}
\end{align}
$$