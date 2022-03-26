We have some sticks with which we can form the letters **I**, **X** and **V**

How many different words can you make with 1000 sticks?

{{ image | ixv_sticks }}

+++
Solution
+++

Instead of trying to figure out how many different words can we create with 1000 sticks, let's try to understand how many different words can we create with $n$ sticks.

Suppose that with $n$ sticks you can create $A(n)$ different words. With some inspection (and with the picture above) we have that 

$$A(1)=1$$
$$A(2)=3$$
$$A(3)=5$$
$$A(4)=11$$
$$A(5)=21$$

Can we go on? The key idea is that we can compute the next numbers form the previous ones. For intance, suppose that we have a word with $5$ sticks. Which is its first letter?

<ul>
  <li>It may be an **I** followed by a 4-sticks word</li>
  <li>Or it may be a **X** followed by a 3-sticks word</li>
  <li>Or perhaps it is a **V** followed by a 3-sticks word</li>
</ul>

So it happens that from this reasoning, $A(5)=2A(3)+A(4)$. And in general, it seems that

$$A(n)=A(n-1)+2A(n-2)$$

Great!! This is a second-order homogeneous recurrence. To solve it, we have to pay attention to its characteristic polynomial:

$$A(n)-A(n-1)-2A(n-2)=0\qquad\leadsto\qquad x^2-x-2=0$$

whose roots are $\alpha=2$, $\beta=-1$. So our recurrence is of the form

$$A(n)=a\times 2^n + b\times(-1)^n$$

Since $A(1)=2a-b=1$ and $A(2)=4a+b=3$, it turns out that $a=\frac{2}{3}$, $b=\frac{1}{3}$. Summing everything up,

$$A(n)=\dfrac{1}{3}\left(2^{n+1} + (-1)^n\right)$$

And finally

$$A(1000)=\dfrac{1}{3}\left(2^{1001} + (-1)^{1000}\right)=\dfrac{2^{1001} + 1}{3}\approx 7.14\times 10^{300}$$

+++