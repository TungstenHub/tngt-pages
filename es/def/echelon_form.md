Hemos dicho que nos gustaría efectuar operaciones elementales en nuestra matriz para obtener otras más simples. ¿Pero qué significa _más simple_? ¿Cuál es la situación ideal que deberíamos perseguir?

---

Una matriz está en **forma escalonada por filas** si

<ul>
<li>Todas las filas nulas (filas que sólo tienen $0$) están por debajo de las no nulas</li>
<li>El primer coeficiente no nulo de una fila no nula (llamado _coeficiente principal_ o _pivote_) es $1$</li>
<li>Cada pivote está estrictamente a la derecha del pivote de la fila superior</li>
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

Una matriz está en **forma escalonada reducida por filas** si además

<ul>
<li>Todos los coeficientes por encima de un pivote son $0$</li>
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