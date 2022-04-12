Las potencias de senos y cosenos se integran de la siguiente manera: 

<ol>
<li>

**Potencias impares**

$$\int \sin^{2n+1}(x)\,\mathrm{d}x=\int \sin^{2n}(x)\sin x\,\mathrm{d}x=\int (1-\cos^2(x))^n\sin x\,\mathrm{d}x$$

Al expandir el binomio $(1-\cos^2(x))^n$ nos salen varias integrales del tipo

$$\int \cos^m(x)\sin x\,\mathrm{d}x$$

que se resuelven con el cambio de variable $t=\cos x$, $\mathrm{d}t=-\sin x \,\mathrm{d}x$.

La integral

$$\int \cos^{2n+1}(x)\,\mathrm{d}x=\int \cos^{2n}(x)\cos x\,\mathrm{d}x=\int (1-\sin^2(x))^n\cos x\,\mathrm{d}x$$

se resuelve de modo completamente análogo

</li>
<li>

**Potencias pares**

$$\int \sin^{2n}(x)\,\mathrm{d}x=\int (\sin^2(x))^n\,\mathrm{d}x=\int \left(\dfrac{1-\cos(2x)}{2}\right)^n\,\mathrm{d}x$$
$$\int \cos^{2n}(x)\,\mathrm{d}x=\int (\cos^2(x))^n\,\mathrm{d}x=\int \left(\dfrac{1+\cos(2x)}{2}\right)^n\,\mathrm{d}x$$

y después de expandir el binomio, el integrando está expresado en términos de potencias más bajas de $\cos$; de este modo seguimos repitiendo el proceso hasta que todo esté integrado

</li>
</ol>