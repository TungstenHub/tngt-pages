Podemos encontrarnos con la integral

$$\int\ln x\dd x$$

y ninguna de las técnicas que hemos aprendido hasta ahora parece funcionar. Pero justamente la [derivada del producto de funciones](thm | derivative_product) va a ser muy útil:

$$(x\ln x)'=(x)'\ln x+x(\ln x)'=1\ln x+x\dfrac{1}{x}=\ln x+1$$

¡que es casi casi lo que necesitamos! De hecho

$$\int\ln x\dd x=\int((x\ln x)'-1)\dd x=x\ln x-x$$

¡Fenomenal! Esta técnica se llama **integración por partes** y funciona así: sean $u(x)$ y $v(x)$ funciones. Sabemos que

$$(uv)'=u'v+uv'$$

así que si nuestro integrando es de la forma $uv'$, podemos cambiarla a una integral completamente diferente, y que quizá con un poco de suerte sea más simple:

$$\int uv'\dd x=\int((uv)'-u'v)\dd x=uv-\int u'v\dd x$$