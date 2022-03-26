Our study of [Gaussian elimination]( thm | gaussian_elimination ) and the [row canonical form]( thm | row_canonical_form ) gives us a method to solve systems of linear equations 

First of all, it is more comfortable to work with the associated matrix of the system

$$
\left\{
\begin{array}{rrrrrrrcl}
a_{11}x_1 & + & a_{12}x_2 & + & \cdots & + & a_{1n}x_n & = & b_1\\
a_{21}x_1 & + & a_{22}x_2 & + & \cdots & + & a_{2n}x_n & = & b_2\\
  &  &  &  &  &  &  & \vdots & \\
a_{m1}x_1 & + & a_{m2}x_2 & + & \cdots & + & a_{mn}x_n & = & b_m\\
\end{array}\right.
\qquad\leadsto\qquad
\left(\begin{array}{cccc|c}
a_{11} & a_{12} & \cdots  & a_{1n} & b_1 \\
a_{21} & a_{22} & \cdots  & a_{2n} & b_2 \\
\vdots  & \vdots  & \ddots  & \vdots  & \vdots \\
a_{m1} & a_{m2} & \cdots  & a_{mn} & b_m \\
\end{array}\right)
$$

To this matrix we perform elementary operations until we reach its row reduced form. We know that elementary operations don't modify the set of solutions, that's the crucial point!

$$
\left(
\begin{array}{cccccccc|c}
 1      & \times & \cdot  & \cdot  & \times & \times & \cdot  & \cdot  & \times \\
 \cdot  & \cdot  & 1      & \cdot  & \times & \times & \cdot  & \cdot  & \times \\
 \cdot  & \cdot  & \cdot  & 1      & \times & \times & \cdot  & \cdot  & \times \\
 \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & 1      & \cdot  & \times \\
 \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & 1      & \times \\
 \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  \\
\end{array}
\right)
$$

The last rows are the simpler ones: that's why we have to analyze the new system from the last row upwards

<ol>
  <li>
  A row full with zeros

  $$
  \left(
  \begin{array}{cccccccc|c}
  0  & 0  & 0  & 0  & 0  & 0  & 0  & 0  & 0  \\
  \end{array}
  \right)
  $$

  represents the equation

  $$0\cdot x_1 + 0\cdot x_2 + \cdots + 0\cdot x_n = 0$$

  which essentially does nothing. So we simply skip such rows
  </li>
  <li>
  A row with a pivot at the very end

  $$
  \left(
  \begin{array}{cccccccc|c}
  0  & 0  & 0  & 0  & 0  & 0  & 0  & 0  & 1  \\
  \end{array}
  \right)
  $$

  represents the equation

  $$0\cdot x_1 + 0\cdot x_2 + \cdots + 0\cdot x_n = 1$$

  which is impossible! If we ever encounter such a row, our system is **incompatible**
  </li>
  <li>
  If we don't encounter such impossible rows, our system will be **compatible**. To find out why, keep in mind that every other row above has a pivot. If there are as many pivots as unknowns, then our reduced canonical form (after removing zero rows) will be something like

  $$
  \left(\begin{array}{cccc|c}
  1      & \cdot  & \cdots  & \cdot  & b_1' \\
  \cdot  & 1      & \cdots  & \cdot  & b_2' \\
  \vdots & \vdots & \ddots  & \vdots & \vdots \\
  \cdot  & \cdot  & \cdots  & 1      & b_n' \\
  \end{array}\right)
  $$

  for some altered coefficients $b_i'$, which represents the system

  $$
  \left\{
  \begin{array}{rrrrrrrcl}
  x_1 & + & 0\cdot x_2 & + & \cdots & + & 0\cdot x_n & = & b_1'\\
  0\cdot x_1 & + & x_2 & + & \cdots & + & 0\cdot x_n & = & b_2'\\
    &  &  &  &  &  &  & \vdots & \\
  0\cdot x_1 & + & 0\cdot x_2 & + & \cdots & + & x_n & = & b_n'\\
  \end{array}\right.
  $$

  that obviously has just one solution

  $$
  \begin{array}{rcl}
  x_1 & = & b_1'\\
  x_2 & = & b_2'\\
    & \vdots & \\
  x_n & = & b_n'\\
  \end{array}
  $$

  and thus is **determinate**

  If there are more unknowns than pivots, the unknowns whose column has no pivot will be *free*: we may choose the value we want for them. Once these values are fixed, the unknowns associated to a pivot may be solved in terms of the free ones. Since we can *choose*, there are many solutions, and the system is **indeterminate**. For instance, the matrix

  $$
  \left(
  \begin{array}{cccccccc|c}
  1      & 8      & \cdot  & \cdot  & -6     & 1      & \cdot  & \cdot  & 7 \\
  \cdot  & \cdot  & 1      & \cdot  & 0      & -4     & \cdot  & \cdot  & 3 \\
  \cdot  & \cdot  & \cdot  & 1      & 5      & 2      & \cdot  & \cdot  & 9 \\
  \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & 1      & \cdot  & -4 \\
  \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & \cdot  & 1      & 2 \\
  \end{array}
  \right)
  $$

  would represent the system

  $$
  \left\{
  \begin{array}{rrrrrrrrcl}
  x_1 & +8x_2 & & & -6x_5 & +x_6 & & & = & 7\\
  & & x_3 & & +0x_5 & -4x_6 & & & = & 3\\
  & & & x_4 & +5x_5 & +2x_6 & & & = & 9\\
  & & & & & & x_7 & & = & -4\\
  & & & & & & & x_8 & = & 2\\
  \end{array}\right.
  $$

  $x_2$, $x_5$ and $x_6$ are free and they may be assigned any value in $\K$; the other variables are solved in terms of these

  $$
  \begin{array}{rcl}
  x_2 & \in & \K\\
  x_5 & \in & \K\\
  x_6 & \in & \K\\
  x_1 & =   & 7-8x_2+6x_5-x_6\\
  x_3 & =   & 3+4x_6\\
  x_4 & =   & 9-5x_5-2x_6\\
  x_7 & =   & -4\\
  x_8 & =   & 2\\
  \end{array}
  $$
  </li>
</ol>

The compatibility and determination of a system $(A|b)$ are found via the number of nonzero rows in the row canonical form of $A$ and $(A|b)$ - this number has a special name, the _rank_, and the discussion has a special name too, the _Rouché-Capelli Theorem_