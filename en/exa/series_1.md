Find the sum of the following series

$$\sum_{n=1}^\infty \frac{1}{1+2+\cdots+n}$$

+++
Solution
+++

First of all let's compute some partial sums to guess about the behaviour of this series

$$\frac{1}{1}+\frac{1}{1+2}=\frac{1}{1}+\frac{1}{3}=\frac{4}{3}\simeq 1.33$$
$$\frac{1}{1}+\frac{1}{1+2}+\frac{1}{1+2+3}=\frac{1}{1}+\frac{1}{3}+\frac{1}{6}=\frac{3}{2}\simeq 1.5$$
$$\frac{1}{1}+\frac{1}{1+2}+\frac{1}{1+2+3}+\frac{1}{1+2+3+4}=\frac{1}{1}+\frac{1}{3}+\frac{1}{6}+\frac{1}{10}=\frac{8}{5}\simeq 1.6$$
$$\frac{1}{1}+\frac{1}{1+2}+\frac{1}{1+2+3}+\frac{1}{1+2+3+4}+\frac{1}{1+2+3+4+5}=\frac{1}{1}+\frac{1}{3}+\frac{1}{6}+\frac{1}{10}+\frac{1}{15}=\frac{5}{3}\simeq 1.66$$
$$
\frac{1}{1}+\frac{1}{1+2}+\frac{1}{1+2+3}+\frac{1}{1+2+3+4}+\frac{1}{1+2+3+4+5}+\frac{1}{1+2+3+4+5+6} = \\
\frac{1}{1}+\frac{1}{3}+\frac{1}{6}+\frac{1}{10}+\frac{1}{15}+\frac{1}{21} = \frac{12}{7}\simeq 1.71
$$

well, it seems to converge! But we have to prove it

The term $a_n=\frac{1}{1+2+\cdots+n}$ is somewhat cumbersome with this increasing sum. Since it is an [arithmetic sum]( lem | arithmetic_sum ), we may simplify it

$$a_n=\frac{1}{1+2+\cdots+n}=\frac{1}{\frac{n(n+1)}{2}}=\frac{2}{n(n+1)}$$

Perfect! But it is not so straightforward to note that 

$$a_n=\frac{2}{n(n+1)}=2\left(\frac{1}{n}-\frac{1}{n+1}\right)$$

but it is true!!

$$a_3=\frac{1}{1+2+3}=\frac{1}{6}=\frac{2}{3\times 4}=2\left(\frac{1}{3}-\frac{1}{4}\right)$$
$$a_7=\frac{1}{1+2+3+4+5+6+7}=\frac{1}{28}=\frac{2}{7\times 8}=2\left(\frac{1}{7}-\frac{1}{8}\right)$$

and this is the key to compute the partial sums exactly because lots of positive and negative terms cancel out:

$$
S_3=a_1+a_2+a_3=2\left(\frac{1}{1}-\frac{1}{2}\right)+2\left(\frac{1}{2}-\frac{1}{3}\right)+2\left(\frac{1}{3}-\frac{1}{4}\right)=2\left(\frac{1}{1}-\frac{1}{4}\right)
$$
$$
S_7=a_1+a_2+a_3+a_4+a_5+a_6+a_7 = \\
2\left(\dfrac{1}{1}-\dfrac{1}{2}\right)+2\left(\dfrac{1}{2}-\dfrac{1}{3}\right)+2\left(\dfrac{1}{3}-\dfrac{1}{4}\right)+2\left(\dfrac{1}{4}-\dfrac{1}{5}\right)+2\left(\dfrac{1}{5}-\dfrac{1}{6}\right)+2\left(\dfrac{1}{6}-\dfrac{1}{7}\right)+2\left(\dfrac{1}{7}-\dfrac{1}{8}\right) = \\
2\left(\dfrac{1}{1}-\dfrac{1}{8}\right)
$$

and in general

$$S_m=\sum_{n=1}^m \frac{1}{1+2+\cdots+n}=2\left(1-\frac{1}{m+1}\right)$$

and when $m$ tends to infinity, the last term vanishes, so

$$\sum_{n=1}^\infty \frac{1}{1+2+\cdots+n}=2$$

Mathematical Software is helpful too:

```sage
k, n = var('k n');
sum(1/(sum(k,k,1,n)), n, 1, oo)
```

```sage
n = var('n');
sum(2/(n*(n+1)), n, 1, oo)
```

+++