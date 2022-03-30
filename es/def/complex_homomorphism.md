Un **homomorfismo de complejos** $f:A_\ast\longrightarrow B_\ast$ es una familia de aplicaciones $f_k:A_k\longrightarrow B_k$ tal que $\partial^B_k\circ f_k=f_{k-1}\circ\partial^A_k$, es decir, el diagrama

$$
\begin{CD}
\cdots @>>> A_{k+1} @>{\partial_{k+1}}>> A_{k} @>{\partial_{k}}>> A_{k-1} @>>> \cdots\\
@.          @V{f_{k+1}}VV                @V{f_{k}}VV              @V{f_{k-1}}VV @.   \\
\cdots @>>> B_{k+1} @>{\partial_{k+1}}>> B_{k} @>{\partial_{k}}>> B_{k-1} @>>> \cdots\\
\end{CD}
$$

es conmutativo

En este caso, $f:A_\ast\longrightarrow B_\ast$ induce 

$$f_k:H_k(A_\ast)\longrightarrow H_k(B_\ast)$$

aplicaciones lineales, definidas por $f_k[\alpha]=[f_k(\alpha)]$. El requisito $\partial^B_k\circ f_k=f_{k-1}\circ\partial^A_k$ asegura que la operación está bien definida

---

[Versión cohomológica]

Un **homomorfismo de complejos** $f:A^\ast\longrightarrow B^\ast$ es una familia de aplicaciones $f^k:A^k\longrightarrow B^k$ tal que $\mathrm{d}_B^k\circ f^k=f^{k+1}\circ\mathrm{d}_A^k$, es decir, el diagrama

$$
\begin{CD}
\cdots @>>> A^{k-1} @>{\mathrm{d}^{k-1}}>> A^{k} @>{\mathrm{d}^{k}}>> A^{k+1} @>>> \cdots\\
@.          @V{f^{k-1}}VV                  @V{f^{k}}VV                @V{f^{k+1}}VV @.   \\
\cdots @>>> B^{k-1} @>{\mathrm{d}^{k-1}}>> B^{k} @>{\mathrm{d}^{k}}>> B^{k+1} @>>> \cdots\\
\end{CD}
$$

es conmutativo

En este caso, $f:A^\ast\longrightarrow B^\ast$ induce 

$$f^k:H^k(A^\ast)\longrightarrow H^k(B^\ast)$$

aplicaciones lineales, definidas por $f^k[\alpha]=[f^k(\alpha)]$. El requisito $\mathrm{d}_B^k\circ f^k=f^{k+1}\circ\mathrm{d}_A^k$ asegura que la operación está bien definida