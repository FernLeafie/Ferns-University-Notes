# Variable Substitution
The method variable substitution works well for integrals of the appearance of:
$$
\begin{align}
\int f(g(x))g'(x) \, dx 
\end{align}
$$
with the method looking like this:
$$
\begin{align}
\int \underbrace{ f(g(x)) }_{ f(t) }\underbrace{ g'(x) \, dx }_{ dt } = \left[ \begin{array}{c}
t =g(x) \\
f(t) =f(g(x)) \\
\dfrac{dt}{dx}=g'(x)  \iff dt=g'(x)dx
\end{array} \right] =\int f(t) \, dt
\end{align}
$$
As the example from yesterday:
$$
\begin{align}
\int e^{ x^{2} }2x \, dx =\left[ \begin{array}{c}
t=x^{2} \\
e^{ t }=e^{ x^{2} } \\
\dfrac{dt}{dx}=2x \iff\\
dt=2xdx
\end{array} \right] l=\int e^{ t } \, dt 
\end{align}
$$
### Example
Calculate ${}\int x^{2}\cos(x^{3}) \, dx{}$
#### Solution:
$$
\begin{align}
\int x^{2}\cos(x^{3}) \, dx = \left[ \begin{array}{c}
t=x^{3} \\
\cos(t)=\cos(x^{3}) \\
\dfrac{dt}{dx}=3x^{2} \iff dt=3x^{2}dx \\
\dfrac{1}{3}dt=x^{2}dx
\end{array} \right] =\int x^{2}\cos(t) \, dx  \\
\int \cos(t)\underbrace{ x^{2} \, dx }_{ \dfrac{1}{3}dt }=\int \cos(t) \dfrac{1}{3} \, dt  =\dfrac{1}{3}\int \cos(t) \, dx =\dfrac{1}{3}\sin(t)+C=\dfrac{1}{3}\sin(x^{3})+C
\end{align}
$$
So if it's not fully following the appearance, and just differs with a constant, we can always just invent constants, and pull them out of the thing air.
### Remember
$$
\int f(x) \, dx =F(x)+C
$$
Then:
$$
\begin{align}
\int f(ax+b) \, dx =\dfrac{F(ax+b)}{a}+C
\end{align}
$$
## Alternative
### Example
Calculate ${}\int \sqrt{ 5x+2 } \, dx{}$
#### Solution:
$$
\begin{align}
\int \sqrt{ 5x+2 } \, dx =\left[ \begin{array}{c}
t=5x+2 \\
\sqrt{ t }=\sqrt{ 5x+2 } \\
\dfrac{dt}{dx}=5\iff  \\
dt=5dx \\
\dfrac{1}{5}dt=dx
\end{array} \right] =\int \sqrt{ t } \, dx =\int \sqrt{ t } \dfrac{1}{5} \, dt  \\
\dfrac{1}{5}\int \sqrt{ t } \, dt =\dfrac{1}{5} \int t^{1/2} \, dt = \dfrac{1}{5} \dfrac{t^{3/2}}{\dfrac{3}{2}}+C=\dfrac{1}{5} \dfrac{2}{3} t^{3/2}+C=\dfrac{2}{15}t^{3/2}+C
\end{align}
$$

> [!WARNING] Easy mistake to make
> "Dividing by inner derivative" only works if the inner derivative is constant!
> ${}\int \cos(3x) \, dx=\dfrac{\sin(3x)}{3}+C{}$ Works perfectly fine.
> ${}\int e^{ x^{2} } \, dx\neq \dfrac{e^{ x^{2} }}{2x}+C{}$ Does not work, as the inner derivative ${}2x{}$ isn't constant
> 
> ${}\left( \dfrac{e^{ x^{2} }}{2x} \right)'{}$ has to be derived with the quotient rule and thus ${}\neq e^{ x^{2} }{}$
> ${}\left( \dfrac{\sin(3x)}{3x} \right)'{}$ doesn't need the quotient rule and thus ${}= \dfrac{1}{\cancel{ 3 }}\cos(3x)\cancel{ 3 }{}$


### Calculate
Calculate ${}\int e^{ \sqrt{ x } } \, dx{}$
#### Solution:
$$
\begin{align}
\int e^{ \sqrt{ x } } \, dx =\left[ \begin{array}{l}
t=\sqrt{ x } \\
e^{ t }=e^{ \sqrt{ x } } \\
\dfrac{dt}{dx}=\dfrac{1}{2\sqrt{ x }} \\
dt=\dfrac{1}{2\sqrt{ x }}dx \\
2\sqrt{ x }dt=dx
\end{array} \right] =\int e^{ t } \, dx =\int e^{ t }2\sqrt{ x } \, dt = \\
\int e^{ t }2t \, dt =2\int te^{ t } \, dt=[\text{yippie partial integration}]=2\int \overset{\downarrow}{t}\overset{\uparrow}{e^{ t }} \, dt  = \\
2\left( te^{ t }-\int 1 e^{ t } \, dt  \right)=2t e^{ t }- 2 e^{ t }+C=2\sqrt{ x }e^{ \sqrt{ x } }-2 e^{ \sqrt{ x } }+C
\end{align}
$$
## Partial Fraction Decomposition
Only used with integration of **rational functions**: ${}f(x)=\dfrac{P(x)}{Q(x)}{}$.
So when ${}P(x){}$ and ${}Q(x){}$ are polynomials.
${}P(x)=a_{0}+a_{1}x+a_{2}x^{2}+\dots+a_{n}x^{n}{}$. Degree of ${}P(x)={}$ the highest ${}x{}$-exponent, expressed as ${}\deg P{}$ 

If ${}\enclose{box}{\deg P\geq\deg Q}{}$ polynomial division works well, at least to get us to a form where partial fraction decomposition works on the rest.
Otherwise, if ${}\enclose{box}{\deg P<\deg Q}{}$ we will have to use partial fraction decomposition. An example of this can be ${}\int \dfrac{x+1}{x^{3}+1} \, dx{}$.
### Building Blocks
the following is true:
1. ${}\int \dfrac{1}{x-1} \, dx=\ln|x-a|+C{}$
2. ${}\int \dfrac{x}{x^{2}+a^{2}} \,dx=\dfrac{1}{2}\ln(x^{2}+a^{2})+C{}$
3. ${}\int \dfrac{1}{x^{2}+a^{2}} \, dx=\dfrac{1}{a}\arctan\left( \dfrac{x}{a} \right)+C{}$
#### Why?

1. 
   $$
   \begin{align}
   \int\dfrac{1}{x-a} \, dx=\left[ \begin{array}{c}
   t=x-a \\
   \dfrac{1}{t}=\dfrac{1}{x-a} \\
   \dfrac{dt}{dx}=1 \\
   dt=dx
   \end{array} \right] =\int \dfrac{1}{t} \, dt=\ln|t|+C =\ln|x-a|+C
   \end{align}
   $$
2. 
   $$
   \begin{align}
   \int \dfrac{x}{x^{2}+a^{2}} \, dx =\int x \dfrac{1}{x^{2}+a^{2}} \, dx=\left[ \begin{array}{c}
   t=x^{2}+a^{2} \\
   \dfrac{1}{t}=\dfrac{1}{x^{2}+a^{2}} \\
   \dfrac{dt}{dx}=2x \\
   dt=2xdx \\
   \dfrac{1}{2}dt=xdx
   \end{array} \right] =\int \dfrac{1}{t} \dfrac{1}{2} \, dt= \\
   \dfrac{1}{2}\int \dfrac{1}{t} \, dt =\dfrac{1}{2}\ln|t|+C =\dfrac{1}{2}\ln(x^{2}+a^{2})+C
   \end{align}
   $$
3. 
   $$
   \begin{align}
   \int \dfrac{1}{x^{2}+a^{2}} \, dx=\int \dfrac{1}{a^{2}\left( \dfrac{x^{2}}{a^{2}}+1 \right)} \, dx =\int \dfrac{1}{a^{2}}\times \dfrac{1}{\dfrac{x^{2}}{a^{2}}+1} \, dx = \\
   \dfrac{1}{a^{2}}\int \dfrac{1}{\dfrac{x^{2}}{a^{2}}+1} \, dx =\dfrac{1}{a^{2}}\int \dfrac{1}{\left( \dfrac{x}{a} \right)^{2}+1} \, dx =\left[ \begin{array}{c}
   t=\dfrac{x}{a}=\dfrac{1}{a}x \\
   \dfrac{1}{t^{2}+1}=\dfrac{1}{\left( \dfrac{x}{a} \right)^{2}+1} \\
   \dfrac{dt}{dx}=\dfrac{1}{a} \\
   dt=\dfrac{1}{a}dx
   \end{array} \right] = \\
   \dfrac{1}{a^{2}}\int \dfrac{1}{t^{2}+1} \, dx =\dfrac{1}{a}\dfrac{1}{a}\int \dfrac{1}{t^{2}+1} \, dx=\dfrac{1}{a}\int \dfrac{1}{t^{2}+1} \dfrac{1}{a} \, dx =\dfrac{1}{a }\int \dfrac{1}{t^{2}+1} \, dt = \\
   \dfrac{1}{a}\arctan(t)+C=\dfrac{1}{a}\arctan\left( \dfrac{x}{a} \right)+C
   \end{align}
   $$
### Example
Calculate ${}\int \dfrac{x+2}{x^{2}+3} \, dx{}$
We will solve this with partial fraction decomposition.
#### Solution:
$$
\begin{align}
\int \dfrac{x+2}{x^{2}+3} \, dx = \\
\int \dfrac{x}{x^{2}+3}+\dfrac{2}{x^{2}+3} \, dx = \\
\int \dfrac{x}{x^{2}+3} \, dx +\int \dfrac{2}{x^{2}+3} \, dx = \\
\int \dfrac{x}{x^{2}+3} \, dx +2\int \dfrac{1}{x^{2}+3} \, dx = \\
[\text{Employing the basic building blocks}]= \\
\dfrac{1}{2}\ln(x^{2}+3)+2 \dfrac{1}{\sqrt{ 3 }}\arctan\left( \dfrac{x}{\sqrt{ 3 }} \right)+C
\end{align}
$$
${}a^{2}=3 \iff a=\sqrt{ 3 }{}$
