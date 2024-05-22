Try doing some maths with lambda calculus. Remember that

```txt
cₙ = λfx.fⁿ(x)

# = λnfx.f(nfx)
+ = λmnfx.mf(nfx)
* = λmnfx.m(nf)x
^ = λmnfx.nmfx
```

and that the operators have to be in Polish notation.

{{ dynamic | lambda/arith }}