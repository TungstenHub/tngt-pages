$$<<< \left[\arctan\left(\dfrac{x+a}{1-ax}\right)\right]' $$

+++
Solution
+++

$$<<< 
\left[\arctan\left(\dfrac{x+a}{1-ax}\right)\right]'
\\ \qquad 
= \dfrac{1}{1+\left(\frac{x+a}{1-ax}\right)^2}\left[\dfrac{x+a}{1-ax}\right]'
\\ \qquad 
= \dfrac{(1-ax)^2}{(1-ax)^2+(x+a)^2}\dfrac{[x+a]'(1-ax)-(x+a)[1-ax]'}{(1-ax)^2}
\\ \qquad 
= \dfrac{(1-ax)-(x+a)(-a)}{(1-ax)^2+(x+a)^2}
\\ \qquad 
= \dfrac{1+a^2}{(1-2ax+a^2x^2)+(x^2+2ax+a^2)}
\\ \qquad 
= \dfrac{1+a^2}{1+a^2x^2+x^2+a^2}
\\ \qquad 
= \dfrac{1+a^2}{(1+x^2)(1+a^2)}
\\ \qquad 
= \hl{\dfrac{1}{1+x^2}}
$$

How can this be possible? We know that $[\arctan x]'=\dfrac{1}{1+x^2}$... Are $\arctan x$ and $\arctan\left(\dfrac{x+a}{1-ax}\right)$ somehow related? Yes, it needs just a small trick. Remember that

$$\tan(\alpha+\beta)=\dfrac{\tan\alpha+\tan\beta}{1-\tan\alpha\tan\beta}$$

then, if $x=\tan\alpha$ and $a=\tan\beta$,

$$
\arctan\left(\dfrac{x+a}{1-ax}\right)=\arctan\left(\dfrac{\tan\alpha+\tan\beta}{1-\tan\alpha\tan\beta}\right) \\
= \arctan(\tan(\alpha+\beta))=\alpha+\beta=\arctan x+\arctan a
$$

and $\arctan a$ is just a constant. Wow!

+++