[{sine}]

$$<<< (\sin x)'=\cos x $$

+++
Proof
+++

$$<<< f(x)=\sin x $$
$$<<< 
\lim_{h\longrightarrow 0}\dfrac{f(x+h)-f(x)}{h}=\lim_{h\longrightarrow 0}\dfrac{\sin(x+h)-\sin x}{h}
$$  

We use the formula for the [sine of the sum of two angles]( TO-DO )

$$ \sin(x+h)-\sin x=\sin x\cos h + \cos x\sin h-\sin x=\sin x(\cos h -1)+ \cos x\sin h $$

And now  

$$<<< 
\lim_{h\longrightarrow 0}\dfrac{\sin(x+h)-\sin x}{h}
\\ \qquad
= \sin x \lim_{h\longrightarrow 0}\dfrac{\cos h-1}{h}+\cos x \lim_{h\longrightarrow 0}\dfrac{\sin h}{h}
\\ \qquad
= \sin x \times 0 + \cos x \times 1 = \cos x
$$

having used the [derivatives of the trigonometric functions in the origin]( lem | derivative_trigonometric_origin )

+++

---
[{cosine}]

$$<<< (\cos x)'=-\sin x $$

+++
Proof
+++

$$<<<f(x)=\cos x$$
$$<<< 
\lim_{h\longrightarrow 0}\dfrac{f(x+h)-f(x)}{h}=\lim_{h\longrightarrow 0}\dfrac{\cos(x+h)-\cos x}{h}
$$  

We use the formula for the [cosine of the sum of two angles]( TO-DO )

$$\cos(x+h)-\cos x=\cos x\cos h - \sin x\sin h-\cos x=\cos x(\cos h -1)- \sin x\sin h$$ 

And now  

$$<<<
\lim_{h\longrightarrow 0}\dfrac{\cos(x+h)-\cos x}{h}
\\ \qquad
= \cos x \lim_{h\longrightarrow 0}\dfrac{\cos h-1}{h}-\sin x \lim_{h\longrightarrow 0}\dfrac{\sin h}{h}
\\ \qquad
= \cos x \times 0 - \sin x \times 1 = -\sin x
$$

having used again the [derivatives of the trigonometric functions in the origin]( lem | derivative_trigonometric_origin )

+++