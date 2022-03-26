{{ sage | plane_stream }}

```python
# Simple Pendulum
f = (y, -sin(x))

# Lotka-Volterra Predator-Prey Model
f = (x-x*y, x*y-y)

# Lotka-Volterra Competitive Model
f = (x-x*y, y-x*y)
```