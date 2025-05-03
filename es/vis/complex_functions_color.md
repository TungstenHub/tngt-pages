Hay un modo muy interesante de visualizar las funciones complejas. Consiste en lo siguiente: vamos a representar números complejos con colores:

{{ d3js | complex_function data = z }}

Cerca del origen los colores tienden al blanco, y en el resto, los colores del círculo cromático se han distribuido según el argumento del número complejo. Además, se han marcado pequeñas curvas de igual módulo o igual argumento y se ha resaltado el círculo unidad.

Dada una función $f(z)$, podemos visualizarla pintando cada $z$ del plano complejo del color de su imagen $f(z)$. Por ejemplo, la función $f(z) = z^2 - 1$ tendría la siguiente representación

{{ d3js | complex_function data = `z^2 - 1` }}

Como $f(-1) = f(1) = 0$, los puntos $z=-1$, $z=1$ aparecen blancos, pues su imagen es $w=0$ que se corresponde con el blanco. Por otro lado, $z=0$ se pinta de azul, puesto que $f(0) = -1$.