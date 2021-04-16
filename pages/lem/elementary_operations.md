The following operations (called **elementary operations**) lead to equivalent systems of equations:

<ol>
<li>

**Swapping rows $i$ and $j$**

$$
\left\{
\begin{array}{rrrrrrrcl}
a_{11}x_1 & + & a_{12}x_2 & + & \cdots & + & a_{1n}x_n & = & b_1\\
&  &  &  &  &  &  & \vdots & \\
a_{i1}x_1 & + & a_{i2}x_2 & + & \cdots & + & a_{in}x_n & = & b_i\\
&  &  &  &  &  &  & \vdots & \\
a_{j1}x_1 & + & a_{j2}x_2 & + & \cdots & + & a_{jn}x_n & = & b_j\\
&  &  &  &  &  &  & \vdots & \\
a_{m1}x_1 & + & a_{m2}x_2 & + & \cdots & + & a_{mn}x_n & = & b_m\\
\end{array}\right.
\qquad\leadsto\qquad
\left\{
\begin{array}{rrrrrrrcl}
a_{11}x_1 & + & a_{12}x_2 & + & \cdots & + & a_{1n}x_n & = & b_1\\
&  &  &  &  &  &  & \vdots & \\
a_{j1}x_1 & + & a_{j2}x_2 & + & \cdots & + & a_{jn}x_n & = & b_j\\
&  &  &  &  &  &  & \vdots & \\
a_{i1}x_1 & + & a_{i2}x_2 & + & \cdots & + & a_{in}x_n & = & b_i\\
&  &  &  &  &  &  & \vdots & \\
a_{m1}x_1 & + & a_{m2}x_2 & + & \cdots & + & a_{mn}x_n & = & b_m\\
\end{array}\right.
$$

$$
\left(\begin{array}{cccc|c}
a_{11} & a_{12} & \cdots  & a_{1n} & b_1 \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{i1} & a_{i2} & \cdots  & a_{in} & b_i \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{j1} & a_{j2} & \cdots  & a_{jn} & b_j \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{m1} & a_{m2} & \cdots  & a_{mn} & b_m \\
\end{array}\right)
\qquad\leadsto\qquad
\left(\begin{array}{cccc|c}
a_{11} & a_{12} & \cdots  & a_{1n} & b_1 \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{j1} & a_{j2} & \cdots  & a_{jn} & b_j \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{i1} & a_{i2} & \cdots  & a_{in} & b_i \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{m1} & a_{m2} & \cdots  & a_{mn} & b_m \\
\end{array}\right)
$$

</li>
<li>

**Multiplying row $i$ by a nonzero scalar $k$**

$$
\left\{
\begin{array}{rrrrrrrcl}
a_{11}x_1 & + & a_{12}x_2 & + & \cdots & + & a_{1n}x_n & = & b_1\\
&  &  &  &  &  &  & \vdots & \\
a_{i1}x_1 & + & a_{i2}x_2 & + & \cdots & + & a_{in}x_n & = & b_i\\
&  &  &  &  &  &  & \vdots & \\
a_{m1}x_1 & + & a_{m2}x_2 & + & \cdots & + & a_{mn}x_n & = & b_m\\
\end{array}\right.
\qquad\leadsto\qquad
\left\{
\begin{array}{rrrrrrrcl}
a_{11}x_1 & + & a_{12}x_2 & + & \cdots & + & a_{1n}x_n & = & b_1\\
&  &  &  &  &  &  & \vdots & \\
ka_{i1}x_1 & + & ka_{i2}x_2 & + & \cdots & + & ka_{in}x_n & = & kb_i\\
&  &  &  &  &  &  & \vdots & \\
a_{m1}x_1 & + & a_{m2}x_2 & + & \cdots & + & a_{mn}x_n & = & b_m\\
\end{array}\right.
$$

$$
\left(\begin{array}{cccc|c}
a_{11} & a_{12} & \cdots  & a_{1n} & b_1 \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{i1} & a_{i2} & \cdots  & a_{in} & b_i \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{m1} & a_{m2} & \cdots  & a_{mn} & b_m \\
\end{array}\right)
\qquad\leadsto\qquad
\left(\begin{array}{cccc|c}
a_{11} & a_{12} & \cdots  & a_{1n} & b_1 \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
ka_{i1} & ka_{i2} & \cdots  & ka_{in} & kb_i \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{m1} & a_{m2} & \cdots  & a_{mn} & b_m \\
\end{array}\right)
$$

</li>
<li>

**Adding $k$ times a row $i$ to a row $j$**

$$
\left\{
\begin{array}{rrrrrrrcl}
a_{11}x_1 & + & a_{12}x_2 & + & \cdots & + & a_{1n}x_n & = & b_1\\
&  &  &  &  &  &  & \vdots & \\
a_{i1}x_1 & + & a_{i2}x_2 & + & \cdots & + & a_{in}x_n & = & b_i\\
&  &  &  &  &  &  & \vdots & \\
a_{j1}x_1 & + & a_{j2}x_2 & + & \cdots & + & a_{jn}x_n & = & b_j\\
&  &  &  &  &  &  & \vdots & \\
a_{m1}x_1 & + & a_{m2}x_2 & + & \cdots & + & a_{mn}x_n & = & b_m\\
\end{array}\right.
\qquad\leadsto\qquad
\left\{
\begin{array}{rrrrrrrcl}
a_{11}x_1 & + & a_{12}x_2 & + & \cdots & + & a_{1n}x_n & = & b_1\\
&  &  &  &  &  &  & \vdots & \\
a_{i1}x_1 & + & a_{i2}x_2 & + & \cdots & + & a_{in}x_n & = & b_i\\
&  &  &  &  &  &  & \vdots & \\
(a_{j1}+ka_{i1})x_1 & + & (a_{j2}+ka_{i2})x_2 & + & \cdots & + & (a_{jn}+ka_{in})x_n & = & (b_j+kb_i)\\
&  &  &  &  &  &  & \vdots & \\
a_{m1}x_1 & + & a_{m2}x_2 & + & \cdots & + & a_{mn}x_n & = & b_m\\
\end{array}\right.
$$

$$
\left(\begin{array}{cccc|c}
a_{11} & a_{12} & \cdots  & a_{1n} & b_1 \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{i1} & a_{i2} & \cdots  & a_{in} & b_i \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{j1} & a_{j2} & \cdots  & a_{jn} & b_j \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{m1} & a_{m2} & \cdots  & a_{mn} & b_m \\
\end{array}\right)
\qquad\leadsto\qquad
\left(\begin{array}{cccc|c}
a_{11} & a_{12} & \cdots  & a_{1n} & b_1 \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{i1} & a_{i2} & \cdots  & a_{in} & b_i \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{j1}+ka_{i1} & a_{j2}+ka_{i2} & \cdots  & a_{jn}+ka_{in} & b_j+kb_i \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{m1} & a_{m2} & \cdots  & a_{mn} & b_m \\
\end{array}\right)
$$

</li>
</ol>