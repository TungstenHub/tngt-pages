Normalmente, la [técnica de cambio de variable](exp | change_of_variable) toma la forma

$$t=g(x)$$
$$\d t = g'(x)\dd x$$

Sin embargo, a veces es útil relacionar la variable nueva y la antigua _implícitamente_:

$$h(t)=g(x)$$
$$h'(t)\dd t = g'(x)\dd x$$

Quizá $t$ se pueda expresar explícitamente en términos de $x$, y esto llevaría a los mismos resultados, si recordamos la [derivada de la función inversa](thm | derivative_inverse_function)

$$t=h^{-1}(g(x))$$
$$
t\dd t = (h^{-1})'(g(x))g'(x)\dd x=\dfrac{1}{h'(h^{-1}(g(x)))}g'(x)\dd x=\dfrac{1}{h'(t)}g'(x)\dd x
$$
$$h'(t)\dd t = g'(x)\dd x$$

pero esto sería mucho más embrollado. Es una cuestión de comodidad