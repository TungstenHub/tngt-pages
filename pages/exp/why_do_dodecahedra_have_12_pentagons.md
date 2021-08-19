[{intro}]

>>>
This article has been written for [**3b1b Summer of Math Exposition #1**](https://www.3blue1brown.com/blog/some1) ::memo::
<<<

Brilliant maths ::sparkles:: usually come from stupid questions.

Today's stupid question is: **_why do dodecahedra have 12 pentagons?_**

---
[{statement}]

Here's your favorite dodecahedron, with exactly 12 pentagons.

{{ threejs | dodecahedron }}

We all know that dodecahedra have 12 pentagons, but one could ask _why_. Why 12, and not 11 or 13? Can we arrange something similar with only 9 pentagons? We may try, but there seems to be no other way to create such regular solid.

Imagine you're given a bunch of pentagons and someone asks you to assemble them so that in each corner three pentagons meet. Since the angles of a pentagon ($108^\circ = \frac{3\pi}{5}$) do not cover a third of a full $2\pi$ angle ($120^\circ = \frac{2\pi}{3}$), it becomes necessary to bring the pentagons into space and the construction progressively encloses a certain spherical region. And it is with the twelfth pentagon that the polyhedron is completely closed. 

But for a mathematical mind, this means that the number 12 should be somehow _derivable_ from the initial information of pentagons, meeting three at each vertex. Had you ever thought about this? No? Really?

It is clear that the defect of angle is the responsible for the rounding. If we could somehow _measure_ this rounding, i.e. how much of the sphere is covered in our pentagon folding, we would be able to guess how many pentagons are needed to cover all the sphere.

{{ image | dodec_sphere_rounding }}

But it is not clear at all how to relate angles and rounding.

---
[{inflating}]

One of the reasons why it is unclear how to relate angles and rounding is the fact that the dodecahedron is still too sharp, too rigid. It doesn't seem a sphere! But that's no problem for mathematicians as long as our imagination is full with original ideas ::unicorn:: so we just inflate our dodecahedron. Why not?

{{ threejs | inflated_dodecahedron }}

Great! What else?

Our pentagons are somewhat strange now. Its angles no longer measure $108^\circ = \frac{3\pi}{5}$, but $120^\circ = \frac{2\pi}{3}$. That's more than it should be. 

You know, the angles of a plane triangle always add to $\pi$:

{{ d3js | sum_angles_triangle }}

And the angles of a plane pentagon always add to $3\pi$:

{{ image | polygon_angle_sum }}

And in general the angles of a plane $k$-gon add to $(k-2)\pi$. But spherical polygons seem to behave quite differently. Look what happens when we inflate the other regular polyhedra! Angles become shamelessly big.

{{ threejs | tetrahedron          stack = 2 }}
{{ threejs | inflated_tetrahedron stack = 2 }}
{{ threejs | hexahedron           stack = 2 }}
{{ threejs | inflated_hexahedron  stack = 2 }}
{{ threejs | octahedron           stack = 2 }}
{{ threejs | inflated_octahedron  stack = 2 }}
{{ threejs | icosahedron          stack = 2 }}
{{ threejs | inflated_icosahedron stack = 2 }}

The angles of a spherical $k$-gon do _not_ add to $(k-2)\pi$. They add _more_. But how much more? It seems that bigger polygons are allowed to exceed much more the plane measure, doesn't it? But that's rather vague, and maths aren't vague; they are extremely precise and beautiful, like in the following amazing theorem: 

>>>
**Girard's Theorem:** The area of a spherical triangle with angles $\alpha$, $\beta$ and $\gamma$ is $\alpha + \beta + \gamma - \pi$, that is, its angle excess. 
<<<

{{ threejs | girard_theorem }}

(oh ::scream:: it has some delightful resemblance to [the traveller machine in _Contact_ movie]( https://i.imgur.com/ZUAfjSx.jpg )!!)

+++
(Sketch of) Proof of Girard's Theorem
+++

Given a spherical triangle $T = \triangle PQR$, the prolongation of its sides to great circles gives rise to a decomposition of the sphere in 8 disjoint triangles: 

<ul>
  <li>The initial triangle $T$</li> 
  <li>The inverted triangle $T' = \triangle P'Q'R'$, where $P'$, $Q'$ and $R'$ are the reflections of $P$, $Q$ and $R$ through the center of the sphere</li> 
  <li>
    Three adjacent triangles:

    <ul>
      <li>$A = \triangle P'QR$</li>
      <li>$B = \triangle PQ'R$</li>
      <li>$C = \triangle PQR'$</li>
    </ul>
  </li>
  <li>
    And its inverted counterparts:

    <ul>
      <li>$A' = \triangle PQ'R'$</li>
      <li>$B' = \triangle P'QR'$</li>
      <li>$C' = \triangle P'Q'R$</li>
    </ul>
  </li>
</ul>

The union of any two touching triangles is delimited by two great circles, and is thus a _lune_, whose area is proportional to the angle at which the great circles meet. It is indeed two times such angle, since a full angle of $2\pi$ would correspond to the area of the whole sphere, which is $4\pi$. This way (naming the area of each triangle after the name of the triangle itself)

$$T + A = 2\alpha$$
$$T + B = 2\beta$$
$$T + C = 2\gamma$$

and summing up,

$$3T + A + B + C = 2(\alpha + \beta + \gamma)$$

On the other hand, the areas of the eight triangles sum the total area of the sphere, $4\pi$:

$$T + A + B + C + T' + A' + B' + C' = 4\pi$$

and since inverted triangles have the same area, we have indeed

$$T + A + B + C = 2\pi$$

Subtracting both expressions we end up with

$$2T = 2(\alpha + \beta + \gamma) - 2\pi$$

that is,

$$T = \alpha + \beta + \gamma - \pi$$

+++

Wonderful!! We finally have a way to _measure_. And with the same additive argument as before, we may state that _the area of a spherical polygon is the quantity in which the sum of the angles exceedes $(k-2)\pi$_.

{{ image | spherical_polygon_angle_sum }}

But before diving into our original problem... let's explore a completely unexpected math connection ::light_bulb::

---
[{gauss_bonnet}]

Mathematicians are experts in developing new theories and results just by _seeing the same phenomenon from another point of view_. Ready?

The angles of spherical $k$-gons add to more than $(k-2)\pi$. But we could also say: they _turn less_.

Imagine you're driving a car. You go around a block and stop in the same place where you started. For this to happen, the car must have turned somewhere. And not just a little bit: the car must have pointed towards any direction in a full $2\pi$ turn during the way. On the whole, you have turned $2\pi$.

If you travel the border of a plane polygon, you still have to turn $2\pi$, only that this time the turns are very abrupt, concentrated in the vertices. If a vertex has angle $\alpha$, the turn is $\pi-\alpha$. If the angles of a $k$-gon add to $(k-2)\pi$, then the total turn is 

$$
\begin{array}{rcl}
(\pi-\alpha_1) + (\pi-\alpha_2) + \cdots + (\pi-\alpha_k) 
& = & k\pi - (\alpha_1 + \alpha_2 + \cdots + \alpha_k) \\
& = & k\pi - (k-2)\pi \\
& = & 2\pi
\end{array}
$$

It makes sense, doesn't it?

{{ image | polygon_path_2pi_turn }}

But the new point of view, even if mathematically equivalent, is much more meaningful and useful: there is a turn of $2\pi$, for every polygon border, _independently of the number of sides_. And when the number of sides gets bigger and bigger, the polygons may faithfully approximate curves - we may thus speak of turning in curves, like with the car.

In the sphere, by contrast, polygons turn less. How much less? Well, the _excess_ of angle sum is exactly the _defect_ of angle turn - so the area of a spherical polygon is the amount in which the border of the polygon turns less than $2\pi$. And with more and more sides we can extend it to curves. How can that happen? This must be a phenomenon related to the surface of the sphere being somehow curved! Don't you feel the presence of a very special result?

>>>
**Gauss-Bonnet Theorem (base & non-technical statement!):** Let $\gamma$ be a closed curve enclosing a simple region $R$ in a surface. Then the total turn of $\gamma$ (measured with the _geodesic curvature_) is $2\pi$ minus the total amount of surface curvature in the enclosed region:

$$\int_{\gamma} k_g\d s = 2\pi - \int_R K \d A$$
<<<

This theorem is very deep and has lots of concepts that should be made precise. But in our case it translates as follows: the sphere surface is curved (with constant positive curvature $K=1$!), so a curve in the sphere turns less than $2\pi$, according to the area of the enclosed region. An extreme case is the equator: it doesn't turn at all (it is a _geodesic_!) while enclosing an hemisphere of area $2\pi$.

It is a very interesting exercise to check this theorem for spherical caps... and we wouldn't like to ruin the reader's marvelous opportunity to check it on their own ::smirk:: so here's a sketch with the main steps to have into account. Good luck! 

{{ image | gauss_bonet_spherical_cap }}

---
[{formula_derivation}]

Let's go back to our main problem! We now have all the ingredients to derive all possible regular polyhedra ::alembic::

Suppose we want to build a regular polyhedron using

<ul>
  <li>Regular $k$-gons</li>
  <li>Meeting $v$ at each vertex</li>
  <li>And using $n$ of them</li>
</ul>

Since $v$ rounded polygons are meeting at each vertex, their inner angles are $\frac{2\pi}{v}$ and the turn is $\pi - \frac{2\pi}{v} = \pi \left(1-\frac{2}{v}\right)$. After $k$ vertices, the total turn of the rounded polygon would be $k\pi \left(1-\frac{2}{v}\right)$, which will be presumably less than the expected $2\pi$ for a plane polygon. The difference

$$2\pi-k\pi \left(1-\frac{2}{v}\right)$$

is the area of the rounded polygon and, since there are $n$ of them, we have

$$n\left(2\pi-k\pi \left(1-\frac{2}{v}\right)\right) = 4\pi$$

or equivalently

$$\frac{2}{k} + \frac{2}{v} = 1 + \frac{4}{nk}$$

This equation dramatically reduces the number of possibilities: $k$ and $v$ are at least $3$, but they can't be too high if $\frac{2}{k} + \frac{2}{v}$ is to be greater than $1$. 

Let's try!! For the dodecahedron, $k$ would be $5$ and $v$ would be $3$, so

$$\frac{2}{5} + \frac{2}{3} = \frac{16}{15} = 1 + \frac{4}{5n} \Longrightarrow \frac{4}{5n} = \frac{1}{15} \Longrightarrow n = \frac{4\times 15}{5} = 12$$

Ohhh!! Amazing!! ::tada:tada:tada:heart:: we finally know where does the 12 come from.

All the other combinations lead to the other regular polyhedra:

<table>
  <thead>
    <tr>
      <td c>Polyhedron</td>
      <td c>$\quad k \quad$</td>
      <td c>$\quad v \quad$</td>
      <td c>$n$</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td c>Tetrahedron</td>
      <td c>$3$</td>
      <td c>$3$</td>
      <td>$\frac{2}{3} + \frac{2}{3} = 1 + \frac{4}{3n} \Longrightarrow \hl{n=4}$</td>
    </tr>
    <tr>
      <td c>Octahedron</td>
      <td c>$3$</td>
      <td c>$4$</td>
      <td>$\frac{2}{3} + \frac{2}{4} = 1 + \frac{4}{3n} \Longrightarrow \hl{n=8}$</td>
    </tr>
    <tr>
      <td c>Icosahedron</td>
      <td c>$3$</td>
      <td c>$5$</td>
      <td>$\frac{2}{3} + \frac{2}{5} = 1 + \frac{4}{3n} \Longrightarrow \hl{n=20}$</td>
    </tr>
    <tr>
      <td c>Hexahedron (cube)</td>
      <td c>$4$</td>
      <td c>$3$</td>
      <td>$\frac{2}{4} + \frac{2}{3} = 1 + \frac{4}{4n} \Longrightarrow \hl{n=6}$</td>
    </tr>
    <tr>
      <td c>Dodecahedron</td>
      <td c>$5$</td>
      <td c>$3$</td>
      <td>$\frac{2}{5} + \frac{2}{3} = 1 + \frac{4}{5n} \Longrightarrow \hl{n=12}$</td>
    </tr>
  </tbody>
</table>

There are also three more cases in which $\frac{2}{k} + \frac{2}{v} = 1$, which would mean $n = \infty$: $(k=3,\,v=6)$, $(k=4,\,v=4)$ and $(k=6,\,v=3)$. Did you notice? These are the plane tesellations with triangles, squares and hexagons respectively! The polygon angles are just right and the polygons themselves don't curve, so one may allocate infinitely many.

And what if $\frac{2}{k} + \frac{2}{v} > 1$? Negative polygons? Well, almost... polygons lying in a surface of negative curvature. Maybe it's time to meet [the hyperbolic plane and its tesellations]( app | hyperbolic_tesellations ).

Wonderful, isn't it? And all this has come from a "stupid" question ::thinking_face:: 

**Conclusion:** there are no such stupid questions in math. Every question may lead to amazing discoveries ::partying_face:: 

---
[{acknowledgements}]

**Acknowledgements:**

This article makes uses of several great visualization tools that I would like to mention.

<ul>
  <li>3D applets use [**three.js**]( https://threejs.org/ ), a WebGL-based 3D computer graphics library.</li>
  <li>Plane geometry applets use [**D3.js**]( https://d3js.org/ ), an interactive data visualization library.</li>
  <li>Pictures are made with [IPE Drawing Editor](https://ipe.otfried.org/).</li>
  <li>There is no [Manim]( https://www.manim.community/ ) video in this article, but you can see the [resolution of the reduced cubic equation]( exp | reduced_cubic_equation_resolution ) instead ::wink::</li>
</ul>

The source code for this article and its applets is available on [GitHub/TungstenHub](https://github.com/TungstenHub).