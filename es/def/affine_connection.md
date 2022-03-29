Una **conexión afín** $\nabla$ en una variedad diferenciable $M$ es una aplicación

$$\nabla:\Gamma(M)\times\Gamma(M)\longrightarrow\Gamma(M)$$

denotada por $\nabla(X,Y)=\nabla_X Y$ y que satisface

<ol>
<li>$\nabla_{X+Y}Z=\nabla_X Z+\nabla_Y Z$</li>
<li>$\nabla_{fX}Z=f\nabla_X Z$</li>
<li>$\nabla_X(Z+W)=\nabla_XZ+\nabla_XW$</li>
<li>$\nabla_X(fZ)=f\nabla_XZ+X(f)Z$</li>
</ol>

---

La linealidad en el primer argumento con respecto a las funciones de $\Gamma(M)$ denota un caracter tensorial, es decir, $(\nabla_XY)_p$ depende de $X_p$ pero no de la extensión de $X$ fuera de $p$. Sin embargo, no es tensorial en el segundo argumento, enfatizado en $\nabla_X(fY)=f\nabla_XY+X(f)Y\neq f\nabla_XY$. Por tanto $(\nabla_XY)_p$ depende de $Y_p$ _y_ de la 'evolución' de $Y$ en la dirección de $X_p$