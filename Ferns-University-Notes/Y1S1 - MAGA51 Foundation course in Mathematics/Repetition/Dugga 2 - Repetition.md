### 1
#### a)
Decreasing
#### b)
Increasing
#### c)
Increasing
### 2
a) or b)
### 3
Decide the functions so the constants ${}a{}$ and ${}b{}$ is continuous for ${}f:\mathbb{R}\to \mathbb{R}{}$ in ${}x=-4{}$

$$
\begin{align}
f(x)=\left\{ \begin{array}{ll}
a+\dfrac{x^{3}+64}{4(|x|-4)}, & x<-4 \\
-\dfrac{ax}{4}-b, & x=-4 \\
\dfrac{8\arctan(x+4)}{\sin(16-x^{2})}, & x>-4
\end{array} \right. 
\end{align}
$$

$$
\begin{align}
l_{l}=l_{h}=f(-4) \\
l_{l}=\lim_{ x \to -4^{-} } a+\dfrac{x^{3}+64}{4(|x|-4)}=a+\lim_{ x \to -4^{-} } \dfrac{x^{3}+64}{4(-x-4)} =a+\ `` \dfrac{0}{0} " \\
\overset{\text{L'H}}{=}a+\lim_{ x \to -4^{-} } \dfrac{3x^{2}}{4(-1)} =a-12 \\
l_{r}=\lim_{ x \to -4^{+} } \dfrac{8\arctan(x+4)}{\sin(16-x^{2})}=\ `` \dfrac{0}{0} "\overset{\text{L'H}}{=}\dfrac{8 \dfrac{1}{1+(x+4)^{2}}1}{\cos(16-x^{2})(-2x)}=\ `` \dfrac{8 \dfrac{1}{1+0}1}{ \underbrace{ \cos 0 }_{ 1 }(-2)(-4)} "=\dfrac{8}{8}=1 \\
a=13
\end{align}
$$
### 4
Decide ${}f'\left( \dfrac{\pi}{4} \right){}$ for ${}f(x)=(\cos x)^{\tan x}{}$

$$
\begin{align}
f(x)=(\cos x)^{\tan x} \\
\lg f(x)=\tan x \lg \cos x \\
(\lg f(x))'= (\tan x \lg \cos x)' \\
\dfrac{1}{f(x)}f'(x)=(\tan x)'(\lg \cos x)+(\tan x)(\lg \cos x)' \\
f'(x)=f(x)\left( \dfrac{1}{\cos ^{2}x}\ln \cos x +\tan x \dfrac{1}{\cos x} (-\sin x) \right) \\
f'\left( \dfrac{\pi}{4} \right)=\left( \underbrace{ \cos \dfrac{\pi}{4} }_{ \frac{1}{\sqrt{ 2 }} } \right)^{\underbrace{ \tan \pi/4 }_{ 1 }}\left( \dfrac{1}{\underbrace{ \cos ^{2}\left( \dfrac{\pi}{4} \right) }_{ \frac{1}{2} }} \lg \underbrace{ \cos\left( \dfrac{\pi}{4} \right) }_{ \frac{1}{\sqrt{ 2 }} }+\underbrace{ \tan\left( \dfrac{\pi}{4} \right) }_{ 1 } \underbrace{ \dfrac{1}{\underbrace{ \cos\left( \dfrac{\pi}{4} \right) }_{ \frac{1}{\sqrt{ 2 }} }} }_{ \frac{\sqrt{ 2 }}{1} }\left( \underbrace{ -\sin\left( \dfrac{\pi}{4} \right) }_{ -\frac{1}{\sqrt{ 2 }} } \right) \right) \\
f'\left( \dfrac{\pi}{4} \right)=\dfrac{1}{\sqrt{ 2 }}\left( \cancelto{ 2 }{ \dfrac{1}{\frac{1}{2}} } \ln \dfrac{1}{\sqrt{ 2 }} -1\right) \\
f'\left( \dfrac{\pi}{4} \right)=\dfrac{1}{\sqrt{ 2 }}(2(-\ln \sqrt{ 2 })-1) \\
f'\left( \dfrac{\pi}{4} \right) =\dfrac{1}{\sqrt{ 2 }}(-\ln 2-1)
\end{align}
$$
### 5
Calculate ${}\lim_{ x \to 2^{+} }\arctan\left( \dfrac{2x-1}{4-x^{2}} \right){}$

$$
\begin{align}
\lim_{ x \to 2^{+} }\arctan\left( \dfrac{2x-1}{4-x^{2}} \right)=\ `` \arctan\left( \dfrac{2x-1}{4-4} \right) "=\ `` \arctan \left( \dfrac{3}{-0} \right) "=\ `` \arctan(-\infty) "=-\dfrac{\pi}{2}
\end{align}
$$
### 6
#### a)
For an inversible function ${}g{}$ , ${}g(-2)=3{}$ and ${}g'(-2)=-1{}$ are given, find ${}(g^{-1})'(3){}$
${}(f^{-1})'(x)=\dfrac{1}{f'(f^{-1}(x)}{}$

$$
\begin{align}
g(-2)=3\iff g^{-1}(3)=-2 \\
(g^{-1})'(3)=\dfrac{1}{g'(g^{-1}(3))}=\dfrac{1}{g'(-2)}=\dfrac{1}{-1}=-1
\end{align}
$$
#### b)
Decide ${}(f^{-1})'(1){}$ when ${}f(x)=x^{3}+x-9{}$

$$
\begin{align}
(f^{-1})'(1)=\dfrac{1}{f'(f^{-1}(1))} \\
f^{-1}(1)=x_{0}\iff f(x_{0})=1 \\
f(x)=1\iff x^{3}+x-9=1\iff x^{3}+x-10=0 \\
x=2 \text{ is a root} \\
\dfrac{x^{3}+x-10}{x-2}=x^{2}+2x+5 \\
(\underbrace{ x-2 }_{ x=2 })(\underbrace{ x^{2}+2x+5 }_{ x \notin \mathbb{R} })=0 \\
f^{-1}(1)=2 \\
\dfrac{1}{f'(2)}
\end{align}
$$
### 7
Decide the tangent and the normal line to the curve

$$
\arcsin(xy^{2})-2x\sin(\pi y)+\ln(x^{2}-x^{2}y-xy)+2\sqrt{ \dfrac{x}{y} }=\dfrac{\pi}{6}
$$
in the point ${}\left( 2, \dfrac{1}{2} \right){}$

$$
\begin{align} \\
\arcsin(xy^{2})-2x\sin(\pi y)+\ln(x^{2}-x^{2}y-xy)+2\sqrt{ \dfrac{x}{y} }=\dfrac{\pi}{6} \\
\arcsin\left( \dfrac{2}{4} \right)-4\sin\left( \dfrac{\pi}{2} \right)+\ln\left( 4-\dfrac{4}{2}-\dfrac{2}{2} \right)+2\sqrt{ \dfrac{2}{\dfrac{1}{2}} }=\dfrac{\pi}{6} \\
\arcsin\left( \dfrac{1}{2} \right)-4+\ln\left( 4-2-1 \right)+2\sqrt{ 4 }=\dfrac{\pi}{6} \\
\dfrac{\pi}{6}-4+0+4=\dfrac{\pi}{6} \\
\left( 2, \dfrac{1}{2} \right) \in G_{y} \\
\underbrace{ \arcsin(xy^{2}) }_{ T_{1} }-2\underbrace{ x\sin(\pi y) }_{ T_{2} }+\underbrace{ \ln(x^{2}-x^{2}y-xy) }_{ T_{3} }+2\underbrace{ \sqrt{ \dfrac{x}{y} } }_{ T_{4} }=\dfrac{\pi}{6}| \dfrac{d}{dx} \\
T'_{1}(x)=(\arcsin xy^{2})'=\dfrac{1}{\sqrt{ 1-x^{2}y^{4} }}(xy^{2})'=\dfrac{1}{\sqrt{ 1-x^{2}y^{4} }}(1y^{2}+x2yy')' \\
T'_{2}(x)=(x\sin(\pi y))'=1\sin(\pi y)+x\cos(\pi y)\pi y' \\
T'_{3}(x)=(\ln (x^{2}-x^{2}y-xy))'=\dfrac{1}{x^{2}-x^{2}y-xy}(x^{2}-x^{2}y-xy)'= \\
=\dfrac{1}{x^{2}-x^{2}y-xy}(2x-(2xy+x^{2}y')-(1y+xy')) \\
T_{4}'(x)=\left( \sqrt{ \dfrac{x}{y} } \right)'=\left( \left( \dfrac{x}{y} \right)^{1/2} \right)'=\dfrac{1}{2}\left( \dfrac{x}{y} \right)^{1/2-1}\times \left( \dfrac{x}{y} \right)'= \\
=\dfrac{1}{2}\left( \dfrac{x}{y} \right)^{-1/2}\dfrac{1y-xy'}{y^{2}} \\
 \\
\dfrac{1}{\sqrt{ 1-x^{2}y^{4} }}(y^{2}+2xyy')-2(\sin (\pi y)+x\cos(\pi y)\pi y')+ \\
\dfrac{1}{x^{2}-x^{2}y-xy}(2x-2xy-x^{2}y'-y-xy')+ \\
\cancel{ 2 }\dfrac{1}{\cancel{ 2 }}\left( \dfrac{x}{y} \right)^{-1/2}\dfrac{1y-xy'}{y^{2}}=0
\end{align}
$$

### 8