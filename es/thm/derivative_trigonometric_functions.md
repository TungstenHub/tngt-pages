[{sine}]

$$<<< (\sin x)'=\cos x $$

+++
Demostración
+++

$$<<< f(x)=\sin x $$
$$<<< 
\lim_{h\longrightarrow 0}\dfrac{f(x+h)-f(x)}{h}=\lim_{h\longrightarrow 0}\dfrac{\sin(x+h)-\sin x}{h}
$$  

Utilizamos la fórmula del [seno del ángulo suma]( TO-DO )

$$ \sin(x+h)-\sin x=\sin x\cos h + \cos x\sin h-\sin x=\sin x(\cos h -1)+ \cos x\sin h $$

Y ahora  

$$<<< 
\lim_{h\longrightarrow 0}\dfrac{\sin(x+h)-\sin x}{h}
\\ \qquad
= \sin x \lim_{h\longrightarrow 0}\dfrac{\cos h-1}{h}+\cos x \lim_{h\longrightarrow 0}\dfrac{\sin h}{h}
\\ \qquad
= \sin x \times 0 + \cos x \times 1 = \cos x
$$

habiendo utilizado las [derivadas de las funciones trigonométricas en el origen]( lem | derivative_trigonometric_origin )

+++

---
[{cosine}]

$$<<< (\cos x)'=-\sin x $$

+++
Demostración
+++

$$<<<f(x)=\cos x$$
$$<<< 
\lim_{h\longrightarrow 0}\dfrac{f(x+h)-f(x)}{h}=\lim_{h\longrightarrow 0}\dfrac{\cos(x+h)-\cos x}{h}
$$  

Utilizamos la fórmula del [coseno del ángulo suma]( TO-DO )

$$\cos(x+h)-\cos x=\cos x\cos h - \sin x\sin h-\cos x=\cos x(\cos h -1)- \sin x\sin h$$ 

Y ahora 

$$<<<
\lim_{h\longrightarrow 0}\dfrac{\cos(x+h)-\cos x}{h}
\\ \qquad
= \cos x \lim_{h\longrightarrow 0}\dfrac{\cos h-1}{h}-\sin x \lim_{h\longrightarrow 0}\dfrac{\sin h}{h}
\\ \qquad
= \cos x \times 0 - \sin x \times 1 = -\sin x
$$

habiendo utilizado de nuevo las [derivadas de las funciones trigonométricas en el origen]( lem | derivative_trigonometric_origin )

+++