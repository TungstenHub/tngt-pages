Which is the radius of the grey circle?

{{ image | touching_circles }}

+++
Solution
+++

The most direct way to get the desired radius is by means of an [inversion]( app | circle_inversion ) with respect to the outer circle: 

$$(a,b)\longmapsto\left(\dfrac{a}{a^2+b^2},\dfrac{b}{a^2+b^2}\right)$$

Inversion has very nice properties: circles map to circles or lines, and tangencies are also preserved. Our construction becomes

{{ image | touching_circles_solution }}

and the radius of the grey circle is

$$\dfrac{1}{2}\left(\dfrac{1}{5}-\dfrac{1}{7}\right)=\dfrac{1}{2}\dfrac{2}{35}=\dfrac{1}{35}$$

+++