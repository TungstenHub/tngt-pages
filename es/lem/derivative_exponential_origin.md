$$<<< \lim_{h\longrightarrow 0} \dfrac{e^h-1}{h}=1 $$

+++
Demostración
+++

$$<<< \dfrac{(e^h-1)}{h}=\dfrac{\left(\lim_{n\longrightarrow\infty}\left(1+\dfrac{h}{n}\right)^n-1\right)}{h} $$

Analicemos la potencia. Por la [expansión binomial]( thm | binomial_expansion )

$$ 
\begin{array}{l}
\left(1+\dfrac{h}{n}\right)^n
\\ \qquad
= 1+n\dfrac{h}{n}+\binom{n}{2}\dfrac{h^2}{n^2}+\cdots
\\ \qquad
= 1+h+h^2\left(\binom{n}{2}\dfrac{1}{n^2}+\binom{n}{3}\dfrac{h}{n^3}+\cdots\right)
\\ \qquad
= 1+h+h^2\alpha_{nh}
\end{array}
$$ 

donde $\alpha_{nh}$ es una cantidad que depende de $n$ y $h$. 

Cuando $n\longrightarrow\infty$, la cantidad $e^h=\lim_{n\longrightarrow\infty}\left(1+\dfrac{h}{n}\right)^n$ se hace estable y por tanto $\alpha_{nh}$ se estabiliza a una cantidad estable $\alpha_h$, y se cumple $e^h=1+h+h^2\alpha_h$. Pero $\alpha_h$ también es estable cuando $h\longrightarrow 0$, pues ya eran estables los $\alpha_{nh}$, que tenían potencias de $h$. El hecho de que $\alpha_h$ sea estable cuando $h\longrightarrow 0$ implica que $h\alpha_h\longrightarrow 0$ (algo que tiende a cero multiplicado por algo que no se mueve mucho es algo que tiende a cero) y por tanto

$$<<< \lim_{h\longrightarrow 0}\dfrac{e^h-1}{h}=\lim_{h\longrightarrow 0}\dfrac{1+h+h^2\alpha_h-1}{h}=\lim_{h\longrightarrow 0} 1+h\alpha_h=1 $$

+++