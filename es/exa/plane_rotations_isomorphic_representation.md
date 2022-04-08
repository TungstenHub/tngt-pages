Volvamos a la [representación de $\Z_n$ como rotaciones en el plano]( exa | representation_finite_group # zn_plane_rotations ):

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

Dijimos que $\rho$ y $\bar{\rho}$ deberían ser consideradas iguales en algún sentido, pero ahora tenemos el concepto apropiado. Rotar en el sentido horario es como reflejar una rotación antihoraria, ¿no? Tomemos la reflexión en el eje $x$:

$$\phi: \C^2 \ll \C^2$$
$$\phi = 
\begin{pmatrix}
1 & 0 \\[0.5em]
0 & -1
\end{pmatrix}
$$

Y efectivamente

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
\end{pmatrix} & \text{\tiny[primero rotar en sentido antihorario, luego reflejar]} \\[1.5em]
& = &
\begin{pmatrix}
 \cos\left(\frac{2\pi k}{n}\right) & -\sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
-\sin\left(\frac{2\pi k}{n}\right) & -\cos\left(\frac{2\pi k}{n}\right)
\end{pmatrix} & \text{\tiny[mezcla de reflexión y rotación]} \\[1.5em]
& = &
\begin{pmatrix}
 \cos\left(\frac{2\pi k}{n}\right) & \sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
-\sin\left(\frac{2\pi k}{n}\right) & \cos\left(\frac{2\pi k}{n}\right)
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\[0.5em]
0 & -1
\end{pmatrix} & \text{\tiny[primero reflejar, luego rotar en sentido horario]} \\[1.5em]
& = &
\bar{\rho}_{[k]}\phi \\
\end{array}
$$

para cada $[k]\in\Z_n$. Así, $\rho$ y $\bar{\rho}$ son representaciones isomorfas vía $\phi$.