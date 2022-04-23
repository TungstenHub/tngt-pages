What can we do to get equivalent systems? There are small tricks. Of course swapping two rows leads to an equivalent system. There is another trick that is quite simple. If we have an equation, say

$$2x-y+5z=8$$

we may multiply it by some number, say $3$, and we get an equivalent equation

$$6x-3y+15z=24$$

Any choice of $x$, $y$ and $z$ that satisfies the first equation (that is, a solution) will satisfy the second equation too. But watch out! _We cannot multiply by $0$_. If we did, we would have

$$0x+0y+0z=0$$

and _every_ choice of $x$, $y$ and $z$ satisfies that. The new equation has many more solutions than the original one, so they're not equivalent. In some sense, equivalency has to do with reversibility: multiplying by a number keeps an implication valid

$$2x-y+5z=8\Longrightarrow 6x-3y+15z=24$$
$$2x-y+5z=8\Longrightarrow 0x+0y+0z=0$$

but whereas the first implication can be reverted by multiplying by $\frac{1}{3}$, the second one cannot be reverted

$$6x-3y+15z=24\Longrightarrow 2x-y+5z=8$$
$$0x+0y+0z=0\kern.4em\not\kern -.4em \Longrightarrow 2x-y+5z=8$$

so

$$2x-y+5z=8\Longleftrightarrow 6x-3y+15z=24$$
$$2x-y+5z=8\kern.6em\not\kern -.6em \Longleftrightarrow 0x+0y+0z=0$$

A final trick is to combine two equations in a suitable way... Suppose one has (among others) a pair of equations:

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
7x+4y+4z & = & 11\\
\end{array}\right.
$$

If both equations have to be satisfied... the equation generated after summing both has to be satisfied too!

$$(2x+3y+4z)+(7x+4y+4z)=24+11$$
$$9x+7y+8z=35$$

This equation alone is not as restrictive as the initial two together... but it is enough to include at least one of the original equations

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
7x+4y+4z & = & 11\\
\end{array}\right.
\qquad \Longleftrightarrow \qquad
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
9x+7y+8z & = & 35\\
\end{array}\right.
$$

simply because one can turn back with the same trick, but subtracting instead of adding. And this would work if we add any multiple of the first equation to the second equation

$$
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
7x+4y+4z & = & 11\\
\end{array}\right.
\qquad \Longleftrightarrow \qquad
\left\{
\begin{array}{rcl}
2x+3y+4z & = & 24\\
7x+4y+4z + k(2x+3y+4z) & = & 11+24k\\
\end{array}\right.
$$

Here $k$ could be any number, even zero! Only that for $k=0$ we're not doing essentially anything

These tricks are so common that they have a special name: **elementary (row) operations**