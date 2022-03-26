A **complex homomorphism** $f:A_\ast\longrightarrow B_\ast$ is a family of maps $f_k:A_k\longrightarrow B_k$ such that $\partial^B_k\circ f_k=f_{k-1}\circ\partial^A_k$, that is, the diagram

$$
\begin{CD}
\cdots @>>> A_{k+1} @>{\partial_{k+1}}>> A_{k} @>{\partial_{k}}>> A_{k-1} @>>> \cdots\\
@.          @V{f_{k+1}}VV                @V{f_{k}}VV              @V{f_{k-1}}VV @.   \\
\cdots @>>> B_{k+1} @>{\partial_{k+1}}>> B_{k} @>{\partial_{k}}>> B_{k-1} @>>> \cdots\\
\end{CD}
$$

is commutative

In this case, $f:A_\ast\longrightarrow B_\ast$ induces 

$$f_k:H_k(A_\ast)\longrightarrow H_k(B_\ast)$$

linear maps, defined by $f_k[\alpha]=[f_k(\alpha)]$. The requirement $\partial^B_k\circ f_k=f_{k-1}\circ\partial^A_k$ ensures that the operation is well-defined

---

[Cohomological version]

A **complex homomorphism** $f:A^\ast\longrightarrow B^\ast$ is a family of maps $f^k:A^k\longrightarrow B^k$ such that $\mathrm{d}_B^k\circ f^k=f^{k+1}\circ\mathrm{d}_A^k$, that is, the diagram

$$
\begin{CD}
\cdots @>>> A^{k-1} @>{\mathrm{d}^{k-1}}>> A^{k} @>{\mathrm{d}^{k}}>> A^{k+1} @>>> \cdots\\
@.          @V{f^{k-1}}VV                  @V{f^{k}}VV                @V{f^{k+1}}VV @.   \\
\cdots @>>> B^{k-1} @>{\mathrm{d}^{k-1}}>> B^{k} @>{\mathrm{d}^{k}}>> B^{k+1} @>>> \cdots\\
\end{CD}
$$

is commutative

In this case, $f:A^\ast\longrightarrow B^\ast$ induces 

$$f^k:H^k(A^\ast)\longrightarrow H^k(B^\ast)$$

linear maps, defined by $f^k[\alpha]=[f^k(\alpha)]$. The requirement $\mathrm{d}_B^k\circ f^k=f^{k+1}\circ\mathrm{d}_A^k$ ensures that the operation is well-defined