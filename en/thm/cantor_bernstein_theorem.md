Let $A$ and $B$ be sets such that $A\preccurlyeq B$ and $B\preccurlyeq A$. Then $A\approx B$

+++
Proof
+++

By hypothesis there exist two injective functions $f:A\longrightarrow B$ and $g:B\longrightarrow A$, and we have to proof that there exists a bijective function $h:A\longrightarrow B$, so that $A\approx B$

First, let's define two sequences of sets: one sequence $(A_n)_{n\in\mathbb{N}}$ of subsets of $A$ and one sequence $(B_n)_{n\in\mathbb{N}}$ of subsets of $B$

$$
\left\{
\begin{array}{rcl}
A_0 & = & A \smallsetminus g[B]\\
A_{n+1} & = & g[B_n]\\
\end{array}
\right.
\qquad\qquad
B_n = f[A_n]
$$

Now we define $h:A\longrightarrow B$ as

$$
h(a)=
\left\{
\begin{array}{rl}
f(a) & \text{if } a\in\bigcup\{A_n\vert n\in\mathbb{N}\}\\
g^{-1}(a) & \text{if } a\in A\smallsetminus\bigcup\{A_n\vert n\in\mathbb{N}\}\\
\end{array}
\right.
$$

{{ image | cantor_bernstein_theorem_construction }}

<ul>
  <li>
    $h$ is well-defined: if $a\in A\smallsetminus\bigcup\{A_n\vert n\in\mathbb{N}\}$, then $a\not\in A_0=A\smallsetminus g[B]$, so $a\in g[B]$ and, since $g$ is injective, $g^{-1}(a)$ makes sense
  </li>
  <li>
    $h$ is injective: let $a$, $a'\in A$ be distinct. We distinguish three cases:
    <ul>
      <li>
        $a$, $a'\in \bigcup\{A_n\vert n\in\mathbb{N}\}$: $h(a)=f(a)\neq f(a')=h(a')$ because $f$ is injective
      </li>
      <li>
        $a$, $a'\not\in \bigcup\{A_n\vert n\in\mathbb{N}\}$: $h(a)=g^{-1}(a)\neq g^{-1}(a')=h(a')$ because $g$ and $g^{-1}$ are injective
      </li>
      <li>
        $a\in \bigcup\{A_n\vert n\in\mathbb{N}\}$, $a'\not\in \bigcup\{A_n\vert n\in\mathbb{N}\}$: there exists some $n$ such that $a\in A_n$ and $h(a)=f(a)\in f[A_n]=B_n$. But $a'\not\in A_{n+1}$ and $h(a')=g^{-1}(a')$ cannot belong to $B_n$. Therefore, $h(a)\neq h(a')$
      </li>
    </ul>
  </li>
  <li>
    $\text{im }h=B$: we first note that $B_n=f[A_n]=h[A_n]$, so $B_n\in\text{im }h$ for each $n\in\mathbb{N}$. Now let $b\in B\smallsetminus\bigcup\{B_n\vert n\in\mathbb{N}\}$. $g(b)\in g[B]$, so $g(b)\not\in A_0$, and since $A_{n+1}=g[B_n]$ and $b\not \in B_n$ for any $n\in\mathbb{N}$, it turns out that $g(b)\not\in A_{n+1}$ for $g$ being injective. So $g(b)\not\in\bigcup\{A_n\vert n\in\mathbb{N}\}$, and $h(g(b))=g^{-1}(g(b))=b$, thus $b$ belongs to the image of $h$ and $\text{im }h=B$
  </li>
</ul>

+++