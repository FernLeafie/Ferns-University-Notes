## Partial Integration Cont.

$$
\begin{align}
\int f(x) \, dx 
\end{align}
$$
1. "Directly see the solution"
   ${}\int \cos(2x) \, dx=\dfrac{\sin(2x)}{2}+C{}$
2. "Not directly see the solution"
   ${}\implies{}$ use integration methods
	1. Partial integration
	2. Variable substitution
	3. Partial fraction decomposition

### Example
Calculate ${}\int x^{2}\cos(x) \, dx{}$
#### Solution:
$$
\begin{align}
\int \overset{\downarrow}{x^{2}}\overset{\uparrow}{\cos(x)} \, dx =x^{2}\sin(x)-\int 2x\sin(x) \, dx \\
 \\
\int \overset{\downarrow}{2x}\overset{\uparrow}{\sin(x)} \, dx=2x(-\cos(x)) -\int 2(-\cos(x)) \, dx = \\
2x(-\cos(x)) +\int 2\cos(x) \, dx  = -2x\cos(x)+2\sin(x) \\
\because \\
\int x^{2}\cos(x) \, dx=x^{2}\sin(x)-\int 2x\sin(x) \, dx = \\
x^{2}\sin(x)-(-2x\cos(x)+2\sin(x))+C= \\
x^{2}\sin(x)+2x\cos(x)-2\sin(x)+C 
\end{align}
$$
### Repetition
$$
\begin{align} \\
\int f(x) \, dx =\text{the function }F(x) \\
\text{so that }F'(x)=f(x) 
\end{align}
$$
### Example
Calculate ${}\int x\ln(x) \, dx{}$
#### Solution:

$$
\begin{align}
\int \overset{\downarrow}{x}\overset{\uparrow}{\ln(x)} \, dx =x ??? \\
\text{nevermind} \\
\int \overset{\uparrow}{x}\overset{\downarrow}{\ln(x)} \, dx =\dfrac{x^{2}}{2}\ln(x)-\int \dfrac{x\cancel{ ^{2} }}{2} \dfrac{1}{\cancel{ x }} \, dx =\dfrac{x^{2}}{2}\ln(x)-\int \dfrac{x}{2} \, dx  \\
\dfrac{x^{2}}{2}\ln(x)-\dfrac{x^{2}}{4}+C
\end{align}
$$
Lesson: deriving the ${}x{}$ away isn't always the smartest way, in this case because we don't know ${}\int \ln(x) \, dx{}$
### Example
Calculate ${}{}$${}\int \ln(x) \, dx{}$
#### Solution:
Partial derivation doesn't seem to apply here since it's not two functions, however we can invent a second one!, and since we yet don't know how to integrate ${}\ln(x){}$, we have no choice and have to derive it.
$$
\begin{align}
\int \ln(x) \, dx =\int \overset{\uparrow}{1} \overset{\downarrow}{\ln(x)} \, dx \\
 = x\ln(x)-\int \cancel{ x } \dfrac{1}{\cancel{ x }} \\
 = x\ln(x)-\int 1 \, dx  \\
 x\ln(x)-x+C
\end{align}
$$
### Integration of Elementary Functions
Since we now know ${}\int \ln(x) \, dx{}$ we can add it to the table!

|  ${}f(x){}$  | ${}F(x){}$        |
| :----------: | ----------------- |
| ${}\ln(x){}$ | ${}x\ln(x)-x+C{}$ |
## Variable Substitution
Switching out variables
### Example
Calculate ${}\int 2x e^{ x^{2} } \, dx{}$
#### Solution:
We so far only know one method, so we attempt partial integration:
$$
\begin{align}
\int \overset{\uparrow}{2x} \overset{\downarrow}{e^{ x^{2} }} \, dx = \\
x^{2} e^{ x^{2} }-\int x^{2} (e^{ x^{2} })' \, dx = \\
x^{2} e^{ x^{2} }-\int x^{2} 2xe^{ x^{2} } \, dx = \\
x^{2}e^{x^{2} }-\int 2x^{3} e^{ x^{2} } \, dx \\
\text{mmm that's not any simpler}  \\
\text{hmm, our calculations show that } \\
(e^{ x^{2} })'=2x e^{ x^{2} } \iff \\
\int 2xe^{x^{2}} \, dx =e^{ x^{2} }+C
\end{align}
$$
But stumbling on the solution randomly isn't that great a method.
Is there a more systematic way of solving the exercise?
#### Variable Substitution
$$
t = t(x) \\
\dfrac{dt}{dx}=t'(x)
$$
$$
\int 2x e^{ x^{2} } \, dx = \left\lceil \begin{array}{c}
t=x^{2} \\
e^{t}=e^{ x^{2} } \\
\dfrac{dt}{dx}\iff dt=2xdx \\
\end{array}\right\rfloor= \\
\int 2x e^{ t } \, dx =\int e^{ t } \underbrace{ 2x\, dx }_{ dt }= \\
\int e^{ t } \, dt =e^{ t }+C= \\
e^{ x^{2} }+C
$$
### Example
Calculate ${}\int \dfrac{2x}{x^{2}+1} \, dx{}$
#### Solution:
$$
\begin{gathered}
\int \dfrac{2x}{x^{2}+1} \, dx =\int \dfrac{1}{x^{2}+1}2x \, dx =\left[ \begin{array}{c}
t=x^{2}+1 \\
\dfrac{1}{t}=\dfrac{1}{x^{2}+1} \\
\dfrac{dt}{dx}=2x \iff dt=2xdx
\end{array} \right] = \\
\int \dfrac{1}{t} 2x \, dx= \\
\int \dfrac{1}{t} \, dt = \\
\ln |t|+C = \\
\ln |x^{2}+1|+C = \\
\ln(x^{2}+1)+C
\end{gathered}
$$
#### Testing:

$$
\begin{align}
\ln(x^{2}+1)'=\dfrac{1}{x^{2}+1}2x = \dfrac{2x}{x^{2}+1}
\end{align}
$$
### Example
Calculate ${}\int \sin ^{2}(x)\cos(x) \, dx{}$
#### Solution:

$$
\begin{gathered}
\int \sin ^{2}(x)\cos(x) \, dx =\left[ \begin{array}{c}
t=\sin x \\
t^{2}=\sin ^{2}x \\
\dfrac{dt}{dx}=\cos(x) \\
dt=\cos xdx
\end{array} \right] = \\
\int t^{2} \, dt = \\
\dfrac{t^{3}}{3}+C \\
\dfrac{\sin^{3}(x)}{3}+C
\end{gathered}
$$
### Method
all the prior functions have been a compound function, where the other term is the derivative of the inner function
$$
\begin{align}
 & \int e^{ x^{2} }\times 2x \, dx  & (x^{2})'=2x \\
 & \int \dfrac{1}{x^{2}+1}\times 2x \, dx  & (x^{2}+1)'=2x \\
 & \int \sin ^{2}(x)\cos(x) \, dx  & (\sin (x))' =\cos(x)
\end{align}
$$
Variable substitution helps simplify functions of the form:
$${}\int f(g(x))g'(x) \, dx{}$$
somewhat close to the chaining rule, although not quite.