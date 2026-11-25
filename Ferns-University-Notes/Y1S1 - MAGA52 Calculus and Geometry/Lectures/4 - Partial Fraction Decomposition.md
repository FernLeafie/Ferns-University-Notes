## Partial Fraction Decomposition
### Building Stones
$$
\begin{align}
\int \dfrac{1}{x\pm a} \, dx =\ln|x\pm a|+C \\
\int \dfrac{x}{x^{2}+a^{2}} \, dx =\dfrac{1}{2}\ln(x^{2}+a^{2})+C \\
\int \dfrac{1}{x^{2}+a^{2}} \, dx =\dfrac{1}{a}\arctan\left( \dfrac{x}{a} \right)+C
\end{align}
$$
But for now, a slight interlude~
### Example
Calculate ${}\int \arctan(x) \, dx{}$
#### Solution
$$
\begin{align}
\int \arctan(x) \, dx =\int \overset{\uparrow}{1} \times \overset{\downarrow}{\arctan(x)} \, dx = \\
x\arctan(x)-\int x\dfrac{1}{1+x^{2}} \, dx = \\
x\arctan(x)-\int \dfrac{x}{x^{2}+1} \, dx = \\
x\arctan(x)-\dfrac{1}{2}\ln(x^{2}+1)+C
\end{align}
$$
### Example
Calculate ${}\int \left( \dfrac{1}{x^{2}+2}-\dfrac{x}{x^{2}+1} \right) \, dx{}$
#### Solution
$$
\begin{align}
\int\left( \dfrac{1}{x^{2}+2}-\dfrac{x}{x^{2}+1} \right) \, dx =\int \dfrac{1}{x^{2}+2} \, dx -\int \dfrac{x}{x^{2}+1} \, dx = \\
\dfrac{1}{\sqrt{ 2 }}\arctan\left( \dfrac{x}{\sqrt{ 2 }} \right)-\dfrac{1}{2}\ln(x^{2}+1)+C
\end{align}
$$
Be careful when integrating fractions to not write them together in an attempt to simplify them, which in this case would yield ${}\dfrac{-x^{3}+x^{2}+2x+1}{x^{4}+3x^{2}+2}{}$, which looks absolutely horrid, and makes applying the building stones incredibly difficult. The goal of partial fraction decomposition is to split up these horrid expressions, into factors that are much easier to deal with as they match the building stones.
## Partial Fraction Decomposition Algorithm
Goal: Integrate ${}\int \dfrac{P(x)}{Q(x)} \, dx{}$
Steps:
0. If ${}\deg P\geqslant\deg Q{}$
   Do a polynomial division
   As that will yield a rest, with the properties ${}\deg P<\deg Q{}$
1. Factorise ${}Q(x){}$
   (Use the factor theorem, ${}Q(x)=0{}$)
   Factorisation gives factors of different types
	-  Linear factor ${}x-a{}$.
	- Square factors ${}x^{2}+a^{2}{}$ that can't be factorised further, irreducible factors, as they have no real roots.
2. Ansatz
   Our educated guess of what the decomposed fractions should look like
	- ${}x-a \to \dfrac{A}{x-a}{}$
	- ${}x^{2}+a^{2}\to \dfrac{Ax+B}{x^{2}+a^{2}}{}$
	- ${}(x-a)^{k}\to \dfrac{A_{1}}{(x-a)}+\dfrac{A_{2}}{(x-a)^{2}}+\dots+\dfrac{A_{k}}{(x-a)^{k}}{}$
3. Decide the values of all unknown constants
   Find the values of all constants from the ansatz step. (Solve a simple equation system, where the relationship between the constants is equal to the previous numerator)
4. Integrate
   ${}\int \dfrac{P(x)}{Q(x)} \, dx=\dots=\int \dfrac{A}{x-a}+\dfrac{Bx+C}{x^{2}+b^{2}}+\dots \, dx{}$
This is because of the Fundamental Theorem of Algebra, which states that any polynomial can be written as a series of factors if we allow complex roots, which we do in the form of the irreducible factors
### Example
Calculate ${}\int \dfrac{5}{x^{3}-x^{2}+4x-4} \, dx{}$
#### Solution
##### Step 1.
Factorise ${}x^{3}-x^{2}+4x-4{}$
$$
\begin{align}
x^{3}-x^{2}+4x-4=0\iff x^{2}(x-1)+4(x-1)=0 \\
(x-1)(x^{2}+4)=0
\end{align}
$$
Otherwise we could have used the PQ method if the solution hadn't been this obvious, and then use polynomial division with that root.
##### Step 2.
$$
\begin{align}
\dfrac{5}{x^{3}-x^{2}+4x-4}=\dfrac{5}{(x-1)(x^{2}+4)}=\dfrac{A}{x-1}+\dfrac{Bx+C}{x^{2}+4}
\end{align}
$$
The goal here is now to find ${}A,B,C{}$ so that the equation above is true.
(Personally i would have just broken out the 5 out of the initial integral, but whatever, this is probably a good example)
(actually never mind that wouldn't have worked)
##### Step 3.
$$
\begin{align}
\dfrac{A}{x-1}+\dfrac{Bx+C}{x^{2}+4}=\dfrac{A(x^{2}+4)}{(x-1)(x^{2}+4)}+\dfrac{(x-1)(Bx+C)}{(x-1)(x^{2}+4)}= \\
\dfrac{Ax^{2}+4A+Bx^{2}+Cx-Bx-C}{(x-1)(x^{2}+4)}=\dfrac{(A+B)x^{2}+(C-B)x+4A-C}{(x-1)(x^{2}+4)}= \\
\because \\
\dfrac{5}{(x-1)(x^{2}+4)}=\dfrac{(A+B)x^{2}+(C-B)x+4A-C}{(x-1)(x^{2}+4)}\iff  \\
\begin{cases}
A+B=0 \\
C-B=0 \\
4A-C=5
\end{cases} \\
A+B=0 \iff A=-B \\
C-B=0 \iff C=B \\
4A-C=5 \iff -4b-b=5 \iff -5b=5 \iff B=-1 \\
A=1, C=-1
\end{align}
$$
$$
\begin{align}
\because \\
\dfrac{5}{(x-1)(x^{2}+4)}=\dfrac{1}{x-1}+ \dfrac{-x-1}{x^{2}+4}= \\
\dfrac{1}{x-1}-\dfrac{x+1}{x^{2}+4}
\end{align}
$$
##### Step 4.
$$
\begin{align}
\int \dfrac{5}{(x-1)(x^{2}+4)} \, dx = \\
\int \left( \dfrac{1}{x-1}-\dfrac{x+1}{x^{2}+4} \right) \, dx = \\
\int \dfrac{1}{x-1} \, dx -\int \dfrac{x}{x^{2}+4} \, dx -\int \dfrac{1}{x^{2}+4} \, dx = \\
\ln|x-1|-\dfrac{1}{2}\ln(x^{2}+4)-\dfrac{1}{2}\arctan\left( \dfrac{x}{2} \right)+C
\end{align}
$$
##### Alternative Method of Finding A
This works with A specifically because A is linear
$$
\begin{align}
\dfrac{5}{(x-1)(x^{2}+4)}=\dfrac{A}{x-1}+\dfrac{Bx+C}{x^{2}+4} \\
\text{Multiply with (x-1)} \\
\dfrac{5\cancel{ (x-1) }}{\cancel{ (x-1) }(x^{2}+4)}=A+\dfrac{Bx+C}{x^{2}+4}(x-1) \\
\dfrac{5}{x^{2}+4}=A+\dfrac{Bx+C}{x^{2}+4}(x-1) | x=1 \\
(\text{as this yields }x-1=0) \\
\dfrac{5}{1^{2}+4}=A+0 \iff A=1 \\
\text{Insert } A=1 \\
\dfrac{5}{(x-1)(x^{2}+4)}=\dfrac{1}{x-1}+\dfrac{Bx+C}{x^{2}+4} \\
\dfrac{5}{(x-1)(x^{2}+4)}-\dfrac{1}{x-1}=\dfrac{Bx+C}{x^{2}+4} \\
\dfrac{5-x^{2}-4}{(x-1)(x^{2}+4)}=\dfrac{Bx+C}{x^{2}+4} \\
\dfrac{1-x^{2}}{(x-1)(x^{2}+4)}=\dfrac{Bx+C}{x^{2}+4} \\
\dfrac{(1-x)(x+1)}{(x-1)(x^{2}+4)}=\dfrac{Bx+C}{x^{2}+4} \\
\dfrac{-\cancel{ (x-1) }(x+1)}{\cancel{ (x-1) }(x^{2}+4)}=\dfrac{Bx+C}{x^{2}+4} \\
\dfrac{-1-x}{x^{2}+4}=\dfrac{Bx+C}{x^{2}+4} \\
-1-x=Bx+c \\
\iff B=-1,C=-1
\end{align}
$$