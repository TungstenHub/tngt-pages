$$f(x,y)=\sqrt{(x-1)^2+y^2}+\sqrt{(x+1)^2+y^2}+0.01x^2$$

La expresión $\sqrt{(x-1)^2+y^2}+\sqrt{(x+1)^2+y^2}$ representa la suma de distancias a los puntos $(-1,0)$ y $(1,0)$; por ello aparecen elipses confocales como curvas de nivel y cualquier punto del segmento que une los dos focos sería un mínimo global con valor $2$. La perturbación $0.01x^2$ hace que el origen sea el único mínimo local y global de la función, pero la forma de barranco sigue siendo dominante y el descenso de gradiente sufre oscilaciones

{{ d3js | gradient_descent_ravine_minimum }}