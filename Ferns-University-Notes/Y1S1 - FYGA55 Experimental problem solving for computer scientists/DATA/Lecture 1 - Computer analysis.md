On scales, messure differences rather than sizes, if size is irrelevant, so relative values as opposed to absolute values
Isolate away noise through different means, like in the example of ligo, damping
The wanted value is called the signal, while everything else is noise, what counts as a signal is subjective and depends on the experiment

Handin supposed to be in by 23rd of september

Learning for life? how can the course material be applied to me
Limit the subject size, break up into smaller more understandable parts

Hypothesis is as much about the idea as how to test the idea, in the experiment themselves, with experiments that have to be done in nature

Dependant and independant variables is important! and you're responsible for deciding which is independant or not, time is usually the independant variable.

Most of this seems like unit and dimentional analysis $A*v=\text{flow}=V/t$
The simpler the messuring process, the better, as you get less errors, and anyone could do it

### Example
messurement of a small carriage traveling a metre

| $t/\pu{ s }$ | $s/\pu{ m }$ |
| :----------: | :----------: |
|    08.05     |      0       |
|    08.53     |     0.5      |
|    09.10     |      1       |
![[Lecture 1 - Computer analysis 2026-09-08 09.17.54.excalidraw]]

$$
\begin{align}
v=\dfrac{\Delta s}{\Delta t}=\dfrac{1}{1.03}\pu{ m/s }=0.97\pu{ m/s }\approx 1\pu{ m/s }\pm()\pu{ m/s }
\end{align}
$$
is it reasonable? yeah
use the simplest method of analysis for troubleshooting

there are no perfect messurements, just good enough

when basing messurement on videos, dont you fucking dare rely on the left and right arrow keys

### Least squares (minsta kvadrat metoden)
#### model (theory, hypothesis):
essentially what graph we try and fit the data to
$$
\begin{align}
\hat{y}_{i}=mx_{i}+c
\end{align}
$$
where $i$ is the index of the messurement
and $m$ and $c$ are parameteres, constants that havent been decided yet, or are variable until we've decided a fit
#### residual:
what's left, how much you're off per point
$$
\begin{align}
\Delta y_{i}=y_{i}-\hat{y}_{i}
\end{align}
$$
where $y_{i}$ is the messurement, and $\hat{y}_{i}$ is the proposed theoretical value
so we wanna minimise the total residues (SSR Sum of Squares of Residuals)
$$
\begin{align}
\text{SSR}=\sum^{n}_{i=1}(\Delta y_{i})^{2}=(\Delta y_{1})^{2}+(\Delta y_{2})^{2}+\dots(\Delta y_{n})^{2}
\end{align}
$$
#### minimise SSR
what we want to do here is fit the constants of the model, $m$ and $c$ so the calculated value of SSR is as low as possible, or the "fit"  is as good as possible


$$
\begin{align}
\dfrac{d}{dm}=\left. \dfrac{d}{dm} \right| _{\text{keep the second variable constant}}
\end{align}
$$