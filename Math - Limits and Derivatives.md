let the derivative: 
$$
\frac{d}{dy} f = \lim_{\Delta x \to 0} \frac{f(x + \Delta x) - f(x)}{\Delta x}
$$
and lets consider the Area under a continuous function $f$ between 0 and b to be: 

$$
\begin{aligned}
\lim_{\Delta x \to 0} \sum_{n=0}^{\frac{b}{\Delta x}}f(n \cdot \Delta x) \cdot \Delta x
	
\end{aligned}
$$

if we now compose: 

$$
\begin{aligned}
\lim_{\Delta x \to 0} \sum_{n=0}^{\frac{b}{\Delta x}} \frac{f(n \cdot \Delta x + \Delta x) - f(n \cdot \Delta x)}{\Delta x} \cdot \Delta x

\end{aligned}
$$

we get by rearranging: 

$$
\begin{aligned}
\lim_{\Delta x \to 0} \sum_{n=0}^{\frac{b}{\Delta x}} f(n \cdot \Delta x + \Delta x) - f(n \cdot \Delta x)

\end{aligned}
$$

we can say that $f(n \cdot \Delta x + \Delta x) - f(n \cdot \Delta x)$ is the change in function, and if we add upp all the changes  of a function up until b (starting at 0) we know that that will equal the difference $f(b) - f(0)$, if we want to know the area under a continuous function $f$ from a to b we can subtract the difference $f(a) - f(0)$ from $f(b) - f(0)$ and get: 


$$
f(b) - f(0) - (f(a) - f(0)) =  f(b) - f(a)
$$
Therefore if we know a function $F$ that wen derived yields $f$ we know that the area under the curve of $f$ from a to b is $F(b) - F(a)$. 

We simplify above notation to: 

$$

\int_{a}^{b}f(x)dx = F(b) - F(a)
$$
and we say that given no bounds $a$ and $b$: 

$$
\int f(x)dx = F(x)
$$

