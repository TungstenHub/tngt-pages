$$<<< (\ln x)'=\dfrac{1}{x} $$

+++
Demostración
+++

$$<<< f(x)=\ln x $$
$$<<< 
\lim_{h\longrightarrow 0}\dfrac{f(x+h)-f(x)}{h}
\\ \qquad
= \lim_{h\longrightarrow 0}\dfrac{\ln(x+h)-\ln x}{h}
$$ 

Ahora bien, por las [propiedades de los logaritmos]( TO-DO ) 

$$<<<
\dfrac{\ln(x+h)-\ln x}{h}
\\ \qquad
= \dfrac{1}{h}\ln\left(\dfrac{x+h}{x}\right)
\\ \qquad
= \ln\left(1+\dfrac{h}{x}\right)^{\frac{1}{h}}
\\ \qquad
= \dfrac{1}{x}\ln\left(1+\dfrac{h}{x}\right)^{\frac{x}{h}}
$$ 

Por la [definición del número $e$]( TO-DO ),

$$<<< \lim_{h\longrightarrow 0}\left(1+\dfrac{h}{x}\right)^{\frac{x}{h}} = e $$

y por tanto

$$<<< 
\lim_{h\longrightarrow 0}\dfrac{\ln(x+h)-\ln x}{h}
\\ \qquad
= \lim_{h\longrightarrow 0}\dfrac{1}{x}\ln\left(1+\dfrac{h}{x}\right)^{\frac{x}{h}}
\\ \qquad
= \dfrac{1}{x}\ln\lim_{h\longrightarrow 0}\left(1+\dfrac{h}{x}\right)^{\frac{x}{h}}
\\ \qquad
= \dfrac{1}{x}\ln e = \dfrac{1}{x}
$$ 

+++