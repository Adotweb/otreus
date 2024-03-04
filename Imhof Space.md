# Imhof Space and Prime Numbers



## 1. The Naturals

### 1.1 Defining the space

Since every natural number can be factorized using prime numbers, we could go as far as to define soew Vector Space $I_n$ that consists of all vectors that can be formed with n entries where every entry is a natural number. Now we can define a mapping $p_n(k)$ that is bijective and takes an input $k \in \mathbb{N}$ that returns a vector of the exponents of the first n prime numbers making up our number $n$.
so for example 12 becomes: 


## $$ \begin{aligned} v = \vec{p}_2(12) &= \vec{p}_2(2^2 \cdot 3^1) = \begin{bmatrix} 2 \\ 1 \end{bmatrix} \\ v &\in  I_2 \end{aligned} $$


### 1.2 Converting back

Now every vector $v \in I_n$ corresponds to exactly one natural number inside $\mathbb{N}_n$ ($\mathbb{N}_n = \mathbb{P}_n \cup \set{a^{k_1} \cdot b^{k_2} : a, b \in \mathbb{P}_n \land k_1, k_2 \in \mathbb{N}}$ where $\mathbb{P}_n = \set{2, 3, 5, 7, ..., p_n}$)   which is all the numbers that can be achieved by multiplying the first $n$ prime numbers in any combination. This means that we can construct a similar function $p_n$ so that 

## $$p_n(\vec{p}_n(k)) = k, k \in \mathbb{N}_n$$


## 1.3 The limiting case 

If we now consider the space 

## $$I = \lim_{n\to\infty} I_n$$ 

we know that $\mathbb{N}_n = \mathbb{N}$. 

## 1.4 Basic Algebra 

If we consider two vectors $v_1, v_2 \in I$ and add them in the traditional way we achieve a multiplication in the corresponding numbers: 

## $$ p_n(\vec{p}(k_1) + \vec{p}(k_2)) = k_1 \cdot k_2$$

and thus: 

## $$ \begin{aligned} p(\vec{p}(k_1) + \vec{p}(k_1)) &= k_1 \cdot k_1 \\  p(2 \cdot \vec{p}(k_1)) &= {k_1}² \end{aligned}  $$

or: 
## $$ \begin{aligned} \vec{p}(k_1) + \vec{p}(k_1) &= \vec{p}(k_1 \cdot k_1) \\  2 \cdot \vec{p}(k_1) &= \vec{p}({k_1}²) \end{aligned}  $$

## 1.5 Linear Algebra 


### 1.5.1 The Dot Product 

Unfortunately we cannot really harness a powerful interpretation for the dot product.

However the following formula:

##  $$ \sigma_n = \vec{v}_n \cdot \vec{d}_n$$
(where $d_n$ = $\begin{bmatrix} 1 \\ 1 \\ 1 \\ \vdots \end{bmatrix}$)


allows us to calculate the exponent sum $\sigma_n$ that indicates the number of primes that were taken from $\mathbb{N}_n$. 
Another measure of similarity is the angle between two numbers in Imhof space: 

## $$ \begin{aligned} \cos{\theta} = \frac{\vec{v}_n \cdot \vec{w}_n}{\lvert\rvert\vec{v}_n\lvert\lvert \cdot \lvert\rvert\vec{w}_n\lvert\lvert}  \end{aligned} $$
if $\cos{\theta} = 1$ or $-1$  we know that $p_n(\vec{v}_n) = p_n(\vec{w}_n)^{k}, k \in \mathbb{Z}$. 
if $\cos{\theta} = 0$ we know that  $\vec{v}_n$ and $\vec{w}_n$ do not have common prime factors.

### 1.5.2 The Magnitude

Since all vectors with the same magnitude lie on the same hypersphere around the origin, we can group numbers by their magnitude. We call these groups circles and their elements dots.


### 1.6 The Rationals 

For now we only looked at vectors in $I$ that only had positive entries, which gave us the range for $p_n(\vec{v}_n)$ as $\mathbb{N}_n$, if we extend our definition to have vectors with negative entries as well however we are able to encode all the rational numbers in $I_n$ our new range for $p_n(\vec{v}_n)$ is now $\mathbb{Q}_n = \set{\frac{a}{b}: a, b \in \mathbb{N}_n}$. Once again if we regard the limiting case: 
## $$ \lim_{n \to \infty}{\mathbb{Q}_n} = \mathbb{Q}^+$$ 
we are able to create a one to one and onto relationship between $I$ and $\mathbb{Q}⁺$.    





