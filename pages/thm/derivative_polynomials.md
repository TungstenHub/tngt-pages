[{constant}]

$$<<< (c)'=0 $$

+++
Proof
+++

$$<<< 
f(x)=c \\
\lim_{h\longrightarrow 0}\dfrac{f(x+h)-f(x)}{h}=\lim_{h\longrightarrow 0}\dfrac{c-c}{h}=\lim_{h\longrightarrow 0} 0 = 0
$$

+++

---
[{linear}]

$$<<< (x)'=1 $$

+++
Proof
+++

$$<<< 
f(x)=x \\
\lim_{h\longrightarrow 0}\dfrac{f(x+h)-f(x)}{h}=\lim_{h\longrightarrow 0}\dfrac{(x+h)-x}{h}=\lim_{h\longrightarrow 0} 1 = 1
$$

+++

---
[{square}]

$$<<< (x^2)'=2x $$

+++
Proof
+++

$$<<< 
f(x)=x^2 \\
\lim_{h\longrightarrow 0}\dfrac{f(x+h)-f(x)}{h} 
\\ \qquad
= \lim_{h\longrightarrow 0}\dfrac{(x+h)^2-x^2}{h}
\\ \qquad
= \displaystyle\lim_{h\longrightarrow 0} \dfrac{x^2+2xh+h^2-x^2}{h}
\\ \qquad 
= \lim_{h\longrightarrow 0} 2x+h 
\\ \qquad
= 2x
$$

+++

---
[{poly}]

$$<<< (x^n)'=nx^{n-1} $$

+++
Proof
+++

$$<<< f(x)=x^n $$  

According to the [binomial expansion]( thm | binomial_expansion )

$$ (x+h)^n=x^n+nx^{n-1}h+\binom{n}{2}x^{n-1}h^2+\cdots+\binom{n}{n-2}x^2h^{n-2}+nxh^{n-1}+h^n $$  

So  

$$<<< 
\lim_{h\longrightarrow 0}\dfrac{f(x+h)-f(x)}{h}
\\ \qquad
= \lim_{h\longrightarrow 0}\dfrac{(x+h)^n-x^n}{h}
\\ \qquad
= \lim_{h\longrightarrow 0}\dfrac{x^n+nx^{n-1}h+\binom{n}{2}x^{n-1}h^2+\cdots+\binom{n}{n-2}x^2h^{n-2}+nxh^{n-1}+h^n-x^n}{h}
\\ \qquad
= \lim_{h\longrightarrow 0} nx^{n-1}+\binom{n}{2}x^{n-1}h+\cdots+\binom{n}{n-2}x^2h^{n-3}+nxh^{n-1}+h^{n-1}
\\ \qquad 
= nx^{n-1}
$$

+++