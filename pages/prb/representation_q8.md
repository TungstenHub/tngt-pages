Give a non-trivial representation of $Q_8=\{\pm 1, \pm\ii, \pm\jj , \pm\kk\}$

+++
Hint
+++

Quaternions acting on other quaternions...?

+++

+++
Solution
+++

Of course there are _many_ non-trivial representations of $Q_8$ (and we'll find out how to describe _all_ of them), but for this problem, let's find out a reasonably natural representation

A representation is like a group making a vector space spin. $Q_8$ is a group by means of quaternion multiplication. But... what if you multiply to all quaternions? For instance, if we have $\ii \in Q_8$, then

$$q = a + b\ii + c\jj + d\kk$$
$$\ii q = -b + a\ii + -d\jj + c\kk$$

Yes, it's like making the vectors spin!

$$\ii\times\cdot: \vect{a,b,c,d}\maps\vect{-b,a,-d,c}$$

In this case, $a$, $b$, $c$ and $d$ would be real numbers, but we may pay attention only to the coefficients and move into $\C^4$. Following the example, our complete representation would be

$$
\begin{array}{rcl}
\rho:Q_8 & \ll & \GL(\C^4) \\[1em]
x & \maps & [q\maps xq] \\[1em]
1 & \maps &
\begin{pmatrix}
 1 &  0 &  0 &  0 \\
 0 &  1 &  0 &  0 \\
 0 &  0 &  1 &  0 \\
 0 &  0 &  0 &  1 
\end{pmatrix} \\[2.5em]
-1 & \maps &
\begin{pmatrix}
-1 &  0 &  0 &  0 \\
 0 & -1 &  0 &  0 \\
 0 &  0 & -1 &  0 \\
 0 &  0 &  0 & -1
\end{pmatrix} \\[2.5em]
\ii & \maps &
\begin{pmatrix}
 0 & -1 &  0 &  0 \\
 1 &  0 &  0 &  0 \\
 0 &  0 &  0 & -1 \\
 0 &  0 &  1 &  0 
\end{pmatrix} \\[2.5em]
-\ii & \maps &
\begin{pmatrix}
 0 &  1 &  0 &  0 \\
-1 &  0 &  0 &  0 \\
 0 &  0 &  0 &  1 \\
 0 &  0 & -1 &  0
\end{pmatrix} \\[2.5em]
\jj & \maps &
\begin{pmatrix}
 0 &  0 & -1 &  0 \\
 0 &  0 &  0 &  1 \\
 1 &  0 &  0 &  0 \\
 0 & -1 &  0 &  0 
\end{pmatrix} \\[2.5em]
-\jj & \maps &
\begin{pmatrix}
 0 &  0 &  1 &  0 \\
 0 &  0 &  0 & -1 \\
-1 &  0 &  0 &  0 \\
 0 &  1 &  0 &  0 
\end{pmatrix} \\[2.5em]
\kk & \maps &
\begin{pmatrix}
 0 &  0 &  0 & -1 \\
 0 &  0 & -1 &  0 \\
 0 &  1 &  0 &  0 \\
 1 &  0 &  0 &  0 
\end{pmatrix} \\[2.5em]
-\kk & \maps &
\begin{pmatrix}
 0 &  0 &  0 &  1 \\
 0 &  0 &  1 &  0 \\
 0 & -1 &  0 &  0 \\
-1 &  0 &  0 &  0 
\end{pmatrix} \\[2.5em]
\end{array}
$$

By the way, does right multiplication $x \maps [q\maps qx]$ lead to another representation? Well... it doesn't. If we denote module multiplication by $\cdot: (x,q)\maps x\cdot q = qx$, then

$$
a\cdot(b\cdot q) = a\cdot(qb) = qba = (ba)\cdot q \neq (ab)\cdot q 
$$

so it does not match with the group structure of $Q_8$, due to non-commutativity

+++