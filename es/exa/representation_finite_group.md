[{trivial_representation}]

Primer ejemplo: la **representación trivial**

$$\rho: G \ll \GL(V)$$
$$g \maps \id_V$$

Es decir, cada $g$ representa _dejar el espacio vectorial en paz_

Como tal,

$$gv = v \qquad \forall g\,\forall v$$

No es muy interesante, pero se debe mencionar
---

[{zn_plane_rotations}]

Otra representación muy útil es ver $\Z_n$ como rotaciones en el plano (como si fuese $\R^2$ en vez de $\C^2$)

$$\rho: \Z_n \ll \GL(\C^2)$$
$$[k] \maps 
\begin{pmatrix}
\cos\left(\frac{2\pi k}{n}\right) & -\sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
\sin\left(\frac{2\pi k}{n}\right) &  \cos\left(\frac{2\pi k}{n}\right)
\end{pmatrix}
$$

¡Chachi!, cada $[k]\in\Z_n$ efectúa una rotación antihoraria de ángulo $\frac{2\pi k}{n}$

Uno también podría pensar en rotar en sentido horario,

$$\bar{\rho}: \Z_n \ll \GL(\C^2)$$
$$[k] \maps 
\begin{pmatrix}
 \cos\left(\frac{2\pi k}{n}\right) & \sin\left(\frac{2\pi k}{n}\right) \\[0.5em]
-\sin\left(\frac{2\pi k}{n}\right) & \cos\left(\frac{2\pi k}{n}\right)
\end{pmatrix}
$$

Y también uno podría pensar que estas representaciones deberían ser consideradas, en algún sentido, _iguales_

---

[{sn_permutation_basis}]

Los grupos simétricos $S_n$ actúan muy bien en espacios de dimensión $n$ permutando los vectores de la base

$$\rho: S_n \ll \GL(\C^n)$$
$$\rho(\sigma)(e_i) = e_{\sigma(i)}$$

Por ejemplo, si $n=4$ y $\sigma=(123)$, entonces

$$\rho(\sigma): \vect{a,b,c,d} \maps \vect{c,a,b,d}$$