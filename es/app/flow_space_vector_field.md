{{ threejs | ode_flow }}

Prueba los siguientes sistemas:

```python
# Atractor de Lorenz
dx = 10*(y-x)
dy = x*(28-(z+27))-y
dz = x*y-8/3*(z+27)

# Atractor de Rössler
dx = -30*(y+4*z)
dy = 30*(x+0.1*y)
dz = 15/8+12*z*(x-35)
```