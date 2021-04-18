The matrix scalar multiplication verifies the following properties

<ol>
  <li>**Distributivity with respect to scalars:** $(\alpha+\beta)A=\alpha A+\beta A\qquad\forall\,\alpha,\beta\in\K,\,A\in \mathcal{M}_{m\times n}(\K)$</li>
  <li>**Distributivity with respect to matrices:** $\alpha(A+B)=\alpha A+\alpha B\qquad\forall\,\alpha\in\K,\,A,B\in \mathcal{M}_{m\times n}(\K)$</li>
  <li>**Pseudoassociativity:** $(\alpha\beta)A=\alpha(\beta A)\qquad\forall\,\alpha,\beta\in\K,\,A\in \mathcal{M}_{m\times n}(\K)$</li>
  <li>**Identity Property:** $1A=A\qquad\forall\,A\in\mathcal{M}_{m\times n}(\K)$</li>
</ol>

+++
Proof
+++

Let $\alpha$ and $\beta$ be two scalars in $\K$ and $A=(a_{ij})_{ij}$ and $B=(b_{ij})_{ij}$ be two matrices in $\mathcal{M}_{m\times n}(\K)$

<ol>
  <li>**Distributivity with respect to scalars: **

  $$
  \begin{split}
  (\alpha+\beta)A & = ([\alpha+\beta] a_{ij})_{ij} \\
  & = (\alpha a_{ij}+\beta a_{ij})_{ij} \\
  & = (\alpha a_{ij})_{ij}+(\beta a_{ij})_{ij} \\
  & = \alpha A+\beta A
  \end{split}
  $$
  </li>
  <li>**Distributivity with respect to matrices: **

  $$
  \begin{split}
  \alpha(A+B) & = \alpha[(a_{ij})_{ij}+(b_{ij})_{ij}] \\
  & = \alpha[(a_{ij}+b_{ij})_{ij}] \\
  & = (\alpha[a_{ij}+b_{ij}])_{ij} \\
  & = (\alpha a_{ij}+\alpha b_{ij}])_{ij} \\
  & = (\alpha a_{ij})_{ij}+(\alpha b_{ij})_{ij} \\
  & = \alpha A+\alpha B
  \end{split}
  $$
  </li>
  <li>**Pseudoassociativity: **
  
  It is not called _associativity_ because where dealing with elements of different sets ($\K$ and $\mathcal{M}_{m\times n}(\K)$), but besides this we may think of it as associativity

  $$
  \begin{split}
  (\alpha\beta)A & = ([\alpha\beta] a_{ij})_{ij} \\
  & = (\alpha[\beta a_{ij}])_{ij} \\
  & = \alpha(\beta a_{ij})_{ij} \\
  & = \alpha(\beta A)
  \end{split}
  $$

  </li>
  <li>**Identity Property: ** 

  $$
  \begin{split}
  1A & = 1(a_{ij})_{ij} \\
  & = (1a_{ij})_{ij} \\
  & = (a_{ij})_{ij} \\
  & = A 
  \end{split}
  $$
  </li>
</ol>

+++