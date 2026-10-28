Material to cover:
- Examples from lectures
- Exercises from discussions in lectures
- Exercises from group exercises
- Exercises from Dugga 1 and Dogga 2
- Recommended exercises
- Old Tentas

Clear presentations

### Areas of Improvement
- Learn different between concave and convex
  concave is negative
  convex is positive
- Maclaurin
## Examples
### 
Decide domain, eventual asymptotes, local extreme and terrace points for the function
$$
\begin{align}
f(x)=\dfrac{5x-x^{3}}{x^{2}-16}
\end{align}
$$
Study the derivative and which intervals the function is concave and convex, and decide possible inflection points, and draw the graph.
#### Step 1
Due to division ${}\implies x^{2}-16 \neq 0 \iff x^{2}\neq 16 \iff x^{2} \neq \pm 4\implies D_{f}=\mathbb{R}\setminus \{ \pm 4 \}, D_{f}:x\neq\pm 4{}$
${}\cap Ox: y=0\iff f(x)=0\iff 5x-x^{3}=0\iff x(5-x^{2})=0\iff \left\{ \begin{array}{ll}x_{1}=0 \\  x_{2}=\sqrt{ 5 } \\  x_{3}=-\sqrt{ 5 }\end{array} \right.{}$
${}\cap Oy:x=0\implies f(0)=0\iff O(0,0){}$
#### Step 2 Symmetry
${}f(-x)=-f(x){}$, the function is odd, and symmetrical around the origin
#### Step 3 Asymptotes
##### A) Vertical Asymptotes

$$
\begin{align}
l_{l}=\lim_{ x \to -4^{-} } \dfrac{5x-x^{3}}{x^{2}-16} =\ `` \dfrac{-20+64}{+0} "\ =+\infty \\
l_{r}=\lim_{ x \to -4^{+} } \dfrac{5x-x^{3}}{x^{2}-16} =\ `` \dfrac{-20+64}{-0} "\ =-\infty \\
\end{align}
$$
${}x=-4, \text{v.a. to}\left\{ \begin{array}{lll}\infty,\text{to the left} \\  -\infty,\text{to the right}\end{array} \right.{}$
$$
\begin{align}
l_{l}=\lim_{ x \to 4^{-} } \dfrac{5x-x^{3}}{x^{2}-16} =\ `` \dfrac{20-64}{-0} "\ =+\infty \\
l_{r}=\lim_{ x \to 4^{+} } \dfrac{5x-x^{3}}{x^{2}-16} =\ `` \dfrac{20-64}{+0} "\ =-\infty \\
\end{align}
$$
${}x=4, \text{v.a. to}\left\{ \begin{array}{lll}\infty,\text{to the left} \\  -\infty,\text{to the right}\end{array} \right.{}$
##### Horizontal Asymptotes

$$
\begin{align}
\lim_{ x \to \infty } \dfrac{5x-x^{3}}{x^{2}-16}=\ `` \dfrac{\infty-\infty}{\infty} "\ =\lim_{ x \to \infty } \dfrac{\cancelto{ x }{ x^{3} }\left( +\dfrac{5x}{x^{2}}-1 \right)}{\cancel{ x^{2} }\left( 1-\dfrac{16}{x^{2}} \right)}=\ `` \dfrac{\infty(0-1)}{1-0} "\ =-\infty
\end{align}
$$
(same with ${}-\infty{}$) ${}\implies \text{no horizozntal asymptotes}{}$
##### Oblique Asymptotes
${}\dfrac{5x-x^{3}}{x^{2}-16}=-x-\dfrac{11x}{x^{2}-16}{}$

$$
\begin{align}
f(x)=-x-\dfrac{11x}{x^{2}-16} \\
\lim_{ x \to \infty } f(x)-(-x)=\lim_{ x \to \infty } -\dfrac{11x}{x^{2}-16}=\ `` -\dfrac{\infty}{\infty} "\ =\lim_{ x \to \infty } \dfrac{-\cancel{ x }11}{\cancelto{ x }{ x^{2} }\left( 1-\dfrac{16}{xs^{2}} \right)}=\ `` \dfrac{-11}{\infty(1-0)} "\ =0
\end{align}
$$
${}y=-x{}$ is an oblique asymptote
#### Step 4 First Derivative

$$
\begin{align}
f'(x)=\dfrac{(5x-x^{3})'(x^{2}-16)-(5x-x^{3})(x^{2}-16)'}{(x^{2}-16)^{2}}=\dfrac{(5-3x^{2})(x^{2}-16)-(5x-x^{3})(2x)}{(x^{2}-16)^{2}} \\
=\dfrac{5x^{2}-80-3x^{4}+48x^{2}-10x^{2}+2x^{4}}{(x^{2}-16)^{2}}=\dfrac{-x^{4}+43x^{2}-80}{(x^{2}-16)^{2}} \\
f'(x)=0 \implies-x^{4}+43x^{2}-80 | x^{2}=t\geq 0 \\
-t^{2}+43t-80=0 \iff t^{2}-43t+80=0 \\
t_{1,2}=\dfrac{43}{2}\pm \sqrt{ \dfrac{43^{2}}{4}-80 }=\dfrac{43}{2}\pm \sqrt{ \dfrac{1849-320}{4} }=\dfrac{43}{2}\pm \sqrt{ \dfrac{1529}{4} }= \\
x^{2}=\dfrac{43}{2}+\dfrac{\sqrt{ 1529 }}{2} \\
x_{1,2}=\sqrt{ \dfrac{43}{2}+\dfrac{\sqrt{ 1529 }}{2} }
\end{align}
$$
Never mind this exercise is fucked, we're giving up.
### 2


$$
\begin{align}
V = \text{volume} \\
r = \text{radius} \\
h = \text{thickness} \\
t_{0}: V'(t_{0})=7\pu{ m^{3}/min } \\
r=\pu{ 100m } \\
h=\pu{ 0.005m } \\
r'(t_{0})=\pu{ 2m/min }
\end{align}
$$

$$
\begin{align}
V=A_{0}h=\pi r^{2}h \\
V(t)=\pi r^{2}(t)h(t) | \dfrac{d}{dt} \\
V'(t)=\pi(2r(t)r'(t)h(t)+r^{2}(t)h'(t)) \\
V'(t_{0})=\pi(2r(t_{0})r'(t_{0})h(t_{0})+r^{2}(t_{0})h'(t_{0})) \\
7=\pi(2*100*2*0.005+100^{2}*h'(t_{0})) \\
h'(t_{0})=\dfrac{7-2\pi}{100^{2}\pi} \\
h'(t_{0}) \text{ is positive, so the thickness is incresing}
\end{align}
$$
### 3
Let ${}f(x)=2\arcsin(2x){}$, and ${}g(x)=\sqrt{ x }{}$
a)
Decide ${}f^{-1}(x){}$, and its domain and range

$$
\begin{align}
\arcsin: [-1,1] \to \left[ -\dfrac{\pi}{2}, \dfrac{\pi}{2} \right] \\
2x \in[-1,1] \iff x \in \left[ -\dfrac{1}{2}, \dfrac{1}{2} \right] \\
D_{f}=\left[ -\dfrac{1}{2}, \dfrac{1}{2} \right] \\
\arcsin(2x) \in\left[ -\dfrac{\pi}{2}, \dfrac{\pi}{2} \right] \iff 2\arcsin(2x) \in\left[ -\pi, \pi \right] \\
V_{f}=\left[ -\pi, \pi \right]
\end{align}
$$

$$
\begin{align} \\
f(x)=y
2\arcsin(2x)=y \\
\arcsin(2x)=\dfrac{y}{2} \\
2x=\sin\left( \dfrac{y}{2} \right) \\
x=\dfrac{\sin\left( \dfrac{y}{2} \right)}{2} \\
f^{-1}(x)=\dfrac{\sin\left( \dfrac{x}{2} \right)}{2} \\
D_{f^{-1}}=[-\pi,\pi] \\
V_{f^{-1}}=\left[ -\dfrac{1}{2}, \dfrac{1}{2} \right]
\end{align}
$$
b)
Decide ${}(f\circ g)(x){}$, and its definition and range

$$
\begin{align}
(f\circ g)(x)=f(g(x))=2\arcsin(2\sqrt{ x })
\end{align}
$$
$$
\begin{align}
\arcsin\implies-1\leq 2\sqrt{ x }\leq 1\implies-\dfrac{1}{2}\leq \sqrt{ x } \leq \dfrac{1}{2}\iff 0\leq x\leq \dfrac{1}{4} \\
\sqrt{  }\implies x\geq 0 \\
D_{f\circ g}=\left[ 0, \dfrac{1}{4} \right] \\
V_{f\circ g}=[0,\pi]
\end{align}
$$
### 3
A cone is inscribed in a circle of radius ${}R=\pu{ 8cm}{}$, decide ${}r{}$ and ${}h{}$ so that the volume of the cone is as big as possible.

$$
\begin{align}
r=\text{radius of the cone} \\
R=\text{radius of the sphere}=\pu{ 8cm } \\
h=\text{height} \\
V_{\text{cone}}=\dfrac{1}{3}A_{b}h=\dfrac{1}{3}\pi r^{2}h
\end{align}
$$
![[Tenta - Repetition 2026-10-29 11.11.21.excalidraw]]

$$
\begin{align}
R^{2}=r^{2}+(h-R)^{2} \\
64=r^{2}+(h-8)^{2} \\
r^{2}=\cancel{ 64 }-(h^{2}-16h+\cancel{ 64 }) \\
r^{2}=-h^{2}+16h \\
 \\
-h^{2}+16h\geq 0 \\
h(h-16)\leq 0 \implies h \in[0,16] \\
 \\
V(h)=\dfrac{\pi}{3}(-h^{2}+16h)h=\dfrac{\pi}{3}(-h^{3}+16h^{2}) \\
V'(h)=\dfrac{\pi}{3}(-3h^{2}+32h) \\
V'(h)=0 \implies -3h^{2}+32h=0 \\
\left. \begin{array}{r}
h(-3h+32)=0 \\
h\neq 0
\end{array} \right\} -3h+32=0\iff  h=\dfrac{32}{3}
\end{align}
$$
Check if h is a max and calculate r
### 4
${}\left( \dfrac{1+i}{\sqrt{ x }} \right)^{17}{}$

$$
\begin{align}
1+i=z \\
|z|=\sqrt{ 1^{2}+i^{2} }=\sqrt{ 2 } \\
\tan \theta=\dfrac{1}{1}=1 \\
\theta = \dfrac{\pi}{4} \\
z=\sqrt{ 2 }\left( \cos \dfrac{\pi}{4}+i\sin \dfrac{\pi}{4} \right) \\
 \\
\dfrac{1+i}{\sqrt{ 2 }}=\dfrac{\cancel{ \sqrt{ 2 } }\left( \cos \dfrac{\pi}{4}+i\sin \dfrac{\pi}{4} \right)}{\cancel{ \sqrt{ 2 } }} \\
\left( \dfrac{1+i}{\sqrt{ x }} \right)^{17}=\cos \dfrac{17\pi}{4}+i\sin \dfrac{17\pi}{4} \\
\cos\left( \dfrac{16\pi+\pi}{4} \right)+i\sin\left( \dfrac{16\pi+\pi}{4} \right) \\
\cos\left( \dfrac{\pi}{4} \right)+i\sin\left( \dfrac{\pi}{4} \right) \\
\dfrac{1}{\sqrt{ 2 }}+i\dfrac{1}{\sqrt{ 2 }}=\dfrac{1+i}{\sqrt{ 2 }}
\end{align}
$$
### 6
Decide the amount ${}M=\{ x \in[0,\pi]| \cos(2x+1)=\sin(2x) \}{}$

$$
\begin{align}
\cos(2x+1)=\sin(2x) \\
\cos(2x+1)=\cos\left( \dfrac{\pi}{2}-2x \right)
\end{align}
$$
#### Case 1
$$
\begin{align}
2x+1=\dfrac{\pi}{2}-2x+2\pi n \\
4x=\dfrac{\pi}{2}-1+2n\pi \\
x=\dfrac{\pi}{8}-\dfrac{1}{4}+\dfrac{n\pi}{2}
\end{align}
$$

$$
\begin{align}
n=-1, & x=\dfrac{\pi}{8}-\dfrac{1}{4}-\dfrac{\pi}{2}, & <0, & \not\in x\\
n=0, & x=\dfrac{\pi}{8}-\dfrac{1}{4}, & >0, & \in x \\
n=1, & x=\dfrac{\pi}{8}-\dfrac{1}{4}+\dfrac{\pi}{2}, & >0, & \in x \\
n=2, & x=\dfrac{\pi}{8}-\dfrac{1}{4}+\dfrac{2\pi}{2}, & >\pi, & \not\in x
\end{align}
$$
#### Case 2
$$
\begin{align}
\cancel{ 2x }+1=-\dfrac{\pi}{2}\cancel{ -2x }+2\pi n \\
1\neq-\dfrac{\pi}{2}+2n\pi \\
x \in \varnothing
\end{align}
$$
#### Result

$$
\begin{align}
M= \left\{  \dfrac{\pi-2}{8}, \dfrac{5\pi-2}{8}  \right\}
\end{align}
$$
### 7

$$
\begin{align}
f(x)=(\sin x)^{\sqrt{ x }} | \ln \\
\ln(f(x))=\sqrt{ x }\ln \sin x \\
\dfrac{1}{f(x)} f'(x)=\dfrac{1}{2\sqrt{ x }}\ln(\sin x)+\sqrt{ x} \dfrac{1}{\sin x}\cos x \\
f'(x)=(\sin x)^{\sqrt{ x }}\left(\dfrac{1}{2\sqrt{ x }}\ln(\sin x)+\sqrt{ x} \dfrac{1}{\sin x}\cos x\right)| x=\dfrac{\pi}{2} \\
f'\left( \dfrac{\pi}{2} \right)=\underbrace{ \underbrace{ \left( \sin \dfrac{\pi}{2} \right) }_{ 1 }^{\sqrt{ \pi/2 }} }_{ 1 }\left( \dfrac{1}{2\sqrt{ \dfrac{\pi}{2} }}\underbrace{ \ln(1) }_{ 0 } +\sqrt{ \dfrac{\pi}{2} }\dfrac{\overbrace{ \cos\left( \dfrac{\pi}{2} \right) }^{ 0 }}{\sin\left( \dfrac{\pi}{2} \right)}\right)=0
\end{align}
$$
### 8 

$$
\begin{align}
\lim_{ x \to -\infty } \dfrac{1}{\sqrt{ 4x^{2}+x }-\sqrt{ 4x^{2}+4 }}=\ `` \dfrac{1}{\infty-\infty} "\ =\lim_{ x \to -\infty } \dfrac{\sqrt{ 4x^{2} +x}+\sqrt{ 4x^{2}+4 }}{(\sqrt{ 4x^{2} +x}+\sqrt{ 4x^{2}+4 })(\sqrt{ 4x^{2}+x }-\sqrt{ 4x^{2}+4 })} \\
\lim_{ x \to -\infty } \dfrac{\sqrt{ 4x^{2}+x }+\sqrt{ 4x^{2}+4 }}{(\cancel{ 4x^{2} }+x)-(\cancel{ 4x^{2} }+4)}=\ `` \dfrac{\infty}{\infty} "\ =\lim_{ x \to -\infty } \dfrac{ \cancelto{ -1 }{ |x| }\left( \sqrt{ 4+\dfrac{1}{x} }+ \sqrt{ 4+\dfrac{4}{x^{2}} } \right)}{\cancel{ x }\left( 1-\dfrac{4}{x} \right)}=\ `` \dfrac{-1(\sqrt{ 4+0 }+\sqrt{ 4+0 }}{1-0}) "\ \\
=-1(\sqrt{ 4 }+\sqrt{ 4 })=-1(2+2)=-4
\end{align}
$$
### 9

$$
\begin{align}
\ln \left( \dfrac{x^{2}+y^{2}}{y} \right)+\cos(xy^{3})+2\arctan y
\end{align}
$$
in ${}(0,1){}$
### 10
Decide ${}\lim_{ x \to 0 }\dfrac{x\sin(3x)}{\arcsin(x^{2})}{}$ with Maclaurin developments

$$
\begin{align}
\sin x=x+O(x^{3}) \\
\arcsin x=0+x+O(x^{3}) \\
\sin 3x=3x+O(x^{3}) \\
\arcsin(x^{2})=x^{2}+O(x^{6}) \\
 \\
\lim_{ x \to 0 } \dfrac{x(3x+O(x^{3}))}{x^{2}+O(x^{6})}=\lim_{ x \to 0 } \dfrac{3x^{2}+O(x^{4})}{x^{2}+O(x^{6})}=\lim_{ x \to 0 } \dfrac{x^{2}(3+O(x^{2}))}{x^{2}(1+O(x^{4}))}=\ `` \dfrac{3+0}{1+0} "\ =3
\end{align}
$$