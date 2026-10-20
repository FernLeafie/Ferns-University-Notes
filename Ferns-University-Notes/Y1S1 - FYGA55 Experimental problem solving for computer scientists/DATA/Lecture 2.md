just trust "AI" ig?

Tips:
- Not too much black box
  however you dont need to know how the functions you use work???, as long as you use `scipy.optimize.minimize`???, no using polyfit
- Ask ai about important things you dont understand
- Make it short, and explain what you understand


| $U /\pu{ V }$ | $I /\pu{ A }$ |
| ------------- | ------------- |
| 0             | 0             |
| 1             | 0.9           |
| 2             | 1.25          |
Have we disproven Ohms law? $U=RI$
no, the resistance just isnt constant, and the material properties of the material in the lightbulb

if we gather more messurement data, we can see that $0, 0$ is an outlier, and the following points form a nice line

### Exercises
#### Exercise

| $U /\pu{ V }$ | $I /\pu{ A }$ |
| ------------- | ------------- |
| 0             | 0             |
| 1             | 0.99          |
| 2             | 1.27          |
a)
calculate the Resistance from the two first points: $R_{1}$
$$
\begin{align}
R_{1}=\dfrac{\Delta U}{\Delta I}=\dfrac{1-0}{0.99-0}\approx 1.01
\end{align}
$$

b)
calculate the Resistance from the two last points: $R_{2}$
$$
\begin{align}
R_{2}=\dfrac{\Delta U}{\Delta I}=\dfrac{2-1}{1.27-0.99}=\dfrac{1}{0.28}\approx 3.57
\end{align}
$$


$$
\begin{align}
R_{1}\neq R_{2}
\end{align}
$$
thus one of these values are likely an outlier, since their difference is so high

Ohms law isnt wrong, it just isnt correct across a big range of voltages

Question everything in science