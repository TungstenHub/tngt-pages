En el contexto de fibrados vectoriales, nos va a ser muy útil reformular el concepto de conexión con analogía a la derivada exterior $\mathrm{d}$:

La derivada exterior (en funciones) es una aplicación $\mathrm{d}:C^\infty(M)=\Omega^0(M)\longrightarrow\Omega^1(M)$, que asocia a cada función una 1-forma que describe el grado de aumento de la función respecto a esa dirección. En esta misma línea, dada una conexión $\nabla$, podemos introducir una **derivada exterior** $\mathrm{d}_\nabla:\Gamma(E)=\Omega^0(E)\longrightarrow\Omega^1(E)=\Omega^1(M)\otimes\Gamma(E)$ 1-formas con valores en $E$, definida por $\mathrm{d}_\nabla(\sigma)(X)=\nabla_X\sigma$, tal que en cada dirección se mide el desvío respecto al transporte paralelo. Esta derivada satisface

<ol>
<li>$\mathrm{d}_\nabla(\sigma+\tau)=\mathrm{d}_\nabla(\sigma)+\mathrm{d}_\nabla(\tau)$</li>
<li>$\mathrm{d}_\nabla(f\sigma)=\mathrm{d} f\otimes\sigma+f\mathrm{d}_\nabla(\sigma)$</li>
</ol>

Por otra parte, es equivalente definir una conexión $\nabla$ o una derivada $\Omega^0(E)\longrightarrow\Omega^1(E)$ satisfaciendo las propiedades de arriba