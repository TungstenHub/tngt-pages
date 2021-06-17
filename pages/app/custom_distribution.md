In this applet, you may find numerically the Cumulative Distribution Function of a custom distribution that you build inside the method `m()`. Try as well some interesting combinations sketched below: 

{{ sage | custom_distribution }}

```python
def m():
    # We square a output of a normal distribution to get a Gamma distribution
    return prandom.gauss(0,1)**2
```

```python
def m():
    if prandom.randint(0,1):
        # Half of the times we sample a value from a uniform distribution
        return prandom.uniform(-1,1)
    else:
        # and the othe half, from a normal distribution
        return prandom.gauss(0,2)
```