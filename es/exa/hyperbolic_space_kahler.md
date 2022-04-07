Por último tenemos el espacio hiperbólico $D^n=\{z\in\C^n:|z|<1\}$. Lo dotamos de la métrica hermítica provinente del siguiente potencial de Kähler global

$$\mathcal{K}=-\log(1-|z|^2)$$

Repitiendo los mismos pasos que para el espacio proyectivo, obtenemos

$$h_{jk}=-2\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1-|z|^2)=-2\dfrac{\partial }{\partial z_j}\left(\dfrac{-z_k}{1-|z|^2}\right)=2\dfrac{\delta_{jk}(1-|z|^2)+\bar{z}_j z_k}{(1-|z|^2)^2}$$

$$\tilde{h}=-2\sum_{jk}\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1-|z|^2)\d z_j\otimes\d \bar{z}_k$$

$$g=-\sum_{jk}\left(\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1-|z|^2)\d z_j\otimes\d \bar{z}_k+\dfrac{\partial ^2}{\partial \bar{z}_j\partial z_k}\log(1-|z|^2)\d \bar{z}_j\otimes\d z_k\right)$$

$$\omega=-\ii\sum_{jk}\left(\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1-|z|^2)\d z_j\otimes\d \bar{z}_k-\dfrac{\partial ^2}{\partial \bar{z}_j\partial z_k}\log(1-|z|^2)\d \bar{z}_j\otimes\d z_k\right)=-\ii\partial\bar{\partial}\log(1-|z|^2)$$

$$\det g=\dfrac{1}{(1-|z|^2)^{n+1}},\qquad\rho=-(n+1)\omega,\qquad R_{j\bar{k}}=-(n+1)g_{j\bar{k}},\qquad Sc=-n(n+1)$$

y de nuevo es una métrica Einstein, de constante $-(n+1)$.