# Primitive Functions
The reverse problem of derivatives, given a derivative ${}f'(x){}$, find the original function ${}f(x){}$.

$$
\begin{align}
f'(x)=3x^{2} \\
f(x)=x^{3}
\end{align}
$$
however, as any constants could have been derived away when getting ${}f'(x){}$, ${}f(x){}$ could have any constant added to it
$$
\begin{align}
f'(x)=3x^{2} \\
f(x)=x^{3}+C
\end{align}
$$
where ${}C{}$ is any arbitrary constant.
This is also known as integration.
## Definition
Let ${}f(x){}$ be an arbitrary function.
The primitive function to ${}f(x){}$ is annotated ${}F(x){}$, and fulfils the requirement ${}F'(x)=f(x){}$.

Primitive in this regard doesn't mean simple, but just original, the original function causing another function by derivation.
It's also known as the anti derivative of ${}f(x){}$.

${}F(x){}$ can also be called an undefined integral of ${}f(x){}$
$$
\begin{align}
F(x)=\int f(x) \, dx
\end{align}
$$
The integration symbol ${}\int{}$ is a large ${}S{}$, which indicates how it has a relation to sum.
${}f(x){}$ is the function to be integrated. And ${}dx{}$ indicates the variable to be integrated over.

The process of defining ${}F(x){}$ is called integrating.

### Example
$$
\begin{align}
\int \cos(x) \, dx 
\end{align}
$$
#### Solution:
seeking a function called ${}F(x){}$ so that ${}F'(x)=\cos(x){}$
$$
\begin{align}
F(x)=\sin(x)+C
\end{align}
$$
## Properties

$$
\begin{align}
\int kf(x) \, dx =k\int f(x) \, dx \\
\int (f(x)\pm g(x)) \, dx =\int f(x) \, dx \pm \int g(x) \, dx  \\
\int f'(x) \, dx =f(x)+C
\end{align}
$$

$$
\int  \, dx =\int 1 \, dx =x+C
$$
this can be thought of as multiplication
### Example
Calculate ${}\int (2\cos(x)-3x) \, dx{}$
#### Solution:
$$
\begin{align}
\int (2\cos(x)-3x) \, dx \\
\int 2\cos(x) \, dx -\int 3x \, dx  \\
2\int \cos(x) \, dx -3\int x \, dx  \\
2(\sin x+C)-3 \left( \dfrac{x^{2}}{2} +C\right) \\
2\sin-\dfrac{3x^{2}}{2}+C
\end{align}
$$
As ${}C{}$ is an arbitrary constant, ${}C+C=C{}$, ${}C-C=C{}$,${}C*n=C{}$, and thus we only need to add it at the end. ${}C{}$ is immortal

How do we get ${}\int x \, dx=\dfrac{x^{2}}{2}+C{}$?
$$
(x^{2})'=2x\iff x=\left( \dfrac{x^{2}}{2} \right)
$$
As constants can be moved in and out of derivations, we've essentially manipulated the derivation as we see fit.
To make it extra obvious:
$$
\int x \, dx =\int \left( \dfrac{x^{2}}{2} \right)' \, dx =\dfrac{x^{2}}{2}+C
$$
## Integration of Elementary Functions
The basic mathematical functions essentially

|            ${}f(x){}$             | ${}F(x){}$                             |
| :-------------------------------: | :------------------------------------- |
|            ${}x^{r}{}$            | ${}\dfrac{x^{r+1}}{r+1}+C,(r\neq-1){}$ |
|    ${} x^{-1}=\dfrac{1}{x}{}$     | ${}\ln \lvert x \rvert+C {}$           |
|          ${}\cos (kx){}$          | ${}\dfrac{1}{k}\sin(kx)+C{}$           |
|          ${}\sin(kx){}$           | ${}-\dfrac{1}{k}\cos(kx)+C{}$          |
|          ${}e^{ kx }{}$           | ${}\dfrac{1}{k}e^{ kx }+C{}$           |
|     ${}\dfrac{1}{x^{2}+1}{}$      | ${}\arctan(x)+C{}$                     |
| ${}\dfrac{1}{\sqrt{ 1-x^{2} }}{}$ | ${}\arcsin(x)+C{}$                     |
|       ${}1+\tan ^{2}(x){}$        | ${}\tan(x)+C{}$                        |
|   ${}\dfrac{1}{\cos ^{2}(x)}{}$   | ${}\tan(x)+C{}$                        |
### Visualisation of Trigonometry
The integration and derivation of the basic trigonometric functions ${}\sin{}$and ${}\cos{}$ can be visually thought as:
![[1 - Primitive functions 2026-11-11 10.01.50.excalidraw]]
using the unit circle.
## Observation
If ${}\int f(x) \, dx=F(x)+C{}$
then:
$$
\begin{align}
\int f(ax+b) \, dx = \dfrac{F(ax+b)}{a}+C
\end{align}
$$
so if we integrate the function of a linear function, then we have to divide by the inner derivative.
To test if a primitive function is correct, we can always derive it and see if we get back the original function.
### Proof

$$
\begin{align}
\left( \dfrac{F(ax+b)}{a} \right)'= \left( \dfrac{F(ax+b)}{a} \right)'+C' \\
\left( \dfrac{F(ax+b)}{a} \right)'+0=\left( \dfrac{1}{a}F(ax+b) \right) \\
\dfrac{1}{a} (F(ax+b))' = [\text{chain rule}] \\
\dfrac{1}{\cancel{ a }} F'(ax+b)\cancel{ a } \\
F'(ax+b)=f(ax+b) \\
\mathrm{Q.E.D.}
\end{align}
$$
### Example
Calculate ${}\int \sqrt{ 2x+1 } \, dx{}$
${}(f(x)=\sqrt{ x },ax+b=2x+1){}$
#### Solution:

$$
\begin{align}
\int \sqrt{ x } \, dx =F(x)+C \iff \int \sqrt{ 2x+1 } \, dx =\dfrac{F(2x+1)}{2}+C  \\
\int \sqrt{ x } \, dx = \int x^{1/2} \, dx = \dfrac{x^{1/2+1}}{\dfrac{1}{2}+1}=\dfrac{x^{3/2}}{3 /2}=\underbrace{ \dfrac{2}{3}x^{3/2} }_{ =F(x) } \\
 \\
\int \sqrt{ 2x+1 } \, dx =\dfrac{F(2x+1)}{2}+C =\dfrac{\dfrac{2}{3}(2x+1)^{3/2}}{2}+C =\dfrac{1}{3}(2x+1)^{3/2}+C
\end{align}
$$
#### Testing:

$$
\begin{align}
\left( \dfrac{1}{3}(2x+1)^{3/2}+C \right)'=\dfrac{1}{\cancel{ 3 }} \dfrac{\cancel{ 3 }}{2}(2x+1)^{1/2}*(2x+1)'=\cancel{ \dfrac{1}{2} }(2x+1)^{1/2}*\cancel{ 2 } \\
=(2x+1)^{1/2}=\sqrt{ 2x+1 }
\end{align}
$$
## Variable Substitution
The previous problem can also be solved with variable substitution, essentially substituting arguments we *don't* know how to deal with, with arguments we *do* know how to deal with
### Example
Calculate ${}\int \cos ^{2}(x) \, dx{}$

$$
\begin{align}
\enclose{box}{\cos ^{2}(x)=\dfrac{\cos(2x)+1}{2} } \\
\cos(2x)=\cos ^{2}(x)-\sin ^{2}(x)=\cos ^{2}(x)+\cos ^{2}(x)-\cos ^{2}(x)-\sin ^{2}(x) \\
\cos ^{2}(x)+\cos ^{2}(x)-(\cos ^{2}(x)+\sin^{2} (x))=\cos ^{2}(x)+\cos ^{2}(x)-1 \\
2\cos ^{2}(x)-1
\end{align}
$$

$$
\begin{align}
\int \cos ^{2}(x) \, dx =\int \dfrac{\cos(2x)+1}{2} \, dx \\
\int \left( \cos \dfrac{2x}{2}+\dfrac{1}{2} \right) \, dx =\dfrac{1}{2}\int \cos (2x) \, dx+\dfrac{1}{2}\int  \, dx  \\
\dfrac{1}{2}\dfrac{\sin (2x)}{2}+\dfrac{1}{2}x+C \\
\dfrac{\sin(2x)}{4}+\dfrac{x}{2}+C
\end{align}
$$
Similarly ${}\int \sin ^{2}(x) \, dx{}$, using ${}\sin ^{2}(x)=\dfrac{1-\cos(2x)}{2}{}$

$$
\begin{align}
\int \cos ^{2}() \, dx = \int \dfrac{1-\cos(2x)}{2} \, dx   \\
\dfrac{x}{2}-\dfrac{\sin(2x)}{4}+C
\end{align}
$$
## Partial Integration
Method to calculate multiplication between functions, ${}\int f(x)g(x) \, dx{}$

> [!WARNING] Dangerous pitfall
> $$
> \int f(x)g(x) \, dx \neq \int f(x) \, dx \times \int g(x) \, dx \\
> \iff  \\
> (f(x)g(x))' \neq f'(x)g'(x)
> $$

Method:

$$
\begin{align}
\int \overset{ \uparrow }{ f(x) }\overset{\downarrow}{g(x)} \, dx =F(x)g(x)-\int F(x)g'(x) \, dx
\end{align}
$$
Note that ${}C{}$ is still relevant here, but it's hiding within the ${}\int F(x)g'(x) \, dx{}$ integral. 
Here ${}\uparrow{}$ indicates integration, and ${}\downarrow{}$ indicates derivation.
- Why is this **true**?
  It's a reverse application of the product rule
- Why is this **useful**?
  we can easily remove annoying to integrate functions withing an integral, since they get reduced to ${}g'(x){}$, through derivation

### Example
Calculate ${}\int x\cos(x) \, dx{}$
#### Solution:
$$
\begin{align}
\int \overset{\downarrow}{x}\overset{\uparrow}{\cos(x)} \, dx =x\sin(x)-\int 1\sin(x) \, dx \\
x\sin(x)-\int \sin(x) \, dx=x\sin(x)-(-\cos(x))+C \\
x\sin(x)+\cos(x)+C
\end{align}
$$
We have to chose our ${}\uparrow{}$ and ${}\downarrow{}$ carefully, so we get a simpler integral than what we started with. If we were to do the reverse here we'd get:

$$
\begin{align}
\int \overset{\uparrow}{x}\overset{\downarrow}{\cos(x)} \, dx = \dfrac{x^{2}}{x}\cos(x)-\int \dfrac{x^{2}}{2}(-\sin(x)) \, dx  \\
\dfrac{x^{2}}{x}\cos(x)+\int \dfrac{x^{2}}{2}(\sin(x)) \, dx 
\end{align}
$$
which while mathematically true, is not any simpler to calculate.
### Example
Calculate ${}\int x e^{ x } \, dx{}$
#### Solution:
$$
\begin{align}
\int x e^{ x } \, dx=x e^{ x }-\int 1 e^{ x } \, dx  \\
x e^{ x }-\int e^{ x } \, dx  \\
x e^{ x }-e^{ x }+C
\end{align}
$$
### Example
Calculate ${}\int x^{2}\sin(x) \, dx{}$
#### Solution