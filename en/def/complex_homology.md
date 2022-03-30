A **complex**

$$C_\ast=\{\cdots \xrightarrow{} C_{k+1}\xrightarrow{\partial_{k+1}}C_k \xrightarrow{\partial_k} C_{k-1}\xrightarrow{}\cdots\}$$

is a chain of abelian groups $C_k$ and homomorphisms $\partial_k$ such that $\partial_k\circ\partial_{k+1}=0$ for all $k$, that is, $\text{im }\partial_{k+1}\subset \text{ker }\partial_k$

Associated with the complex $C_\ast$ we define the **homology groups**

$$H_k(C_\ast)=\dfrac{\text{ker }\partial_k}{\text{im }\partial_{k+1}}$$

---

[Cohomological version]

A **complex**

$$C^\ast=\{\cdots \xrightarrow{} C^{k-1}\xrightarrow{\mathrm{d}^{k-1}}C^k \xrightarrow{\mathrm{d}^k} C^{k+1}\xrightarrow{}\cdots\}$$

is a chain of abelian groups $C^k$ and homomorphisms $\mathrm{d}^k$ such that $\mathrm{d}^k\circ\mathrm{d}^{k-1}=0$ for all $k$, that is, $\text{im }\mathrm{d}^{k-1}\subset \text{ker }\mathrm{d}^k$

Associated with the complex $C^\ast$ we define the **cohomology groups**

$$H^k(C^\ast)=\dfrac{\text{ker }\mathrm{d}^k}{\text{im }\mathrm{d}^{k-1}}$$