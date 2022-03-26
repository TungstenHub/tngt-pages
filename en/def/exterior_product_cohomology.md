The **exterior product $\wedge$** is inherited in cohomology: 

$$\wedge:H^k(M)\times H^l(M)\longrightarrow H^{k+l}(M)$$
$$[\alpha]\wedge[\beta]=[\alpha\wedge\beta]$$

For $\wedge$ to be well-defined, we have to check two properties: 

<ol>
  <li>
  If $\alpha$ and $\beta$ are closed, $\alpha\wedge\beta$ is also closed: 
  
  $$\mathrm{d} \alpha=0,\,\mathrm{d} \beta=0\Longrightarrow\mathrm{d}(\alpha\wedge\beta)=\mathrm{d} \alpha\wedge\beta+(-1)^k\alpha\wedge\mathrm{d}\beta=0$$ 
  
  Therefore, 

  $$\wedge:\Omega^k(M)\times \Omega^l(M)\longrightarrow \Omega^{k+l}(M)$$
  
  induces 
  
  $$\wedge:Z^k(M)\times Z^l(M)\longrightarrow Z^{k+l}(M)$$
  
  and also 
  
  $$\wedge:Z^k(M)\times Z^l(M)\longrightarrow \left[Z^{k+l}(M)/B^{k+l}(M)=H^{k+l}(M)\right]$$
  </li>

  <li>
  If moreover $\alpha$ or $\beta$ is exact, $\alpha\wedge\beta$ is also exact: 
  
  $$\alpha=\mathrm{d} \gamma\Longrightarrow\alpha\wedge\beta=\mathrm{d}\gamma\wedge\beta=\mathrm{d}(\gamma\wedge\beta)-(-1)^{k-1} \gamma\wedge\mathrm{d}\beta=\mathrm{d}(\gamma\wedge\beta)$$

  Therefore, 

  $$\wedge:Z^k(M)\times Z^l(M)\longrightarrow \left[Z^{k+l}(M)/B^{k+l}(M)=H^{k+l}(M)\right]$$
  
  induces 
  
  $$\wedge:\left[Z^k(M)/B^k(M)=H^k(M)\right]\times \left[Z^l(M)/B^l(M)=H^l(M)\right]\longrightarrow \left[Z^{k+l}(M)/B^{k+l}(M)=H^{k+l}(M)\right]$$
  </li>
</ol>