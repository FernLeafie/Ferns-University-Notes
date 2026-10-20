L'Hôpital's rule says that if a limit evaluates to $\dfrac{0}{0}$ or $\dfrac{\infty}{\infty}$, the $\lim_{ x \to a } \dfrac{f(x)}{g(x)}=\lim_{ x \to a } \dfrac{f'(x)}{g'(x)}=k$
$L'H \iff \ {}$only applies if the question is using limits

Couple speeds
When multiple quantities change over time, and there's an equation to connect them, then there can be derived an equation that couples the speed changes
### Random volume tangent
Volume
#### Straight volumes
Blocks, cylinders, prisms
${}V=h*A_{\text{base}}{}$
${}A_{\text{mantle}}=h*O_{\text{base}}{}$
${}A=2A_{\text{base}}+A_{\text{mantle}}{}$
#### Pointy volumes
Cones, pyramids, and whatnot
${}V=\dfrac{h*A_{\text{base}}}{3}{}$
## Examples
### 1
Decide a relation between the constants $a$ and $b$ so that the function $f: \mathbb{R} \to \mathbb{R}$,
$$
\begin{align}
f(x)=\left\{ \begin{array}{lll}
\dfrac{e^{ 2a(x-1) }-1}{x^{3}-1}, &x<1 \\
\dfrac{b\ln x^{2}}{\arctan(x^{2}-1)}, &x>1
\end{array} \right. 
\end{align}
$$
$\exists \lim_{ x \to a }f(a)\iff l_{l}=l_{r}$

$$
\begin{align}
l_{l}=\lim_{ x \to 1^{-} } \dfrac{e^{ 2a(x-1) }-1}{x^{3}-1}=`` \dfrac{0}{0} "=\lim_{ x \to 1^{-} } \dfrac{e^{ 2a(x-1) }-1}{2a(x-1)} \dfrac{2a(x-1)}{x^{3}-1}=1\lim_{ x \to 1^{-} } \dfrac{2a(x-1)}{(x-1)(x^{2}+x+1)}=`` \dfrac{2a}{3} " \\
l_{l}=\lim_{ x \to 1^{-} } \dfrac{e^{ 2a(x-1) }-1}{x^{3}-1} \overset{\text{L'H}}{\iff} \lim_{ x \to 1^{-} }\dfrac{e^{ 2a(x+1) }2a}{3x^{2}} =`` \dfrac{1*2a}{3}"=\dfrac{2a}{3}  \\
 \\
l_{h}=\lim_{ x \to 1^{+} } \dfrac{b\ln x^{2}}{\arctan(x^{2}-1)}=\lim_{ x \to 1^{+} } \dfrac{2b\ln x}{\arctan(x^{2}-1)}= \\
\end{align}
$$
### 2
The radius of a cylinder is increasing with the constant speed ${}10\pu{ cm/s }{}$. The cylinders height is increasing with the constant speed ${}5\pu{ cm/s }{}$. How fast is the cylinders volume and the total area when the radius is ${}5\pu{ cm }{}$ and the height is ${}10\pu{ cm }{}$.

$$
\begin{align} \\
R=\text{radius} \\
h=\text{height} \\
V=\text{volume} \\
A=\text{total area} \\
 \text{Given }  \\
R'(t)=5 \pu{ cm/s } \\
h'(t)=10 \pu{ cm/s } \\
t_{o}: R=5\text{cm},h=10\pu{ cm } \\
\text{Wanted} \\
V'(t_{0})=?, A'(t_{0})=?  \\
V=\pi R^{2}h \\
A=2\pi Rh+2\pi R^{2}
\end{align}
$$

$$
\begin{align}
V(t)=\pi R^{2}(t)*h(t) | \dfrac{d}{dt} \\
V'(t)=\pi(2R(t)*R'(t)h(t)+R^{2}(t)*h'(t)) |t=t_{0} \\
V'(t)=\pi(2\underbrace{ R(t_{0}) }_{ 5 }*\underbrace{ R'(t_{0}) }_{ 10 }\underbrace{ h(t_{0}) }_{ 10 }+\underbrace{ R^{2}(t_{0}) }_{ 25 }*\underbrace{ h'(t_{0}) }_{ 5 }) \\
V'(t_{0})=\pi(\underbrace{ 2*5*10*10 }_{ 1000 }+\underbrace{ 25*5 }_{ 125 })=\pi 1125
\end{align}
$$

$$
\begin{align}
A(t)=2\pi R(t)h(t)+2\pi R(t)^{2} | \dfrac{d}{dt} \\
A'(t)=2\pi(R'(t)h(t)+R(t)h'(t))+4\pi R(t)*R'(t) | t=t_{0} \\
A'(t_{0})=2\pi(R'(t_{0})h(t_{0})+R(t_{0})h'(t_{0}))+4\pi R(t_{0})*R'(t_{0}) \\
A'(t_{0})=2\pi(\underbrace{ 10*10 }_{ 100 }+\underbrace{ 5*5 }_{ 25 })+\underbrace{ 4\pi*5*10 }_{ 200\pi } \\
A'(t_{0})=\pi 250+200\pi=450\pi \pu{ cm^{2}/s }
\end{align}
$$
### 3
#### a
A cop stands at a straight stretch of highway to measure speeds with a radar gun. He aims the gun towards a car that just passed his position, and when the pistol is aimed in ${}45\degree{}$ towards the highway, he notes the distance between the car and the gun increases with a speed of ${}\pu{100 km/h}{}$. How fast is the car driving?

$$
\begin{align}
d = \text{distance between car and cop} \\
s = \text{distance car has travelled} \\
b = \text{the roads width} \\
\theta = \text{angle between cop and car} \\
s^{2}(t)+b^{2}(t)=d^{2}(t) \\
s'(t)=? \\
\theta(t_{0})=45\degree \\
d'(t_{0})=\pu{ 100 km/h }
\end{align}
$$

$$
\begin{align}
s^{2}(t)+b^{2}=d^{2}(t) | \dfrac{d}{dt} \\
2s(t)s'(t)+0=2d(t)d'(t) \\
s'(t)=\dfrac{d(t)*d('t)}{s(t)}=\dfrac{d'(t)}{\cos(\theta(t))} | t=t_{0} \\
s'(t_{0})=\dfrac{d'(t_{0})}{\cos(\theta(t_{0}))}= \dfrac{100}{\dfrac{1}{\sqrt{ 2 }}}=\pu{ 100\sqrt{2} km/h }
\end{align}
$$
#### b)
If the radar system in a) is aimed towards a car travelling in ${}\pu{ 90km/h}{}$, how fast is the distance between the car and the radar changing when it's aimed towards the car in ${}30\degree{}$
### 6
The radius of a conical tank is ${}\pu{ 4m}{}$ and the tanks height is ${}\pu{ 9m }{}$. Water is streaming into the tank of a constant speed of ${}\pu{ 25m^{3}/min }{}$, At that moment the water depth is ${}\pu{ 3m }{}$ answer the following:
#### a)
With what speed is the water depth changing?

$$
\begin{align}
R=\text{radius} \\
H=\text{the cones height} \\
h=\text{the waters depth} \\
V=\text{Volume of the water} \\
V'(t)=\pu{ 25m^{3}/min } \\
r=\text{Water surface area} \\
\text{Given }  \\
R=\pu{ 4m } \\
H=\pu{ 9m } \\
t_{0}:h=3m, V'(t) \\
\text{Sought} \\
a) \ h'(t_{0})=? \\
b) \ r'(t_{0}) \\
V(t)=\dfrac{\pi r^{2}(t)*h(t)}{3}
\end{align}
$$

$$
\begin{align}
V(t)=\dfrac{\pi r^{2}(t)*h(t)}{3} | \dfrac{d}{dt} \\
V'(t)=\dfrac{\pi}{3}(2r(t)r'(t)h(t)+r^{2}(t)*h'(t)) \\
\text{I think she just mixed up the direction of the cone}  \\
\text{Just use the formula for a triangle inscribed in another one} 
\end{align}
$$
It's the next day and she figured out the direction of the cone

$$
\begin{align}
\dfrac{h}{H}=\dfrac{r}{R} | t_{0} \\
\dfrac{3}{9}=\dfrac{r(t_{0})}{4} \\
r(t_{0})=\dfrac{4}{3} \\
\dfrac{h(t)}{H}=\dfrac{r(t)}{R}\iff \dfrac{h(t)}{9}=\dfrac{r(t)}{4} | \dfrac{d}{dt}\\
h'(t)=\dfrac{9}{4}r'(t)
\end{align}
$$

$$
\begin{align}
V'(t)=\dfrac{\pi}{3}(2r(t)r'(t)h(t)+r^{2}(t)*h'(t)) | t=t_{0} \\
25=\dfrac{\pi}{3}(8r'(t_{0})+4r'(t_{0}))
\end{align}
$$
#### b)
With what speed does the water surfaces radius change
### Surprise exercises
$$
\begin{align}
\lim_{ x \to -\infty } \dfrac{\sqrt{ x^{2}-1 }}{x}=`` \dfrac{\infty}{-\infty} "\overset{\text{L'H}}{=}\lim_{ x \to -\infty } \dfrac{\dfrac{1}{\cancel{ 2 }\sqrt{ x^{2}-1 }}\cancel{ 2 }x}{1}= \dfrac{x}{\sqrt{ x^{2}-1 }}=`` \dfrac{-\infty}{\infty} " \\
\text{Woops cyclical} \\
\lim_{ x \to -\infty } \dfrac{\cancelto{-1}{ |x| }\sqrt{ 1-\dfrac{1}{x^{2}} }}{\cancel{ x }}=`` -\dfrac{1*\sqrt{ 1-0 }}{1} "=-1
\end{align}
$$

$$
\begin{align}
\lim_{ x \to \infty } \dfrac{x+\sin x}{x}=`` \dfrac{\infty}{\infty} "\overset{\text{L'H}}{=}\lim_{ x \to \infty } 1+\cos x \\
\text{oh gods, what is } \cos \infty  \\
\text{however this just means the L'H derivation doesnt exist} \\
\text{the original limit can still exist} \\
\lim_{ x \to \infty } \left( 1+\dfrac{\sin x}{x} \right)=1+\overbrace{ \lim_{ x \to \infty } \dfrac{\sin x}{x} }^{ =0 }=1 \\
-1\leq \sin x\leq1 \\
\dfrac{-1}{x} \leq \dfrac{\sin x}{x} \leq \dfrac{1}{x} \\
0\leq \dfrac{\sin x}{x}\leq0
\end{align}
$$
$$
\begin{align}
\lim_{ x \to \infty } \dfrac{e^{ x }-e^{ -x }}{e^{ x }+e^{ -x }} =`` \dfrac{\infty-0}{\infty+0} "=`` \dfrac{\infty}{\infty} " \overset{\text{L'H}}{=} \lim_{ x \to \infty } \dfrac{e^{ x }-e^{ -x }(-1)}{e^{ x }+e^{ -x }(-1)}=\lim_{ x \to \infty } \dfrac{e^{ x }+e^{ -x }}{e^{ x }-e^{ -x }} \\
\text{womp womp cyclical }  \\
\lim_{ x \to \infty } \dfrac{\cancel{ e^{ x } }(1+e^{ -2x })}{\cancel{ e^{ x } }(1-e^{ 2-x })}=`` \dfrac{1}{1} "=1
\end{align}
$$
