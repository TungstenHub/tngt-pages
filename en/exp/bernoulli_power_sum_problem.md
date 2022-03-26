Have you ever tried to compute the sum of the $n$ first $p$ powers? 

$$S=1^p+2^p+3^p+\cdots+n^p$$

For instance, we already know that

$$1+2+3+\cdots+n=\dfrac{n(n+1)}{2}$$
$$1^2+2^2+3^2+\cdots+n^2=\dfrac{1}{6}n(n+1)(2n+1)$$
$$1^3+2^3+3^3+\cdots+n^3=\left(\dfrac{n(n+1)}{2}\right)^2$$

But what happens with larger values of $p$? Well, the Swiss mathematician Jacob Bernoulli found out a "nearly-closed" formula, using an extremely curious idea. Ready? It all has to do with a _magic_ quantity called $B$ 

For now, we will assume $B$ is just a plain number, and so will be $a$. According to the [binomial expansion]( thm | binomial_expansion ), 

$$(a+B)^q=a^q+qa^{q-1}B+\binom{q}{2}a^{q-2}B^2+\binom{q}{3}a^{q-3}B^3+\cdots$$

for $q$ some positive integer. In our case we'll need $q=p+1$, so

$$(a+B)^q=a^q+qa^pB+\binom{q}{2}a^{p-1}B^2+\binom{q}{3}a^{p-2}B^3+\cdots$$

and in the same way,

$$(a+B-1)^q=a^q+qa^p(B-1)+\binom{q}{2}a^{p-1}(B-1)^2+\binom{q}{3}a^{p-2}(B-1)^3+\cdots$$

Substracting these two quantities leads to

$$(a+B)^q-(a+B-1)^q=qa^p+\binom{q}{2}a^{p-1}\left[B^2-(B-1)^2\right]+\binom{q}{3}a^{p-2}\left[B^3-(B-1)^3\right]+\cdots$$

This is very interesting: if we temporarily forget about the terms having $B$, we have

$$(a+B)^q-(a+B-1)^q\simeq qa^p$$

and this resembles a lot a telescopic sum! That is, the sum $S=1^p+2^p+3^p+\cdots+n^p$ would be nearly straightforward to compute. But the fact is that we cannot forget about the terms having $B$. And there is no quantity $B$ that simultaneously satisfies 

$$B^2-(B-1)^2=0$$
$$B^3-(B-1)^3=0$$
$$B^4-(B-1)^4=0$$
$$B^5-(B-1)^5=0$$
$$...$$

so instead, our quantity $B$ will be a _magic_ quantity, such that _all_ previous statements hold

The previous structure containing $a$ and $B$ is very helpful for us to some extent, but after that we will manipulate the quantity $B$. The manipulation will be as follows: after expanding the binomials, the powers of $B$ will be replaced by some other quantities

$$B^m\leadsto B_m$$

which will be carefully chosen for everything to work nice. We will denote this trick like this

$$\check{\overline{expression}}$$

For instance,

$$\check{\overline{(1+B)^5}}=\check{\overline{1+5B+10B^2+10B^3+5B^4+B^5}}=1+5B_1+10B_2+10B_3+5B_4+B_5$$

With this trick, we would have

$$\check{\overline{(a+B)^q}}=a^q+qa^p\check{\overline{B}}+\binom{q}{2}a^{p-1}\check{\overline{B^2}}+\binom{q}{3}a^{p-2}\check{\overline{B^3}}+\cdots$$
$$\check{\overline{(a+B-1)^q}}=a^q+qa^p\check{\overline{(B-1)}}+\binom{q}{2}a^{p-1}\check{\overline{(B-1)^2}}+\binom{q}{3}a^{p-2}\check{\overline{(B-1)^3}}+\cdots$$

and also

$$\check{\overline{(a+B)^q}}-\check{\overline{(a+B-1)^q}}=qa^p+\binom{q}{2}a^{p-1}\left[\check{\overline{B^2}}-\check{\overline{(B-1)^2}}\right]+\binom{q}{3}a^{p-2}\left[\check{\overline{B^3}}-\check{\overline{(B-1)^3}}\right]+\cdots$$

and supposing that we're clever enough to find coefficients $B_m$ for which

$$\check{\overline{B^k}}-\check{\overline{(B-1)^k}}=0\qquad \forall\,k$$

then

$$\check{\overline{(a+B)^q}}-\check{\overline{(a+B-1)^q}}=qa^p$$

and also

$$
\begin{array}{rcl}
\check{\overline{(1+B)^q}}-\check{\overline{(1+B-1)^q}} & = & q\cdot 1^p \\
\check{\overline{(2+B)^q}}-\check{\overline{(2+B-1)^q}} & = & q\cdot 2^p \\
\check{\overline{(3+B)^q}}-\check{\overline{(3+B-1)^q}} & = & q\cdot 3^p \\
& \vdots & \\
\check{\overline{(n+B)^q}}-\check{\overline{(n+B-1)^q}} & = & q\cdot n^p \\
\end{array}
$$

so that

$$\check{\overline{(n+B)^q}}-\check{\overline{B^q}}=qS$$

and finally

$$1^p+2^p+3^p+\cdots+n^p=\dfrac{\check{\overline{(n+B)^q}}-\check{\overline{B^q}}}{q}$$

Yeah!! Now let's determine these mysterious coefficients $B_m$:

$$
\begin{array}{rccl}
\check{\overline{B^2}}-\check{\overline{(B-1)^2}} & = && \\
\check{\overline{B^2}}-\check{\overline{B^2-2B+1}} & = && \\
B_2-(B_2-2B_1+1) & = & 0 & \Longrightarrow B_1=\dfrac{1}{2} \\\\
\check{\overline{B^3}}-\check{\overline{(B-1)^3}} & = && \\
\check{\overline{B^3}}-\check{\overline{B^3-3B^2+3B-1}} & = && \\
B_3-(B_3-3B_2+3B_1-1) & = && \\
3B_2-3B_1+1 & = & 0 & \Longrightarrow B_2=\dfrac{1}{3}(3B_1-1)=\dfrac{1}{6}\\\\
\check{\overline{B^4}}-\check{\overline{(B-1)^4}} & = && \\
\check{\overline{B^4}}-\check{\overline{B^4-4B^3+6B^2-4B+1}} & = && \\
B_4-(B_4-4B_3+6B_2-4B_1+1) & = && \\
4B_3-6B_2+4B_1-1 & = & 0 & \Longrightarrow B_3=\dfrac{1}{4}(6B_2-4B_1+1)=0\\\\
&& \cdots & \Longrightarrow B_4=-\dfrac{1}{30}\\\\
&& \cdots & \Longrightarrow B_5=0\\\\
&& \cdots & \Longrightarrow B_6=\dfrac{1}{42}\\\\
&& \cdots & \Longrightarrow B_7=0\\\\
&& \vdots &
\end{array}
$$

If you think this may be a very important sequence in mathematics, you're right! These are the **Bernoulli numbers** and are of crucial importance in Number Theory. And yes, odd coefficients other than $B_1$ are zero! Can you see why? 

To end with, let's calculate some of these sums! $p=1$: 

$$
\begin{array}{rcl}
1+2+3+\cdots+n & = & \dfrac{\check{\overline{(n+B)^2}}-\check{\overline{B^2}}}{2}\\\\
& = & \dfrac{\check{\overline{n^2+2nB+B^2}}-\check{\overline{B^2}}}{2}\\\\
& = & \dfrac{n^2+2nB_1+B_2-B_2}{2}\\\\
& = & \dfrac{n^2+2n\frac{1}{2}}{2}\\\\
& = & \dfrac{n(n+1)}{2}
\end{array}
$$

$p=2$: 

$$
\begin{array}{rcl}
1^2+2^2+3^2+\cdots+n^2 & = & \dfrac{\check{\overline{(n+B)^3}}-\check{\overline{B^3}}}{3}\\\\
& = & \dfrac{\check{\overline{n^3+3n^2B+3nB^2+B^3}}-\check{\overline{B^3}}}{3}\\\\
& = & \dfrac{n^3+3n^2B_1+3nB_2+B_3-B_3}{3}\\\\
& = & \dfrac{n^3+3n^2\frac{1}{2}+3n\frac{1}{6}}{3}\\\\
& = & \dfrac{2n^3+3n^2+n}{6}\\\\
& = & \dfrac{1}{6}n(n+1)(2n+1)
\end{array}
$$

$p=3$: 

$$
\begin{array}{rcl}
1^3+2^3+3^3+\cdots+n^3 & = & \dfrac{\check{\overline{(n+B)^4}}-\check{\overline{B^4}}}{4}\\\\
& = & \dfrac{\check{\overline{n^4+4n^3B+6n^2B^2+4nB^3+B^4}}-\check{\overline{B^4}}}{4}\\\\
& = & \dfrac{n^4+4n^3B_1+6n^2B_2+4nB_3+B_4-B_4}{4}\\\\
& = & \dfrac{n^4+4n^3\frac{1}{2}+6n^2\frac{1}{6}+4n\cdot 0}{4}\\\\
& = & \dfrac{n^4+2n^3+n^2}{4}\\\\
& = & \left(\dfrac{n(n+1)}{2}\right)^2
\end{array}
$$

which leads to the well-known identity

$$1^3+2^3+3^3+\cdots+n^3=(1+2+3+\cdots+n)^2$$

$p=4$: 

$$
\begin{array}{rcl}
1^4+2^4+3^4+\cdots+n^4 & = & \dfrac{\check{\overline{(n+B)^5}}-\check{\overline{B^5}}}{5}\\\\
& = & \dfrac{\check{\overline{n^5+5n^4B+10n^3B^2+10n^2B^3+5nB^4+B^5}}-\check{\overline{B^5}}}{5}\\\\
& = & \dfrac{n^5+5n^4B_1+10n^3B_2+10n^2B_3+5nB_4+B_5-B_5}{5}\\\\
& = & \dfrac{n^5+5n^4\frac{1}{2}+10n^3\frac{1}{6}+10n^2\cdot 0+5n\left(-\frac{1}{30}\right)}{5}\\\\
& = & \dfrac{6n^5+15n^4+10n^3-n}{30}\\\\
& = & \dfrac{1}{30}n(n+1)(2n+1)(3n^2+3n+1)
\end{array}
$$