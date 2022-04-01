Sean $A$ y $B$ dos matrices de los siguientes tamaños:

$$A=(a_{ik})_{ik}\in\mathcal{M}_{m\times p}(\mathbb{K})\qquad\text{(\(m\) filas y \(p\) columnas)}$$
$$B=(b_{kj})_{kj}\in\mathcal{M}_{p\times n}(\mathbb{K})\qquad\text{(\(p\) filas y \(n\) columnas)}$$

Definimos su producto como la matriz

$$C=(c_{ij})_{ij}\in\mathcal{M}_{m\times n}(\mathbb{K})\qquad\text{(\(m\) filas y \(n\) columnas)}$$

donde

$$c_{ij}=\sum_{k=1}^p a_{ik}b_{kj}=a_{i1}b_{1j}+a_{i2}b_{2j}+\cdots+a_{ip}b_{pj}$$

Así que el producto de matrices no está definido para cualquier par de matrices - sólo para aquéllas en que las dimensiones coinciden como sigue

$$
\begin{array}{ccccc}
A & \cdot & B  & = & C\\
\textcolor{#E91E63}{m} \times \textcolor{#2196F3}{p} &  & \textcolor{#2196F3}{p}\times \textcolor{#FF9800}{n}  &  & \textcolor{#E91E63}{m}\times \textcolor{#FF9800}{n}
\end{array}
$$