Imagina que variamos un poquito la [representación de $\Z_n$ como rotaciones en el plano]( exa | representation_finite_group # zn_plane_rotations ) para que pase a ser una representación _como rotaciones en el espacio_:

$$
\rho': \Z_n \ll \GL(\C^3)\qquad
[k] \maps 
\begin{pmatrix}
\cos\left(\frac{2\pi k}{n}\right) & -\sin\left(\frac{2\pi k}{n}\right) & 0 \\[0.5em]
\sin\left(\frac{2\pi k}{n}\right) &  \cos\left(\frac{2\pi k}{n}\right) & 0 \\[0.5em]
0 & 0 & 1
\end{pmatrix}
$$

Bueno, ciertamente _es_ una representación válida... pero uno se podría preguntar si añade algo nuevo. Es esencialmente $\rho$ en el plano $xy$ y nada (mejor dicho: la representación trivial) en el eje $z$

Por supuesto se podría haber presentado de un modo más intrincado:

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

Haz las cuentas, ¡funciona! En el sentido de que, bueno, $\rho''([0])=\id_{\C^3}$ y las matrices se multiplican como $\Z_n$ y todo eso. ¿No es maravilloso?

Pues no - si miras bien se trata de una rotación alrededor del eje $(1,0,1)$. ¡No hay nada nuevo! Es una rotación en un plano y una representación trivial en un eje, justo como antes

Así que nos gustaría saber cuándo una representación es genuina, _irreducible_, es decir, no un revuelto de otras representaciones. Y mejor, dada una representación, ser capaz de saber si es unión de piezas más pequeñas

Por otra parte, ¿podemos encontrar una representación de $\Z_n$ que no sea "una especie de rotación"?