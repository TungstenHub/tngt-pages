{{ sage | plane_stream }}

```python
# Péndulo Simple
f = (y, -sin(x))

# Modelo Presa-Depredador de Lotka-Volterra
f = (x-x*y, x*y-y)

# Modelo Competitivo de Lotka-Volterra
f = (x-x*y, y-x*y)
```