Each matrix is (row) equivalent to a matrix in reduced row echelon form

+++
Proof
+++

We will describe an algorithm (**Gaussian elimination**) that transforms a given matrix $A$ into another one in reduced row echelon form

<ol>
  <li>
    If all elements in the first column are $0$, then we ignore this column and start again with the remaining submatrix
    
    $$
    \left(
    \begin{array}{c|cccccccc}
    0 & \times & \times & \times & \times & \times & \times & \times & \times \\
    0 & \times & \times & \times & \times & \times & \times & \times & \times \\
    0 & \times & \times & \times & \times & \times & \times & \times & \times \\
    0 & \times & \times & \times & \times & \times & \times & \times & \times \\
    0 & \times & \times & \times & \times & \times & \times & \times & \times \\
    0 & \times & \times & \times & \times & \times & \times & \times & \times \\
    \end{array}
    \right)
    $$
  </li>
  <li>
    There is some nonzero element in the column; swap rows if necessary so that the element $a_{11}$ of the first column and the first row is nonzero

    $$
    \left(
    \begin{array}{ccccccccc}
    a_{11} & \times & \times & \times & \times & \times & \times & \times & \times \\
    \times & \times & \times & \times & \times & \times & \times & \times & \times \\
    \times & \times & \times & \times & \times & \times & \times & \times & \times \\
    \times & \times & \times & \times & \times & \times & \times & \times & \times \\
    \times & \times & \times & \times & \times & \times & \times & \times & \times \\
    \times & \times & \times & \times & \times & \times & \times & \times & \times \\
    \end{array}
    \right)
    $$
  </li>
  <li>
    Multiply the first row by $\dfrac{1}{a_{11}}$ so that the new corner element (which will be called a _pivot_) is $1$

    $$
    \left(
    \begin{array}{ccccccccc}
    1      & \times & \times & \times & \times & \times & \times & \times & \times \\
    \times & \times & \times & \times & \times & \times & \times & \times & \times \\
    \times & \times & \times & \times & \times & \times & \times & \times & \times \\
    \times & \times & \times & \times & \times & \times & \times & \times & \times \\
    \times & \times & \times & \times & \times & \times & \times & \times & \times \\
    \times & \times & \times & \times & \times & \times & \times & \times & \times \\
    \end{array}
    \right)
    $$
  </li>
  <li>
    Add $-a_{21}$ times the first row to the second row, $-a_{31}$ times the first row to the third row, and so on, until each coefficient below the pivot is zero. Ignore the first row and first column and start the process again with the remaining submatrix

    $$
    \left(
    \begin{array}{c|cccccccc}
    1 & \times & \times & \times & \times & \times & \times & \times & \times \\
    \hline
    0 & \times & \times & \times & \times & \times & \times & \times & \times \\
    0 & \times & \times & \times & \times & \times & \times & \times & \times \\
    0 & \times & \times & \times & \times & \times & \times & \times & \times \\
    0 & \times & \times & \times & \times & \times & \times & \times & \times \\
    0 & \times & \times & \times & \times & \times & \times & \times & \times \\
    \end{array}
    \right)
    $$
  </li>
</ol>

With this process, we would arrive to a matrix in row echelon form. To get a matrix in reduce row echelon form, repeat the last step to get zeros _above_ the pivots - since there are already zeros to the left of the pivots, these operations won't undo the row echelon form

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
\qquad\leadsto\qquad
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

+++