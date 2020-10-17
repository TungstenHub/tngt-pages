First example: the **trivial representation**

$$\rho: G \ll \GL(V)$$
$$g \maps \id_V$$

That is, each $g$ represents _leaving the vector space alone_

As such,

$$gv = v \qquad \forall g\,\forall v$$

Not very interesting, but worth mentioning 

---

Another useful representation is seeing $\Z_n$ as rotations in the plane (as if it was $\R^2$ instead of $\C^2$)

$$\rho: \Z_n \ll \GL(\C^2)$$
$$[k] \maps 
\begin{pmatrix}
\cos\left(\frac{2\pi k}{n}\right) & -\sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
\sin\left(\frac{2\pi k}{n}\right) &  \cos\left(\frac{2\pi k}{n}\right)
\end{pmatrix}
$$

Cool, each $[k]\in\Z_n$ performs an anti-clockwise rotation of angle $\frac{2\pi k}{n}$

One could also think in rotating clockwise,

$$\bar{\rho}: \Z_n \ll \GL(\C^2)$$
$$[k] \maps 
\begin{pmatrix}
 \cos\left(\frac{2\pi k}{n}\right) & \sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
-\sin\left(\frac{2\pi k}{n}\right) & \cos\left(\frac{2\pi k}{n}\right)
\end{pmatrix}
$$

And one would argue that these representations should be, in some sense, _equal_

---

Permutation groups $S_n$ act nicely on spaces of dimension $n$ by permuting base vectors

$$\rho: S_n \ll \GL(\C^n)$$
$$\rho(\sigma)(e_i) = e_{\sigma(i)}$$

For instance, if $n=4$ and $\sigma=(123)$, then

$$\rho(\sigma): \vect{a,b,c,d} \maps \vect{c,a,b,d}$$