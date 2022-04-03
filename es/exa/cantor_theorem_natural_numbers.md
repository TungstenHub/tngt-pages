Alice y Bob están discutiendo sobre cuán grande es $\mathcal{P}(\N)$, es decir, la colección de todos los subconjuntos de los números naturales. Cuanto más piensan en ello, más cuenta se dan de que esta colección ¡es realmente grande! Se les ocurren ejemplos y ejemplos de subconjuntos de $\N$:

<ul>
  <li>Los números pares: $2 \N=\{0,2,4,6,8,10,12,14,...\}$</li>
  <li>Los números entre 50 y 83: $[50,83]=\{50, 51, 52,...,81, 82,83\}$</li>
  <li>El subconjunto vacío: $\varnothing=\{\}$</li>
  <li>Los números primos: $Primo=\{2,3,5,7,11,13,17,19,23,29,31,...\}$</li>
  <li>La edad de Bob (¡un solo elemento!): $EdadBob=\{14\}$</li>
  <li>Los números no primos: $NoPrimo=\{0,1,4,6,8,9,10,12,14,15,16,18,20,21,22,24,25,26,27,28,30,32,...\}$</li>
  <li>El conjunto de los números de la suerte entre los amigos de Alice y Bob: $NumerosSuerte=\{3,4,5,6,7,12,13,16,99,777,12345\}$</li>
  <li>¡Todos los números! $\N=\{0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,...\}$</li>
  <li>Las potencias de $2$: $Potencias2=\{1,2,4,8,16,32,64,128,256,512,1024,...\}$</li>
  <li> ... y más ...</li>
</ul>

Alice y Bob se preguntan si esta colección es _numerable_, es decir, si uno podría de modo hipotético escribir todos los subconjuntos de  $\N$ en una lista sin dejarse ninguno sin incluir. Alice tiende a pensar que no es posible; Bob, por el otro lado, está seguro de que esta colección es numerable y dice que además está pensando en una estrategia para conseguir este orden

"¿Ah sí? ¡Pues muéstramelo!" - dice Alice 

Y Bob toma un trozo de papel y empieza a escribir

$$2 \N=\{0,2,4,6,8,10,12,14,...\}$$
$$[50,83]=\{50, 51, 52,...,81, 82,83\}$$
$$\varnothing=\{\}$$
$$Primo=\{2,3,5,7,11,13,17,19,23,29,31,...\}$$
$$EdadBob=\{14\}$$
$$NoPrimo=\{0,1,4,6,8,9,10,12,14,15,16,18,20,21,22,24,25,26,27,28,30,32,...\}$$
$$NumerosSuerte=\{3,4,5,6,7,12,13,16,99,777,12345\}$$
$$\N=\{0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,...\}$$
$$Potencias2=\{1,2,4,8,16,32,64,128,256,512,1024,...\}$$
$$...$$
$$...$$
$$...$$

"Uff, esto va a ser muy pesado" - piensa Alice. No confía mucho en que Bob sea capaz de escribir infinitos elementos en un trozo de papel... e incluso cuando pudiese, ella no iría a repasar la lista infinita para comprobar que no se ha dejado ningún subconjunto de $\N$. "Tiene que haber un modo más elegante"

Y recuerda - el [Teorema de Cantor]( thm | cantor_theorem ). ¿Cómo se le ha podido pasar?

En efecto, al intentar enumerar todos los subconjuntos de $\N$, Bob está construyendo una función $g:\N\longrightarrow\mathcal{P}(\N)$. Todavía no ha terminado, pero dice que tiene una regla con la que enumerar todo

<table>
  <thead>
    <tr>
      <td>$a$</td>
      <td>$g(a)$</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>$0$</td>
      <td>$2 \N=\{0,2,4,6,8,10,12,14,...\}$</td>
    </tr>
    <tr>
      <td>$1$</td>
      <td>$[50,83]=\{50, 51, 52,...,81, 82,83\}$</td>
    </tr>
    <tr>
      <td>$2$</td>
      <td>$\varnothing=\{\}$</td>
    </tr>
    <tr>
      <td>$3$</td>
      <td>$Primo=\{2,3,5,7,11,13,17,19,23,29,31,...\}$</td>
    </tr>
    <tr>
      <td>$4$</td>
      <td>$EdadBob=\{14\}$</td>
    </tr>
    <tr>
      <td>$5$</td>
      <td>$NoPrimo=\{0,1,4,6,8,9,10,12,14,15,16,18,20,21,22,24,25,26,27,28,30,32,...\}$</td>
    </tr>
    <tr>
      <td>$6$</td>
      <td>$NumerosSuerte=\{3,4,5,6,7,12,13,16,99,777,12345\}$</td>
    </tr>
    <tr>
      <td>$7$</td>
      <td>$\N=\{0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,...\}$</td>
    </tr>
    <tr>
      <td>$8$</td>
      <td>$Potencias2=\{1,2,4,8,16,32,64,128,256,512,1024,...\}$</td>
    </tr>
    <tr>
      <td>$...$</td>
      <td>$...$</td>
    </tr>
    <tr>
      <td>$...$</td>
      <td>$...$</td>
    </tr>
    <tr>
      <td>$...$</td>
      <td>$...$</td>
    </tr>
  </tbody>
</table>

y según el Teorema de Cantor, $g$ nunca será sobreyectiva, es decir, ¡Bob no va a ser capaz de enumerar _todos_ los subconjuntos de $\N$! ¡Ella tiene razón! Venga, vamos a seguir el argumento de la prueba de Cantor.

Entre los números naturales, algunos pertenecen a su subconjunto asociado, pero otros no

<table>
  <thead>
    <tr>
      <td>$a$</td>
      <td>$g(a)$</td>
      <td c>$a\in g(a)$</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>$0$</td>
      <td>$2 \mathbb{N}=\{\hl{0},2,4,6,8,10,12,14,...\}$</td>
      <td c>::check::</td>
    </tr>
    <tr>
      <td>$1$</td>
      <td>$[50,83]=\{50, 51, 52,...,81, 82,83\}$</td>
      <td c>::cross::</td>
    </tr>
    <tr>
      <td>$2$</td>
      <td>$\varnothing=\{\}$</td>
      <td c>::cross::</td>
    </tr>
    <tr>
      <td>$3$</td>
      <td>$Primo=\{2,\hl{3},5,7,11,13,17,19,23,29,31,...\}$</td>
      <td c>::check::</td>
    </tr>
    <tr>
      <td>$4$</td>
      <td>$EdadBob=\{14\}$</td>
      <td c>::cross::</td>
    </tr>
    <tr>
      <td>$5$</td>
      <td>$NoPrimo=\{0,1,4,6,8,9,10,12,14,15,16,18,20,21,22,24,25,26,27,28,30,32,...\}$</td>
      <td c>::cross::</td>
    </tr>
    <tr>
      <td>$6$</td>
      <td>$NumerosSuerte=\{3,4,5,\hl{6},7,12,13,16,99,777,12345\}$</td>
      <td c>::check::</td>
    </tr>
    <tr>
      <td>$7$</td>
      <td>$\mathbb{N}=\{0,1,2,3,4,5,6,\hl{7},8,9,10,11,12,13,14,15,...\}$</td>
      <td c>::check::</td>
    </tr>
    <tr>
      <td>$8$</td>
      <td>$Potencias2=\{1,2,4,\hl{8},16,32,64,128,256,512,1024,...\}$</td>
      <td c>::check::</td>
    </tr>
    <tr>
      <td>$...$</td>
      <td>$...$</td>
      <td c>::question_mark::</td>
    </tr>
    <tr>
      <td>$...$</td>
      <td>$...$</td>
      <td c>::question_mark::</td>
    </tr>
    <tr>
      <td>$...$</td>
      <td>$...$</td>
      <td c>::question_mark::</td>
    </tr>
  </tbody>
</table>

Así que nos tenemos que centrar en el conjunto de los "números rojos"

$$\color{#DD2C00}{B=\{1,2,4,5,...\}}$$

"¡Bob! ¡Sé que este subconjunto no está en tu lista!"

Bob puso los ojos en blanco - "¿Cómo lo sabes, si ni siquiera he terminado?"

Pero Alice le explica el argumento. "Imagina que $B$ está en la lista, como la imagen de algún número $b$. En ese caso, $b$ es un _número verde_ o un _número rojo_?"

<table>
  <tr>
    <td>$b$</td>
    <td>$B=\{1,2,4,5,...,\mathbf{\color{#00C853}{b}},...\}$</td>
    <td>::check::</td>
  </tr>
  <tr>
    <td>$b$</td>
    <td>$B=\{1,2,4,5,...\}$</td>
    <td>::cross::</td>
  </tr>
</table>

"¡No puede ser ninguno, porque $B$ es exactamente el conjunto de los números rojos!" dijo Alice. "¿No es ingenioso?"

"¡Ostras, tienes razón!", dijo finalmente Bob...