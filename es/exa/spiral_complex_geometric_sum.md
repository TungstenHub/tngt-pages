Las espirales geométricas con ángulo variable describen círculos perfectos:

{{ d3js | spiral_complex_geometric_sum }}

Esto se puede probar fácilmente con números complejos: sea $a\in\mathbb{C}$, $\vert a \vert \lt 1$, y

$$S=\sum_{k=0}^\infty a^k = 1+a+a^2+a^3+\cdots = \dfrac{1}{1-a}$$

que represente una suma infinita como la espiral geométrica. Si $a$ cambia en argumento pero no en módulo, entonces $1-a$ describe un círculo centrado en $z=1$ y $S=\frac{1}{1-a}$ describe un círculo también, ya que la inversión compleja $z\mapsto \frac{1}{z}$ está estrechamente relacionada con la inversión geométrica, que [transforma círculos en círculos]( app | circle_inversion_circles_lines )