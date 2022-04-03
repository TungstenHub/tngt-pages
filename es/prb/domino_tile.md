¿Se puede embaldosar con fichas de dominó de $2\times 1$ una cuadrícula de $10\times 10$ a la que se le han quitado las piezas superior izquierda e inferior derecha? Si no, ¿por qué?

{{ image | domino_tile }}

+++
Solución
+++

Este problema es realmente interesante y agudo. Aunque parezca muy sencillo, después de probar unas cuantas veces se comienza a sospechar que ningún embaldosado sirve para el tablero descrito - siempre quedan al menos dos casillas vacías. De hecho, no es posible embaldosar este tablero con fichas de dominó. ¿Pero cómo probarlo? Intentar todas las combinaciones es sencillamente descabellado

Hay un argumento sorprendentemente simple y efectivo: pintar el tablero de blanco y negro, como si fuera de ajedrez. Cada pieza de dominó cubre una casilla blanca y otra negra. Pero las casillas que se han quitado son del mismo color, por lo que _nuestro tablero tiene un número distinto de casillas blancas y negras_. Y por eso no podemos embaldosar el tablero

{{ image | domino_tile_chess }}

+++