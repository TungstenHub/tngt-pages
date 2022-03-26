Carl Friedrich Gauss proved the constructibility with straightedge and compass of the regular heptadecagon in 1796. This was a major discovery that shook mathematics - besides the equilateral triangle and the regular pentagon, and from these the regular pentadecagon, no more odd-sided regular polygons were known to be constructible. This construction was a masterpiece of fine mathematics, and contains the core ideas of a richest and vastest field in Algebra - Galois Theory

And we would like to dig in from scratch... so switch on your math neurons!! 

Gauss was clever enough to translate this geometric problem into an algebraic one. Vertices of regular polygons - this sounds like complex numbers! Yes, the geometric plane becomes the complex plane, and finding points is finding complex numbers. And because of the geometric properties of the product of complex numbers, the $n$-th roots of the unit, that is, the $n$ solutions of the equation 

$$x^n=1$$

form a regular $n$-agon around the origin, one of its vertices being the most obvious root $x=1$

{{ image | regular_polygons }}

The first root encountered counterclockwise after $1$ is usually called $\omega_n$. Look, it works!

$$\omega_3^2=\left(-\dfrac{1}{2}+\dfrac{\sqrt{3}}{2}i\right)^2=\dfrac{1}{4}-2\cdot\dfrac{1}{2}\cdot\dfrac{\sqrt{3}}{2}i+\dfrac{3}{4}i^2=-\dfrac{1}{2}-\dfrac{\sqrt{3}}{2}i$$
$$\omega_3^3=\omega_3\cdot\omega_3^2=\left(-\dfrac{1}{2}+\dfrac{\sqrt{3}}{2}i\right)\left(-\dfrac{1}{2}-\dfrac{\sqrt{3}}{2}i\right)=\dfrac{1}{4}-\dfrac{3}{4}i^2=1$$

$$\omega_4^2=i^2=-1\qquad \omega_4^3=-1\cdot i=-i\qquad \omega_4^4=-i\cdot i=1$$

The computations for the pentagon would be much longer. But it's also more subtle. It involves _nested square roots_

$$\omega_5=\dfrac{\sqrt{5}-1}{4}+\sqrt{\dfrac{5+\sqrt{5}}{8}}i$$

Well, that's not so bad for our straightedge-and-compass first steps. Circles enable drawing square roots of given measures, and we may draw as many circles as we want. Yes, constructible points are exactly those whose complex coordinates involve additions, substractions, products, quotients, and square roots, combined again and again finitely many times. Think about it. But in spite of this apparent flexibility and the ease of the first cases, not every $\omega_n$ follows (not at all!) this pattern; if not entirely convinced, try to find an expression for $\omega_7$ and it'll soon turn out a nice headache. $\omega_7$ is not constructible. But $\omega_{17}$ _is_ constructible - that's precisely what Gauss proved, and what shook mathematics so heavily

Let's begin by meeting our new friends - $\zeta=\omega_{17}$ and all its powers, which compose our regular heptadecagon (there are just 17 different powers, because $\zeta^{17}=1$!)

{{ image | heptadecagon_roots }}

Just to get familiar with them, remember that they all satisfy the equation

$$x^{17}-1$$

but $x=1$ is one of these roots, and we may factor out

$$x^{17}-1=(x-1)(x^{16}+x^{15}+x^{14}+x^{13}+x^{12}+x^{11}+x^{10}+x^{9}+x^{8}+x^{7}+x^{6}+x^{5}+x^{4}+x^{3}+x^{2}+x+1)$$

so all the powers of $\zeta$ except $\zeta^0=1$ make up the 16 roots of 

$$x^{16}+x^{15}+x^{14}+x^{13}+x^{12}+x^{11}+x^{10}+x^{9}+x^{8}+x^{7}+x^{6}+x^{5}+x^{4}+x^{3}+x^{2}+x+1=0$$

Multiplying powers of $\zeta$ yields powers of $\zeta$ (no big discovery...); exponents add up, but since $\zeta^{17}=1$, addition works modulo 17

$$\zeta^3\cdot\zeta^5=\zeta^8$$
$$\zeta^9\cdot\zeta^{14}=\zeta^{23}=\zeta^6$$

This is indeed isomorphic to $(\Z_{17},+)$, the cyclic group of order 17. The set of powers of $\zeta$ works with product, $\Z_{17}$ work with addition modulo 17. $0$ is the identity element and $1$ is a generator

$$+1:\qquad 0\rightarrow 1\rightarrow 2\rightarrow 3\rightarrow 4\rightarrow 5\rightarrow 6\rightarrow 7\rightarrow 8\rightarrow 9\rightarrow 10\rightarrow 11\rightarrow 12\rightarrow 13\rightarrow 14\rightarrow 15\rightarrow 16\rightarrow 0$$

In Group Theory, though, it's very common to study the _group of units_ of a cyclic group: given $(\Z_{n},+)$, we rule out the integers not being coprime with $n$, and the remaining set of coprime integers $\Z_{n}^\times$ is an abelian group with the product modulo $n$. That's because the product of two coprime numbers is again coprime with $n$. In our case, $\Z_{17}^\times$ only rules out $0$, because $17$ is prime. So the set

$$\{1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16\}$$

is an abelian group (of order $16$) under product modulo $17$. Well, it happens that it is _cyclic_ of order $16$ - $3$ is a generator

$$\times 3:\qquad 1\rightarrow 3\rightarrow 9\rightarrow 10\rightarrow 13\rightarrow 5\rightarrow 15\rightarrow 11\rightarrow 16\rightarrow 14\rightarrow 8\rightarrow 7\rightarrow 4\rightarrow 12\rightarrow 2\rightarrow 6\rightarrow 1$$

Very interesting! And... what does it mean in terms of the powers of $\zeta$? Well, we have to move to... powers? Yes! It means that _cubing_ permutes all the powers of $\zeta$ except $\zeta^0=1$ in a cyclic way

$$\square^3:\qquad \zeta^{1}\rightarrow \zeta^{3}\rightarrow \zeta^{9}\rightarrow \zeta^{10}\rightarrow \zeta^{13}\rightarrow \zeta^{5}\rightarrow \zeta^{15}\rightarrow \zeta^{11}\rightarrow \zeta^{16}\rightarrow \zeta^{14}\rightarrow \zeta^{8}\rightarrow \zeta^{7}\rightarrow \zeta^{4}\rightarrow \zeta^{12}\rightarrow \zeta^{2}\rightarrow \zeta^{6}\rightarrow \zeta^{1}$$

And here's the key to it all. Anyone of us would have thought that this is getting too weird. Gauss, instead, found this _very meaningful_. So meaningful, that he thought this new order was more convenient

$$
\begin{array}{ccccccc}
z_{0}=\zeta       & \qquad & z_{1}=\zeta^{3}   & \qquad & z_{2}=\zeta^{9}   & \qquad & z_{3}=\zeta^{10} \\
z_{4}=\zeta^{13}  & \qquad & z_{5}=\zeta^{5}   & \qquad & z_{6}=\zeta^{15}  & \qquad & z_{7}=\zeta^{11} \\
z_{8}=\zeta^{16}  & \qquad & z_{9}=\zeta^{14}  & \qquad & z_{10}=\zeta^{8}  & \qquad & z_{11}=\zeta^{7} \\
z_{12}=\zeta^{4}  & \qquad & z_{13}=\zeta^{12} & \qquad & z_{14}=\zeta^{2}  & \qquad & z_{15}=\zeta^{6} \\
\end{array}
$$

and started to define new quantities (called _periods_) in terms of this new order:

$$
\begin{array}{rcl}
\alpha_0 & = & z_{0} + z_{2} + z_{4} + z_{6} + z_{8} + z_{10} + z_{12} + z_{14}\\
                 & = & \zeta + \zeta^{9} + \zeta^{13} + \zeta^{15} + \zeta^{16} + \zeta^{8} + \zeta^{4} + \zeta^{2}\\
                 &   & \\
\alpha_1 & = & z_{1} + z_{3} + z_{5} + z_{7} + z_{9} + z_{11} + z_{13} + z_{15}\\
                 & = & \zeta^{3} + \zeta^{10} + \zeta^{5} + \zeta^{11} + \zeta^{14} + \zeta^{7} + \zeta^{12} + \zeta^{6}\\
\end{array}
$$

{{ image | heptadecagon_periods_1 }}

That is, $z_n=\zeta^{(3^n)}$. And what is this useful for? Well, keep reading. Because of the symmetry, the sum of the $17$ roots of the unit is zero, so the sum of all the units except $1$ is $-1$, and therefore

$$\alpha_0+\alpha_1=-1$$

Ok, no big deal so far. But the shocking point is that

$$
\begin{array}{rcl}
\alpha_0\cdot\alpha_1 & = & (\zeta + \zeta^{9} + \zeta^{13} + \zeta^{15} + \zeta^{16} + \zeta^{8} + \zeta^{4} + \zeta^{2})\cdot(\zeta^{3} + \zeta^{10} + \zeta^{5} + \zeta^{11} + \zeta^{14} + \zeta^{7} + \zeta^{12} + \zeta^{6})\\
&   & ...\\
&   & ...\\
&   & ...\\
& = & 4(\zeta+\zeta^{2}+\zeta^{3}+\zeta^{4}+\zeta^{5}+\zeta^{6}+\zeta^{7}+\zeta^{8}+\zeta^{9}+\zeta^{10}+\zeta^{11}+\zeta^{12}+\zeta^{13}+\zeta^{14}+\zeta^{15}+\zeta^{16})\\
& = & -4\\
\end{array}
$$

{{ image | heptadecagon_sum_product_periods_1 }}

and therefore $\alpha_0$ and $\alpha_1$ are solutions of the quadratic equation

$$x^2+x-4=0$$

that is, $\alpha_0 = \dfrac{-1+\sqrt{17}}{2}$, $\alpha_1 = \dfrac{-1-\sqrt{17}}{2}$ (the components in $\alpha_0$ are more headed to the right whereas those of $\alpha_1$ are more headed to the left)

What??!! No, no, that's not trivial. Try to do the product by hand, and you'll get all sorts of tedious stuff and horrible calculations that miraculously turns out to be four times the sum of all powers of $\zeta$ distint to $1$. And believe me that if you take some random sums of powers of $\zeta$, its product will hardly ever fit so nicely. The product rule

$$z^a\cdot z^b=\zeta^{(3^a)}\cdot\zeta^{(3^b)}=\zeta^{3^a+3^b}$$

is of no help here, so _why_ does this work? It's time to talk about _automorphisms_.

An automorphism in a field $\K$ (for now say $\Q\subset\K\subset\C$) is a map $\varphi:\K\longrightarrow\K$ that satisfies

$$\varphi(0)=0$$
$$\varphi(1)=1$$
$$\varphi(a+b)=\varphi(a)+\varphi(b)$$
$$\varphi(ab)=\varphi(a)\varphi(b)$$

Quite demanding!! But not impossible to fulfill. For instance complex conjugation meets the definition, doesn't it? But yes, it is quite rigid: rational numbers are always fixed by such automorphism

$$\varphi(5)=\varphi(1)+\varphi(1)+\varphi(1)+\varphi(1)+\varphi(1)=1+1+1+1+1=5$$
$$\varphi\left(\dfrac{5}{3}\right)+\varphi\left(\dfrac{5}{3}\right)+\varphi\left(\dfrac{5}{3}\right)=\varphi\left(\dfrac{5}{3}+\dfrac{5}{3}+\dfrac{5}{3}\right)=\varphi(5)=5\Longrightarrow\varphi\left(\dfrac{5}{3}\right)=\dfrac{5}{3}$$

Ok. Now consider the field

$$
\K=\Q(\zeta)=\{a_{1}\zeta^{1}+a_{2}\zeta^{2}+a_{3}\zeta^{3}+a_{4}\zeta^{4}+a_{5}\zeta^{5}+a_{6}\zeta^{6}+a_{7}\zeta^{7}+a_{8}\zeta^{8} \\
+a_{9}\zeta^{9}+a_{10}\zeta^{10}+a_{11}\zeta^{11}+a_{12}\zeta^{12}+a_{13}\zeta^{13}+a_{14}\zeta^{14}+a_{15}\zeta^{15}+a_{16}\zeta^{16}:a_i\in\Q\}
$$

That's indeed a field; addition and product work nicely, quotient may be more subtle, although for this argument we may forget about division and think of the $a_i$ coefficients as being integers. There's no need to add $a_{0}\zeta^{0}$, since 

$$\zeta^{0}=1=-(\zeta+\zeta^{2}+\zeta^{3}+\zeta^{4}+\zeta^{5}+\zeta^{6}+\zeta^{7}+\zeta^{8}+\zeta^{9}+\zeta^{10}+\zeta^{11}+\zeta^{12}+\zeta^{13}+\zeta^{14}+\zeta^{15}+\zeta^{16})$$

Now, in the very spirit of the idea that Gauss found so meaningful, we want our $\varphi$ to _cube_ $\zeta$:

$$\zeta\longmapsto\zeta^3$$

but $\varphi$ is an automorphism, so it has to work well with products

$$\zeta^2\longmapsto\zeta^6$$

and with sums!

$$4\zeta^2+7\zeta^{10}+\zeta^5\longmapsto 4\zeta^6+7\zeta^{13}+\zeta^{15}$$

Great! Just cube every power of $\zeta$. It couldn't be simpler! Sums and products work well: the left hand side before cubing, the right hand side after cubing. Simplifications involving $\zeta^{17}=1$ may arise in the left hand side, then these match other simplifications involving $(\zeta^3)^{17}=1$. What could go wrong? Uhm, it just has a little black point

The definition of $\varphi$ is quite a fudge

Imagine one has

$$4\zeta^2+7\zeta^{10}+\zeta^5=\zeta^2-2\zeta^4+\zeta^7$$

Now what? Our definition of $\varphi$ is broken! Well, our automorphism should certainly be rigorously defined... but it is not inconsistent. This automorphism exists. The main reason is that equalities like the one before do not hold. Supposing it is true, then

$$3\zeta^2+2\zeta^4+\zeta^5-\zeta^7+7\zeta^{10}=0$$

that is, $\zeta$ is a root of 

$$P(x)=3x^2+2x^4+x^5-x^7+7x^{10}$$

but it is also a root of

$$Q(x)=x^{16}+x^{15}+x^{14}+x^{13}+x^{12}+x^{11}+x^{10}+x^{9}+x^{8}+x^{7}+x^{6}+x^{5}+x^{4}+x^{3}+x^{2}+x+1$$

Weird, isn't it? Some polynomial handling would lead to absurd. So the decomposition of an element of $\Q(\zeta)$ into powers of $\zeta$ as above is unique and $\varphi$ exists and works well. Take your time to play with it.

And now comes the magic! $\varphi$ permutes the powers of $\zeta$

$$
\begin{array}{rl}
\varphi: & \qquad \zeta^{1}\mapsto \zeta^{3}\mapsto \zeta^{9}\mapsto \zeta^{10}\mapsto \zeta^{13}\mapsto \zeta^{5}\mapsto \zeta^{15}\mapsto \zeta^{11}\mapsto \zeta^{16}\mapsto \zeta^{14}\mapsto \zeta^{8}\mapsto \zeta^{7}\mapsto \zeta^{4}\mapsto \zeta^{12}\mapsto \zeta^{2}\mapsto \zeta^{6}\mapsto \zeta^{1}\\
& \qquad z_0\mapsto z_1\mapsto z_2\mapsto z_3\mapsto z_4\mapsto z_5\mapsto z_6\mapsto z_7\mapsto z_8\mapsto z_9\mapsto z_{10}\mapsto z_{11}\mapsto z_{12}\mapsto z_{13}\mapsto z_{14}\mapsto z_{15}\mapsto z_0\\
\end{array}
$$

And the $\alpha_i$

$$\varphi(\alpha_0)=\varphi(z_{0} + z_{2} + z_{4} + z_{6} + z_{8} + z_{10} + z_{12} + z_{14})=z_{1} + z_{3} + z_{5} + z_{7} + z_{9} + z_{11} + z_{13} + z_{15}=\alpha_1$$
$$\varphi(\alpha_1)=\varphi(z_{1} + z_{3} + z_{5} + z_{7} + z_{9} + z_{11} + z_{13} + z_{15})=z_{0} + z_{2} + z_{4} + z_{6} + z_{8} + z_{10} + z_{12} + z_{14}=\alpha_0$$

_But its product remains fixed_

$$\varphi(\alpha_0 \alpha_1)=\alpha_1 \alpha_0=\alpha_0\alpha_1$$

and thus it has to be an integer, because no combination

$$
a_{1}\zeta^{1}+a_{2}\zeta^{2}+a_{3}\zeta^{3}+a_{4}\zeta^{4}+a_{5}\zeta^{5}+a_{6}\zeta^{6}+a_{7}\zeta^{7}+a_{8}\zeta^{8} \\
+a_{9}\zeta^{9}+a_{10}\zeta^{10}+a_{11}\zeta^{11}+a_{12}\zeta^{12}+a_{13}\zeta^{13}+a_{14}\zeta^{14}+a_{15}\zeta^{15}+a_{16}\zeta^{16}
$$

remains fixed if all the coefficients are not equal!! Can you see how very clever? Great Gauss! So

$$\alpha_0 = \dfrac{-1+\sqrt{17}}{2}$$
$$\alpha_1 = \dfrac{-1-\sqrt{17}}{2}$$

and it's time to repeat our procedure. These are our new periods! The index of $z$ increasing in steps of 4

$$
\begin{array}{rcl}
\alpha_{00} & = & z_{0} + z_{4} + z_{8} + z_{12}\\
                        & = & \zeta + \zeta^{13} + \zeta^{16} + \zeta^{4}\\
                        &   & \\
\alpha_{01} & = & z_{2} + z_{6} + z_{10} + z_{14}\\
                        & = & \zeta^{9} + \zeta^{15} + \zeta^{8} + \zeta^{2}\\
                        &   & \\
\alpha_{10} & = & z_{1} + z_{5} + z_{9} + z_{13}\\
                        & = & \zeta^{3} + \zeta^{5} + \zeta^{14} + \zeta^{12}\\
                        &   & \\
\alpha_{11} & = & z_{3} + z_{7} + z_{11} + z_{15}\\
                        & = & \zeta^{10} + \zeta^{11} + \zeta^{7} + \zeta^{6}\\
\end{array}
$$

{{ image | heptadecagon_periods_2 }}

Now the automorphism we have to focus on is $\varphi^2$, that permutes the periods

$$\varphi^2(\alpha_{00})=\alpha_{01}\qquad\varphi^2(\alpha_{01})=\alpha_{00}$$
$$\varphi^2(\alpha_{10})=\alpha_{11}\qquad\varphi^2(\alpha_{11})=\alpha_{10}$$

and leaves unchanged the sums and products. And what leaves $\varphi^2$ unchanged? Exactly combinations of $\alpha_0$ and $\alpha_1$. So it's no surprise that the sums and products are "nice quantities" (which now may be easily checked by hand)

$$
\begin{array}{rcccl}
\alpha_{00} & + & \alpha_{01} & = & \alpha_{0}\\
\alpha_{00} & \cdot & \alpha_{01} & = & -1\\
\alpha_{10} & + & \alpha_{11} & = & \alpha_{1}\\
\alpha_{10} & \cdot & \alpha_{11} & = & -1\\
\end{array}
$$

{{ image | heptadecagon_sum_product_periods_2 }}

and now

$$\alpha_{00}=\dfrac{\alpha_{0}+\sqrt{\alpha_{0}^2+4}}{2}=\dfrac{\frac{-1+\sqrt{17}}{2}+\sqrt{\left(\frac{-1+\sqrt{17}}{2}\right)^2+4}}{2}$$
$$\alpha_{01}=\dfrac{\alpha_{0}-\sqrt{\alpha_{0}^2+4}}{2}=\dfrac{\frac{-1+\sqrt{17}}{2}-\sqrt{\left(\frac{-1+\sqrt{17}}{2}\right)^2+4}}{2}$$
$$\alpha_{10}=\dfrac{\alpha_{1}+\sqrt{\alpha_{1}^2+4}}{2}=\dfrac{\frac{-1-\sqrt{17}}{2}+\sqrt{\left(\frac{-1-\sqrt{17}}{2}\right)^2+4}}{2}$$
$$\alpha_{11}=\dfrac{\alpha_{1}-\sqrt{\alpha_{1}^2+4}}{2}=\dfrac{\frac{-1-\sqrt{17}}{2}-\sqrt{\left(\frac{-1-\sqrt{17}}{2}\right)^2+4}}{2}$$

Periods once again!! And having in mind $\varphi^4$

$$
\begin{array}{rclcrcl}
\alpha_{000} & = & z_{0} + z_{8}          & \qquad & \alpha_{001} & = & z_{4} + z_{12}\\
             & = & \zeta + \zeta^{16}     & \qquad &              & = & \zeta^{13} + \zeta^{4}\\
             &   &                        & \qquad &              &   & \\
\alpha_{010} & = & z_{2} + z_{10}         & \qquad & \alpha_{011} & = & z_{6} + z_{14}\\
             & = & \zeta^{9} + \zeta^{8}  & \qquad &              & = & \zeta^{15} + \zeta^{2}\\
             &   &                        & \qquad &              &   & \\
\alpha_{100} & = & z_{1} + z_{9}          & \qquad & \alpha_{101} & = & z_{5} + z_{13}\\
             & = & \zeta^{3} + \zeta^{14} & \qquad &              & = & \zeta^{5} + \zeta^{12}\\
             &   &                        & \qquad &              &   & \\
\alpha_{110} & = & z_{3} + z_{11}         & \qquad & \alpha_{111} & = & z_{7} + z_{15}\\
             & = & \zeta^{10} + \zeta^{7} & \qquad &              & = & \zeta^{11} + \zeta^{6}\\
\end{array}
$$

{{ image | heptadecagon_product_periods_3 }}

Works like a charm! $\alpha_{000}$ and $\alpha_{001}$ are roots of

$$x^2-\alpha_{00}x+\alpha_{10}=0$$

and

$$
\alpha_{000}=\dfrac{\alpha_{00}+\sqrt{\alpha_{00}^2-4\alpha_{10}}}{2}= \\ 
\dfrac{\dfrac{\frac{-1+\sqrt{17}}{2}+\sqrt{\left(\frac{-1+\sqrt{17}}{2}\right)^2+4}}{2}+\sqrt{\left(\dfrac{\frac{-1+\sqrt{17}}{2}+\sqrt{\left(\frac{-1+\sqrt{17}}{2}\right)^2+4}}{2}\right)^2-4\dfrac{\frac{-1-\sqrt{17}}{2}+\sqrt{\left(\frac{-1-\sqrt{17}}{2}\right)^2+4}}{2}}}{2}
$$

And since $\mathrm{Re}(\zeta)=\dfrac{\alpha_{000}}{2}$, we have all we need to construct our regular heptadecagon with straightedge and compass. Great Gauss!!