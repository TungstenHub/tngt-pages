For the Euclidean space $\C^n$ we have the flat metric:

$$h_{jk}=\delta_{jk};\qquad \tilde{h}=\sum_{j}(\d x_j\otimes\d x_j-\ii\d x_j\otimes\d y_j+\ii\d y_j\otimes\d x_j+\d y_j\otimes\d y_j)=\sum_{j}\d z_j\otimes\d \bar{z}_j$$

$$g=\sum_{j}(\d x_j\otimes\d x_j+\d y_j\otimes\d y_j)=\dfrac{1}{2}\sum_{j}(\d z_j\otimes\d \bar{z}_j+\d \bar{z}_j\otimes\d z_j);\qquad g_{j\bar{k}}=\dfrac{\delta_{jk}}{2}$$

$$\omega=\ii\sum_{j}(\d x_j\otimes\d y_j-\d y_j\otimes\d x_j+\d y_j\otimes\d y_j)=\dfrac{\ii}{2}\sum_{j}(\d z_j\otimes\d \bar{z}_j-\d \bar{z}_j\otimes\d z_j)=\dfrac{\ii}{2}\sum_{j}\d z_j\wedge\d \bar{z}_j;\qquad \omega_{j\bar{k}}=\dfrac{\ii\delta_{jk}}{2}$$

It is a Kähler manifold: $\d(\omega)=\dfrac{\ii}{2}\sum_{j}(\d^2 z_j\wedge\d \bar{z}_j-\d z_j\wedge\d^2 \bar{z}_j)=0$. Indeed the metric is described by a _global_ Kähler potential:

$$\mathcal{K}=\sum_{j}z_j\bar{z}_j=|z|^2;\qquad g_{j\bar{k}}=\dfrac{\partial ^2\mathcal{K}}{\partial z_j \partial \bar{z}_k}=\dfrac{\delta_{jk}}{2}$$

Since the coefficients of the metric are constant, the other tensors, that always involve derivatives, vanish:

$$\Gamma_{jk}^l=g^{l\bar{m}}\dfrac{\partial g_{k\bar{m}}}{\partial z_j}=2\delta^{lm}\dfrac{\partial \left(\dfrac{1}{2}\delta_{km}\right)}{\partial z_j}=0;\qquad \Gamma_{\bar{j}\bar{k}}^{\bar{l}}=\overline{\Gamma_{jk}^l}=0$$

$$R_{j\bar{k}l\bar{m}}=\dfrac{\partial ^2 g_{l\bar{m}}}{\partial z_j \partial \bar{z}_k}-g^{s\bar{t}}\dfrac{\partial g_{l\bar{t}}}{\partial z_j}\dfrac{\partial g_{s\bar{m}}}{\partial \bar{z}_k}=\dfrac{\partial ^2 \left(\dfrac{1}{2}\delta_{lm}\right)}{\partial z_j \partial \bar{z}_k}-2\delta^{st}\dfrac{\partial \left(\dfrac{1}{2}\delta_{lt}\right)}{\partial z_j}\dfrac{\partial \left(\dfrac{1}{2}\delta_{sm}\right)}{\partial \bar{z}_k}=0$$

$$R_{j\bar{k}}=-\dfrac{\partial ^2}{\partial z_j \partial \bar{z}_k}(\log \det g)=-\dfrac{\partial ^2\left((-1)^n\left(\dfrac{1}{2}\right)^{2n}\right)}{\partial z_j \partial \bar{z}_k}=0;\qquad\rho=0$$

$$Sc=g^{j\bar{k}}R_{j\bar{k}}=0$$

Therefore the flat metric $\C^n$ is Einstein of constant 0.