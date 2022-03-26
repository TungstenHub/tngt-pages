$$f(x,y)=\sqrt{(x-1)^2+y^2}+\sqrt{(x+1)^2+y^2}+0.01x^2$$

The expression $\sqrt{(x-1)^2+y^2}+\sqrt{(x+1)^2+y^2}$ represents the sum of the distances to the points $(-1,0)$ and $(1,0)$; thus confocal ellipses appear as level curves and every point in the segment joining the two points would be a global minimum with value $2$. The perturbation $0.01x^2$ makes the origin the only local and global minimum of the function, but the ravine shape is still dominant and gradient descent suffers from oscillations

{{ d3js | gradient_descent_ravine_minimum }}