>>> 
**Problema de Tangencia de Apolonio:** dibujar un círculo que sea tangente a tres círculos dados.
<<<

Este problema, junto con la solución de Gergonne que se desarrollará aquí, es una auténtica joya de la geometría clásica.

{{ image | ap }}

Vamos por el principio: ¿qué estamos buscando? Buscamos un círculo que sea tangente a los círculos $A$, $B$ y $C$. ¿Y cuántos círculos de estos hay?

{{ image | ap_0 }}

Hay 8, porque para cada uno de $A$, $B$ y $C$ se puede tener tangencia interior o exterior.

Gergonne los tomó por pares: en este caso, trabajaremos con $\Gamma^+$ and $\Gamma^-$, los círculos que tienen las tres tangencias exteriores e interiores respectivamente.

{{ image | ap_1 }}

$A$ es bitangente a $\Gamma^+$ y $\Gamma^-$: sabemos que [los puntos de tangencia están alineados con el punto de similaridad $R$ de $\Gamma^+$ y $\Gamma^-$]( exp | circle_power ), de donde resulta que su potencia a $A$ es $\Pi_{A}(R)=\sqrt{\Pi_{\Gamma^+}(R)\Pi_{\Gamma^-}(R)}$.

{{ image | ap_2 }}

Pero esto también es verdad para $B$ y para $C$, es decir, $\Pi_{A}(R)=\Pi_{B}(R)=\Pi_{C}(R)$. ¡Luego $R$ es de hecho el [centro radical de $A$, $B$ y $C$]( app | circles_radical_center )! ¡Y esto lo sabemos dibujar!

{{ image | ap_3 }}

Por otra parte, teniendo tres círculos, no podemos sino pensar en el [Teorema de d'Alembert]( app | circles_dalembert ): los tres puntos de similaridad (exteriores) $e_{BC}$, $e_{CA}$ y $e_{AB}$ están en una recta $l$. ¿Y esto es útil? Bueno, es crucial.

{{ image | ap_4 }}

Lo círculos $\Gamma$ son bitangentes a $B$ y $C$, luego $\Pi_{\Gamma^+}(e_{BC}) = \Pi_{\Gamma^-}(e_{BC}) = \sqrt{\Pi_{B}(e_{BC})\Pi_{B}(e_{BC})}$. Pero del mismo modo $\Pi_{\Gamma^+}(e_{CA}) = \Pi_{\Gamma^-}(e_{CA})$ y $\Pi_{\Gamma^+}(e_{AB}) = \Pi_{\Gamma^-}(e_{AB})$... ¡así que $l$ debe ser el eje radical de $\Gamma^+$ y $\Gamma^-$!

{{ image | ap_5 }}

Las tangentes a $A$ dibujadas desde los puntos de tangencia con $\Gamma^+$ y $\Gamma^-$ se encuentran en $q$. Son de igual longitud, por lo que la potencia de $q$ respecto a los círculos $\Gamma$ es la misma - esto es, $q$ está sobre el eje radical $l$.

{{ image | ap_6 }}

$q$ es el [polo]( app | circle_polar_line ) de la recta verde con respecto a $A$, y está sobre $l$. Por [reciprocidad polar]( app | circle_polar_recip ), el polo de $l$ respecto a $A$ está sobre la recta verde. Y podemos dibujar tal recta verde, porque tenemos un segundo punto en $R$.

{{ image | ap_7 }}

¡Ésta es la solución de Gergonne! Dibuja el centro radical $R$, después la recta de d'Alembert $l$, con sus polos $p_A$, $p_B$ y $p_C$, y únelos con $R$ - puntos de tangencia encontrados ::heart::

{{ image | ap_label }}

Tomando rectas de d'Alembert con pares de puntos de similaridad interiores obtenemos los otros tres pares de círculos tangentes.