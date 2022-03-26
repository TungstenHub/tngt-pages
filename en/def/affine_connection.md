An **affine connection** $\nabla$ on a differentiable manifold $M$ is a mapping 

$$\nabla:\Gamma(M)\times\Gamma(M)\longrightarrow\Gamma(M)$$

denoted $\nabla(X,Y)=\nabla_X Y$ and satisfying

<ol>
<li>$\nabla_{X+Y}Z=\nabla_X Z+\nabla_Y Z$</li>
<li>$\nabla_{fX}Z=f\nabla_X Z$</li>
<li>$\nabla_X(Z+W)=\nabla_XZ+\nabla_XW$</li>
<li>$\nabla_X(fZ)=f\nabla_XZ+X(f)Z$</li>
</ol>

---

The linearity in the first argument with respect to functions of $\Gamma(M)$ denotes a tensorial character, that is, $(\nabla_XY)_p$ depends on $X_p$ but not on the extension of $X$ out of $p$. It is not, however, tensorial in the second argument, stressed in $\nabla_X(fY)=f\nabla_XY+X(f)Y\neq f\nabla_XY$. Thus $(\nabla_XY)_p$ depends on $Y_p$ _and_ on the 'evolution' of $Y$ along the direction $X_p$