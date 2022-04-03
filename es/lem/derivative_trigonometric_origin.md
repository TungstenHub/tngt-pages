$$<<< \lim_{h\longrightarrow 0} \dfrac{\sin h}{h}=1 $$
$$<<< \lim_{h\longrightarrow 0} \dfrac{\cos h - 1}{h}=0 $$

+++
Demostración
+++

Si tomamos un ángulo $h$, las cantidades $\dfrac{\sin h}{h}$ y $\dfrac{1-\cos h}{h}$ (hemos tomado el opuesto, $1-\cos h=-(\cos h - 1)$) son respectivamente el tramo verde partido por el azul y el tramo rojo partido por el azul

{{ image | sin_cos_derivatives_origin }}

Cuando $h\longrightarrow 0$, los tramos verde y azul tienden a ser iguales, mientras que el rojo es mucho más pequeño que el azul en una proporción que tiende a anularse. Es por tanto que

$$ \dfrac{\sin h}{h}\longrightarrow 1 \qquad \dfrac{\cos h -1}{h}=-\dfrac{1-\cos h}{h}\longrightarrow 0 $$

+++