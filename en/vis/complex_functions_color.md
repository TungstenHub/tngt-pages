There is a very interesting way to visualize complex functions. It consists of the following: let's represent complex numbers with colors:

{{ d3js | complex_function data = z }}

Near the origin the colors tend to white, and in the rest, the colors of the chromatic circle have been distributed according to the argument of the complex number. In addition, small curves of equal modulus or equal argument have been marked and the unit circle has been highlighted.

Given a function $f(z)$, we can visualize it by painting each $z$ of the complex plane the color of its image $f(z)$. For example, the function $f(z) = z^2 - 1$ would have the following representation.

{{ d3js | complex_function data = `z^2 - 1` }}

Since $f(-1) = f(1) = 0$, the points $z=-1$, $z=1$ appear white, since their image is $w=0$ which corresponds to white. On the other hand, $z=0$ is painted blue, since $f(0) = -1$.