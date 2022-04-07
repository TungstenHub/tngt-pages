The [representation of $\Z_n$ as plane rotations]( exa | representation_finite_group # zn_plane_rotations ) seems a good candidate of irreducible one. All the plane gets rotated, there seem to be no fixed vectors or subspaces!

But appearances are deceptive, especially if working with complex numbers

$$\rho: \Z_n \ll \GL(\C^2)\qquad
[k] \maps 
\begin{pmatrix}
\cos\left(\frac{2\pi k}{n}\right) & -\sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
\sin\left(\frac{2\pi k}{n}\right) &  \cos\left(\frac{2\pi k}{n}\right)
\end{pmatrix}
$$

All these rotations have common eigenvectors: if $\alpha = \frac{2\pi k}{n}$

$$
\begin{pmatrix}
\cos\alpha & -\sin\alpha \\[0.5em]
\sin\alpha &  \cos\alpha
\end{pmatrix}
\vect{1,\ii} =
\vect{
\cos\alpha-\ii\sin\alpha,
\sin\alpha+\ii\cos\alpha,
} = 
e^{-\ii\alpha}\vect{1,\ii}
$$
$$
\begin{pmatrix}
 \cos\alpha & \sin\alpha \\[0.5em]
-\sin\alpha & \cos\alpha
\end{pmatrix}
\vect{1,-\ii} =
\vect{
\cos\alpha+\ii\sin\alpha,
\sin\alpha-\ii\cos\alpha,
} = 
e^{\ii\alpha}\vect{1,-\ii}
$$

So choosing another base, the previous representation is 

$$
[k] \maps 
\begin{pmatrix}
\zeta_n^k & 0 \\[0.5em]
0 & \overline{\zeta_n}^k
\end{pmatrix}, \qquad 
\zeta_n = e^{\frac{2\pi\ii}{n}}
$$

which is the direct sum of two representations of degree 1, and thus reducible

$$ 
\begin{array}{l}
\rho_{+} : [k] \maps \zeta_n^k \\[0.5em]
\rho_{-} : [k] \maps \overline{\zeta_n}^k \\
\end{array}
$$

It certainly works well with the structure of $\Z_n$, because $\zeta_n^n = 1$. And it also shows that it is completely different to work with $\R$ or with $\C$!