A veces un espacio $X$ se aplica sobre otro espacio $Y$ por dos aplicaciones que son diferentes, pero que en cierto modo son compatibles, en el sentido de que "una aplicación se puede deformar continuamente hasta coincidir con la otra aplicación"

{{ image | homotopic_maps }}

¿Cómo describir formalmente esta propiedad?

---

Sean $X$, $Y$ dos espacios topológicos, $f$ y $g:X\longrightarrow Y$ dos aplicaciones. Decimos que $f$ y $g$ son **aplicaciones homótopas** si existe $H:X\times [0,1]\longrightarrow Y$ tal que $H(x,0)=f(x)$, $H(x,1)=g(x)$, para todo $x\in X$.

Se denota por $f\sim g$ (o $f\sim_H g$ si se quiere poner $H$ explícitamente). $H$ es la _homotopía_ (entre $f$ y $g$).

---

Puede ocurrir también que queramos describir el proceso anterior pero remarcando al mismo tiempo que la imagen de algún subconjunto de $X$ permanece quieta durante la deformación

{{ image | homotopic_maps_relative }}

---

Sean $A\subset X$, $f$, $g:X\longrightarrow Y$ con $f\vert_A=g\vert_A$. Decimos que $f$ y $g$ son **aplicaciones homótopas relativo a $A$** si existe $H:X\times [0,1]\longrightarrow Y$ tal que $H(x,0)=f(x)$, $H(x,1)=g(x)$, para todo $x\in X$, y $H(a,s)=f(a)=g(a)$, para todos $a\in A$, $s\in [0,1]$. Se denota por $f\sim g (A)$.