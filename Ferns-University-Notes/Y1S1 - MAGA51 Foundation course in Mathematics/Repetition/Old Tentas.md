# 2026-05-04
## 1
### a

$$
\begin{align}
2x^{2}-4x-3y^{2}-6y=7 \\
(2x^{2}-4x)-(3y^{2}+6y)=7 \\
\text{square completion of } x \\
2x^{2}-4x=2(x^{2}-2x)=2(x^{2}-2x+1-1)=2((x-1)^{2}-1)=2(x-1)^{2}-2 \\
\text{square completion of } y \\
3y^{2}+6y=3(y^{2}+2y)=3(y^{2}+2y+1-1)=3(y+1)^{2}-3 \\
 \\
2(x-1)^{2}-2-(3(y+1)^{2}-3)=7 \\
2(x-1)^{2}-2-3(y+1)^{2}+3=7 \\
2(x-1)^{2}-3(y+1)^{2}=6 \\
\dfrac{2(x-1)^{2}}{6}-\dfrac{3(y+1)^{2}}{6}=1 \\
\dfrac{(x-1)^{2}}{3}-\dfrac{(y+1)^{2}}{2}=1 \\
\dfrac{(x-1)^{2}}{\sqrt{ 3 }^{2}}-\dfrac{(y+1)^{2}}{\sqrt{ 2 }^{2}}=1 \\
\end{align}
$$
the hyperbola should therefore have the asymptotes
${}\dfrac{x-1}{\sqrt{ 3 }}-\dfrac{y+1}{\sqrt{ 2 }}=0{}$ and ${}\dfrac{x-1}{\sqrt{ 3 }}+\dfrac{y+1}{\sqrt{ 2 }}=0{}$
### b

$$
\begin{align}
M=\{ x \in [0,3\pi]|4\cos ^{2}x-4\sin x=5 \} \\
 \\
\cos ^{2}+\sin ^{2}=1\iff \cos ^{2}=1-\sin ^{2} \\
4\cos ^{2}x-4\sin x=5\iff 4(1-\sin ^{2}x)-4\sin x=5 \\
4-4\sin ^{2}x-4\sin x=5 | \sin x=t, t\in[-1,1] \\
4-4t^{2}-4t=5\iff -4t^{2}-4t-1=0 \\
t^{2}+t+\dfrac{1}{4}=0 \\
t_{1,2}=-\dfrac{1}{2}\pm \sqrt{ \left( \dfrac{1}{2} \right)^{2} -\dfrac{1}{4}}\iff t_{1,2}=-\dfrac{1}{2}\pm 0 \in[-1,1] \\
 \\
\sin x=-\dfrac{1}{2} \\ 
\text{case 1} \\
\sin x=\sin\left( \dfrac{\pi}{6}+2\pi n \right)  \\
x=\dfrac{\pi}{6}+2\pi n \\
\begin{array}{lll}
n=-1, & \dfrac{\pi}{6}-2\pi=-\dfrac{11\pi}{6} & \not\in[0,3\pi] \\
n=0, & \dfrac{\pi}{6} & \in[0,3\pi] \\
n=1, & \dfrac{\pi}{6}+2\pi=\dfrac{13\pi}{6} & \in[0,3\pi] \\
n=2, & \dfrac{\pi}{6}+4\pi=\dfrac{25\pi}{6} & \not\in[0,3\pi]
\end{array} \\
\text{case 2} \\
\sin x=\sin\left( \pi-\dfrac{\pi}{6}+2\pi n \right) \\ \\
x=\pi-\dfrac{\pi}{6}+2\pi n=\dfrac{5\pi}{6}+2\pi n \\
\begin{array}{lll}
n=-1, & \dfrac{5\pi}{6}-2\pi=-\dfrac{7\pi}{6} & \not\in[0,3\pi] \\
n=0, & \dfrac{5\pi}{6} & \in[0,3\pi] \\
n=1, & \dfrac{5\pi}{6}+2\pi=\dfrac{17\pi}{6} & \in[0,3\pi] \\
n=2, & \dfrac{5\pi}{6}+4\pi=\dfrac{29\pi}{6} & \not\in[0,3\pi]
\end{array} \\
M=\left\{  \dfrac{\pi}{6}, \dfrac{5\pi}{6}, \dfrac{13\pi}{6}, \dfrac{17\pi}{6}  \right\}
\end{align}
$$
### c

$$
\begin{align}
f(x)=\sin (3x)^{\ln(x^{2})} \\
\ln(f(x))=\ln(x^{2})\ln\sin(3x)| \dfrac{d}{dx} \\
\dfrac{1}{f(x)}f'(x)=(\ln(x^{2}))'(\ln \sin 3x)+\ln(x^{2})(\ln \sin 3x)' \\
f'(x)=\sin (3x)^{\ln(x^{2})}\left( \dfrac{2}{x}(\ln \sin 3x)+\ln(x^{2}) \dfrac{3\cos 3x}{\sin 3x} \right) \\
f'\left( \dfrac{\pi}{6} \right)=\underbrace{ \sin \left( \dfrac{\pi}{2} \right) }_{ 1 }{}^{\ln(\pi^{2}/36)}\left( \dfrac{12}{\pi}\left( \underbrace{ \ln \underbrace{ \sin \dfrac{\pi}{2} }_{ 1 } }_{ 0 } \right) +\ln\left( \dfrac{\pi^{2}}{36}\dfrac{3\overbrace{ \cos \dfrac{\pi}{2} }^{ 0 }}{\underbrace{ \sin \dfrac{\pi}{2} }_{ 1 }} \right) \right)=1(0+0)=0
\end{align}
$$
### d

$$
\begin{align}
(f^{-1})'(5)=\dfrac{1}{f'(f^{-1}5)} \\
f(x)=x^{3}-x^{2}-x-10 \\
f^{-1}(5)=x_{0}\iff f(x_{0})=5 \\
x^{3}-x^{2}-x-10=5\iff x^{3}-x^{2}-x-15=0 \\
(\underbrace{ x-3 }_{ x=3 })(\underbrace{ x^{2}+2x+4 }_{ \not\in \mathbb{R} })=0 \\
x_{0}=3 \\
f'(x)=3x^{2}-2x-1 \\
(f^{-1})'(5)=\dfrac{1}{f'(3)}=\dfrac{1}{3*3^{2}-2*3-1}=\dfrac{1}{27-6-1}=\dfrac{1}{20}
\end{align}
$$
## 2
### b

$$
\begin{align}
\arccos\left( \dfrac{1}{\sqrt{ 3 }}\sin\left( \arctan\left( \dfrac{1}{\sqrt{ x }} \right) \right) \right)=\dfrac{\pi}{3} \\
\dfrac{1}{\sqrt{ 3 }}\sin\left( \arctan\left( \dfrac{1}{\sqrt{ x }} \right) \right) =\dfrac{1}{2} \\
\sin\left( \arctan\left( \dfrac{1}{\sqrt{ x }} \right) \right) =\dfrac{\sqrt{ 3 }}{2} \\
\arctan\left( \dfrac{1}{\sqrt{ x }} \right)=\dfrac{\pi}{3} \\
\dfrac{1}{\sqrt{ x }}=\tan\left( \dfrac{\pi}{3} \right) \\
\dfrac{1}{\sqrt{ x }}=\dfrac{\sin\left( \dfrac{\pi}{3} \right)}{\cos\left( \dfrac{\pi}{3} \right)} \\
\dfrac{1}{\sqrt{ x }}=\dfrac{\dfrac{\sqrt{ 3 }}{2}}{\dfrac{1}{2}} \\
\dfrac{1}{\sqrt{ x }}=\sqrt{ 3 } \\
\dfrac{1}{\sqrt{ 3 }}=\sqrt{ x } \\
\sqrt{ \dfrac{1}{3} }=\sqrt{ x } \\
x=\dfrac{1}{3}
\end{align}
$$
## 5

$$
\begin{align}
f(x)=\left\{ \begin{array}{lll}
\dfrac{\arctan(x^{2}-9)}{27+x^{3}}, & x<-3 \\
ax+b,  & x=-3 \\
\dfrac{e^{ 3a(x+3) }-1}{\ln(|x+2|)}, & x>-3
\end{array} \right. 
\end{align}
$$
${}l_{l}=l_{r}=f(-3){}$

$$
\begin{align}
l_{l}=\lim_{ x \to -3^{-} } \dfrac{\arctan(x^{2}-9)}{27+x^{3}}=\lim_{ x \to -3^{-} } \dfrac{\arctan(x^{2}-9)}{x^{2}-9} \dfrac{x^{2}-9}{27+x^{3}} \\
\lim_{ x \to -3^{-} } \dfrac{1(x^{2}-9)}{27+x^{3}}=\ `` \dfrac{0}{0} "\ =\lim_{ x \to -3^{-} } \dfrac{(x-3)(x+3)}{(x+3)(x^{2}-3x+9)}=\ `` \dfrac{-6}{9+9+9} "\ =-\dfrac{2}{9}
\end{align}
$$

$$
\begin{align}
l_{r}=\lim_{ x \to -3^{+} } \dfrac{e^{ 3a(x+3) }-1}{\ln(|x+2|)}=\lim_{ x \to -3^{+} } \dfrac{e^{ 3a(x+3) }-1}{3a(x+3)} \dfrac{3a(x+3)}{\ln(|x+2|)} \\
1a\lim_{ x \to -3^{+} } \dfrac{3x+9}{\ln(|x+2|)}=\ `` \dfrac{0}{0} "\ \overset{\text{L'H}}{=}a \lim_{ x \to -3^{+} } \dfrac{3}{\dfrac{1}{|x+2|}}=a\lim_{ x \to -3^{+} } 3|x+2|=a\ `` 3*1 "\ =3a
\end{align}
$$

$$
\begin{align}
3a=-\dfrac{2}{9}\iff a=-\dfrac{2}{27} \\
-\dfrac{2}{9}=f(-3)\iff-\dfrac{2}{9}=\left( -\dfrac{2}{27} \right)\times(-3)+b \\
\dfrac{2\times 3}{27}+b=-\dfrac{2}{9}\iff \dfrac{2}{9}+b=-\dfrac{2}{9}\iff b=-\dfrac{4}{9}
\end{align}
$$
Answer: ${}a=-\dfrac{2}{27}{}$ and ${}b=-\dfrac{4}{9}{}$
# 2025-12-18
## 2
### b

$$
\begin{align}
\arctan\left( 2\sin\left( \arctan \dfrac{1}{x} \right) \right)=\dfrac{\pi}{3} \\
\tan\left( \arctan\left( 2\sin\left( \arctan \dfrac{1}{x} \right) \right) \right)= \dfrac{\sin\left( \dfrac{\pi}{3} \right)}{\cos\left( \dfrac{\pi}{3} \right)} \\
2\sin\left( \arctan \dfrac{1}{x} \right) =\dfrac{\dfrac{\sqrt{ 3 }}{2}}{\dfrac{1}{2}} \\
\sin\left( \arctan\left( \dfrac{1}{x} \right) \right)=\dfrac{\sqrt{ 3 }}{2} \\
\arctan\left( \dfrac{1}{x} \right)=\dfrac{\pi}{3} \\
\dfrac{1}{x}=\dfrac{\dfrac{\sqrt{ 3 }}{2}}{\dfrac{1}{2}}=\sqrt{ 3 } \\
\dfrac{1}{x}=\sqrt{ 3 }\iff \dfrac{1}{\sqrt{ 3 }}=x
\end{align}
$$