Una vez definidos los espacios de formas y la derivada exterior, tenemos la siguiente cadena de aplicaciones

$$
\Omega^0(M)\xrightarrow{\mathrm{d}}\Omega^1(M)\xrightarrow{\mathrm{d}}\Omega^2(M)\xrightarrow{\mathrm{d}}\cdots \xrightarrow{\mathrm{d}}\Omega^{k-1}(M)\xrightarrow{\mathrm{d}}\Omega^k(M)\xrightarrow{\mathrm{d}}\Omega^{k+1}(M)\xrightarrow{\mathrm{d}}\cdots\xrightarrow{\mathrm{d}}\Omega^n(M)
$$

llamado **complejo de De Rham**. Un [_complejo_]( def | complex_homology ) es una cadena de homomorfismos entre grupos abelianos tal que $\mathrm{d}\circ\mathrm{d}=0$

Buscamos formas cerradas que no sean exactas. Como en la homología, los cocientes son el modo apropiado de proceder:

Sea 

$$
\Omega^0(M)\xrightarrow{\mathrm{d}^0}\Omega^1(M)\xrightarrow{\mathrm{d}^1}\Omega^2(M)\xrightarrow{\mathrm{d}^2}\cdots \xrightarrow{\mathrm{d}^{k-1}}\Omega^k(M)\xrightarrow{\mathrm{d}^k}\cdots\xrightarrow{\mathrm{d}^{n-1}}\Omega^n(M)
$$

el complejo de De Rham asociado a la variedad $M$. Definimos los **grupos de cohomología de $M$**

$$H^k(M)=\dfrac{\text{ker }\mathrm{d}^k}{\text{im }\mathrm{d}^{k-1}}=\dfrac{Z^k(M)}{B^k(M)}$$