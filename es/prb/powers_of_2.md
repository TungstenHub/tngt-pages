Consider the powers of $2$:

$$
\begin{array}{rcl}
2^1 & = & 2\\
2^2 & = & 4\\
2^3 & = & 8\\
2^4 & = & 16\\
2^5 & = & 32\\
2^6 & = & 64\\
2^7 & = & 128\\
2^8 & = & 256\\
2^9 & = & 512\\
2^{10} & = & 1024\\
\end{array}
$$
$$\cdots$$

They always end in $2$, $4$, $6$ or $8$, but we know little about their beginnings

<ol>
<li>Is there a power of $2$ starting with $9$?</li>
<li>Is there a power of $2$ starting with $9999\cdots 9999$ ($99$ nines)?</li>
<li>When considering more and more powers of $2$, which is the average of powers starting with $9$ in the limit?</li>
</ol>

+++
Solution
+++

<ol>
  <li>
    There are powers of $2$ starting with $9$, for instance $2^{53} = 9007199254740992$
  </li>
  <li>
    Now we can't proceed by direct inspection, because humongous numbers are involved... The right direction to prove that there are powers of $2$ starting with $9999\cdots 9999$ ($99$ nines) is to work with logarithms to the base $10$ (denoted $\log$): if some power starts with $9999\cdots 9999$ 

    $$2^n=9999\cdots 9999\cdots\cdots\cdots$$

    then

    $$n\log 2=\log(2^n)=\log(9999\cdots 9999\cdots\cdots\cdots)=\log(9.999\cdots 9999\cdots\cdots\cdots)+m$$

    where $m$ is the number of digits of $9999\cdots 9999\cdots\cdots\cdots$ minus $1$. Considering the fractional part,

    $$\{n\log 2\}=\log(9.999\cdots\cdots\cdots)$$

    that is, we're looking for some $n$ that satisfies

    $$\log(9.999\cdots 9999)\leqslant\{n\log 2\}\lt\log(10)=1$$

    and this is possible, because $\log 2$ is an irrational number (check it out! $2^q\neq 10^p$ for positive integers $p$ and $q$)! And this ensures that the fractional parts of $n\log 2$ are _dense_ in the interval [0,1]: one may find arbitrarily close elements of this set to any given number $0\leqslant x\leqslant 1$. So we only have to wait for some $\{n\log 2\}$ to fall into $[\log(9.999\cdots 9999),1)$; we will have to wait a lot, sure, but there will be such powers

    {{ image | log_2_unity }}

    And with the same argument, we find out that _there are powers of $2$ starting with any given finite sequence of numbers_. Cool, isn't it?

  </li>
  <li>
    Since in the limit the values $\{n\log 2\}$ are equally distributed in the interval $[0,1]$, the average of powers starting with $9$ is

    $$\log 10-\log 9\simeq 0.0458$$

    That's quite interesting: there are powers of $2$ starting with any number, but bigger numbers appear _less_. Had you ever thought about it?
  </li>
</ol>

+++