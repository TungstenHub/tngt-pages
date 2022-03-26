The product of matrices verifies the following properties

<ul>
  <li>**Associativity:** $(AB)C=A(BC)$</li>
  <li>**Left Distributivity:** $A(B+C)=AB+AC$</li>
  <li>**Right Distributivity:** $(A+B)C=AC+BC$</li>
  <li>**Pseudoassociativity with respect to scalars:** $(\alpha A)B=\alpha(AB)$</li>
</ul>

whenever the shapes of the matrices make sense for the product to take place. Moreover, if $A\in\mathcal{M}_{m\times n}(\K)$, then also holds

<ul>
  <li>**Identity Property:** $I_m A=AI_n=A$</li>
</ul>

+++
Proof
+++

<ul>
  <li>**Associativity:** Suppose $A$, $B$ and $C$ are of shape $m\times p$, $p\times q$ and $q\times n$ respectively for the product to make sense 

  $$
  \begin{split}
  (AB)C & = \left(\sum_k a_{ik}b_{kl}\right)_{il}(c_{lj})_{lj} \\
  & = \left(\sum_{l}\left[\sum_k a_{ik}b_{kl}\right]c_{lj}\right)_{ij} \\
  & = \left(\sum_{kl}a_{ik}b_{kl}c_{lj}\right)_{ij} \\
  & = \left(\sum_{k}a_{ik}\left[\sum_l b_{kl}c_{lj}\right]\right)_{kj} \\
  & = (a_{ik})_{ik}\left(\sum_k b_{kl}c_{lj}\right)_{kj} \\
  & = A(BC) 
  \end{split}
  $$

  </li>
  <li>**Left Distributivity:** Suppose $A$, $B$ and $C$ are of shape $m\times p$, $p\times n$ and $p\times n$ respectively

  $$
  \begin{split}
  A(B+C) & = (a_{ik})_{ik}(b_{kj}+c_{kj})_{kj} \\
  & = \left(\sum_k a_{ik}[b_{kj}+c_{kj}]\right)_{ij} \\
  & = \left(\sum_k a_{ik}b_{kj}+\sum_k a_{ik}c_{kj}\right)_{ij} \\
  & = AB+AC
  \end{split}
  $$
  </li>
  <li>**Right Distributivity:** Suppose $A$, $B$ and $C$ are of shape $m\times p$, $m\times p$ and $p\times n$ respectively

  $$
  \begin{split}
  (A+B)C & = (a_{ik}+b_{ik})_{ik}(c_{kj})_{kj} \\
  & = \left(\sum_k [a_{ik}+b_{ik}]c_{kj}\right)_{ij} \\
  & = \left(\sum_k a_{ik}c_{kj}+\sum_k b_{ik}c_{kj}\right)_{ij} \\
  & = AC+BC
  \end{split}
  $$
  </li>
  <li>**Pseudoassociativity with respect to scalars:**

  $$
  \begin{split}
  (\alpha A)B & = (\alpha a_{ik})_{ik}(b_{kj})_{kj} \\
  & = \left(\sum_k[\alpha a_{ik}]b_{kj}\right)_{ij} \\
  & = \left(\sum_k\alpha a_{ik}b_{kj}\right)_{ij} \\
  & = \left(\sum_k\alpha [a_{ik}b_{kj}]\right)_{ij} \\
  & = \left(\alpha\sum_k [a_{ik}b_{kj}]\right)_{ij} \\
  & = \alpha\left(\sum_k [a_{ik}b_{kj}]\right)_{ij} \\
  & = \alpha(AB)
  \end{split}
  $$

  </li>
  <li>**Identity Property:** Let $I_m=(\delta_{ik})_{ik}$ and $A=(a_{kj})_{kj}$. When computing the product $I_mA$ in the row $i$ and column $j$, the corresponding coefficient will be

  $$\sum_k \delta_{ik}a_{kj}=\delta_{i1}a_{1j}+\delta_{i2}a_{2j}+\cdots+\delta_{im}a_{mj}$$

  but we know that $\delta_{ik}$ is always $0$ except when $i=k$, so only one term will survive

  $$\sum_k \delta_{ik}a_{kj}=\delta_{i1}a_{1j}+\delta_{i2}a_{2j}+\cdots+\delta_{im}a_{mj}=\delta_{ii}a_{ij}=a_{ij}$$

  so we end up with exactly the same matrix $A$. Likewise,

  $$
  \begin{split}
  AI_n & = (a_{ik})_{ik}(\delta_{kj})_{kj} \\
  & = \left(\sum_k a_{ik}\delta_{kj}\right)_{ij} \\
  & = (a_{ij}\delta_{jj})_{ij} \\
  & = (a_{ij})_{ij} \\
  & = A 
  \end{split}
  $$
  </li>
</ul>

+++