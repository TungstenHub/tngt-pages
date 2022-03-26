Each matrix is (row) equivalent to a _unique_ matrix in reduced row echelon form, to be called **row canonical form**

+++
Proof
+++

We already know, according to the [Gaussian Elimination algorithm]( thm | gaussian_elimination ), that any matrix is equivalent to a matrix in reduced row echelon form. But we wonder whether different sequences of elementary operations may lead to different matrices in reduced row echelon form. In this case, these two reduced matrices would be also equivalent, because the elementary operations are reversible. We will show that this is not possible: if two matrices in reduced row echelon form are equivalent, then they are the same matrix. This will prove the unicity

Suppose that $A$ and $B$ are two matrices in reduced row echelon form of shape $m\times n$ (because elementary operations don't modify the shape of a matrix) that are equivalent. Let's focus on the first column. If the first column of $A$ is full with zeros, so is the first column of $B$, because elementary operations cannot transform a column full of zeros into a column with some nonzero entry. And if both $A$ and $B$ have a nonzero entry in the first column, both columns are necessary 

$$\vect{1, 0, 0, \vdots, 0, 0}$$

since otherwise they're not in row echelon form (think about it!). So the first column is the same. Where is the disagreement? Is it possible that the first $k$ columns are equal, but the $k+1$ columns are different? No, the $k+1$ columns are equal too (and thus the whole matrices). Suppose that there are $l\leqslant k$ pivots in these first $k$ columns (in this example, $l=3$, $k=4$). 

$$
\left(
\begin{array}{cccc|ccccc}
1      & \times & \cdot  & \cdot  & \times & \times & \times & \times & \times \\
\cdot  & \cdot  & 1      & \cdot  & \times & \times & \times & \times & \times \\
\cdot  & \cdot  & \cdot  & 1      & \times & \times & \times & \times & \times \\
\hline
\cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times & \times \\
\cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times & \times \\
\cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times & \times \\
\end{array}
\right)
$$

<ol>
  <li>
    The $l$ first rows are equal in $A$ and $B$

    $$
    \left(
    \begin{array}{cccc|ccccc}
    \color{#1565C0}{1     } & \color{#1565C0}{\times} & \color{#1565C0}{\cdot } & \color{#1565C0}{\cdot } & \color{#1565C0}{\times} & \color{#1565C0}{\times} & \color{#1565C0}{\times} & \color{#1565C0}{\times} & \color{#1565C0}{\times} \\
    \color{#1565C0}{\cdot } & \color{#1565C0}{\cdot } & \color{#1565C0}{1     } & \color{#1565C0}{\cdot } & \color{#1565C0}{\times} & \color{#1565C0}{\times} & \color{#1565C0}{\times} & \color{#1565C0}{\times} & \color{#1565C0}{\times} \\
    \color{#1565C0}{\cdot } & \color{#1565C0}{\cdot } & \color{#1565C0}{\cdot } & \color{#1565C0}{1     } & \color{#1565C0}{\times} & \color{#1565C0}{\times} & \color{#1565C0}{\times} & \color{#1565C0}{\times} & \color{#1565C0}{\times} \\
    \hline
    \cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times & \times \\
    \cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times & \times \\
    \cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times & \times \\
    \end{array}
    \right)
    $$

    Why? The equivalence implies that the rows of one matrix are a linear combination (a sum with coefficients) of the rows of the other matrix; in some sense, elementary operations just mix all the rows in a matrix. This being so, a particular row in $B$, say the second, is a linear combination of the rows in $A$

    $$
    \begin{array}{rccccccccclcrcccccccccl}
    ( & \cdot  & \cdot  & 1      & \cdot  & \times & \times & \times & \times & \times & )_B 
              & = & \lambda_1( & 1      & \times & \cdot  & \cdot  & \times & \times & \times & \times & \times & )_A\\
    &&&&&&&&&&& + & \lambda_2( & \cdot  & \cdot  & 1      & \cdot  & \times & \times & \times & \times & \times & )_A\\
    &&&&&&&&&&& + & \lambda_3( & \cdot  & \cdot  & \cdot  & 1      & \times & \times & \times & \times & \times & )_A\\
    &&&&&&&&&&& + & \lambda_4( & \cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times & \times & )_A\\
    &&&&&&&&&&& + & \lambda_5( & \cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times & \times & )_A\\
    &&&&&&&&&&& + & \lambda_6( & \cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times & \times & )_A\\
    &&&&&&&&&&& + & \lambda_7( & \cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times & \times & )_A\\
    \end{array}
    $$

    where $\lambda_i$ are some numbers. But the second row having a pivot makes everything different - look at the first four columns! It is mandatory that $\lambda_2=1$ and the rest of the coefficients are $0$. And this is exactly that the second row in $B$ is equal to the second row in $A$ - and likewise for the rest of the $l$ first rows
  </li>
  <li>
    The coefficients in the $k+1$ column are equal in $A$ and $B$

    $$
    \left(
    \begin{array}{cccc|ccccc}
    1      & \times & \cdot  & \cdot  & \color{#1565C0}{\times} & \times & \times & \times & \times \\
    \cdot  & \cdot  & 1      & \cdot  & \color{#1565C0}{\times} & \times & \times & \times & \times \\
    \cdot  & \cdot  & \cdot  & 1      & \color{#1565C0}{\times} & \times & \times & \times & \times \\
    \hline
    \cdot  & \cdot  & \cdot  & \cdot  & \color{#1565C0}{\times} & \times & \times & \times & \times \\
    \cdot  & \cdot  & \cdot  & \cdot  & \color{#1565C0}{\times} & \times & \times & \times & \times \\
    \cdot  & \cdot  & \cdot  & \cdot  & \color{#1565C0}{\times} & \times & \times & \times & \times \\
    \end{array}
    \right)
    $$

    Why? We already know that the first $l$ coefficients are equal. Now, if there is some nonzero coefficient among them, the remaining ones are $0$ both in $A$ and $B$, otherwise we would have another pivot, which imposes that all the coefficients above it are zero. And if the $l$ first coefficients are $0$, then it happens like in the initial case and for the same reasons: we may have everything else being $0$, or we may have a pivot in the $l+1$ coefficient

    $$
    \left(
    \begin{array}{cccc|ccccc}
    1      & \times & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times \\
    \cdot  & \cdot  & 1      & \cdot  & \cdot  & \times & \times & \times & \times \\
    \cdot  & \cdot  & \cdot  & 1      & \cdot  & \times & \times & \times & \times \\
    \hline
    \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times \\
    \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times \\
    \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times \\
    \end{array}
    \right)
    \qquad\qquad\qquad
    \left(
    \begin{array}{cccc|ccccc}
    1      & \times & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times \\
    \cdot  & \cdot  & 1      & \cdot  & \cdot  & \times & \times & \times & \times \\
    \cdot  & \cdot  & \cdot  & 1      & \cdot  & \times & \times & \times & \times \\
    \hline
    \cdot  & \cdot  & \cdot  & \cdot  & 1      & \times & \times & \times & \times \\
    \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times \\
    \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \times & \times & \times & \times \\
    \end{array}
    \right)
    $$
  </li>
</ol>

So the $k+1$ column is equal in $A$ and $B$, and so are the rest of the columns

+++