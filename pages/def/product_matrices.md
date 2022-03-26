Let $A$ and $B$ be two matrices with the following shapes:

$$A=(a_{ik})_{ik}\in\mathcal{M}_{m\times p}(\mathbb{K})\qquad\text{(\(m\) rows and \(p\) columns)}$$
$$B=(b_{kj})_{kj}\in\mathcal{M}_{p\times n}(\mathbb{K})\qquad\text{(\(p\) rows and \(n\) columns)}$$

We define their product as a matrix

$$C=(c_{ij})_{ij}\in\mathcal{M}_{m\times n}(\mathbb{K})\qquad\text{(\(m\) rows and \(n\) columns)}$$

where

$$c_{ij}=\sum_{k=1}^p a_{ik}b_{kj}=a_{i1}b_{1j}+a_{i2}b_{2j}+\cdots+a_{ip}b_{pj}$$

So the product of matrices is not defined for every pair of matrices - only when the shapes match as follows

$$
\begin{array}{ccccc}
A & \cdot & B  & = & C\\
\textcolor{#E91E63}{m} \times \textcolor{#2196F3}{p} &  & \textcolor{#2196F3}{p}\times \textcolor{#FF9800}{n}  &  & \textcolor{#E91E63}{m}\times \textcolor{#FF9800}{n}
\end{array}
$$