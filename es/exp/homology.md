La homología describe la forma de un espacio de modo verdaderamente asombroso. Aunque al principio parece raro y confuso, luego aparece de modo natural en muchos fenómenos matemáticos. Por ejemplo, en la Característica de Euler-Poincaré: tomamos un espacio, lo triangulamos (lo dividimos en "trocitos") y hacemos la suma alternada del número de trozos utilizados de cada tipo:

$$\chi(X)=\sum_i (-1)^i c_i(X)$$

donde $c_i(X)$ es el número de caras $i$-dimensionales de $X$. Sorprendentemente, no depende de la triangulación

<table>
  <thead>
    <tr>
      <td c cs=2>$X$</td>
      <td c>$c_0$ vertices</td>
      <td c>$c_1$ edges</td>
      <td c>$c_2$ faces</td>
      <td c>$\chi=c_0-c_1+c_2$</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td c>{{ image | point }}</td>
      <td c>{{ image | point }}</td>
      <td c>1</td>
      <td c>-</td>
      <td c>-</td>
      <td c>1</td>
    </tr>
    <tr>
      <td c rs=2>{{ image | curve }}</td>
      <td c>{{ image | curve_4 }}</td>
      <td c>4</td>
      <td c>3</td>
      <td c>-</td>
      <td c rs=2>1</td>
    </tr>
    <tr>
      <td c>{{ image | curve_7 }}</td>
      <td c>7</td>
      <td c>6</td>
      <td c>-</td>
    </tr>
    <tr>
      <td c rs=2>{{ image | circ }}</td>
      <td c>{{ image | circ_5 }}</td>
      <td c>5</td>
      <td c>5</td>
      <td c>-</td>
      <td c rs=2>0</td>
    </tr>
    <tr>
      <td c>{{ image | circ_9 }}</td>
      <td c>9</td>
      <td c>9</td>
      <td c>-</td>
    </tr>
    <tr>
      <td c rs=3>{{ image | disc }}</td>
      <td c>{{ image | disc_5 }}</td>
      <td c>5</td>
      <td c>5</td>
      <td c>1</td>
      <td c rs=3>1</td>
    </tr>
    <tr>
      <td c>{{ image | disc_9 }}</td>
      <td c>9</td>
      <td c>9</td>
      <td c>1</td>
    </tr>
    <tr>
      <td c>{{ image | disc_5c }}</td>
      <td c>6</td>
      <td c>10</td>
      <td c>5</td>
    </tr>
    <tr>
      <td c rs=3>{{ image | sphere_ep }}</td>
      <td c>{{ image | cube_ep }}</td>
      <td c>8</td>
      <td c>12</td>
      <td c>6</td>
      <td c rs=3>2</td>
    </tr>
    <tr>
      <td c>{{ image | oct_ep }}</td>
      <td c>6</td>
      <td c>12</td>
      <td c>8</td>
    </tr>
    <tr>
      <td c>{{ image | icos_ep }}</td>
      <td c>12</td>
      <td c>30</td>
      <td c>20</td>
    </tr>
    <tr>
      <td c rs=2>{{ image | torus_ep }}</td>
      <td c>{{ image | torus_cub_ep }}</td>
      <td c>32</td>
      <td c>64</td>
      <td c>32</td>
      <td c rs=2>0</td>
    </tr>
    <tr>
      <td c>{{ image | torus_6_ep }}</td>
      <td c>36</td>
      <td c>72</td>
      <td c>36</td>
    </tr>
  </tbody>
</table>

Sin embargo, esta misma característica se expresa en términos homológicos (sin necesidad de triangulación), y de hecho, éste es el modo más apropiado. Así que la homología acierta efectivamente al describir la forma de un espacio topológico

$$\chi(X)=\sum_i (-1)^i \text{rk }H_i(X)=\sum_i (-1)^i b_i(X)$$

donde $b_i=\text{rk }H_i(X)$ son los _números de Betti_

<table>
  <thead>
    <tr>
      <td c>$X$</td>
      <td c>$b_0$</td>
      <td c>$b_1$</td>
      <td c>$b_2$</td>
      <td c>$\chi=b_0-b_1+b_2$</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td c>{{ image | point }}</td>
      <td c>1</td>
      <td c>-</td>
      <td c>-</td>
      <td c>1</td>
    </tr>
    <tr>
      <td c>{{ image | curve }}</td>
      <td c>1</td>
      <td c>0</td>
      <td c>-</td>
      <td c>1</td>
    </tr>
    <tr>
      <td c>{{ image | circ }}</td>
      <td c>1</td>
      <td c>1</td>
      <td c>-</td>
      <td c>0</td>
    </tr>
    <tr>
      <td c>{{ image | disc }}</td>
      <td c>1</td>
      <td c>0</td>
      <td c>0</td>
      <td c>1</td>
    </tr>
    <tr>
      <td c>{{ image | sphere_ep }}</td>
      <td c>1</td>
      <td c>0</td>
      <td c>1</td>
      <td c>2</td>
    </tr>
    <tr>
      <td c>{{ image | torus_ep }}</td>
      <td c>1</td>
      <td c>2</td>
      <td c>1</td>
      <td c>0</td>
    </tr>
  </tbody>
</table>

---

Nuestro objetivo es entender la forma de un espacio. ¿Cómo distinguiremos una esfera de un toro? La homología tiene un lema:

**BUSCA ALGO SIN FRONTERA QUE NO SEA LA FRONTERA DE ALGO**

... y curiosamente, ¡funciona! Claro, las cosas que tienen frontera (por ejemplo, curvas sin cerrar) no son muy útiles para encontrar diferencias, se pueden mover demasiado

{{ image | sphere_torus_boundary }}

pero las cosas que no tienen frontera, que están cerradas, quizá nos pueden decir algo más

{{ image | sphere_torus_no_boundary }}

En la esfera, una curva sin frontera es la frontera de algo... y sin embargo en el toro tenemos una curva sin frontera que no es la frontera de nada... ¡ya tenemos una diferencia! ¡Parece que funciona!

{{ image | sphere_torus_is_boundary }}

En general estos objetos sin frontera que no son la frontera de nada capturan "agujeros" de distintas dimensiones... los agujeros de dimensión 0 son componentes separadas, los agujeros de dimensión 1 son rodeables por un lazo, los de dimensión 2 por una superficie...

{{ image | homology }}

Pero muchos podrían rebatir, "¿no es el lazo en el toro la frontera del resto del toro?"

{{ image | torus_loop_boundary }}

Bueno... estamos utilizando el concepto de frontera sin definirlo demasiado... Por eso hay que definir mejor el _operador frontera_ $\partial$

---

Sobre el **operador frontera** $\partial$, vamos por pasos:

<ol>
  <li>
    $\partial$ lleva cosas de dimensión $k$ a dimensión $k-1$, siempre una dimensión menos

    {{ image | boundary_operator_non_oriented }}

    Los objetos de dimensión 0 son puntos, los de dimensión 1 son curvas, los de dimensión 2 son superficies... Al conjunto de "objetos de dimensión $k$" en el espacio $X$ le llamaremos $C_k(X)$, así que lo que tenemos es

    $$\partial:C_k(X)\longrightarrow C_{k-1}(X)$$

    para cada $k\geqslant 0$ (la frontera de un punto es nada, o dicho más algebraicamente, es 0)
  </li>
  <li>
    La frontera de algo ya no tiene frontera (es 0). Es algo de lo que nos podemos convencer con los ejemplos anteriores. Algebraicamente, esto se expresa como

    $$\partial^2=0$$

    una propiedad tan importante y que aparece tanto en matemáticas que da pie al _Álgebra Homológica_
  </li>
  <li>
    Para que todo funcione bien, todos los objetos de dimensión $k$ deben estar _orientados_. El concepto de orientación es delicado; por ahora, para nosotros esto se traducirá que nuestros objetos tienen incorporados una característica que toma dos valores opuestos ("uno el negativo del otro")

    <ul>
      <li>Los puntos estarán etiquetados con $+$ o $-$</li>
      <li>Las curvas tienen una dirección</li>
      <li>Las superficies están pintadas de azul por una cara y de amarillo por la otra; el color azul denota sentido de giro _antihorario_ y el color amarillo giro _horario_</li>
      <li>Los volúmenes tienen una cierta "helicidad"...</li>
    </ul>

    ¡y todo esto se tiene en cuenta para el operador frontera! Una curva comienza en un punto $-$ y acaba en un punto $+$; el giro en las superficies debe coincidir con la dirección de la curva frontera...

    {{ image | boundary_operator }}

    ¿Por qué es importante esto? Para que el operador frontera $\partial$ funcione bien al dividir objetos

    {{ image | boundary_operator_division }}

    ¡Magnífico! Los objetos iguales con distinta orientación actúan como opuestos y se cancelan. Esto hace que todo funcione bien. Además nuestro problema anterior del toro se ha solucionado: si cortamos un toro, cada extremo de la superficie da un borde, pero como éstos tienen orientaciones opuestas, ¡se cancelan!

    {{ image | cut_torus_boundary }}

    Por eso, podemos volver a afirmar: el lazo anterior en el toro no es frontera de nada.
  </li>
</ol>

---

Así que debemos buscar objetos sin frontera que no sean la frontera de algo. En general lo denotaremos con tres letras:

<ul>
  <li>$C$: objetos (con o sin frontera)</li>
  <li>$Z$: objetos sin frontera</li>
  <li>$B$: objetos sin frontera que además son la frontera de algo</li>
</ul>

Y se tiene la inclusión $B\subset Z\subset C$. Aparentemente, nos debemos fijar en el conjunto $Z\smallsetminus B$. ¿Pero es éste el tratamiento más adecuado, el más "matemático"?

Por ejemplo, fijémonos en los enteros $\mathbb{Z}$. Dentro de los enteros hay un fenómeno que es _ser múltiplo de $5$_. Este fenómeno tiene interés precisamente porque hay enteros que _no_ tienen esta propiedad. Es como si $Z=\mathbb{Z}$ y $B=5\mathbb{Z}$ los múltiplos de $5$. Uno puede describir el hecho de que hay números que no son múltiplos de $5$ fijándose en el conjunto

$$Z\smallsetminus B=\{\cdots,-6,-4,-3,-2,-1,1,2,3,4,6,7,8,9,11,12,13,14,\cdots\}$$

Pero para un matemático, trabajar con este conjunto es un poco incómodo. No es cerrado para la suma ($2$ y $3$ están en $Z\smallsetminus B$ pero $2+3=5\not\in Z\smallsetminus B$), no se puede dotar de alguna estructura interesante... En oposición a esto, tomamos otro acercamiento.

$1$ y $6$ son ambos no múltiplos de $5$, y son distintos, pero se puede decir que ambos recogen la misma _no-multiplicidad-de-$5$_, porque en realidad los dos son del tipo $5k+1$. Podemos abstraer el objeto y quedarnos con su _clase_, y diremos que

$$[1]=[6]\qquad\text{ porque }\qquad 1-6\in B=5\mathbb{Z}$$

En ese mismo espíritu, definimos

$$[a]=[b]\qquad\text{ if }\qquad a-b\in B=5\mathbb{Z}$$

Esto nos lleva a distinguir cinco clases, que forman $\mathbb{Z}_5=\{[0],[1],[2],[3],[4]\}$, y que resulta ser un objeto estructuralmente riquísimo, pues con la suma y el producto módulo $5$ no sólo es grupo y anillo sino además _cuerpo finito_. Y esta construcción es estándar en matemáticas: es el cociente $Z/B$.

De tal modo que, también para la homología, el modo correcto de pensar no es con la sustracción $Z\smallsetminus B$, sino con el cociente $Z/B$. Y unos cuantos ejemplos avalarán el acierto de esta construcción

---

Sea $C_k(X)$ el conjunto de los objetos de dimensión $k$ en $X$. Como estamos interesados en un enfoque algebraico, trabajaremos con combinaciones lineales (formales) que podemos sumar y restar fácilmente. Es decir, los elementos de  $C_k(X)$ pueden ser de la forma

{{ image | chains }}

donde $\lambda_i$, $\mu_j$, $\eta_k$ son números enteros. Éstas son _cadenas_. Y contamos con que una "cantidad" negativa de objetos equivale a cambiar la orientación, como se discutía más arriba: intercambiar $-$ y $+$, invertir la dirección de una curva, conmutar azul y amarillo... De modo que el operador frontera $\partial$ se ve mejor como un operador lineal

$$\partial_k:C_k(X)\longrightarrow C_{k-1}(X)$$

que satisface $\partial_{k-1}\circ\partial_k=0$ (o más sucintamente $\partial^2=0$). Esto implica

$$\text{im }\partial_{k+1} \subset\text{ker }\partial_k$$

y tiene sentido definir

$$Z_k(X)=\text{ker }\partial_k$$
$$B_k(X)=\text{im }\partial_{k+1}$$

(llamados _ciclos_ and _fronteras_ respectivamente) y sí, $B_k(X)\subset Z_k(X)\subset C_k(X)$. Y en este contexto, definimos los **grupos de homología**

$$H_k(M)=\dfrac{\text{ker }\partial_k}{\text{im }\partial_{k+1}}=\dfrac{Z_k(M)}{B_k(M)}$$

¿Extraño? Un poco. Pero extremadamente útil. Los grupos de homología están hechos de clases de homología, que aúnan _ciclos homólogos_, es decir, ciclos cuya diferencia es una frontera. Y, en efecto, los ciclos homólogos, esos cuya diferencia es una frontera, son precisamente los que detectan el mismo "agujero". Increíble, ¿no? Tan increíble que ha fascinado y sigue fascinando a todo tipo de científicos durante décadas

{{ image | boundaries }}

---

Vamos a explorar algunos ejemplos concretos de homología. La homología más sencilla de calcular es la homología de orden cero, _que detecta el número de componentes conexas (por caminos)_. ¿Por qué? Para $k=0$, cada elemento de $C_0(X)$ es simplemente una suma entera de puntos en $X$, por ejemplo $\sigma=7p-3q$, $p$, $q\in X$. Los puntos no tienen frontera, por lo que $\partial_0:C_0(X)\longrightarrow 0$ es la aplicación nula y $Z_0(X)=C_0(X)$. Por otro lado, $\partial_1:C_1(X)\longrightarrow C_0(X)$ aplica cada camino abierto a un par de puntos, uno con un signo $+$ y otro con un signo $-$. Y cualquier par de tales puntos pertenece a la imagen de $\partial_1$ siempre y cuando haya algún camino en $X$ desde el punto $-$ al punto $+$, es decir, ¡siempre que estén en la misma componente conexa! Como consecuencia, en $H_0(X)=Z_0(X)/B_0(X)$ tenemos libertad para mover un punto dentro de su componente, como se ve en la imagen de arriba, y también podemos cancelar puntos $+$ y $-$ en la misma componente. Si esto es así, cada clase de homología en $H_0(X)$ asigna un número de puntos neto a cada componente, y por eso $H_0(X)\simeq \mathbb{Z}^n$, donde $n$ es el número de componentes conexas del espacio. Fantástico, ¿verdad?

{{ image | homology_connected_components }}

En esta misma línea, $H_1(X)$ detecta agujeros que se pueden rodear con un lazo. El cociente asegura que lazos distintos rodeando el mismo agujero pertenecen a la misma clase

{{ image | homologous_loops }}

Ahora podemos razonar la homología de espacios sencillos

<table>
  <thead>
    <tr>
      <td c>$X$</td>
      <td c>$H_0(X)$</td>
      <td c>$H_1(X)$</td>
      <td c>$H_2(X)$</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td c>{{ image | point }}</td>
      <td c>$\mathbb{Z}$</td>
      <td c>-</td>
      <td c>-</td>
    </tr>
    <tr>
      <td c>{{ image | curve }}</td>
      <td c>$\mathbb{Z}$</td>
      <td c>0</td>
      <td c>-</td>
    </tr>
    <tr>
      <td c>{{ image | circ }}</td>
      <td c>$\mathbb{Z}$</td>
      <td c>$\mathbb{Z}$</td>
      <td c>-</td>
    </tr>
    <tr>
      <td c>{{ image | disc }}</td>
      <td c>$\mathbb{Z}$</td>
      <td c>0</td>
      <td c>0</td>
    </tr>
    <tr>
      <td c>{{ image | sphere_ep }}</td>
      <td c>$\mathbb{Z}$</td>
      <td c>0</td>
      <td c>$\mathbb{Z}$</td>
    </tr>
    <tr>
      <td c>{{ image | torus_ep }}</td>
      <td c>$\mathbb{Z}$</td>
      <td c>$\mathbb{Z}^2$</td>
      <td c>$\mathbb{Z}$</td>
    </tr>
  </tbody>
</table>

---

Incluso en los espacios más simples, los conjuntos $C_k(X)$, $Z_k(X)$, $B_k(X)$ son normalemente extremadamente grandes. Piensa, por ejemplo, que $C_1(X)$ contiene todas las funciones $f:[0,1]\longrightarrow X$ - eso es _enorme_. Así que hay una versión "más ligera" de la homología, llamada _homología simplicial_ (a la que marcaremos con una $\Delta$), que funciona en espacios triangulados, y que calcula los mismos grupos de homología (bueno, grupos isomorfos). La idea es simple: usa sólo objetos de la triangulación. Luego $C^\Delta_0(X)$ consiste en combinaciones enteras de vértices, $C^\Delta_1(X)$ consiste en combinaciones enteras de aristas orientadas, etcétera. Todo lo demás es igual y funciona perfectamente:

$$\partial^\Delta_k:C^\Delta_k(X)\longrightarrow C^\Delta_{k-1}(X)$$
$$Z^\Delta_k(X)=\text{ker }\partial^\Delta_k$$
$$B^\Delta_k(X)=\text{im }\partial^\Delta_{k+1}$$
$$H^\Delta_k(M)=\dfrac{Z^\Delta_k(M)}{B^\Delta_k(M)}$$

¡Y sí, calcula los mismo grupos de homología, detecta los mismos agujeros! Solo que ahora estamos trabajando con espacios de dimensión finita (suponiendo que la triangulación es finita) que se manejan incomparablemente mejor. Podemos _computar_ los grupos de homología simplicial. Pero como un espacio tiene muchas triangulaciones... nos gustaría tener una homología absoluta, que es la que se describe arriba. Ésta es la _homología singular_, y es una de las construcciones más bellas en matemáticas

Y toda esta digresión vuelve a la característica de Euler-Poincaré. ¿Cómo? Ya que estamos trabajando con espacios vectoriales de dimensión finita (a ver, no son espacios vectoriales, porque estamos trabajando sobre $\mathbb{Z}$, pero no importa - usaremos el rango $\text{rk}$ como el análogo de $\text{dim}$), el álgebra lineal corriente aplica. Por una parte, 

$$H_k=Z_k/B_k\Longrightarrow \text{rk }H_k=\text{rk }Z_k-\text{rk }B_k$$

pero por la otra, 

$$B_{k-1}=\text{im }\partial_k\simeq C_k/\text{ker }\partial_k=C_k/Z_k$$
$$\text{rk }B_{k-1}=\text{rk }C_k-\text{rk }Z_k$$

y esto necesariamente se cumple en toda la cadena

{{ image | homology_chain_dimensions }}

Si insertamos esto en la característica de Euler-Poincaré, tenemos que

$$
\begin{array}{rcl}
\chi & = & \sum_i (-1)^i c_i \\
& = & \sum_i (-1)^i \text{rk }C_i \\
& = & \sum_i (-1)^i (\text{rk }Z_i + \text{rk }B_{i-1}) \\
& & \text{[truco: \(\sum_i (-1)^i\text{rk }B_{i-1} = -\sum_i (-1)^i\text{rk }B_i\)]} \\
& = & \sum_i (-1)^i (\text{rk }Z_i - \text{rk }B_i) \\
& = & \sum_i (-1)^i \text{rk }H_i \\
\end{array}
$$

_Este resultado es muy profundo_: las cantidades $c_i$ dependen de la triangulación elegida en el espacio $X$, pero la característica de Euler-Poincaré $\chi$ _no depende_ de la triangulación, y por tanto constituye un invariante topológico, porque se puede expresar en términos de homología. Y como nota adicional, muestra que la homología, aunque parezca muy extraña al principio, es de una importancia crucial en la topología algebraica