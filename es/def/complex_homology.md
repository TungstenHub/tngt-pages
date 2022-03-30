Un **complejo**

$$C_\ast=\{\cdots \xrightarrow{} C_{k+1}\xrightarrow{\partial_{k+1}}C_k \xrightarrow{\partial_k} C_{k-1}\xrightarrow{}\cdots\}$$

es una cadena de grupos abelianos $C_k$ y homomorfismos $\partial_k$ tal que $\partial_k\circ\partial_{k+1}=0$ para todo $k$, es decir, $\text{im }\partial_{k+1}\subset \text{ker }\partial_k$

Asociado al complejo $C_\ast$ definimos los **grupos de homología**

$$H_k(C_\ast)=\dfrac{\text{ker }\partial_k}{\text{im }\partial_{k+1}}$$

---

[Versión cohomológica]

Un **complejo**

$$C^\ast=\{\cdots \xrightarrow{} C^{k-1}\xrightarrow{\mathrm{d}^{k-1}}C^k \xrightarrow{\mathrm{d}^k} C^{k+1}\xrightarrow{}\cdots\}$$

es una cadena de grupos abelianos $C^k$ y homomorfismos $\mathrm{d}^k$ tal que $\mathrm{d}^k\circ\mathrm{d}^{k-1}=0$ para todo $k$, es decir, $\text{im }\mathrm{d}^{k-1}\subset \text{ker }\mathrm{d}^k$

Asociado al complejo $C^\ast$ definimos los **grupos de cohomología**

$$H^k(C^\ast)=\dfrac{\text{ker }\mathrm{d}^k}{\text{im }\mathrm{d}^{k-1}}$$