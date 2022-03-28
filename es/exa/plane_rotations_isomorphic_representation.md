Let's revisit the [representation of $\Z_n$ as plane rotations]( exa | representation_finite_group # zn_plane_rotations ):

$$\rho: \Z_n \ll \GL(\C^2)\qquad
[k] \maps 
\begin{pmatrix}
\cos\left(\frac{2\pi k}{n}\right) & -\sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
\sin\left(\frac{2\pi k}{n}\right) &  \cos\left(\frac{2\pi k}{n}\right)
\end{pmatrix}
$$

$$\bar{\rho}: \Z_n \ll \GL(\C^2)\qquad
[k] \maps 
\begin{pmatrix}
 \cos\left(\frac{2\pi k}{n}\right) & \sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
-\sin\left(\frac{2\pi k}{n}\right) & \cos\left(\frac{2\pi k}{n}\right)
\end{pmatrix}
$$

We said $\rho$ and $\bar{\rho}$ should be considered equal in some sense, but now we have the proper concept. Rotating clockwise is like reflecting anti-clockwise rotation, isn't it? Let's take the $x$-axis reflection:

$$\phi: \C^2 \ll \C^2$$
$$\phi = 
\begin{pmatrix}
1 & 0 \\[0.5em]
0 & -1
\end{pmatrix}
$$

And effectively

$$
\begin{array}{rcll}
\phi\rho_{[k]} & = & 
\begin{pmatrix}
1 & 0 \\[0.5em]
0 & -1
\end{pmatrix} 
\begin{pmatrix}
\cos\left(\frac{2\pi k}{n}\right) & -\sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
\sin\left(\frac{2\pi k}{n}\right) &  \cos\left(\frac{2\pi k}{n}\right)
\end{pmatrix} & \text{\tiny[first rotate clockwise, then reflect]} \\[1.5em]
& = &
\begin{pmatrix}
 \cos\left(\frac{2\pi k}{n}\right) & -\sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
-\sin\left(\frac{2\pi k}{n}\right) & -\cos\left(\frac{2\pi k}{n}\right)
\end{pmatrix} & \text{\tiny[mix of reflection and rotation]} \\[1.5em]
& = &
\begin{pmatrix}
 \cos\left(\frac{2\pi k}{n}\right) & \sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
-\sin\left(\frac{2\pi k}{n}\right) & \cos\left(\frac{2\pi k}{n}\right)
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\[0.5em]
0 & -1
\end{pmatrix} & \text{\tiny[first reflect, then rotate anti-clockwise]} \\[1.5em]
& = &
\bar{\rho}_{[k]}\phi \\
\end{array}
$$

for each $[k]\in\Z_n$. This way, $\rho$ and $\bar{\rho}$ are isomorphic representations via $\phi$.