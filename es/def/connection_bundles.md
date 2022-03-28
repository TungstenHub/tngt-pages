A question that arises when dealing with vector bundles is that of the _parallel transport_. Just like happens in [Riemannian geometry]( def | affine_connection ), there is no canonical way to move vectors along the manifold, but this requires an additional structure, a _connection_. But the more direct way to describe it is by a function that, given a direction and a field along this direction, points out the (infinitesimal) deviation with respect to the parallel transport.

---

A **connection $\nabla$ in a vector bundle $E$** is a map $\nabla:\chi(M)\times \Gamma(E)\longrightarrow \Gamma(E)$ satisfying ($\nabla_X\sigma=\nabla(X,\sigma)$)

<ol>
<li>$\nabla_{X+Y}\sigma=\nabla_X\sigma+\nabla_Y\sigma$</li>
<li>$\nabla_{fX}\sigma=f\nabla_X\sigma$</li>
<li>$\nabla_X(\sigma+\tau)=\nabla_X\sigma+\nabla_X\sigma$</li>
<li>$\nabla_X(f\sigma)=X(f)\sigma+f\nabla_X\sigma$</li>
</ol>

$\forall X$, $Y\in\chi(M)$, $\sigma$, $\tau\in \Gamma(E)$, $f\in C^\infty(M)$.