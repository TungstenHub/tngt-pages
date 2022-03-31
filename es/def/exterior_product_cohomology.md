El **producto exterior $\wedge$** se hereda en cohomología: 

$$\wedge:H^k(M)\times H^l(M)\longrightarrow H^{k+l}(M)$$
$$[\alpha]\wedge[\beta]=[\alpha\wedge\beta]$$

Para que $\wedge$ esté bien definido, hay que comprobar dos propiedades: 

<ol>
  <li>
  Si $\alpha$ y $\beta$ son cerradas, $\alpha\wedge\beta$ también es cerrada: 
  
  $$\mathrm{d} \alpha=0,\,\mathrm{d} \beta=0\Longrightarrow\mathrm{d}(\alpha\wedge\beta)=\mathrm{d} \alpha\wedge\beta+(-1)^k\alpha\wedge\mathrm{d}\beta=0$$ 
  
  Por lo tanto, 

  $$\wedge:\Omega^k(M)\times \Omega^l(M)\longrightarrow \Omega^{k+l}(M)$$
  
  induce 
  
  $$\wedge:Z^k(M)\times Z^l(M)\longrightarrow Z^{k+l}(M)$$
  
  y también 
  
  $$\wedge:Z^k(M)\times Z^l(M)\longrightarrow \left[Z^{k+l}(M)/B^{k+l}(M)=H^{k+l}(M)\right]$$
  </li>

  <li>
  Si además $\alpha$ o $\beta$ es exacta, $\alpha\wedge\beta$ también es exacta: 
  
  $$\alpha=\mathrm{d} \gamma\Longrightarrow\alpha\wedge\beta=\mathrm{d}\gamma\wedge\beta=\mathrm{d}(\gamma\wedge\beta)-(-1)^{k-1} \gamma\wedge\mathrm{d}\beta=\mathrm{d}(\gamma\wedge\beta)$$

  De este modo, 

  $$\wedge:Z^k(M)\times Z^l(M)\longrightarrow \left[Z^{k+l}(M)/B^{k+l}(M)=H^{k+l}(M)\right]$$
  
  induce 
  
  $$\wedge:\left[Z^k(M)/B^k(M)=H^k(M)\right]\times \left[Z^l(M)/B^l(M)=H^l(M)\right]\longrightarrow \left[Z^{k+l}(M)/B^{k+l}(M)=H^{k+l}(M)\right]$$
  </li>
</ol>