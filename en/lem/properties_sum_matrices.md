$(\mathcal{M}_{m\times n}(\K),+)$ is an abelian group. That is, the sum of matrices verifies the following properties

<ol>
  <li>**Associativity:** $(A+B)+C=A+(B+C)\qquad\forall\,A,B,C\in \mathcal{M}_{m\times n}(\K)$</li>
  <li>**Commutativity:** $A+B=B+A\qquad\forall\,A,B\in \mathcal{M}_{m\times n}(\K)$</li>
  <li>**Identity Element:** $\exists\, 0\in\mathcal{M}_{m\times n}(\K)\,|\,A+0=0+A=A\qquad\forall\,A\in \mathcal{M}_{m\times n}(\K)$</li>
  <li>**Inverse Element:** $\forall\,A\in\mathcal{M}_{m\times n}(\K)\quad\exists\,-A\in\mathcal{M}_{m\times n}(\K)\,|\,A+(-A)=(-A)+A=0$</li>
</ol>

+++
Proof
+++

Let $A=(a_{ij})_{ij}$, $B=(b_{ij})_{ij}$ and $C=(c_{ij})_{ij}$ be any three matrices in $\mathcal{M}_{m\times n}(\K)$

<ul>
  <li>**Associativity: **

  $$
  \begin{split}
  (A+B)+C & = [(a_{ij})_{ij}+(b_{ij})_{ij}]+(c_{ij})_{ij} \\
  & = (a_{ij}+b_{ij})_{ij}+(c_{ij})_{ij} \\
  & = ([a_{ij}+b_{ij}]+c_{ij})_{ij} \\
  & = (a_{ij}+[b_{ij}+c_{ij}])_{ij} \\
  & = (a_{ij})_{ij}+(b_{ij}+c_{ij})_{ij} \\
  & = (a_{ij})_{ij}+[(b_{ij})_{ij}+(c_{ij})_{ij}] \\
  & = A+(B+C)
  \end{split}
  $$
  </li>
  <li>**Commutativity: **

  $$
  \begin{split}
  A+B & = (a_{ij})_{ij}+(b_{ij})_{ij} \\
  & = (a_{ij}+b_{ij})_{ij} \\
  & = (b_{ij}+a_{ij})_{ij} \\
  & = (b_{ij})_{ij}+(a_{ij})_{ij} \\
  & = B+A
  \end{split}
  $$
  </li>
  <li>**Identity Element: **

  The identity element suitable for this sum is the matrix filled up with zeros, that is 

  $$
  0 = (0)_{ij} = 
  \left(\begin{array}{cccc}
  0 & 0 & \cdots  & 0\\
  0 & 0 & \cdots  & 0\\
  \vdots  & \vdots  & \ddots  & \vdots \\
  0 & 0 & \cdots  & 0\\
  \end{array}\right)
  $$

  and it does indeed meet the requirements of identity element:

  $$
  \begin{split}
  A+0 & = (a_{ij})_{ij}+(0)_{ij} \\
  & = (a_{ij}+0)_{ij} \\
  & = (a_{ij})_{ij} \\
  & = A 
  \end{split}
  $$
  $$
  \begin{split}
  0+A & = (0)_{ij}+(a_{ij})_{ij} \\
  & = (0+a_{ij})_{ij} \\
  & = (a_{ij})_{ij} \\
  & = A 
  \end{split}
  $$
  </li>
  <li>**Opposite Element: ** Each matrix $A$ has an opposite matrix - namely $-A=(-a_{ij})_{ij}$, that is, the matrix whose elements are exactly the opposite of those of $A$. Let's check:

  $$
  \begin{split}
  A+(-A) & = (a_{ij})_{ij}+(-a_{ij})_{ij} \\
  & = (a_{ij}+(-a_{ij}))_{ij} \\
  & = (0)_{ij} \\
  & = 0 
  \end{split}
  $$

  $$
  \begin{split}
  (-A)+A & = (-a_{ij})_{ij}+(a_{ij})_{ij} \\
  & = ((-a_{ij})+a_{ij})_{ij} \\
  & = (0)_{ij} \\
  & = 0 
  \end{split}
  $$
  </li>

+++