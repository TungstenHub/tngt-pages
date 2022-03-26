**Archimedean Spiral** 

$r=a\theta$

```sage
var('theta');
polar_plot(theta, (theta, 0, 6*pi), thickness=3, rgbcolor=(0.1,0.4,0.9), adaptive_recursion = 10, adaptive_tolerance = 0.001)
```

**Logarithmic Spiral** 

$r=e^{a\theta}$

```sage
var('theta');
polar_plot(exp(0.1*theta), (theta, -6*pi, 6*pi), thickness=3, rgbcolor=(0.9,0,0.4), adaptive_recursion = 10, adaptive_tolerance = 0.0001)
```

**Hyperbolic Spiral** 

$r=\frac{a}{\theta}$

```sage
var('theta');
polar_plot(1/theta, (theta, 0.1*pi, 12*pi), thickness=3, rgbcolor=(0.1,0.9,0.4))
```

**Galileo's Spiral** 

$r=a-b\theta^2$

```sage
var('theta');
polar_plot(1-theta**2, (theta, -1.75*pi, 1.75*pi), thickness=3, rgbcolor=(0.1,0.1,0.1))
```

**Poinsot's Spiral** 

$r=\frac{a}{\cosh(\theta)}$

```sage
var('theta');
polar_plot(1/cosh(theta/3), (theta, -18*pi, 18*pi), thickness=3, rgbcolor=(0.9,0.9,0.1), adaptive_recursion = 10, adaptive_tolerance = 0.0001)
```

**Fermat's Spiral** 

$r=a\sqrt{\theta}$

```sage
var('theta');
polar_plot([sqrt(theta), -sqrt(theta)], (theta, 0, 6*pi), thickness=3, rgbcolor=(0.7,0.2,0.2))
```

**Cochleoid Spiral** 

$r=a\frac{sin(\theta)}{\theta}$

```sage
var('theta');
polar_plot(sin(theta)/theta, (theta, -6*pi, 6*pi), thickness=3, rgbcolor=(0.1,0.2,0.3), adaptive_recursion = 10, adaptive_tolerance = 0.0001)
```