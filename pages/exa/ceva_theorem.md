Let's see some checks / applications of Ceva's Theorem

---

**Centroid**

This case is very easy: each median in the triangle cuts the opposite side by half. This way,

$$AF=FB$$
$$BD=DC$$
$$CE=EA$$

and thus

$$\dfrac{AF}{FB}\dfrac{BD}{DC}\dfrac{CE}{EA}=1\times 1\times 1=1$$

---

**Incenter**

According to the [bisector theorem]( exa | bisector_theorem ),

$$
\dfrac{AF}{FB}=\dfrac{AC}{CB}\qquad
\dfrac{BD}{DC}=\dfrac{BA}{AC}\qquad
\dfrac{CE}{EA}=\dfrac{CB}{BA}
$$

and we have

$$\dfrac{AF}{FB}\dfrac{BD}{DC}\dfrac{CE}{EA}=\dfrac{AC}{CB}\dfrac{BA}{AC}\dfrac{CB}{BA}=1$$

---

**Orthocenter**

In this case computations are somewhat more involved, but not too much.

Let's try to find out the length of the two parts in which an altitude splits a side:

{{ image | triangle_altitude_projection }}

Applying the Pythagorean Theorem to the two right triangles yields

$$x^2 + h^2 = b^2$$
$$(a-x)^2 + h^2 = c^2$$

Expanding the second equation and injecting the first one

$$c^2 = (a-x)^2 + h^2 = a^2 - 2ax + x^2 + h^2 = a^2 - 2ax + b^2$$

provides a way to isolate $x$:

$$c^2 = a^2 - 2ax + b^2 \Longrightarrow 2ax = a^2 + b^2 - c^2 \Longrightarrow x = \dfrac{a^2 + b^2 - c^2}{2a} $$

Therefore

$$ AF = \dfrac{c^2 + b^2 - a^2}{2c} $$
$$ FB = \dfrac{c^2 + a^2 - b^2}{2c} $$
$$ BD = \dfrac{a^2 + c^2 - b^2}{2a} $$
$$ DC = \dfrac{a^2 + b^2 - c^2}{2a} $$
$$ CE = \dfrac{b^2 + a^2 - c^2}{2b} $$
$$ EA = \dfrac{b^2 + c^2 - a^2}{2b} $$

$$
\dfrac{AF}{FB}\dfrac{BD}{DC}\dfrac{CE}{EA} = 
\dfrac{\frac{c^2 + b^2 - a^2}{2c}}{\frac{c^2 + a^2 - b^2}{2c}}
\dfrac{\frac{a^2 + c^2 - b^2}{2a}}{\frac{a^2 + b^2 - c^2}{2a}}
\dfrac{\frac{b^2 + a^2 - c^2}{2b}}{\frac{b^2 + c^2 - a^2}{2b}}
= 1
$$