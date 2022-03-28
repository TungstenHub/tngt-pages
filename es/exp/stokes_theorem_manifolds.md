When a form of order $n-1$ is integrated in the boundary of a small ball of dimension $n$, the final value is very close to zero, not only because the domain of integration is small, but also because opposite parts of the boundary tend to cancel out. Of course, this effect dissapears as the ball grows bigger. The definition of the exterior derivative $\d$ is motivated as a measure of divergence of this computed value in the boundary with respect to the volume of the ball

{{ image | exterior_derivative_small_domain }}

Whether this approximation is accurate enough for "big" balls o "big" domains requires further study. However, the concepts we have built so far (differential forms, exterior derivative, integration) certainly benefit from linearity, i.e. behave very well with addition. This usually implies that local facts may become global, as long as the join of small patches works well. In our case, the boundary of small adjacent patches cancels out in a nice way, after having introduced the concept of orientation

{{ image | adjacent_charts }}

If this is so, the phenomenon would be valid for any manifold with boundary, no matter how "big": integrating a form along the boundary or integrating its exterior derivative in the manifold itself should be equivalent

{{ image | stokes_theorem_sum }}

Now the question is, does this really hold? This is the very celebrated _Stokes' Theorem_