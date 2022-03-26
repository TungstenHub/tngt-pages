En este applet puedes hallar numéricamente la Función de Distribución de una distribución cualquiera que construyas dentro del método `m()`. Prueba también las combinaciones interesantes indicadas más abajo:

{{ sage | custom_distribution }}

```python
def m():
    # Elevamos al cuadrado la salida de una distribución normal para obtener una distribución Gamma
    return prandom.gauss(0,1)**2
```

```python
def m():
    if prandom.randint(0,1):
        # La mitad de las veces tomamos un valor de una distribución uniforme
        return prandom.uniform(-1,1)
    else:
        # la otra mitad de las veces, de una distribución normal
        return prandom.gauss(0,2)
```