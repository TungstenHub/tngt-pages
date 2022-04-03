Un **toro** es lo que todos conocemos: una "rosquilla" (hueca)

{{ threejs | torus }}

Topológicamente, el toro es el producto de dos circunferencias, $\T^2=\S^1\times \S^1$. Para verlo, hay que pensar en la descomposición en paralelos y meridianos

```sage
u, v = var('u,v')
t = parametric_plot3d((cos(u)*(2+cos(v)), sin(u)*(2+cos(v)), sin(v)), (u,0,2*pi), (v,0,2*pi), rgbcolor=(1,1,0), opacity=0.7, viewer='threejs', axes_labels=False)
t += sum([parametric_plot3d((cos(u)*(2+cos(k*pi/6)), sin(u)*(2+cos(k*pi/6)), sin(k*pi/6)), (u,0,2*pi), thickness=5, color='darkred') for k in range(12)])
t += sum([parametric_plot3d((cos(k*pi/6)*(2+cos(v)), sin(k*pi/6)*(2+cos(v)), sin(v)), (v,0,2*pi), thickness=5, color='cadetblue') for k in range(12)])
show(t)
```