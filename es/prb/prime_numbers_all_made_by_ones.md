Show that for each prime number $p$ different from $2$ and $5$, there exist some number $1111\cdots 1111$ all made by ones that is a multiple of $p$

For instance, $3$ divides $111$ and $7$ divides $111111$

+++
Solution
+++

Consider the number $\dfrac{1}{p}$. Since $p$ is not $2$ or $5$, its decimal representation is a pure periodic decimal number, which can be converted back to a fraction whose denominator is a number all made by $9$

$$\dfrac{1}{7}=0.142857142857142857\cdots=0.\overline{142857}=\dfrac{142857}{999999}$$
$$\dfrac{1}{p}=0.\overline{period}=\dfrac{period}{999\cdots 999}$$

So $period\cdot p=999\cdots 999$ and $p|999\cdots 999$. If $p\neq 3$, it also happens that $p|111\cdots 111$, as we wanted to prove; for $p=3$, just remind that $3|111$

A deeper proof is available with the theory of congruences and [Fermat Little Theorem]( TO-DO ) 
	
+++