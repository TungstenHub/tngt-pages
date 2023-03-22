Ok, las reglas del juego son: unos elementos y una relación binaria

<ul>
<li>Una colección de elementos</li>
<li>Una relación binaria $\in$</li>
</ul>

{{ image | set_theory_universe width = 480 }}

¿Pero qué es una relación binaria? En lógica, una relación binaria es cierta entidad que dados dos elementos $a$ y $b$, dice si $a\in b$ (_$a$ in $b$_). Lo podemos ver como una máquina etérea con dos huecoss, de tal modo que cuando dos elementos se colocan en los huecoss, la máquina dicta

>>>
_Sí, el primer elemento está en el segundo elemento: $a\in b$_ 
<<<

o

>>>
_No, el primer elemento no está en el segundo elemento: $a\notin b$_
<<<

{{ image | set_theory_universe_comp width = 480 }}

¡Cuidado! Desde el punto de vista de la lógica, los dos "huecoss" de la relación binaria pueden ser ocupados por el mismo elemento, y la máquina debe encargarse de decir si un elemento está en sí mismo, lo que, por ahora, no está prohibido

{{ image | set_theory_universe_comp_self width = 480 }}

La máquina, o la relación binaria, no tiene ninguna restricción en este momento. El concepto _$a$ está en $b$_ no tiene ningún sentido de _pertenencia_, simplemente afirma que la máquina lo ha determinado así con una luz verde. Por lo que podrían ocurrir un montón de casos raros. Por ejemplo, puede ser que nuestra máquina siempre declare _cierto_ para cualesquiera dos elementos, ¡y esto sería perfectamente válido!

{{ image | set_theory_universe_true width = 480 }}

O imagina que no tenemos ningún elemento. ¡También es perfectamente válido! Sólo necesitábamos unos elementos y una máquina con dos huecos. No hay elementos, nada que comprobar, todo bien

{{ image | set_theory_universe_empty width = 480 }}

En sentido estricto, uno sólo tiene que "rellenar una tabla"

{{ image | set_theory_full_comp }}

%% to elaborate further %%

{{ image | set_theory_meaning width = 480 }}

Tenemos que regular todo esto con axiomas