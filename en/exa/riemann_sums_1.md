Compute the following limit

$$\lim_{n\longrightarrow\infty}\frac{1}{n}\left[\left(\cos\frac{\pi}{2n}\right)^4+\left(\cos\frac{2\pi}{2n}\right)^4+\cdots+\left(\cos\frac{n\pi}{2n}\right)^4\right]$$

+++
Solution
+++

This limit involves summing up $n$ quantities that range between 0 and 1 (being the cosine to the fourth power) and dividing the sum by $n$ - like taking the average. Now the average must range between 0 and 1 too, but it is not clear whether it becomes stable as $n$ grows bigger and bigger.

The key for this limit is to realize that this sum, when multiplying $\frac{1}{n}$ to all the terms,

$$\frac{1}{n}\left(\cos\frac{\pi}{2n}\right)^4+\frac{1}{n}\left(\cos\frac{2\pi}{2n}\right)^4+\cdots+\frac{1}{n}\left(\cos\frac{n\pi}{2n}\right)^4$$

is indeed a multiple of the Riemann sum for the function $f(x)=\cos(x)^4$. To identify the associated interval and partition, let's rewrite everything in terms of this function

$$\frac{1}{n}f\left(\frac{\pi}{2n}\right)+\frac{1}{n}f\left(\frac{2\pi}{2n}\right)+\cdots+\frac{1}{n}f\left(\frac{n\pi}{2n}\right)=\frac{1}{n}f(x_1)+\frac{1}{n}f(x_2)+\cdots+\frac{1}{n}f(x_n)$$

with $x_k=\frac{k\pi}{2n}$, $k$ from $1$ to $n$. These points seem to fit nicely into the interval $\left[0,\frac{\pi}{2}\right]$ with the partition $P=\left\{x_0=0,x_1=\frac{\pi}{2n},x_2=\frac{2\pi}{2n},\cdots,x_n=\frac{n\pi}{2n}\right\}$. The points in this partition are equally spaced and the distance between points is $\frac{\pi}{2n}$ - very similar to $\frac{1}{n}$! So tidying up everything, if 

$$S_n=\frac{1}{n}\left[\left(\cos\frac{\pi}{2n}\right)^4+\left(\cos\frac{2\pi}{2n}\right)^4+\cdots+\left(\cos\frac{n\pi}{2n}\right)^4\right]=\frac{1}{n}f(x_1)+\frac{1}{n}f(x_2)+\cdots+\frac{1}{n}f(x_n)$$

then

$$\frac{\pi}{2}S_n=\frac{\pi}{2n}f(x_1)+\frac{\pi}{2n}f(x_2)+\cdots+\frac{\pi}{2n}f(x_n)$$

is exactly the Riemann sum associated to the partition mentioned before and using the right endpoint. And therefore

$$\frac{\pi}{2}S_n\longrightarrow\int_0^{\frac{\pi}{2}}\cos(x)^4=\left[\frac{3}{8}x + \frac{1}{32}\sin(4x) + \frac{1}{4}\sin(2x)\right]_0^{\frac{\pi}{2}}=\frac{3\pi}{16}$$

and readjusting,

$$S_n\longrightarrow \frac{3}{8}$$

+++