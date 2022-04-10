Calcula el siguiente límite

$$\lim_{n\longrightarrow\infty}\frac{1}{n}\left[\left(\cos\frac{\pi}{2n}\right)^4+\left(\cos\frac{2\pi}{2n}\right)^4+\cdots+\left(\cos\frac{n\pi}{2n}\right)^4\right]$$

+++
Solución
+++

Este límite involucra sumar $n$ cantidades que oscilan entre 0 y 1 (siendo un coseno a la cuarta potencia) y dividir la suma por $n$ - como tomar la media. Por supuesto, la media también debe oscilar entre 0 y 1, pero no está claro si se va a estabilizar conforme $n$ va creciendo.

La clave para este límite es darse cuenta de que esta suma, al multiplicar por $\frac{1}{n}$ cada uno de los términos,

$$\frac{1}{n}\left(\cos\frac{\pi}{2n}\right)^4+\frac{1}{n}\left(\cos\frac{2\pi}{2n}\right)^4+\cdots+\frac{1}{n}\left(\cos\frac{n\pi}{2n}\right)^4$$

es de hecho un múltiplo de la suma de Riemann de la función $f(x)=\cos(x)^4$. Para identificar el intervalo y partición asociados, vamos a rescribir todo en términos de esta función

$$\frac{1}{n}f\left(\frac{\pi}{2n}\right)+\frac{1}{n}f\left(\frac{2\pi}{2n}\right)+\cdots+\frac{1}{n}f\left(\frac{n\pi}{2n}\right)=\frac{1}{n}f(x_1)+\frac{1}{n}f(x_2)+\cdots+\frac{1}{n}f(x_n)$$

con $x_k=\frac{k\pi}{2n}$, $k$ desde $1$ hasta $n$. Estos puntos parecen ajustarse bien al intervalo $\left[0,\frac{\pi}{2}\right]$ con la partición $P=\left\{x_0=0,x_1=\frac{\pi}{2n},x_2=\frac{2\pi}{2n},\cdots,x_n=\frac{n\pi}{2n}\right\}$. Los puntos en esta partición están equiespaciados y la distancia entre puntos es $\frac{\pi}{2n}$ - ¡muy parecido a $\frac{1}{n}$! Así que arreglando todo un poco, si 

$$S_n=\frac{1}{n}\left[\left(\cos\frac{\pi}{2n}\right)^4+\left(\cos\frac{2\pi}{2n}\right)^4+\cdots+\left(\cos\frac{n\pi}{2n}\right)^4\right]=\frac{1}{n}f(x_1)+\frac{1}{n}f(x_2)+\cdots+\frac{1}{n}f(x_n)$$

entonces

$$\frac{\pi}{2}S_n=\frac{\pi}{2n}f(x_1)+\frac{\pi}{2n}f(x_2)+\cdots+\frac{\pi}{2n}f(x_n)$$

es exactamente la suma de Riemann asociada a la partición anterior y usando el extremo derecho. Y por tanto

$$\frac{\pi}{2}S_n\longrightarrow\int_0^{\frac{\pi}{2}}\cos(x)^4=\left[\frac{3}{8}x + \frac{1}{32}\sin(4x) + \frac{1}{4}\sin(2x)\right]_0^{\frac{\pi}{2}}=\frac{3\pi}{16}$$

y reajustando,

$$S_n\longrightarrow \frac{3}{8}$$

+++