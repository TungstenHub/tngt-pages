Ever wondered what does it mean that a parabola is tangent to the line of infinity, or that a hyperbola cuts it twice?

```sage
x,y,a,b = var('x,y,a,b')

@interact
def _(p = input_box(x^2-y)):
    def proj(alpha):
        u = a/(cos(alpha) - b*sin(alpha))
        v = (b*cos(alpha) + sin(alpha))/(cos(alpha) - b*sin(alpha))
        g = Graphics()
        for k in [-6,-4,-2,0,2,4,6]:
            g += line([(k*(cos(alpha)+7*sin(alpha)),-7), (k*(cos(alpha)-7*sin(alpha)),7)], color='grey')
        for k in [-6,-4,-2,0,2,4,6]:
            g += line([(-7,(k*cos(alpha)-sin(alpha))/(cos(alpha)+k*sin(alpha))), (7,(k*cos(alpha)-sin(alpha))/(cos(alpha)+k*sin(alpha)))], color='grey')
        if alpha != 0:
            g += line([(-7,1/tan(alpha)), (7,1/tan(alpha))], color='red')
        g += implicit_plot(p.substitute(x=u).substitute(y=v), (a,-7,7), (b,-7,7), region= abs(b*tan(alpha)-1)-0.01, fill=False, plot_points=300, linewidth=3)  
        return g
       
    shift = [proj(alpha) for alpha in sxrange(0,0.5,0.02)]
    animate(shift, xmin=-7, xmax=7, ymin=-7, ymax=7, frame=False).show(delay=15)
```

```python
# Parabola - tangent to the line of infinity
p = x^2-y

# Hyperbola - cuts twice the line of infinity
p = x^2-y^2+16


# Singular Cubic - has a point of inflection tangent to the line of infinity
p = x^2+x^3/2-y^2
```