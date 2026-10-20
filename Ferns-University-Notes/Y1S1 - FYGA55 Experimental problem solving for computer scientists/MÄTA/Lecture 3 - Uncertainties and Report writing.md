## Uncertainties
The **range** is defined as $\text{range} =\text{largest value}-\text{smallest value}$
The **average** $\bar{x}$ is defined as the sum of all the values, divided by the number of valuesx

Standard deviation of a single value:
$$
\begin{align}
\sigma_{x}=\sqrt{ \dfrac{1}{n-1} \sum^{n}_{i=1}(x_{i}-\bar{x})^{2} }
\end{align}
$$
(shows the quantified scatter of individual values)

why divide by $n-1$
because we dont have $n$ independant values, we only have $n-1$ independant values, since the $n$th value is dependant

Histograms can be used to represent how often values apear in certain ranges

wow if the range is small enough, you get a normal distribution curve
normal distribution
$$
\begin{align}
f(x)=\dfrac{1}{\sqrt{ 2\pi }*\sigma}\exp\left( -\dfrac{(x-\bar{x})^{2}}{2\sigma^{2}} \right)
\end{align}
$$
Standard deviation of the average value:
$$
\begin{align}
\sigma_{\bar{x}}=\sqrt{ \dfrac{1}{n(n-1)} \sum^{n}_{i=1}(x_{i}-\bar{x})^{2} }
\end{align}
$$
(it gets more precise since it's taking into account the number of values)

The standard deviation of the average value can only be used as the unsertanty for an infinite number of values.

For low amount of messurements, the normal distribution might not reflect reality, instead the t distribution curve might be more fitting with its wider base
so instead of $\pm\sigma_{\bar{x}}$ we use $\pm t_{c}\sigma_{\bar{x}}$ where $t_{c}$ is a value that can be looked up in tables for the numbers of messurements

For functions the uncertainty of the function value can be calculated as the uncertainty of the independant messurements corresponding height on the dependant values axis for the tangent in the average independant value

For quantities depending on multiple messurements with uncertainties, where the uncertanties are $u_{a}$, $u_{b}$, and $u_{c}$
We can use the error propagation law
$$
\begin{align}
u_{y}=\sqrt{ \left( \dfrac{\partial y}{\partial a}u_{a} \right)^{2}+\left( \dfrac{\partial y}{\partial b}u_{b} \right)^{2}+\left( \dfrac{\partial y}{\partial c}u_{c} \right)^{2}+\dots }
\end{align}
$$
For a partial derivative, all values other than the one derived for, are treated as constant

Report only as many values as ur uncertanty allows
## Report writing
why write reports?
- spread information
- increase reputation
- get funding

To remember experiments, write notes or logbooks

Writing style
- write for a reader, who might not know anything
- be specific
- write concise
- use past tense, unless reffering to parts of the report like figures
- avoid first person, and pronouns, instead *The temperature was measured every minute*
- write what was done and obtained, not your thoughts
- for abbreviations, declare them the first time in the text they're used
- declare quantities in formulae

Structure
- title
- authors
- abstract
	- Motivation
	- Techniques
	- An overview of the results
- introduction
	- Motivation of why this is tested, and what to find out
	- Background and previous works
	- Summary without details
	- Hypothesis
- theory (principle)
	- Underlying principles
	- Explanations of terms
	- Declaration of quantities
	- Formulas
	- Derivations of formulas
	- Explain how data analysis is done
- materials and methods (experiment)
	- Be specific enough that an independant reader without knowledge of the experiment, could recreate it
	- Sketch (a photo can optionally be added, but is unimportant compared to the sketch)
	- Captions for figures like sketches and images
	- Include how the setup works, describing all the parts and their functions
	- Describe how the experiment was performed, and what was messured
	- Describe what samples were used
	  
	- Do not write in a recipe style, or a step by step style
- results
	- Present calculated numbers
	- Include the data needed to support your conclusions
	- Use graphs for larger amounts of data
	- Tables should be labled and numbered above, as opposed to figures (as they may stretch multiple pages)
	- Refer to the tables and figures in the body text of the chapter (with pretty links :3)
	- In the table header, state what variables could be varied, but were kept constants, and give them a quantity
	- Be precise with your units, and dont substitute them with $y$ and $x$, in regression and formulae
- discussion
	- an interpretation of the results
	- avoid too much details, give an overview
	- discuss plausability, is some hypothesis or model supported
- conclusion
	- What was the goal?
	- Was the goal achieved?
	- Compare or confirm others work or publications
- acknowledgement
	- If in a professional setting
	- Acknowledge persons who contributed to the experiment
	- Acknowledge funding sources
- appendicies
	  Material that disturbs readability
	- Long tables
	- Lengthy derivations
	- Source code of computer programs
- references
	- Publications that are helpful in the context of your work and relate to the report
	- Publications in which material originates from, graphs, and non common formulae
	- All necessary information about publications
	- Use a standard citation form
	- Preferably dont site webpages as they are volotile
		- if cited, give the retriaval date

