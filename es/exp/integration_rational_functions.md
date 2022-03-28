Every rational function $\dfrac{P(x)}{Q(x)}$ (quotient of polynomials with real coefficients) [may be decomposed into a sum of a polynomial and multiples of partial fractions](thm | partial_fraction_decomposition) of the type  

$$\dfrac{1}{(x-a)^n}$$
$$\dfrac{A+Bx}{\left((x-a)^2+b^2\right)^n}$$

Therefore integration of rational functions is always solvable, as long as we know how to integrate the previous functions. The first type is immediate:

$$\int \dfrac{1}{x-a}\dd x=\ln\vert x-a\vert+k$$
$$\int \dfrac{1}{(x-a)^n} \dd x=-\dfrac{1}{n-1}\dfrac{1}{(x-a)^{n-1}}+k\qquad \text{if \(n\neq 1\)}$$

For the second type, after changes of variable and manipulations, we are left with fractions of the form

$$\dfrac{1}{(x^2+1)^n}$$
$$\dfrac{x}{(x^2+1)^n}$$

The change of variable $t=x^2+1$ is well-suited for the second case

$$
\int \dfrac{x}{(x^2+1)^n} \dd x
\oveq{ t=x^2+1\\ \d t=2x\dd x }
\dfrac{1}{2}\int \dfrac{1}{t^n} \dd t
$$

As for the first case, the implicit change of variable $\tan t=x$ turns everything into [powers of cosines](exp | integration_powers_trig_functions)

$$
\int \dfrac{1}{(x^2+1)^n} \dd x
\oveq{ \tan t=x\\ \frac{1}{\cos^2(t)}\dd t=\d x }
\int \dfrac{1}{\left(\tan^2(t)+1\right)^n}\dfrac{1}{\cos^2(t)} \dd t \\
= \int \dfrac{1}{\left(\frac{1}{\cos^2(t)}\right)^n}\dfrac{1}{\cos^2(t)} \dd t=
\int \cos^{2n-2}(t) \dd t
$$