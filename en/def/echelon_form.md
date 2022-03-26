We have said that we would like to perform elementary operations in our matrix to get simpler ones. But what does _simpler_ mean? Which is the ideal situation we should pursue?

---

A matrix is said to be in **row echelon form** if 

<ul>
<li>All zero rows (rows containing only $0$) are below the nonzero ones</li>
<li>The first nonzero coefficient in a nonzero row (called _leading coefficient_ or _pivot_) is $1$</li>
<li>Each pivot is strictly to the right of the pivot of the row above it</li>
</ul>

$$
\left(
\begin{array}{ccccccccc}
1      & \times & \times & \times & \times & \times & \times & \times & \times \\
\cdot  & \cdot  & 1      & \times & \times & \times & \times & \times & \times \\
\cdot  & \cdot  & \cdot  & 1      & \times & \times & \times & \times & \times \\
\cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & 1      & \times & \times \\
\cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & 1      & \times \\
\cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  \\
\end{array}
\right)
$$

A matrix is said to be in **reduced row echelon form** if moreover

<ul>
<li>All coefficients above a pivot are $0$</li>
</ul>

$$
\left(
\begin{array}{ccccccccc}
 1      & \times & \cdot  & \cdot  & \times & \times & \cdot  & \cdot  & \times \\
 \cdot  & \cdot  & 1      & \cdot  & \times & \times & \cdot  & \cdot  & \times \\
 \cdot  & \cdot  & \cdot  & 1      & \times & \times & \cdot  & \cdot  & \times \\
 \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & 1      & \cdot  & \times \\
 \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & 1      & \times \\
 \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  \\
\end{array}
\right)
$$