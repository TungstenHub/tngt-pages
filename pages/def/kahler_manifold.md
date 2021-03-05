In a Riemannian manifold there is a canonical connection, the Levi-Civita connection, which imposes compatibility with respect to the metric and symmetry. If the Riemannian metric comes from a Hermitian metric on a complex manifold, we would also like some compatibility with respect to the complex structure. More concretely, we're looking for a connection $\nabla$ that is compatible with the Riemannian metric ($\nabla g=0$) and with the Hermitian metric ($\nabla \tilde{h}=0$), which necessarily implies $\nabla\omega=0$.

However, since $\omega(u,v)=g(Ju,v)$, the following relation holds:

$$
\begin{array}{rcl}
(\nabla_w\omega)(u,v) & = & w[\omega(u,v)]-\omega(\nabla_w u,v)-\omega(u,\nabla_w v)\\
& = & w[g(Ju,v)]-g(J(\nabla_w u),v)-g(Ju,\nabla_w v)\\
& = & g(\nabla_w(Ju),v)+g(Ju,\nabla_wv)-g(J(\nabla_w u),v)-g(Ju,\nabla_w v)\\
& = & g(\nabla_w(Ju)-J(\nabla_w u),v)=g((\nabla_w J)(u),v)\\
\end{array}
$$

and this relation implies that for a Hermitian manifold $(M,J,h)$ the following are equivalent

<ol>
<li>$\nabla J=0$</li>
<li>$\nabla \omega=0$</li>
<li>$\mathrm{d} \omega=0$</li>
</ol>

A **Kähler manifold** is a Hermitian manifold satisfying the equivalent statements above, and in this case the Levi-Civita connection is compatible with the Hermitian metric.