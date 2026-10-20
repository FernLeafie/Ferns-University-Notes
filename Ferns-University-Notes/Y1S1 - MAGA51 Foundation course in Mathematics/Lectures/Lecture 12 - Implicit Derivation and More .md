$$
\begin{align}
(e^{ u })'=e^{ y }u'
\end{align}
$$
## Exercises
#### 1
Decide $f'(x)$ where $f(x)=\sin ^{2}\left( \dfrac{x+1}{x-1} \right)$ by using the chain rule
#### 2
Decide what intervals the function $f(x)=x-\cos 2x$ growing or shrinking
$$
\begin{align}
f(x)=x-\cos 2x \\
f'(x)=1+\sin(2x)2 \\
f'(x)=0 \iff \sin(2x)=-\dfrac{1}{2}\iff \sin(2x)=\sin\left( -\dfrac{\pi}{6} \right) \\
\left\{ \begin{array}{ll}
2x_{1}=-\dfrac{\pi}{6}+2n\pi \\
2x_{2}=\pi+\dfrac{\pi}{6}+2n\pi
\end{array} \right. \iff  \left\{ \begin{array}{ll}
x_{1}=-\dfrac{\pi}{12}+n\pi \\
x_{2}=\dfrac{7\pi}{12}+n\pi
\end{array} \right. 
\end{align}
$$
In the range $[-\pi,\pi]$ we have the solutions $-\dfrac{\pi}{12},\dfrac{11\pi}{12},-\dfrac{5\pi}{12},\dfrac{7\pi}{12}$

| $x$     | $-\pi$ |            | $-\dfrac{5\pi}{12}$ |            | $-\dfrac{\pi}{12}$ |            | $\dfrac{7\pi}{12}$ |            | $\dfrac{11\pi}{12}$ |            | $\pi$ |
| ------- | ------ | ---------- | ------------------- | ---------- | ------------------ | ---------- | ------------------ | ---------- | ------------------- | ---------- | ----- |
| $f'(x)$ |        | +          | $0$                 | $-$        | $0$                | +          | $0$                | $-$        | $0$                 | +          |       |
| $f(x)$  |        | $\nearrow$ |                     | $\searrow$ |                    | $\nearrow$ |                    | $\searrow$ |                     | $\nearrow$ |       |


#### 3
Decide $f'(x)$ where $f(x)=\sqrt{ 2x^{2}-x }$ by using the chain rule, check using the derivatives definition
$$
\begin{align}
f(x)=\sqrt{ 2x^{2}-x } \\
f'(x)=(\sqrt{ 2x^{2}-x })'=\dfrac{1}{2\sqrt{ 2x^{2}-x }}(2x^{2}-x)'=\dfrac{1}{2\sqrt{ 2x^{2}-x }}(4x-1) \\
 \\
f'(x)=\lim_{ h \to 0 } \dfrac{\sqrt{ 2(x+h)^{2}-(x+h) }-\sqrt{ 2x^{2}-x }}{h}=``\dfrac{0}{0}"= \\
\lim_{ h \to 0 }  \dfrac{\dfrac{2(x+h)^{2}-(x+h)-(2x^{2}-x)}{\sqrt{ 2(x+h)^{2}-(x+h) }+\sqrt{ 2x^{2}-x }}}{h} \\
\lim_{ h \to 0 }  \dfrac{{2x^{2}+4xh+2h^{2}-x-h-2x^{2}+x}}{h({\sqrt{ 2(x+h)^{2}-(x+h) }+\sqrt{ 2x^{2}-x }})} \\
\lim_{ h \to 0 }  \dfrac{{4xh+2h^{2}-h}}{h({\sqrt{ 2(x+h)^{2}-(x+h) }+\sqrt{ 2x^{2}-x }})} \\
\lim_{ h \to 0 }  \dfrac{{\cancel{ h }(4x+2h-1)}}{\cancel{ h }({\sqrt{ 2(x+h)^{2}-(x+h) }+\sqrt{ 2x^{2}-x }})}=`` \dfrac{4x-1}{2\sqrt{ 2x^{2}-x }}"
\end{align}
$$
#### 3
Decide the equation for the tangent and normal line in the point of the coordinate $\left( \dfrac{\pi}{4},1 \right)$ for the curve $y=y(x)$ given the implicit equation $2x+\sqrt{ y }-\sqrt{ 2 }\sin(xy)=\dfrac{\pi}{2}$.
Start by checking if $\left( \dfrac{\pi}{4},1 \right) \in Gy$
$$
\begin{align}
2 \dfrac{\pi}{4}+\sqrt{ 1 }-\sqrt{ 2 }\sin\left( \dfrac{\pi}{4}*1 \right)=\dfrac{\pi}{2} \\
\dfrac{\pi}{2}+1-\sqrt{ 2 } \dfrac{1}{\sqrt{ 2 }}=\dfrac{\pi}{2} \\
\dfrac{\pi}{2}+1-1=\dfrac{\pi}{2} \\
\dfrac{\pi}{2}=\dfrac{\pi}{2}
\end{align}
$$

$$
\begin{align}
\dfrac{d}{dx}2x+\sqrt{ y }-\sqrt{ 2 }\sin(xy)=\dfrac{\pi}{2} \\
2+\dfrac{1}{2\sqrt{ y }}y'-\sqrt{ 2 }\cos(xy) (xy)'_{x}=0 \\
2+\dfrac{1}{2\sqrt{ y }}y'-\sqrt{ 2 }\cos(xy) (1y + xy')=0 \\
 \\
x=\dfrac{\pi}{4},y=1,y'=k_{t} \\
2+\dfrac{1}{2\sqrt{ 1 }}k_{t}-\sqrt{2}\cos\left( \dfrac{\pi}{4}1 \right)\left( 1*1+\dfrac{\pi}{4}k_{t} \right)=0 \\
2+\dfrac{k_{t}}{2}-\cancel{ \sqrt{ 2 } } \dfrac{1}{\cancel{ \sqrt{ 2 } }}\left( 1+\dfrac{\pi}{4}k_{t} \right)=0 \\
k_{t}\left( \dfrac{1}{2}-\dfrac{\pi}{4} \right)=-2+1 \\
k_{t}=-\dfrac{1}{\dfrac{1}{2}-\dfrac{\pi}{4}} \\
 \\
t:y-1=\dfrac{-1}{\frac{1}{2}-\frac{\pi}{4}}\left( x-\dfrac{\pi}{4} \right) \\
n:y-1=\dfrac{\frac{1}{2}-\frac{\pi}{4}}{1}\left( x-\dfrac{\pi}{4} \right)
\end{align}
$$
#### 3
Decide the number of real solutions for the equation $x^{3}-15x+1=0$ in the range $[-4,4]$
Binary search and make a rate change table
#### 4
show that an odd function $f$ is right continuous in $x=0$ which means $f$ is continuous in $x=0$ and $f(0)=0$
$f$-odd $f(-x)=-f(x)$

$$
\begin{align}
l_{r}=\lim_{ x \to 0^{+} } f(x)=f(0) \\
l_{l}=\lim_{ x \to 0^{-} } f(x)=\left[ \begin{array}{lll}
t=-x \\
x=-t
\end{array} \right]  =\lim_{ t \to 0^{+} } f(-t)
=-\lim_{ t \to 0^{+} } f(t)=-f(0)=0 \\
l_{l}=l_{r}=f(0)=0
\end{align}
$$
#### 7
Can $f(x)=\tan x$ have any horizontal tangents, visualise graphically and motivate algebraically, do the same with $g(x)=4x+\sin ^{2}x$ 
$$
\begin{align}
(\tan x)'=\dfrac{1}{\cos ^{2}x}=1+\tan ^{2}(x) \\
\end{align}
$$
$\tan ^{2}(x)$ falls between $0$ and $\infty$, so the lowest value of tan must be $1$, and thus there are no horizontal tangents

$$
\begin{align}
(4x+\sin ^{2}x)'=4+\cos(x)\sin(x)+\sin(x)\cos(x)=2\cos(x)\sin(x)+4 \\
g'(x)\geq2
\end{align}
$$
#### 8
decide the tangent and normal line in the point $()$
#### 9
Decide the slope of the tangent line to the curve $y=y(x)$, where $\sqrt{ x }e^{ x^{2}y }=\sqrt{ x^{2}+y^{2} }$ in the point $(1,0)$.
$(1,0)\in Gy$
$$
\begin{align}
\sqrt{ 1 }e^{1^{2}\times0}=\sqrt{ 1^{2}+0^{2} } \\
1=1
\end{align}
$$
$y'(1)=k_{t}$
$$
\begin{align}
(\sqrt{ x }e^{ x^{2}y })'_{x}=(\sqrt{ x^{2}+y^{2} })'_{x} \\
\dfrac{1}{2\sqrt{ x }}e^{ x^{2}y }+\sqrt{ x }(\underbrace{ e^{ x^{2}y } }_{ D_{1} })'_{x}=(\underbrace{ \sqrt{ x^{2}+y^{2} } }_{ D_{2} })'_{x} \\
 \\
D_{1}=(e^{ x^{2}y })'_{x}=e^{ x^{2}y }\times(x^{2}y)'_{x}=e^{ x^{2}y }\times (2xy+x^{2}y') \\
D_{2}=(\sqrt{ x^{2}+y^{2} })'_{x}=\dfrac{1}{2\sqrt{ x^{2}+y^{2}}}\times(x^{2}+y^{2})'_{x}=\dfrac{1}{2\sqrt{ x^{2}+y^{2} }}\times(2x+2y\times y') \\
 \\
\dfrac{1}{2\sqrt{ x }}e^{ x^{2}y }+\sqrt{ x }(e^{ x^{2}y }\times (2xy+x^{2}y'))=\left(\dfrac{1}{2\sqrt{ x^{2}+y^{2} }}\times(2x+2y\times y')\right) \\
 \\
x=1,y(1)=0,y'(1)=k_{t} \\
\dfrac{1}{2\sqrt{ 1 }}e^{ 1^{2}\times 0 }+\sqrt{ 1 }(e^{ 1^{2}\times 0 }\times (2\times 1\times 0+1^{2}k_{t}))=\left(\dfrac{1}{2\sqrt{ 1^{2}+0^{2} }}\times(2\times1+2 \times0\times k_{t})\right) \\
\dfrac{1}{2}+k_{t}=\dfrac{1}{2}*2 \iff \dfrac{1}{2}+k_{t}=1\iff k_{t} =\dfrac{1}{2}
\end{align}
$$