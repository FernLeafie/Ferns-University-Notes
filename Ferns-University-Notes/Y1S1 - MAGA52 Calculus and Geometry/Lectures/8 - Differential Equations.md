# Differential Equations
We will be working with:
- Ordinary Differential Equations (ODE)
As opposed to:
- Partial Differential Equations (PDE)

Some equations we've solved earlier:
${}x^{3}-x^{2}+x-1=0{}$
A solution to an equation is one, or many, values of ${}x{}$ which fulfils the relationship, for example ${}x=1{}$

A differential equation (ordinary differential equation), is a relationship between an unknown function ${}y{}$ and derivatives of ${}y{}$.
A solution to a differential function, is a function ${}y{}$ which fulfils the relationship.

### Example
${}y''+2y'-y=\cos(x){}$
The solution is an ${}y=y(x){}$ that fulfils the relationship.
But this one is too hard for us to solve now supposedly.
### Example
Solve ${}y'=2x+1{}$
#### Solution
$$
\begin{align}
y= \int 2x+1 \, dx = \int 2x \, dx +\int 1 \, dx =\\
y=x^{2}+x+C
\end{align}
$$
There are always an infinite amount of solutions to a differential equation, since ${}C{}$ can take on any value, and we get the same diff equation.
If we have extra constraints, we can be looking for a particular solution, this is called a particular solution, which involves selecting a specific value of ${}C{}$.
- General solution
  ${}y=x^{2}+x+C{}$
- Particular solution
  ${}y=x^{2}+x+2{}$

## Different Notation
The opposite operation of the differential ${}d{}$ is the integral ${}\int{}$, which we can use to do algebraic rewriting if we just use Leibniz's notation as opposed to Lagrange's notation
$$
\begin{align}
y'=2x+1 \\
\dfrac{dy}{dx}=2x+1 \iff dy=(2x+1)dx \\
\int  \, dy =\int (2x+1) \, dx \iff \int 1 \, dy =\int (2x+1) \, dx  \\
y=\int 2x+1 \, dx \iff y=x^{2}+x+C
\end{align}
$$
### Example
Solve ${}y'=x\sin(x){}$, and find the particular solution that fulfils the condition ${}y(0)=1{}$.
#### Solution
$$
\begin{align}
\dfrac{dy}{dx}=x\sin(x)\iff dy=x\sin(x)dx \\
y=\int x\sin(x) \, dx \iff y=-x\cos(x)-\int 1(-\cos(x)) \, dx \\
\iff y=-x\cos(x)+\int \cos(x) \, dx \iff y=-x\cos(x)+\sin(x)+C
\end{align}
$$
General solution: ${}y=-x\cos(x)+\sin(x)+C{}$
Particular solution with ${}y(0)=1{}$
$$
\begin{align}
y=-x\cos(x)+\sin(x)+C \\
y(0)=\sin(0)+C =1 \\
0+C=1 \\
C=1
\end{align}
$$
Particular solution: ${}y= -x\cos(x)+\sin(x)+1{}$
## Order
The order of a differential equation is the highest derivative that's included.
${}y'=x^{91}{}$ is still a diff equation of the first order, since the highest derivative is of the first degree.
${}y''+2y'-y=\cos(x){}$ is a differential equation of the second order, since the highest derivative is ${}y''{}$.

Most diff equations we will see will be around the second order, as that's what's mostly seen in nature.
## First Orders Separable Equations
### Example
Solve ${}\begin{cases}y'y=x \\  y(0)=1\end{cases}{}$

> [!EXAMPLE] Particular or General Solutions
> Generally if a question doesn't have any conditions, the general solution is sought
> > Solve ${}y'y=x{}$
> 
> If a question has conditions, the particular solution is sought
> > Solve ${}\begin{cases}y'y=x \\  y(0)=1\end{cases}{}$
#### Solution
Let's try what we did on the previous question
$$
\begin{align}
yy'=x \iff y \dfrac{dy}{dx}=x \\
ydy=xdx \iff \int y \, dy =\int x \, dx \\
\dfrac{y^{2}}{2}=\dfrac{x^{2}}{2}+C \iff y^{2}=x^{2}+C
\end{align}
$$

> [!INFO] Intricacies of ${}C{}$
> Since ${}C{}$ is any arbitrary constant, we can divide and multiply it however we want, as it will just result in a new arbitrary constant ${}C{}$

$$
\begin{align}
y^{2}=x^{2}+C \iff y=\pm\sqrt{ x^{2}+C }
\end{align}
$$
General solution: ${}y=\pm \sqrt{ x^{2} +C}{}$
For our condition, we only need to consider the positive side, as the square root is always positive, and our solution is positive.
$$
\begin{align}
y(0)=1 \iff \sqrt{ 0^{2}+C } =1 \\
\sqrt{ C }=1 \\
C=1
\end{align}
$$
Particular solution: ${}y=\sqrt{ x^{2}+1 }{}$

### The Idea of Separable Equations
A diff equation of the first order is separable if it can be written as ${}y'=f(x)g(y){}$

$$
\begin{align}
\dfrac{dy}{dx}=f(x)g(y) \iff dy=f(x)g(y)dx \\
\dfrac{1}{g(y)}dy=f(x)dx \iff \int \dfrac{1}{g(y)} \, dy =\int f(x) \, dx 
\end{align}
$$

> [!TLDR] Variable separation
> This is called variable separation, and our goal with it is separating out the ${}x{}$ dependent functions from the ${}y{}$ dependent functions. 
> Which allows us to integrate each side with respect to their variables.

Assuming the above can be calculated, our goal is to solve for ${}y{}$, which gives us the solution to the separable differential equation.
### Example
Solve ${}y'=x\cos ^{2}(y){}$
#### Solution
$$
\begin{align}
y'=\underbrace{ x }_{ f(x) }\underbrace{ \cos ^{2}(y) }_{ g(y) } \iff \dfrac{dy}{dx}=x\cos ^{2}(y) \\
dy=x\cos ^{2}(y)dx \iff \dfrac{1}{\cos ^{2}(y)}=xdx \\
\int \dfrac{1}{\cos ^{2}(y)} \, dy =\int x \, dx \iff \int \dfrac{1}{\cos ^{2}(y)} \, dy =\dfrac{x^{2}}{2}+C \\
\tan(y)=\dfrac{x^{2}}{2}+C \iff y=\arctan\left( \dfrac{x^{2}}{2}+C \right)
\end{align}
$$
### Two Challenges
Two difficulties when using this method.
1. The integrals ${}\int \frac{1}{g(y)} \, dy=\int f(x) \, dx{}$ may be complicated
   Integrals in general are pretty complicated.
2. It's not always easy to solve for ${}y{}$.
   We may not always have an easy way to invert functions, as finding inverses is complex.
### Example
Solve ${}\begin{cases}xy'+y=y^{2} \\  y(1)=\dfrac{1}{3}\end{cases}{}$
#### Solution
$$
\begin{align}
xy'+y=y^{2} \iff xy'=y^{2}-y \\
y'=\dfrac{y^{2}-y}{x} \iff y'=\dfrac{1}{x}(y^{2}-y) \\
\dfrac{dy}{dx}=\dfrac{1}{x}(y^{2}-y)\iff dy=\dfrac{1}{x}(y^{2}-y)dx \\
\dfrac{1}{y^{2}-y}dy =\dfrac{1}{x}dx \iff \int \dfrac{1}{y^{2}-y} \, dy =\int \dfrac{1}{x} \, dx  \\
\int \dfrac{1}{y^{2}-y} \, dy = \ln|x|+C \\
 \\
\text{Partial fraction decomposition in } \mathrm{R.H.S.} \\
y^{2}-y=y(y-1) \\
\dfrac{1}{y^{2}-y}=\dfrac{A}{y}+\dfrac{B}{y-1}=\dfrac{A(y-1)+By}{y(y-1)} \\
\dfrac{(A+B)y-A}{y(y-1)} \\
\begin{cases}
A+B=0 \\
-A=1
\end{cases} \iff A=-1,B=1 \\
 \\
\int \dfrac{1}{y^{2}-y} \, dy =\int \left( -\dfrac{1}{y}+\dfrac{1}{y-1} \right) \, dy =-\ln|y|+\ln |y-1| \\
 \\
-\ln|y|+\ln|y-1|=\ln|x|+C \iff \ln|y-1|-\ln|y|=\ln|x|+C \\
\ln \dfrac{|y-1|}{|y|}=\ln |x|+C
\end{align}
$$