Given two points $A$ and $B$ and a circle $c$, draw another circle that passes through $A$ and $B$ and cuts $c$ in diametrically opposite points 

{{ image | two_points_circle_diametrically_opposite }}

+++
Solution
+++

The key to this problem is the following auxiliary result: given $A$ and $c$, any circle passing through $A$ and cutting $c$ in diametrically opposite points necessarily passes through $\tilde{A}$ too, where $\tilde{A}$ is the reflection (with respect to the center of $c$, $O$) of the [inversion]( app | circle_inversion ) of $A$; that is: $O$ lies in $\overline{A\tilde{A}}$ and 

$$\overline{AO}\cdot\overline{O\tilde{A}}=r^2$$

{{ image | two_points_circle_diametrically_opposite_conjugate }}

This auxiliary result is most easily proved by means of [circle powers]( exp | circle_power ): if $P$ and $Q$ are diametrically opposite points in $c$, then

$$\overline{AO}\cdot\overline{O\tilde{A}}=\overline{PO}\cdot\overline{OQ}$$

and thus $A$, $\tilde{A}$, $P$ and $Q$ are concyclical, i.e. there exists a circle containing the four of them  (the picture takes $r=1$)

{{ image | two_points_circle_diametrically_opposite_power }}

An alternative and smart proof may be found by means of the stereographic projection, associating $c$ with the equator of the sphere: this involves antipodal points and great circles - check it out!

The solution to the original problem is now strightforward: find $\tilde{A}$ and $\tilde{B}$, and draw the circle passing through all four points

{{ image | two_points_circle_diametrically_opposite_construction }}

+++