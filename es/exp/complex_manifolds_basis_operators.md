Sea $M$ una variedad compleja de dimensión $n$. Esto es, en cada punto de $M$ tenemos una carta compleja $\varphi:U\longrightarrow \C^n$, que parametriza localmente $U\subset M$ por medio de $n$ coordenadas complejas $z^1$, ... , $z^n$. Desde un punto de vista diferenciable, $\C^n\simeq\R^{2n}$, con lo que $M$ también tiene estructura de variedad diferenciable (real) de dimensión $2n$, descrita localmente por las coordenadas $x^1$, $y^1$, ... , $x^n$, $y^n$, con $z^j=x^j+\ii y^j$. Asociada a esta estructura, tenemos el espacio tangente real, que se puede ver como el conjunto de derivaciones actuando en funciones reales:

$$TM=\left\langle\frac{\partial}{\partial x^1},\frac{\partial}{\partial y^1},...,\frac{\partial}{\partial x^n},\frac{\partial}{\partial y^n}\right\rangle_\R$$

y su espacio dual:

$$T^*M=\langle\d x^1,\d y^1,...,\d x^n,\d y^n\rangle_\R$$

Si quisiéramos trabajar con el conjunto de derivaciones sobre funciones complejas, basta con complexificar el espacio anterior:

$$TM_\C=\left\langle\frac{\partial}{\partial x^1},\ii\frac{\partial}{\partial x^1},...,\frac{\partial}{\partial y^n},\ii\frac{\partial}{\partial y^n}\right\rangle_\R=\left\langle\frac{\partial}{\partial x^1},\frac{\partial}{\partial y^1},...,\frac{\partial}{\partial x^n},\frac{\partial}{\partial y^n}\right\rangle_\C=TM\otimes\C$$

y lo mismo con el espacio dual:

$$T^*M_\C=\langle\d x^1,\ii\d x^1,...,\d y^n,\ii\d y^n\rangle_\R=\langle\d x^1,\d y^1,...,\d x^n,\d y^n\rangle_\C=T^*M\otimes\C$$

Pero para estos dos últimos espacios otra base será más útil

$$\frac{\partial}{\partial z^j}=\dfrac{1}{2}\left(\frac{\partial}{\partial x^j}-\ii\frac{\partial}{\partial y^j}\right)\qquad
\frac{\partial}{\partial \bar{z}^j}=\dfrac{1}{2}\left(\frac{\partial}{\partial x^j}+\ii\frac{\partial}{\partial y^j}\right)$$

$$\d z^j=\d x^j+\ii\d y^j\qquad
\d \bar{z}^j=\d x^j-\ii\d y^j$$

respecto de la cual aparecen las siguientes descomposiciones:

$$T^{1,0}M=\left\langle\frac{\partial}{\partial z^1},...,\frac{\partial}{\partial z^n}\right\rangle_\C\qquad T^{0,1}M=\left\langle\frac{\partial}{\partial \bar{z}^1},...,\frac{\partial}{\partial \bar{z}^n}\right\rangle_\C$$

$$(T^{1,0}M)^*=\Lambda^{1,0}M=\langle\d z^1,...,\d z^n\rangle_\C\qquad(T^{0,1}M)^*=\Lambda^{0,1}M=\langle\d \bar{z}^1,...,\d \bar{z}^n\rangle_\C$$

$$TM_\C=T^{1,0}M\oplus T^{0,1}M\qquad T^*M_\C=\Lambda^{1,0}M\oplus \Lambda^{0,1}M$$

Pues bien, esta descomposición está bien definida independientemente de las cartas, porque las derivaciones $\left\{\dfrac{\partial}{\partial \bar{z}^1},...,\dfrac{\partial}{\partial \bar{z}^n}\right\}$ se anulan en funciones holomorfas. Y esta descomposición alcanza el espacio de formas:

$$\Omega^k(M)=\bigoplus_{p+q=k}\Lambda^{p,q}(M)$$

donde $\Lambda^{p,q}(M)$ está generado por las formas con $p$ términos holomorfos y $q$ términos antiholomorfos $\omega(z)=\eta(z)\d z^{j_1}\wedge\cdots\wedge\d z^{j_p}\wedge\d\bar{z}^{k_1}\wedge\cdots\wedge \d\bar{z}^{k_q}$.

Además tenemos los siguientes operadores diferenciales:

$$\partial=\frac{\partial}{\partial z^j}\d z^j:\Lambda^{p,q}(M)\longrightarrow\Lambda^{p+1,q}(M)$$
$$\bar{\partial}=\frac{\partial}{\partial \bar{z}^j}\d \bar{z}^j:\Lambda^{p,q}(M)\longrightarrow\Lambda^{p,q+1}(M)$$

esto es, 

$$\partial(f\d z^I)=\frac{\partial f}{\partial z^j}\d z^j\wedge\d z^I$$
$$\bar{\partial}(f\d z^I)=\frac{\partial f}{\partial \bar{z}^j}\d \bar{z}^j\wedge\d z^I$$ 

Estos operadores satisfacen

$$\d=\partial+\bar{\partial}\qquad\partial\partial=0\qquad \bar{\partial}\bar{\partial}=0\qquad\partial\bar{\partial}=-\bar{\partial}\partial$$

De hecho,

$$\partial+\bar{\partial}=\frac{\partial}{\partial z^j}\d z^j+\frac{\partial}{\partial \bar{z}^j}\d \bar{z}^j=\frac{\partial}{\partial x^j}\d x^j+\frac{\partial}{\partial y^j}\d y^j=\d$$

$$0=\d^2=(\partial+\bar{\partial})(\partial+\bar{\partial})=\partial^2+\partial\bar{\partial}+ \bar{\partial}\partial+\bar{\partial}^2$$

$\partial^2$ añade dos términos holomorfos, $\bar{\partial}^2$ añade dos términos antiholomorfos y $\partial\bar{\partial} + \bar{\partial}\partial$ añade un término de cada tipo, con lo que cada término debe ser idénticamente cero. 

Hay un isomorfismo canónico

$$\theta:TM\xrightarrow{\simeq} T^{1,0}M,\qquad\frac{\partial}{\partial x^j}\longmapsto\frac{\partial}{\partial z^j},\qquad\frac{\partial}{\partial y^j}\longmapsto\ii\frac{\partial}{\partial z^j}$$

dado por la igualdad de derivaciones con respecto a funciones holomorfas. Multiplicar por $\ii$ en $T^{1,0}M$ induce, junto con $\theta$, la siguiente aplicación lineal:

$$J:TM\longrightarrow TM,\qquad\frac{\partial}{\partial x^j}\longmapsto\frac{\partial}{\partial y^j},\qquad\frac{\partial}{\partial y^j}\longmapsto -\frac{\partial}{\partial x^j},\qquad J^2=-\text{id}$$

llamada _estructura casi compleja_.