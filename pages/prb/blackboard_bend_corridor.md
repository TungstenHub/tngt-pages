A new blackboard has been bought for a classroom in the Faculty of Mathematics - hooray! But (yikes!) it has to cross a somewhat narrow bend in a corridor. Which is the **maximum length** of the blackboard for it to cross the bend nicely?

{{ image | blackboard_bend_corridor }}

+++
Solution
+++

There are essentially two ways to solve this problem: the first one is analytical, the second one is geometrical

The analytical way: when the blackboard is as big as possible, it will eventually touch the inner corner. Touching the corner and with a definite slope, one may compute a fixed length between the intersection with the exterior walls. But for the blackboard to cross the bend, it will have to rotate through all slopes, and thus has to be smaller than all of the beforementioned lengths. _So the maximum length of the blackboard is the minimum of the lengths of the segments joining the two exterior walls that contain the inner corner_

{{ image | blackboard_bend_corridor_slope }}

Achieving this minimum is a simple calculus problem. Let's work with the general problem with corridor widths $a$ and $b$. With the help of the two similar triangles, we find $y$ in terms of $x$

$$\dfrac{x-a}{b}=\dfrac{a}{y-b}$$
$$ab=(x-a)(y-b)$$
$$y=b+\dfrac{ab}{x-a}$$

Now the length $l$ (or even better, its square $l^2$, to simplify the calculations) is expressed in terms of $x$; we differenciate and equate to zero

$$l^2(x)=x^2+y^2=x^2+b^2+2b\dfrac{ab}{x-a}+\dfrac{a^2b^2}{(x-a)^2}$$
$$(l^2(x))'=2x-2\dfrac{ab^2}{(x-a)^2}-2\dfrac{a^2b^2}{(x-a)^3}=0$$
$$[x-a\neq 0]$$
$$x(x-a)^3-ab^2(x-a)-a^2b^2=0$$
$$x(x-a)^3-ab^2x=0$$
$$[x\neq 0]$$
$$(x-a)^3=ab^2$$
$$x=a+\sqrt[3]{ab^2}$$
$$y=b+\dfrac{ab}{x-a}=b+\dfrac{ab}{\sqrt[3]{ab^2}}=b+\sqrt[3]{a^2b}$$

And plugging the real values returns our desired length!!

$$x=5+\sqrt[3]{20}\simeq 7.71$$
$$y=2+\sqrt[3]{50}\simeq 5.68$$
$$l=\sqrt{x^2+y^2}\simeq \mathbf{9.58}$$

But there's also a geometrical solution! It has to do with the [astroid]( app | astroid ), which is the envelope of a stick of length $1$ whose edges lie in the axis. The equation of the astroid is $x^{\frac{2}{3}}+y^{\frac{2}{3}}=1$

```sage
var("x y");
implicit_plot((x^2)^(1/3) + (y^2)^(1/3) - 1, (x,-1.5,1.5), (y,-1.5,1.5), linewidth=6, color='#1565C0', plot_points=200)
```

(watch out! $x$ and $y$ denote now coordinates, not our bend lengths). And for a stick of length $l$, the equation would be 

$$x^{\frac{2}{3}}+y^{\frac{2}{3}}=l^{\frac{2}{3}}$$

But for the length to be as big as possible, the point $(a,b)$ should lie in the astroid!

{{ image | blackboard_bend_corridor_astroid }}

and thus

$$l^{\frac{2}{3}}=a^{\frac{2}{3}}+b^{\frac{2}{3}}$$

It seems a different result... but it isn't! Some handling is enough to see that both solutions are equivalent

$$
\begin{array}{rcl}
l^2 & = & x^2+y^2\\
& = & \left(a+a^{\frac{1}{3}}b^{\frac{2}{3}}\right)^2+\left(b+a^{\frac{2}{3}}b^{\frac{1}{3}}\right)^2\\
& = & \left(a^2+2a^{\frac{4}{3}}b^{\frac{2}{3}}+a^{\frac{2}{3}}b^{\frac{4}{3}}\right)+\left(b^2+2a^{\frac{2}{3}}b^{\frac{4}{3}}+a^{\frac{4}{3}}b^{\frac{2}{3}}\right)\\
& = & a^2+3a^{\frac{4}{3}}b^{\frac{2}{3}}+3a^{\frac{2}{3}}b^{\frac{4}{3}}+b^2\\
& = & \left(a^{\frac{2}{3}}+b^{\frac{2}{3}}\right)^3\\
&   & \\
l^{\frac{2}{3}} & = & a^{\frac{2}{3}}+b^{\frac{2}{3}}\\
\end{array}
$$

+++