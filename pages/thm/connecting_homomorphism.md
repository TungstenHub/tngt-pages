Given a short exact sequence of complexes, there exists a **connecting homomorphism** $\partial_\ast:H_k(C_\ast)\longrightarrow H_{k-1}(A_*)$, defined by 

$$\partial_\ast([c])=\left[\left(f_{k-1}\right)^{-1}\left(\partial^B_k\left(\left(g_k\right)^{-1}(c)\right)\right)\right]$$

such that the complex

$$\cdots\xrightarrow{}H_k(A_*)\xrightarrow{f_k}H_k(B_*)\xrightarrow{g_k}H_k(C_*) \xrightarrow{\partial_\ast}H_{k-1}(A_*)\xrightarrow{f_{k-1}}\cdots$$

is an exact sequence

+++
Proof
+++

$$
\begin{CD}
        @.      0           @.                0               @.              \\
@.              @VVV                          @VVV                    @.      \\
\cdots  @>>>    A_{k}       @>{\partial_k}>>  \hl{A_{k-1}}    @>>>    \cdots  \\
@.              @VV{f_k}V                     @VV{f_{k-1}}V           @.      \\
\cdots  @>>>    \hl{B_{k}}  @>{\partial_k}>>  \hl{B_{k-1}}    @>>>    \cdots  \\
@.              @VV{g_k}V                     @VV{g_{k-1}}V           @.      \\
\cdots  @>>>    \hl{C_{k}}  @>{\partial_k}>>  C_{k-1}         @>>>    \cdots  \\
@.              @VVV                          @VVV                    @.      \\
        @.      0           @.                0               @.              \\
\end{CD}
$$

%%TO-DO%%

+++

---

[Cohomological version]

Given a short exact sequence of complexes, there exists a **connecting homomorphism** $\mathrm{d}^\ast:H^k(C^\ast)\longrightarrow H^{k+1}(A^*)$, defined by 

$$\mathrm{d}^\ast([c])=\left[\left(f^{k+1}\right)^{-1}\left(\mathrm{d}_B^k\left(\left(g^k\right)^{-1}(c)\right)\right)\right]$$

such that the complex

$$\cdots\xrightarrow{}H^k(A^*)\xrightarrow{f^k}H^k(B^*)\xrightarrow{g^k}H^k(C^*) \xrightarrow{\mathrm{d}^\ast}H^{k+1}(A^*)\xrightarrow{f^{k+1}}\cdots$$

is an exact sequence

+++
Proof
+++

$$
\begin{CD}
        @.      0           @.          0               @.              \\
@.              @VVV                    @VVV                    @.      \\
\cdots  @>>>    A^{k}       @>{\d^k}>>  \hl{A^{k+1}}    @>>>    \cdots  \\
@.              @VV{f^k}V               @VV{f^{k+1}}V           @.      \\
\cdots  @>>>    \hl{B^{k}}  @>{\d^k}>>  \hl{B^{k+1}}    @>>>    \cdots  \\
@.              @VV{g^k}V               @VV{g^{k+1}}V           @.      \\
\cdots  @>>>    \hl{C^{k}}  @>{\d^k}>>  C^{k+1}         @>>>    \cdots  \\
@.              @VVV                    @VVV                    @.      \\
        @.      0           @.          0               @.              \\
\end{CD}
$$

%%TO-DO%%

+++