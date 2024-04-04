let the derivative: 
$$
\frac{d}{dx} f = \lim_{\Delta x \to 0} \frac{f(x + \Delta x) - f(x)}{\Delta x}
$$
and the Area under a continuous function can be approximated using: 

$$
\begin{aligned}
A = \sum_{n=0}^{\frac{b - a}{\Delta x}}f(a + n \cdot \Delta x) \cdot \Delta x
	
\end{aligned}
$$
this becomes exact when we look at the limiting case as $\Delta x \to 0$. 

if we now compose, we get the Area under $\frac{d}{dx}f$: 

$$
\begin{aligned}
A = \lim_{\Delta x \to 0} \sum_{n=0}^{\frac{b - a}{\Delta x}} \frac{f(a+ n \cdot \Delta x + \Delta x) - f(a + n \cdot \Delta x)}{\Delta x} \cdot \Delta x

\end{aligned}
$$

by cancelling we get: 

$$
\begin{aligned}
\lim_{\Delta x \to 0} \sum_{n=0}^{\frac{b}{\Delta x}} f(n \cdot \Delta x + \Delta x) - f(n \cdot \Delta x)

\end{aligned}
$$


if we expand this out we get: 

$$\begin{aligned}
A = &&f(a + \Delta x) - f(a) \\ 
&& +  f(a + 2 \Delta x) - f(a + \Delta x) \\
&& +  f(a + 3 \Delta x) - f(a + 2\Delta x) \\
&&.\\ 
&&. \\
&&.\\ 
&&+ f\left(a + \frac{b - a}{\Delta x} \Delta x\right)- f\left(a + \left(\frac{b - a}{\Delta x}-1\right)\Delta x\right)

\end{aligned}$$

and we notice that every second term cancels the first term of the previous column, and so we are left with: 
$$
A = f\left(a + \frac{b - a}{\Delta x}\Delta x\right)- f(a)
$$
which in turn simplifies to: 

$$
A = f(b) - f(a)
$$

Therefore, the area under the curve of $\frac{d}{dx}f$ is equal to $f(b) - f(a)$. 

We are now able to find the area under any curve $f$ if we know the function $g$ so that $\frac{d}{dx}g = f$.


