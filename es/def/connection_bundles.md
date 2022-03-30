Una cuestión que surge al trabajar con fibrados vectoriales es el del _transporte paralelo_. Justo como ocurre en la [geometría riemanniana]( def | affine_connection ), no hay un modo canónico de desplazar vectores a lo largo de la variedad, sino que esto requiere una estructura adicional, una _conexión_. Pero la manera más directa de describirla es mediante una función que, dada una dirección y un campo sobre esa dirección, indique la desviación (infinitesimal) respecto al transporte paralelo.

---

Una **conexión $\nabla$ en un fibrado vectorial $E$** es una aplicación $\nabla:\chi(M)\times \Gamma(E)\longrightarrow \Gamma(E)$ satisfaciendo ($\nabla_X\sigma=\nabla(X,\sigma)$)

<ol>
<li>$\nabla_{X+Y}\sigma=\nabla_X\sigma+\nabla_Y\sigma$</li>
<li>$\nabla_{fX}\sigma=f\nabla_X\sigma$</li>
<li>$\nabla_X(\sigma+\tau)=\nabla_X\sigma+\nabla_X\sigma$</li>
<li>$\nabla_X(f\sigma)=X(f)\sigma+f\nabla_X\sigma$</li>
</ol>

$\forall X$, $Y\in\chi(M)$, $\sigma$, $\tau\in \Gamma(E)$, $f\in C^\infty(M)$.