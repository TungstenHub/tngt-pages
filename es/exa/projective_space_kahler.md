El espacio proyectivo $\C P^n$ tiene una métrica especial, la métrica de Fubini-Study, en la que las proyectividades son isometrías. Está descrita por un potencial de Kähler en cada carta afín: 

$$\mathcal{K}=\log(1+|z|^2)$$

de donde se deriva el resto de coeficientes de la métrica:

$$h_{jk}=2\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1+|z|^2)=2\dfrac{\partial }{\partial z_j}\left(\dfrac{z_k}{1+|z|^2}\right)=2\dfrac{\delta_{jk}(1+|z|^2)-\bar{z}_j z_k}{(1+|z|^2)^2}$$

$$\tilde{h}=2\sum_{jk}\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1+|z|^2)\d z_j\otimes\d\bar{z}_k$$

$$g=\sum_{jk}\left(\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1+|z|^2)\d z_j\otimes\d\bar{z}_k+\dfrac{\partial ^2}{\partial \bar{z}_j\partial z_k}\log(1+|z|^2)\d\bar{z}_j\otimes\d z_k\right)$$

$$\omega=\ii\sum_{jk}\left(\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1+|z|^2)\d z_j\otimes\d\bar{z}_k-\dfrac{\partial ^2}{\partial \bar{z}_j\partial z_k}\log(1+|z|^2)\d\bar{z}_j\otimes\d z_k\right)=\ii\partial\bar{\partial}\log(1+|z|^2)$$

Calcular los símbolos de Christoffel y los otros coeficientes de curvatura puede ser bastante difícil, así que vamos a intentar un enfoque distinto. En vez de derivarlos directamente, vamos a calcular el determinante de la métrica.

$$
g=(g_{j\bar{k}})_{jk}=\left(\dfrac{\partial ^2}{\partial z_j\partial \bar{z}_k}\log(1+|z|^2)\right)_{jk}=\dfrac{1}{(1+|z|^2)^2}(\delta_{jk}(1+|z|^2)-\bar{z}_j z_k)_{jk}=\dfrac{-1}{(1+|z|^2)^2}(B-(1+|z|^2)I)
$$
$$
B=
\begin{pmatrix}
\bar{z}_1 z_1 & \cdots & \bar{z}_1 z_n \\
\vdots        & \ddots & \vdots        \\
\bar{z}_n z_1 & \cdots & \bar{z}_n z_n \\
\end{pmatrix}
$$

De este modo, 

$$\det g=\left(\dfrac{-1}{(1+|z|^2)^2}\right)^n\det(B-(1+|z|^2)I)=\left(\dfrac{-1}{(1+|z|^2)^2}\right)^n P_B(1+|z|^2)$$  

donde $P_B(\lambda)=\det(B-\lambda I)$ es el polinomio característico de $B$. ¿Pero cómo es este polinomio característico? Puesto que $B$ tiene rango 1, tiene el autovalor 0 con multiplicidad $n-1$, por lo que de hecho

$$P_B(\lambda)=(-1)^n \lambda^{n-1}(\lambda-\text{tr} B)$$

(ya que la traza viene con el término de grado $n-1$), y al final

$$\det g=\left(\dfrac{-1}{(1+|z|^2)^2}\right)^n(-1)^n(1+|z|^2)^{n-1}(1+|z|^2-|z|^2)=\dfrac{1}{(1+|z|^2)^{n+1}}$$

Teniendo el determinante, tenemos el tensor y la forma de Ricci

$$\rho=-\ii\partial\bar{\partial}\log\det g=\ii(n+1)\partial\bar{\partial}\log(1+|z^2|)=(n+1)\omega$$

y del mismo modo

$$R_{j\bar{k}}=(n+1)g_{j\bar{k}}$$

Es decir, la métrica de Fubini-Study en $\C P^n$ es Einstein con constante $n+1$, y en particular tiene curvatura escalar constante

$$Sc=(n+1)g^{j\bar{k}}g_{j\bar{k}}=n(n+1)$$