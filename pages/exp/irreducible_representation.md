Imagine we tweak a little bit the [representation of $\Z_n$ as plane rotations]( exa | representation_finite_group # zn_plane_rotations ) so that it becomes a representation _as space rotations_:

$$
\rho': \Z_n \ll \GL(\C^3)\qquad
[k] \maps 
\begin{pmatrix}
\cos\left(\frac{2\pi k}{n}\right) & -\sin\left(\frac{2\pi k}{n}\right) & 0 \\[0.5em]
\sin\left(\frac{2\pi k}{n}\right) &  \cos\left(\frac{2\pi k}{n}\right) & 0 \\[0.5em]
0 & 0 & 1
\end{pmatrix}
$$

Well, it certainly _is_ a valid representation... but one could argue whether it adds something new. It's essentially $\rho$ on the $xy$-plane and nothing (better said: the trivial representation) on the $z$-axis

Of course it could have been presented in a more obscure way:

$$
\rho'': \Z_n \ll \GL(\C^3)
$$
$$
[k] \maps 
\begin{pmatrix}
\frac{1}{2}\left[1+\cos\left(\frac{2\pi k}{n}\right)\right] & 
 \frac{1}{\sqrt{2}}\sin\left(\frac{2\pi k}{n}\right) & 
\frac{1}{2}\left[1-\cos\left(\frac{2\pi k}{n}\right)\right] \\[0.5em]
 \frac{1}{\sqrt{2}}\sin\left(\frac{2\pi k}{n}\right) &  
\cos\left(\frac{2\pi k}{n}\right) & 
-\frac{1}{\sqrt{2}}\sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
\frac{1}{2}\left[1-\cos\left(\frac{2\pi k}{n}\right)\right] & 
-\frac{1}{\sqrt{2}}\sin\left(\frac{2\pi k}{n}\right) & 
\frac{1}{2}\left[1+\cos\left(\frac{2\pi k}{n}\right)\right]
\end{pmatrix}
$$

Make the computations, it works!! In the sense that, well, $\rho''([0])=\id_{\C^3}$ and the matrices multiply like $\Z_n$ and so on. Isn't that marvelous?

Well, it's not - careful inspection shows that this is a rotation around the $(1,0,1)$-axis. That's nothing new! It behaves as a rotation on one plane and as a trivial representation on an axis, just like before

So we would like to define when a representation is genuine, _irreducible_, i.e. not a clumsy mix of other representations. And even more, given some representation, be able to know whether it is a mix of smaller pieces

On the other hand, can we find a representation of $\Z_n$ that is not "some kind of rotation"?