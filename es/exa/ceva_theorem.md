Veamos algunas comprobaciones / aplicaciones del Teorema de Ceva

---

[{centroid}]

**Baricentro**

Este caso es muy fácil: cada mediana del triángulo corta el lado opuesto por la mitad. Así,

$$AF=FB$$
$$BD=DC$$
$$CE=EA$$

y de este modo

$$\dfrac{AF}{FB}\dfrac{BD}{DC}\dfrac{CE}{EA}=1\times 1\times 1=1$$

---

[{incenter}]

**Incentro**

Según el [teorema de la bisectriz]( exa | bisector_theorem ),

$$
\dfrac{AF}{FB}=\dfrac{AC}{CB}\qquad
\dfrac{BD}{DC}=\dfrac{BA}{AC}\qquad
\dfrac{CE}{EA}=\dfrac{CB}{BA}
$$

y tenemos

$$\dfrac{AF}{FB}\dfrac{BD}{DC}\dfrac{CE}{EA}=\dfrac{AC}{CB}\dfrac{BA}{AC}\dfrac{CB}{BA}=1$$

---

[{orthocenter}]

**Ortocentro**

En este caso los cálculos son un poco más liosos, pero tampoco mucho.

Vamos a intentar encontrar la longitud de las dos partes en que una altura divide un lado:

{{ image | triangle_altitude_projection }}

Aplicando el Teorema de Pitágoras a los dos triángulos rectángulos queda

$$x^2 + h^2 = b^2$$
$$(a-x)^2 + h^2 = c^2$$

Expandiendo la segunda ecuación y sustituyéndola en la primera

$$c^2 = (a-x)^2 + h^2 = a^2 - 2ax + x^2 + h^2 = a^2 - 2ax + b^2$$

obtenemos el modo de despejar $x$:

$$c^2 = a^2 - 2ax + b^2 \Longrightarrow 2ax = a^2 + b^2 - c^2 \Longrightarrow x = \dfrac{a^2 + b^2 - c^2}{2a} $$

Por tanto

$$ AF = \dfrac{c^2 + b^2 - a^2}{2c} $$
$$ FB = \dfrac{c^2 + a^2 - b^2}{2c} $$
$$ BD = \dfrac{a^2 + c^2 - b^2}{2a} $$
$$ DC = \dfrac{a^2 + b^2 - c^2}{2a} $$
$$ CE = \dfrac{b^2 + a^2 - c^2}{2b} $$
$$ EA = \dfrac{b^2 + c^2 - a^2}{2b} $$

y finalmente

$$
\dfrac{AF}{FB}\dfrac{BD}{DC}\dfrac{CE}{EA} = 
\dfrac{\frac{c^2 + b^2 - a^2}{2c}}{\frac{c^2 + a^2 - b^2}{2c}}
\dfrac{\frac{a^2 + c^2 - b^2}{2a}}{\frac{a^2 + b^2 - c^2}{2a}}
\dfrac{\frac{b^2 + a^2 - c^2}{2b}}{\frac{b^2 + c^2 - a^2}{2b}}
= 1
$$