Let $\varpi: (X',q_0)\longrightarrow (X,p_0)$ be a covering, and let $f:[0,1]\longrightarrow X$ be a path with $f(0)=p_0$. Then there exists a unique path (lifting path) $\tilde f:[0,1]\longrightarrow X'$ with $\tilde f(0)=q_0$ and $\varpi\circ \tilde f=f$ 

+++
Proof
+++

Let $X=\bigcup U_\alpha$ be expressed as union of trivializing open sets, and taking the preimage of this open cover, we get an open cover for $[0,1]$. Using [Lebesgue's Number Lemma]( lem | lebesgue_number_lemma ), we may divide $[0,1]=\bigcup_{k=1}^N I_k$, $I_k=\left[ \frac{k-1}{N}, \frac{k}{N}\right]$, $k=1,\ldots,N$, such that each $f(I_k)$ is contained in some $U_{\alpha_k}$. We'll define $\tilde f_k:\left[0,\frac{k}{N}\right] \longrightarrow X'$ inductively, satisfying $\varpi \circ \tilde f_k= f|_{\left[0,\frac{k}{N}\right]}$ and $\tilde f_k(0)=q_0$; then $\tilde f=\tilde f_N$ meets the requirements

For $k=0$ there's nothing to do. Suppose we have everything done up to $k-1$. Then $p_k=f\left(\frac{k-1}{N}\right)\in U_{\alpha_k}$. We know that $\varpi^{-1}(U_{\alpha_k})=\bigsqcup V_i$. There is some $i_0$ with $q_{k-1}=\tilde f_{k-1}\left(\frac{k-1}{N}\right) \in V_{i_0}$. Now we define

$$
\tilde f_k (t)= \left\{ \begin{array}{ll} \tilde f_{k-1}(t), \quad & t\in \left[0,\frac{k-1}{N}\right]. \\
(\varpi|_{V_{i_0}})^{-1}(f(t)), & t\in \left[\frac{k-1}N,\frac{k}N\right]. \end{array}\right.
$$

$\tilde f_k$ is continuous (pasting lemma) and meets the requirements

For the unicity: suppose we have $\tilde f_1$ and $\tilde f_2$ with $\tilde f_1(0)=\tilde f_2(0)=q_0$ and $\varpi\circ \tilde f_1=\varpi\circ \tilde f_2=f$. Where do these liftings match? Let

$$
A=\{t\in [0,1] \, | \, \tilde f_1(t)=\tilde f_2(t)\}.
$$

$A$ is non empty, because $0\in A$. Moreover $A$ is open: let $t_0\in A$, $p=f(t_0)\in U_\alpha$ and $q=\tilde f_1(t_0)=\tilde f_2(t_0) \in V_{i_0}$ with $\varpi^{-1}(U_\alpha)=\bigsqcup V_i$, for some $i_0$. Since $f$ is continuous, there is some $\epsilon>0$ such that $f(J)\subset U_\alpha$, being $J=(t_0-\epsilon,t_0+\epsilon)$. So $\tilde f_j(J)\subset \bigsqcup V_i$, $j=1,2$. But $\tilde f_j(J)$ is connected, and has to be contained entirely in some $V_i$, that is, $\tilde f_j(J)\subset V_{i_0}$. So $\tilde f_j|_{J}= (\varpi|_{V_{i_0}})^{-1}\circ f|_J$ and $\tilde f_1|_{J}=\tilde f_2|_{J}$. Therefore $J\subset A$ and $A$ is open.

A similar reasoning shows that $A$ is closed: let $t_0\in \overline{A}$, $p=f(t_0)\in U_\alpha$, $\varpi^{-1}(U_\alpha)=\bigsqcup V_i$. Again there is some $\epsilon>0$ with $f(J)\subset U_\alpha$, $J=(t_0-\epsilon,t_0+\epsilon)$. Since $t_0\in \overline{A}$, we may find some $t\in J\cap A$. For some $i_0$, $\tilde f_1(t)=\tilde f_2(t) \in V_{i_0}$. And $\tilde f_j(J)\subset V_{i_0}$ for $j=1,2$. So $\tilde f_1(t_0)=\tilde f_2(t_0)$ and $t_0\in A$, i.e. $A$ is closed. 

Since $[0,1]$ is connected, $A=[0,1]$.

+++