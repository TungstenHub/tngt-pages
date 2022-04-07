La [representación de $\Z_n$ como rotaciones del plano]( exa | representation_finite_group # zn_plane_rotations ) parece un buen candidato de representación irreducible. Todo el plano se rota, ¡no parece que haya vectores o subespacios fijos!

Pero las apariencias engañan, especialmente si trabajamos con números complejos

$$\rho: \Z_n \ll \GL(\C^2)\qquad
[k] \maps 
\begin{pmatrix}
\cos\left(\frac{2\pi k}{n}\right) & -\sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
\sin\left(\frac{2\pi k}{n}\right) &  \cos\left(\frac{2\pi k}{n}\right)
\end{pmatrix}
$$

Todas estas rotaciones tienen autovectores comunes: si $\alpha = \frac{2\pi k}{n}$

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

Con lo que eligiendo otra base, la representación anterior es

$$
[k] \maps 
\begin{pmatrix}
\zeta_n^k & 0 \\[0.5em]
0 & \overline{\zeta_n}^k
\end{pmatrix}, \qquad 
\zeta_n = e^{\frac{2\pi\ii}{n}}
$$

que es la suma directa de dos representaciones de grado 1, y por tanto reducible

$$ 
\begin{array}{l}
\rho_{+} : [k] \maps \zeta_n^k \\[0.5em]
\rho_{-} : [k] \maps \overline{\zeta_n}^k \\
\end{array}
$$

Ciertamente todo esto funciona bien con la estructura de $\Z_n$, porque $\zeta_n^n = 1$. Y de paso muestra que las cosas son muy diferentes de trabajar con $\R$ a trabajar con $\C$...