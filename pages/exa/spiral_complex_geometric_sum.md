Geometric spirals with variable angle describe perfect circles:

{{ d3js | spiral_complex_geometric_sum }}

This can be easily proved with complex numbers: let $a\in\mathbb{C}$, $\vert a \vert \lt 1$, and let

$$S=\sum_{k=0}^\infty a^k = 1+a+a^2+a^3+\cdots = \dfrac{1}{1-a}$$

represent an infinite sum as well as a geometric spiral. If $a$ changes in argument but not in modulus, then $1-a$ describes a circle centered in $z=1$ and $S=\frac{1}{1-a}$ describes a circle as well, since complex inversion $z\mapsto \frac{1}{z}$ is closely related to circle inversion, which [transforms circles in circles]( app | circle_inversion_circles_lines )