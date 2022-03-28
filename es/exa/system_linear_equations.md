The expression

$$2x_1+3x_2+4x_3=24$$

is a linear equation, with coefficients $a_1=2$, $a_2=3$, $a_3=4$ and independent term $b=24$. When few unknowns are used, it is customary to call them $x$, $y$, $z$, $t$... just to avoid many subindexes

$$2x+3y+4z=24$$

For instance $(x=1,y=2,z=4)$ is a solution of this linear equation, because replacing the unknowns with the chosen values satisfies the equality

$$2\cdot 1+3\cdot 2+4\cdot 4=24$$

$(x=10,y=-8,z=7)$ is a solution too

$$2\cdot 10+3\cdot (-8)+4\cdot 7=24$$

but $(x=1,y=1,z=1)$ is not a solution

$$2\cdot 1+3\cdot 1+4\cdot 1= 9 \neq 24$$

that is, some choices may be solutions but others may not. We would like to find _all_ solutions

Now we may add a second equation

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
7x+y-3z  & = & -5\\
\end{array}\right.
$$

thus having a system of linear equations. For this system, our first choice $(x=1,y=2,z=4)$ is still a solution:

$$
\left\{
\begin{array}{rcl}
2\cdot 1+3\cdot 2+4\cdot 4 & = & 24\\
7\cdot 1+1\cdot 2-3\cdot 4 & = & -5\\
\end{array}\right.
$$

but the second choice $(x=10,y=-8,z=7)$ is no longer a solution

$$
\left\{
\begin{array}{rcl}
2\cdot 10+3\cdot (-8)+4\cdot 7 & = & 24\\
7\cdot 10+1\cdot (-8)-3\cdot 7 & = & 41\neq -5\\
\end{array}\right.
$$

This is kind of obvious: the more equations we have to satisfy, the less solutions we find. As before, we would like to find _all_ solutions - how should we proceed?