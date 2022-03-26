We may encounter the integral

$$\int\ln x\dd x$$

and none of the techniques learnt so far seems to work. But here the [derivative of a product of functions](thm | derivative_product) will be very useful:

$$(x\ln x)'=(x)'\ln x+x(\ln x)'=1\ln x+x\dfrac{1}{x}=\ln x+1$$

which is nearly what we need! Indeed

$$\int\ln x\dd x=\int((x\ln x)'-1)\dd x=x\ln x-x$$

Great! This technique is called **integration by parts** and works as follows: let $u(x)$ and $v(x)$ be some functions. We know that

$$(uv)'=u'v+uv'$$

so if our integrand is of the form $uv'$, we may switch to a completely different, and perhaps simpler, integral:

$$\int uv'\dd x=\int((uv)'-u'v)\dd x=uv-\int u'v\dd x$$