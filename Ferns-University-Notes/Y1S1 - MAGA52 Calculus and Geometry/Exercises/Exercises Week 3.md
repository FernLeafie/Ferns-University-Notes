### Generalised Integrals
#### 1
$$
\begin{align}
\int_{2}^{\infty} \dfrac{1}{x^{3}} \, dx = \lim_{ R \to \infty } \int_{2}^{R} \dfrac{1}{x^{3}} \, dx =\lim_{ R \to \infty } \int_{2}^{R} x^{-3} \, dx = \lim_{ R \to \infty } \left[ \dfrac{x^{-2}}{-2} \right]_{2}^{R} \\
=\lim_{ R \to \infty } \left[ -\dfrac{1}{2x^{2}} \right]_{2}^{R}=\lim_{ R \to \infty } -\dfrac{1}{2R^{2}}+\dfrac{1}{2\times 2^{2}}=\ `` 0+\dfrac{1}{8} "\ =\dfrac{1}{8}
\end{align}
$$
#### 2
$$
\begin{align}
\int_{1}^{\infty} \dfrac{1}{3+x^{2}} \, dx =\int_{1}^{\infty} \dfrac{1}{3\left( \dfrac{x^{2}}{3}+1 \right)} \, dx =\int_{1}^{\infty} \dfrac{1}{3}\times \dfrac{1}{\dfrac{x^{2}}{3}+1} \, dx =\dfrac{1}{3}\int_{1}^{\infty} \dfrac{1}{\left( \dfrac{x}{\sqrt{ 3 }} \right)^{2}+1} \, dx  \\
=\left[ \begin{array}{ccc}
t=\dfrac{x}{\sqrt{ 3 }} \\
\left( \dfrac{x}{\sqrt{ 3 }} \right)^{2}=t^{2} \\
\dfrac{dt}{dx}=\dfrac{1}{\sqrt{ 3 }}\iff dt=\dfrac{dx}{\sqrt{ 3 }} \\
x=1\implies \dfrac{1}{\sqrt{ 3 }}
\end{array} \right]  =\dfrac{1}{3}\int_{1/\sqrt{ 3 }}^{\infty} \sqrt{ 3 }\dfrac{1}{t^{2}+1} \, dt =\dfrac{\sqrt{ 3 }}{3}\int_{1/\sqrt{ 3 }}^{\infty} \dfrac{1}{t^{2}+1} \, dt =\dfrac{\sqrt{ 3 }}{3}[\arctan(t)]_{1/\sqrt{ 3 }}^{\infty} \\
= \dfrac{\sqrt{ 3 }}{3}\left( (\lim_{ R \to \infty } \arctan(R))-\arctan\left( \dfrac{1}{\sqrt{ 3 }} \right) \right)=\dfrac{\sqrt{ 3 }}{3}\left( \dfrac{\pi}{2}-\dfrac{\pi}{6} \right)=\dfrac{\sqrt{ 3 }}{3}\left( \dfrac{3\pi}{6}-\dfrac{\pi}{6} \right)=\dfrac{\sqrt{ 3 }}{3} \dfrac{2\pi}{6}=\dfrac{1}{\sqrt{ 3 }} \dfrac{\pi}{3}=\dfrac{\pi}{3\sqrt{ 3 }}
\end{align}
$$
#### 3
$$
\begin{align}
\int_{e}^{\infty} \dfrac{1}{x(\ln(x))^{2}} \, dx =\int_{e}^{\infty} (x(\ln(x))^{2})^{-1} \, dx =\int_{e}^{\infty} x ^{-1}(\ln(x))^{-2} \, dx \\
\int \overset{\uparrow}{x^{-1}}\overset{\downarrow}{(\ln(x))^{-2}} \, dx =\ln|x|(\ln(x))^{-2}+2\int \dfrac{\ln|x|}{\ln(x)^{3}x}
\end{align}
$$
### ODE
#### 1
$$
\begin{align}
\dfrac{dy}{dx}=xy \iff dy=xydx \iff \dfrac{1}{y}dy=xdx \\
\int \dfrac{1}{y} \, dy = \int x \, dx \iff \ln|y|=\dfrac{x^{2}}{2}+C \\
e^{\ln|y|} =e^{x^{2}/2+C} \iff |y|=e^{ x^{2}/2 }e^{ C }\iff|y|=C e^{ x^{2}/2 } \iff y=Ce^{ x^{2}/2 }
\end{align}
$$
#### 2
$$
\begin{align}
\dfrac{dy}{dx}=x^{2}y^{2} \iff \dfrac{1}{y^{2}}dy=x^{2}dx \\
\int \dfrac{1}{y^{2}} \, dy =\int x^{2} \, dx \iff \int y^{-2} \, dy = \int x^{2} \, dx  \\
\dfrac{y^{-1}}{-1}=\dfrac{x^{3}}{3} +C\iff -\dfrac{1}{y}=\dfrac{x^{3}}{3}+C \\
-1=\dfrac{x^{3}+C}{3}y \iff-\dfrac{3}{x^{3}+C}=y
\end{align}
$$
#### 3
$$
\begin{align}
\dfrac{dy}{dx}=x+xy^{2}\iff dy=x(1+y^{2})dx \\
\dfrac{1}{1+y^{2}}dy=xdx \iff \int \dfrac{1}{1+y^{2}} \, dy = \int x \, dx  \\
\arctan y=\dfrac{x^{2}}{2}+C \iff y=\tan\left( \dfrac{x^{2}}{2}+C \right)
\end{align}
$$
#### 4
$$
\begin{align}
\dfrac{dy}{dx}=x e^{ x-2y }\iff \dfrac{dy}{dx}=x e^{ x } \dfrac{1}{e^{ 2y }} \\
e^{ 2y }dy=x e^{ x }dx \iff \int e^{ 2y } \, dy =\int x e^{ x } \, dx  \\
\dfrac{1}{2}e^{ 2y }=\int \overset{\downarrow}{x} \overset{\uparrow}{e^{ x }} \, dx \iff \dfrac{1}{2} e^{ 2y }=x e^{ x }-\int e^{ x } \, dx  \\
\dfrac{1}{2}e^{ 2y }=x e^{ x }-e^{ x }+C\iff \dfrac{e^{ 2y }}{2}=e^{ x }(x-1)+C \\
\ln(e^{ 2y })-\ln(2)=\ln(e^{ x }(x-1)+C) \iff 2y=\ln(e^{ x }(x-1)+C)+\ln(2) \\
y=\dfrac{\ln(2e^{ x }(x-1)+C)}{2}
\end{align}
$$