Powers of sinus and cosinus are integrated in the following way: 

<ol>
<li>

**Odd powers**

$$\int \sin^{2n+1}(x)\,\mathrm{d}x=\int \sin^{2n}(x)\sin x\,\mathrm{d}x=\int (1-\cos^2(x))^n\sin x\,\mathrm{d}x$$

Expanding the binomial $(1-\cos^2(x))^n$ results in several integrals of the form 

$$\int \cos^m(x)\sin x\,\mathrm{d}x$$

all of which are solvable with the change of variable $t=\cos x$, $\mathrm{d}t=-\sin x \,\mathrm{d}x$.

The integral

$$\int \cos^{2n+1}(x)\,\mathrm{d}x=\int \cos^{2n}(x)\cos x\,\mathrm{d}x=\int (1-\sin^2(x))^n\cos x\,\mathrm{d}x$$

is solved in an analogous manner

</li>
<li>

**Even powers**

$$\int \sin^{2n}(x)\,\mathrm{d}x=\int (\sin^2(x))^n\,\mathrm{d}x=\int \left(\dfrac{1-\cos(2x)}{2}\right)^n\,\mathrm{d}x$$
$$\int \cos^{2n}(x)\,\mathrm{d}x=\int (\cos^2(x))^n\,\mathrm{d}x=\int \left(\dfrac{1+\cos(2x)}{2}\right)^n\,\mathrm{d}x$$

and after expanding the binomial, the integrand is expressed in terms of lower powers of $\cos$; this way we may proceed iterating until everything is integrated

</li>
</ol>