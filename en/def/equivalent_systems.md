Two systems of linear equations are said to be **equivalent** when they have exactly the same solutions. For instance 

$$
\left\{
\begin{array}{rrrrr}
x_1 & -2x_2 & + x_3 & = & 7\\
2x_1 & -5x_2 & +2x_3 & = & 6\\
3x_1 &  2x_2 & - x_3 & = & 1\\
\end{array}\right.
\qquad\qquad
\left\{
\begin{array}{rrrrr}
2x_1 & -5x_2 & +2x_3 & = & 6\\
x_1 & -2x_2 & + x_3 & = & 7\\
3x_1 &  2x_2 & - x_3 & = & 1\\
\end{array}\right.
$$

are equivalent, because we have just swapped the two first rows, and the requirements to fulfill are the same. On the other hand, 

$$
\left\{
\begin{array}{rrrrr}
x_1 & -2x_2 & + x_3 & = & 7\\
2x_1 & -5x_2 & +2x_3 & = & 6\\
3x_1 &  2x_2 & - x_3 & = & 1\\
\end{array}\right.
\qquad\qquad
\left\{
\begin{array}{rrrrr}
x &  &  & = & 2\\
& y &  & = & 8\\
&  & z & = & 21\\
\end{array}\right.
$$

are equivalent too (and thus both systems have only one solution $(x=2,y=8,z=21)$), but this is not so obvious for the naked eye

Our strategy to solve systems of linear equations will be to get simpler and simpler equivalent systems, until we reach a system whose solutions are straightforward to find