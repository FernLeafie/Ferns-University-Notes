No need to remember most of trig, just draw up the unit circle

|        | $0\degree$ |       $30\degree$       |       $45\degree$       |       $60\degree$       |   $90\degree$    |
| :----: | :--------: | :---------------------: | :---------------------: | :---------------------: | :--------------: |
|        |    $0$     |    $\dfrac{\pi}{6}$     |    $\dfrac{\pi}{4}$     |    $\dfrac{\pi}{3}$     | $\dfrac{\pi}{2}$ |
| $\cos$ |    $1$     | $\dfrac{\sqrt{ 3 }}{2}$ | $\dfrac{\sqrt{ 2 }}{2}$ |     $\dfrac{1}{2}$      |       $0$        |
| $\sin$ |    $0$     |     $\dfrac{1}{2}$      | $\dfrac{\sqrt{ 2 }}{2}$ | $\dfrac{\sqrt{ 3 }}{2}$ |       $1$        |
| $\tan$ |    $0$     | $\dfrac{1}{\sqrt{ 3 }}$ |           $1$           |      $\sqrt{ 3 }$       |       N/A        |

$$
\begin{align}
\sin a=\cos\left( \dfrac{\pi}{2}-a \right) \\
\cos a=\sin\left( \dfrac{\pi}{2}-a \right)
\end{align}
$$


$$
\begin{align}
A\sin \omega x+B\cos \omega x = 
\end{align}
$$
## Discussion
#### 1
Define the amount $M=\{ x \in [0,2\pi]|\cos(2x-\pi)=\sin 2x \}$

$$
\begin{align}
\cos(2x-\pi)=\sin 2x \iff \sin\left(\dfrac{\pi}{2}-( 2x-\pi) \right)=\sin 2x \\
\sin\left( \dfrac{\pi}{2}-2x+\pi \right)=\sin 2x\iff \sin\left( \dfrac{3\pi}{2}-2x \right)=\sin2x \\
\text{Case 1} \\
\dfrac{3\pi}{2}-2x=2x+2n\pi \iff -4x=-\dfrac{3\pi}{2}+2n\pi \\
x=\dfrac{3\pi}{2}-\dfrac{n\pi}{2}, n \in \mathbb{Z} \\
\text{Case 2} \\
\dfrac{3\pi}{2}-2x=\pi-2x+2n\pi\iff \dfrac{3\pi}{2}=\pi-2\pi n \\
\text{No solutions}
\end{align}
$$

$$
\begin{align}
n = 0 & x=\dfrac{3\pi}{8} \text{ Ok}\\
n = -1 & x=\dfrac{3\pi}{8}+\dfrac{\pi}{2}=\dfrac{7\pi}{8} \text{ Ok}\\
n = -2 & x=\dfrac{3\pi}{8}+\dfrac{2\pi}{2}=\dfrac{11\pi}{8} \text{ Ok}\\
n = -3 & x=\dfrac{3\pi}{8}+\dfrac{3\pi}{2}=\dfrac{15\pi}{8} \text{ Ok}\\
n = -4 & x=\dfrac{3\pi}{8}+\dfrac{4\pi}{2}=\dfrac{19\pi}{8} \text{ Nope}
\end{align}
$$

$$
\begin{align}
M=\left\{ \dfrac{7\pi}{8},\dfrac{11\pi}{8},\dfrac{15\pi}{8},\dfrac{19\pi}{8} \right\} 
\end{align}
$$
#### 2
solve $4\cos ^{2}x-4\sin x=5$
$$
\begin{align}
\cos ^{2}x+\sin ^{2}x=1\iff \cos ^{2}x=1-\sin ^{2}x
\end{align}
$$
$$
\begin{align}
4\cos ^{2}x-4\sin x=5\iff 4(1-\sin ^{2}x)-4\sin x=5\iff 4-4\sin ^{2}x-4\sin x=5 \\
 \\
\sin x=t, t \in[-1,1] \\
4-4t^{2}-4t=5\iff 4t^{2}+4t+1=0 \\
(2t+1)^{2}=0 \\
t_{1,2}=-\dfrac{1}{2} \\
 \\
\sin x=-\dfrac{1}{2} \\
\text{Case 1} \\
\sin x = \sin \left( -\dfrac{\pi}{6} +2\pi n\right) \\
x_{1}=-\dfrac{\pi}{6} +2\pi n \\
\text{Case 2} \\
\sin x = \sin \left( \pi+\dfrac{\pi}{6} +2\pi n\right) \\
\sin x = \sin \left( \dfrac{7\pi}{6} +2\pi n\right) \\
x_{2}=\dfrac{7\pi}{6} +2\pi n
\end{align}
$$

$$
\begin{align}
\left\{ \begin{array}{lll}
x_{1}=-\dfrac{\pi}{6} +2\pi n \\
x_{2}=\dfrac{7\pi}{6} +2\pi n
\end{array} \right. 
\end{align}
$$
#### 3.
Decide $\tan\left( \dfrac{\pi}{8} \right)$


$$
\begin{align}
\tan\left( \dfrac{\pi}{8} \right)=\dfrac{\sin\left( \dfrac{\pi}{8} \right)}{\cos\left( \dfrac{\pi}{8} \right)} \\
 \\
\cos\left( 2\dfrac{\pi}{8} \right)=2\cos ^{2}\left( \dfrac{\pi}{8} \right)-1\iff \dfrac{\sqrt{ 2 }}{2}=2\cos ^{2}\left( \dfrac{\pi}{8} \right)-1 \\
\dfrac{\dfrac{\sqrt{ 2 }}{2}+1}{2}=\cos ^{2}\left( \dfrac{\pi}{8} \right)=\dfrac{2+\sqrt{ 2 }}{4}
\end{align}
$$

$$
\begin{align}
\dfrac{\sqrt{ 2-\sqrt{ 2 } }}{\sqrt{ 2+\sqrt{ 2 } }}=\sqrt{ \dfrac{2-\sqrt{ 2 }}{2+\sqrt{ 2 }} }=\sqrt{ \dfrac{(2-\sqrt{2 })(2-\sqrt{2 })}{(2+\sqrt{2 })(2-\sqrt{2 })} }=\sqrt{ \dfrac{(2-\sqrt{2 })^{2}}{4-2} }=\dfrac{2-\sqrt{ 2 }}{\sqrt{ 2 }}=\dfrac{2}{\sqrt{ 2 }}-\dfrac{\sqrt{ 2 }}{\sqrt{ 2 }}=\dfrac{2}{\sqrt{ 2 }}-1
\end{align}
$$
#### 4.
what is the domain of $f(x)=\tan(\sqrt{ x })$
$$
\begin{align}
f(x)=\tan(\sqrt{ x })
\end{align}
$$
due to $\sqrt{ x }$: $x\geq0$
due to $\tan$:  $\sqrt{ x } \neq \dfrac{\pi}{2}+n\pi\iff x \neq \left( \dfrac{\pi}{2}+n\pi \right)^{2}$
$$
\begin{align}
D_{f}=\left\{ \begin{array}{l}
x\neq\left( \dfrac{\pi}{2}+n\pi \right)^{2} \\
x\geq0
\end{array} \right.  \\
D_{f}=\left\{  x \in \mathbb{R}_{+},x\neq\left( \dfrac{\pi}{2}+n\pi \right)^{2},n \in \mathbb{Z}  \right\}
\end{align}
$$

Derived from [[Lectures]]