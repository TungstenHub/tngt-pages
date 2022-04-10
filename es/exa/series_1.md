Encuentra la suma de la siguiente serie

$$\sum_{n=1}^\infty \frac{1}{1+2+\cdots+n}$$

+++
Solución
+++

En primer lugar vamos a calcular algunas sumas parciales para entrever cómo se comporta esta serie

$$\frac{1}{1}+\frac{1}{1+2}=\frac{1}{1}+\frac{1}{3}=\frac{4}{3}\simeq 1.33$$
$$\frac{1}{1}+\frac{1}{1+2}+\frac{1}{1+2+3}=\frac{1}{1}+\frac{1}{3}+\frac{1}{6}=\frac{3}{2}\simeq 1.5$$
$$\frac{1}{1}+\frac{1}{1+2}+\frac{1}{1+2+3}+\frac{1}{1+2+3+4}=\frac{1}{1}+\frac{1}{3}+\frac{1}{6}+\frac{1}{10}=\frac{8}{5}\simeq 1.6$$
$$\frac{1}{1}+\frac{1}{1+2}+\frac{1}{1+2+3}+\frac{1}{1+2+3+4}+\frac{1}{1+2+3+4+5}=\frac{1}{1}+\frac{1}{3}+\frac{1}{6}+\frac{1}{10}+\frac{1}{15}=\frac{5}{3}\simeq 1.66$$
$$
\frac{1}{1}+\frac{1}{1+2}+\frac{1}{1+2+3}+\frac{1}{1+2+3+4}+\frac{1}{1+2+3+4+5}+\frac{1}{1+2+3+4+5+6} = \\
\frac{1}{1}+\frac{1}{3}+\frac{1}{6}+\frac{1}{10}+\frac{1}{15}+\frac{1}{21} = \frac{12}{7}\simeq 1.71
$$

Bueno, ¡parece que converge! Pero tenemos que probarlo

El término $a_n=\frac{1}{1+2+\cdots+n}$ es un poco armatoste dentro de esta suma creciente. Pero como es una [suma aritmética]( lem | arithmetic_sum ), la podemos simplificar

$$a_n=\frac{1}{1+2+\cdots+n}=\frac{1}{\frac{n(n+1)}{2}}=\frac{2}{n(n+1)}$$

¡Perfecto! Y ya no es tan directo notar que

$$a_n=\frac{2}{n(n+1)}=2\left(\frac{1}{n}-\frac{1}{n+1}\right)$$

¡pero es verdad!

$$a_3=\frac{1}{1+2+3}=\frac{1}{6}=\frac{2}{3\times 4}=2\left(\frac{1}{3}-\frac{1}{4}\right)$$
$$a_7=\frac{1}{1+2+3+4+5+6+7}=\frac{1}{28}=\frac{2}{7\times 8}=2\left(\frac{1}{7}-\frac{1}{8}\right)$$

y es la clave para calcular estas sumas parciales precisamente porque mogollón de términos positivos y negativos se cancelan:

$$
S_3=a_1+a_2+a_3=2\left(\frac{1}{1}-\frac{1}{2}\right)+2\left(\frac{1}{2}-\frac{1}{3}\right)+2\left(\frac{1}{3}-\frac{1}{4}\right)=2\left(\frac{1}{1}-\frac{1}{4}\right)
$$
$$
S_7=a_1+a_2+a_3+a_4+a_5+a_6+a_7 = \\
2\left(\dfrac{1}{1}-\dfrac{1}{2}\right)+2\left(\dfrac{1}{2}-\dfrac{1}{3}\right)+2\left(\dfrac{1}{3}-\dfrac{1}{4}\right)+2\left(\dfrac{1}{4}-\dfrac{1}{5}\right)+2\left(\dfrac{1}{5}-\dfrac{1}{6}\right)+2\left(\dfrac{1}{6}-\dfrac{1}{7}\right)+2\left(\dfrac{1}{7}-\dfrac{1}{8}\right) = \\
2\left(\dfrac{1}{1}-\dfrac{1}{8}\right)
$$

y en general

$$S_m=\sum_{n=1}^m \frac{1}{1+2+\cdots+n}=2\left(1-\frac{1}{m+1}\right)$$

y cuando $m$ tiende a infinito, el último término desaparece, con lo que

$$\sum_{n=1}^\infty \frac{1}{1+2+\cdots+n}=2$$

Y el software matemático también nos echa un cable:

```sage
k, n = var('k n');
sum(1/(sum(k,k,1,n)), n, 1, oo)
```

```sage
n = var('n');
sum(2/(n*(n+1)), n, 1, oo)
```

+++