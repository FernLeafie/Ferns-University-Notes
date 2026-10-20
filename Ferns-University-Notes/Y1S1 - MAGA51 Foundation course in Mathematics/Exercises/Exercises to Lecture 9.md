## Examples
#### 1.
$$
\begin{align}
\lim_{ x \to \infty } \dfrac{x^{3}-1}{x-1}=\lim_{ x \to \infty } \dfrac{(x-1)(x^{2}+x+1)}{(x-1)}=\lim_{ x \to \infty } (x^{2}+x+1)=\infty \\
\lim_{ x \to 1 } \dfrac{x^{3}-1}{x-1}=\lim_{ x \to 1 } (x^{2}+x+1)=3
\end{align}
$$
#### 2.
$$
\begin{align}
f(x)=\left\{ \begin{array}{lll}
a+\dfrac{x^{3}-1}{|x|-1},&x<1 \\
ax-b, &x=1 \\
\dfrac{2\tan(x-1)}{x^{2}-1}, &x>1
\end{array} \right.  \\
\lim_{ x \to 1- } a+\dfrac{x^{3}-1}{|x|-1}=a-b =\lim_{ x \to 1+ } \dfrac{2\tan(x-1)}{x^{2}-1} \\
\lim_{ x \to 1- } a+\dfrac{x^{3}-1}{|x|-1}=a-b\iff 3=-b \\
\lim_{ x \to 1+ } \dfrac{2\tan(x-1)}{x^{2}-1}=\lim_{ x \to 1+ } 2\dfrac{\sin(x-1)}{\cos(x-1)(x-1)(x+1)}=\lim_{ x \to 1+ }2 \dfrac{1}{\cos(x-1)(x+1)}\dfrac{\sin(x-1)}{x-1}=2*\dfrac{1}{2}*1=1 \\
a-b=1\iff a+3=1\iff a=-2
\end{align}
$$
#### 3.
$$
\begin{align}
f(x)=\dfrac{\sqrt{ x^{2}-4 }}{|x|-4} \\
D_{f}:|x|-4\neq0,x^{2}-4\geq0=(x-2)(x+2) \iff D_{f}=(-\infty,-2]\cup[2,\infty)\setminus \{ -4,4 \} \\
\lim_{ x \to -\infty } \dfrac{\sqrt{ x^{2}-4 }}{|x|-4} =\lim_{ x \to -\infty }\dfrac{\dfrac{\sqrt{ x^{2}-4 }}{x}}{\dfrac{|x|-4}{x}} =\lim_{ x \to -\infty }\dfrac{\sqrt{\dfrac{ x^{2}-4 }{x^{2}}}}{\dfrac{|x|-4}{x}} =\lim_{ x \to -\infty }\dfrac{\sqrt{\dfrac{ x^{2}}{x^{2}}-\dfrac{4}{x^{2}}}}{\dfrac{|x|}{x}-\dfrac{4}{x}} =`` \dfrac{\sqrt{ 1-0 }}{1-0}"=`` \dfrac{\sqrt{ 1 }}{1}"=1
\end{align}
$$
Derived from [[Lectures]]