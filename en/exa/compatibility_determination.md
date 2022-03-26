The system (of only one equation)

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
\end{array}\right.
$$

is compatible and indeterminate, because it has lots of solutions. Indeed, give $x$ and $y$ the values you want, and then solve for $z$. If we choose $x=3$ and $y=1$, then

$$2x+3y+4z = 2\cdot 3+3\cdot 1 +4z = 24\Longrightarrow 4z=15\Longrightarrow z=\dfrac{15}{4}$$

and $\left(x=3,y=1,z=\frac{15}{4}\right)$ is a solution. If we choose instead $x=0$ and $y=0$, then

$$2x+3y+4z = 2\cdot 0+3\cdot 0 +4z = 24\Longrightarrow 4z=24\Longrightarrow z=6$$

and $(x=0,y=0,z=6)$ is a solution. Do you see? Lots of solutions

---

The system

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
7x+4y+4z & = & 11\\
\end{array}\right.
$$

is compatible and indeterminate, too. It is not so loose though. We may choose the value we like for $x$, but once this choice is fixed, there is no room for other choices. Why? Well, when the value of $x$ is fixed, we are left with something like

$$
\left\{
\begin{array}{rcl}
3y+4z & = & a\\
4y+4z & = & b\\
\end{array}\right.
$$

for some values $a$ and $b$. But the second row is exactly one $y$ bigger than the first row! So $y$ is necessarily $b-a$. And $z$ would be determined thereafter. Lots of solutions again, but _less_ than in the previous example

---

The system

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
2x+3y+4z & = & 27\\
\end{array}\right.
$$

is incompatible: it can't be that $2x+3y+4z = 24$ and $2x+3y+4z = 27$ at the same time! The prototype ("minimal example") of incompatible equation, though, is

$$
\left\{
\begin{array}{rcl}
0x+0y+0z & = & 1\\
\end{array}\right.
$$

Very sad, isn't it?

---

The system

$$
\left\{
\begin{array}{rrrrr}
x & -2y & + z & = & 7\\
2x & -5y & +2z & = & 6\\
3x &  2y & - z & = & 1\\
\end{array}\right.
$$

has exactly one solution, $(x=2,y=8,z=21)$, and therefore is compatible and determinate. But how do we know this? We'll study this in more detail. In the other hand, a system that would be very easily classified as compatible and determinate is

$$
\left\{
\begin{array}{rrrrr}
x &  &  & = & 2\\
 & y &  & = & 8\\
 &  & z & = & 21\\
\end{array}\right.
$$

It seems a stupidity to care about this kind of systems... but it's not! And the reason is that to solve the first system, we will somehow transform it into the second one

$$
\left\{
\begin{array}{rrrrr}
x & -2y & + z & = & 7\\
2x & -5y & +2z & = & 6\\
3x &  2y & - z & = & 1\\
\end{array}\right.
\qquad\leadsto\qquad
\left\{
\begin{array}{rrrrr}
x &  &  & = & 2\\
 & y &  & = & 8\\
 &  & z & = & 21\\
\end{array}\right.
$$

which is straightforward to solve. So... ready to know more?