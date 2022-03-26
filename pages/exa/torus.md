We all know what a **torus** is: a (hollow) 'donut' 

{{ threejs | torus }}

Topologically, the torus is the product of two circumferences, $\T^2=\S^1\times \S^1$. To understand it, one must imagine the decomposition in meridians and parallels

```sage
u, v = var('u,v')
t = parametric_plot3d((cos(u)*(2+cos(v)), sin(u)*(2+cos(v)), sin(v)), (u,0,2*pi), (v,0,2*pi), rgbcolor=(1,1,0), opacity=0.7, viewer='threejs', axes_labels=False)
t += sum([parametric_plot3d((cos(u)*(2+cos(k*pi/6)), sin(u)*(2+cos(k*pi/6)), sin(k*pi/6)), (u,0,2*pi), thickness=5, color='darkred') for k in range(12)])
t += sum([parametric_plot3d((cos(k*pi/6)*(2+cos(v)), sin(k*pi/6)*(2+cos(v)), sin(v)), (v,0,2*pi), thickness=5, color='cadetblue') for k in range(12)])
show(t)
```