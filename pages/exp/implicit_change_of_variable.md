The usual [change of variable technique](exp | change_of_variable) takes the form 

$$t=g(x)$$
$$\d t = g'(x)\dd x$$

However, sometimes it is useful to relate the new variable and the old one _implicitely_:

$$h(t)=g(x)$$
$$h'(t)\dd t = g'(x)\dd x$$

$t$ may be explicitely expressed in terms of $x$, and this would lead to the same results, if we remember the [derivative of the inverse function](thm | derivative_inverse_function)

$$t=h^{-1}(g(x))$$
$$
t\d t = (h^{-1})'(g(x))g'(x)\dd x=\dfrac{1}{h'(h^{-1}(g(x)))}g'(x)\dd x=\dfrac{1}{h'(t)}g'(x)\dd x
$$
$$h'(t)\dd t = g'(x)\dd x$$

but this may be much more awkward. It is just a question of ease