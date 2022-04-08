Una prueba bastante simple de que $\pi$ ligeramente menor, aunque muy cercano, a $\dfrac{22}{7}$: puesto que $\dfrac{x^4(1-x)^4}{1+x^2}$ es estrictamente positiva,

$$
\begin{split}   
0 & < \int_0^1 \frac{x^4(1-x)^4}{1+x^2}\d x \\\\
  & = \int_0^1 \frac{x^4-4x^5+6x^6-4x^7+x^8}{1+x^2}\d x \\\\
  & = \int_0^1 \frac{(x^6-4x^5+5x^4-4x^2+4)(1+x^2)-4}{1+x^2}\d x \\\\
  & = \int_0^1 \left(x^6-4x^5+5x^4-4x^2+4-\frac{4}{1+x^2}\right)\d x \\\\
  & = \left[\frac{x^7}{7}-\frac{4x^6}{6}+x^5-\frac{4x^3}{3}+4x-4\arctan x\right]_0^1 \\\\
  & = \dfrac{1}{7}-\dfrac{4}{6}+1-\dfrac{4}{3}+4-4\dfrac{\pi}{4}\\\\
  & = \dfrac{22}{7}-\pi \quad \Longrightarrow \quad \hl{\pi < \dfrac{22}{7}}
\end{split}
$$