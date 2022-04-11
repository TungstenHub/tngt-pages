Hemos dicho que no hay un conjunto de reglas que funcionen en todos los casos. Pero de hecho es mucho más delicado que todo esto. Hay funciones cuya integral _no se puede expresar usando funciones elementales_:

$$\int e^{-x^2}\dd x=???$$

¿Qué significa esto? Bueno, _hay_ funciones (únicas salvo constante) cuya derivada es $e^{-x^2}$

```sage
plot([exp(-x^2), sqrt(pi)/2*erf(x)], (x,-2,2), legend_label=['$e^{-x^2}$','$F(x)$'], thickness=3)
```

pero éstas no se pueden expresar como una combinación de sumas, productos, cocientes, potencias, raíces, senos o cosenos, exponenciales o logaritmos, o cualquier cosa que hayamos usado hasta ahora, lo combinemos como lo combinemos. Así tal cual. Si queremos, podemos ponerle un nombre nuevo, igual que le pusimos nombre al resto de funciones. De hecho, a esta función (a un múltiplo, más bien) se le ha dado un nombre, y es de una importancia mayor en Probabilidad, Estadística y en Ecuaciones en Derivadas Parciales: es la **Función de Error de Gauss**:

$$\mathrm{erf}(x)=\dfrac{2}{\sqrt{\pi}}\int_0^x e^{-t^2}\dd t$$

(puedes pasar de esta definición por ahora; es una _integral definida_). Y de hecho cualquier "función maliciosa al azar" no va a tener en general una integral expresable en términos de funciones elementales

$$\int \sin(\sin(\sin(\sin x)))\dd x=???$$

con lo que el conjunto de funciones cuya integral se puede resolver explícitamente (es decir, cuya integral es expresable en términos de funciones elementales) es de hecho muy pequeño