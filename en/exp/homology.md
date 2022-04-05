Homology describes the shape of a space in a really amazing way. At first it seems strange and confusing, but after a careful study, it comes implicit in a lot of mathematical phenomena. For instance, in the Euler-Poincaré Characteristic: we take some space, triangulate it (break it up in "small pieces") and compute the alternate sum of the number of pieces of each dimension:

$$\chi(X)=\sum_i (-1)^i c_i(X)$$

where $c_i(X)$ is the number of $i$-dimensional "faces" of $X$. Surprisingly enough, it does not depend on the chosen triangulation

<table>
  <thead>
    <tr>
      <td c cs=2>$X$</td>
      <td c>$c_0$ vertices</td>
      <td c>$c_1$ edges</td>
      <td c>$c_2$ faces</td>
      <td c>$\chi=c_0-c_1+c_2$</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td c>{{ image | point }}</td>
      <td c>{{ image | point }}</td>
      <td c>1</td>
      <td c>-</td>
      <td c>-</td>
      <td c>1</td>
    </tr>
    <tr>
      <td c rs=2>{{ image | curve }}</td>
      <td c>{{ image | curve_4 }}</td>
      <td c>4</td>
      <td c>3</td>
      <td c>-</td>
      <td c rs=2>1</td>
    </tr>
    <tr>
      <td c>{{ image | curve_7 }}</td>
      <td c>7</td>
      <td c>6</td>
      <td c>-</td>
    </tr>
    <tr>
      <td c rs=2>{{ image | circ }}</td>
      <td c>{{ image | circ_5 }}</td>
      <td c>5</td>
      <td c>5</td>
      <td c>-</td>
      <td c rs=2>0</td>
    </tr>
    <tr>
      <td c>{{ image | circ_9 }}</td>
      <td c>9</td>
      <td c>9</td>
      <td c>-</td>
    </tr>
    <tr>
      <td c rs=3>{{ image | disc }}</td>
      <td c>{{ image | disc_5 }}</td>
      <td c>5</td>
      <td c>5</td>
      <td c>1</td>
      <td c rs=3>1</td>
    </tr>
    <tr>
      <td c>{{ image | disc_9 }}</td>
      <td c>9</td>
      <td c>9</td>
      <td c>1</td>
    </tr>
    <tr>
      <td c>{{ image | disc_5c }}</td>
      <td c>6</td>
      <td c>10</td>
      <td c>5</td>
    </tr>
    <tr>
      <td c rs=3>{{ image | sphere_ep }}</td>
      <td c>{{ image | cube_ep }}</td>
      <td c>8</td>
      <td c>12</td>
      <td c>6</td>
      <td c rs=3>2</td>
    </tr>
    <tr>
      <td c>{{ image | oct_ep }}</td>
      <td c>6</td>
      <td c>12</td>
      <td c>8</td>
    </tr>
    <tr>
      <td c>{{ image | icos_ep }}</td>
      <td c>12</td>
      <td c>30</td>
      <td c>20</td>
    </tr>
    <tr>
      <td c rs=2>{{ image | torus_ep }}</td>
      <td c>{{ image | torus_cub_ep }}</td>
      <td c>32</td>
      <td c>64</td>
      <td c>32</td>
      <td c rs=2>0</td>
    </tr>
    <tr>
      <td c>{{ image | torus_6_ep }}</td>
      <td c>36</td>
      <td c>72</td>
      <td c>36</td>
    </tr>
  </tbody>
</table>

However, this characteristic is also expressed in homological terms (with no need of triangulation), and this is the proper way indeed. So homology effectively describes the shape of a topological space

$$\chi(X)=\sum_i (-1)^i \text{rk }H_i(X)=\sum_i (-1)^i b_i(X)$$

where $b_i=\text{rk }H_i(X)$ are the _Betti numbers_

<table>
  <thead>
    <tr>
      <td c>$X$</td>
      <td c>$b_0$</td>
      <td c>$b_1$</td>
      <td c>$b_2$</td>
      <td c>$\chi=b_0-b_1+b_2$</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td c>{{ image | point }}</td>
      <td c>1</td>
      <td c>-</td>
      <td c>-</td>
      <td c>1</td>
    </tr>
    <tr>
      <td c>{{ image | curve }}</td>
      <td c>1</td>
      <td c>0</td>
      <td c>-</td>
      <td c>1</td>
    </tr>
    <tr>
      <td c>{{ image | circ }}</td>
      <td c>1</td>
      <td c>1</td>
      <td c>-</td>
      <td c>0</td>
    </tr>
    <tr>
      <td c>{{ image | disc }}</td>
      <td c>1</td>
      <td c>0</td>
      <td c>0</td>
      <td c>1</td>
    </tr>
    <tr>
      <td c>{{ image | sphere_ep }}</td>
      <td c>1</td>
      <td c>0</td>
      <td c>1</td>
      <td c>2</td>
    </tr>
    <tr>
      <td c>{{ image | torus_ep }}</td>
      <td c>1</td>
      <td c>2</td>
      <td c>1</td>
      <td c>0</td>
    </tr>
  </tbody>
</table>

---

Our goal is to understand the shape of a space. How shall we distinguish a sphere from a torus? Homology has a clear motto:

**FIND SOMETHING WITHOUT BOUNDARY, THAT IS NOT THE BOUNDARY OF ANYTHING**

and... it works! Of course, objects with boundary (e.g. open curves) aren't very useful, they may move wildly

{{ image | sphere_torus_boundary }}

but objects without boundary... closed objects... these may be more meaningful

{{ image | sphere_torus_no_boundary }}

In the sphere, a curve without boundary is always the boundary of something... but in the torus we have a curve without boundary that is not the boundary of anything. This is a true difference! It seems to work!

{{ image | sphere_torus_is_boundary }}

Generally speaking, these objects without boundary that are not the boundary of anything catch "holes" in different dimensions... the holes of dimension 0 are unconnected components, the holes of dimension 1 may be surrounded by a loop, whereas those of dimension 2 may be enclosed by surfaces...

{{ image | homology }}

But one could argue, "isn't the loop in the torus the boundary of the rest of the torus?"

{{ image | torus_loop_boundary }}

Well... we're talking about the boundary without knowing exactly what it is... So let's spend some time to define the _boundary operator_ $\partial$

---

To define the **boundary operator** $\partial$, we'll proceed one step at a time:

<ol>
  <li>
    $\partial$ maps objects of dimension $k$ to objects of dimension $k-1$, always one dimension below

    {{ image | boundary_operator_non_oriented }}

    Objects of dimension 0 are points, those of dimension 1 are curves, those of dimension 2 are surfaces... The set of "objects of dimension $k$" will be denoted $C_k(X)$, so we have

    $$\partial:C_k(X)\longrightarrow C_{k-1}(X)$$

    for every $k\geqslant 0$ (the boundary of a point is nothing, or more algebraically stated, is 0)
  </li>
  <li>
    The boundary of something has no boundary (is 0). We may convince ourselves with the examples above. Algebraically, we express it like this

    $$\partial^2=0$$

    and is such an important and ubiquitous property in mathematics that gives rise to the whole field of _Homological Algebra_
  </li>
  <li>
    For this to work well, all the objects must be _oriented_. The very concept of orientation is very subtle; for now it will be some additional property that takes two opposite values ("one the negative of the other one")

    <ul>
      <li>Points will be labelled as $+$ or $-$</li>
      <li>Curves have a direction</li>
      <li>Surfaces are painted blue in one face and yellow in the other face; blue denotes _counterclockwise_ rotation and yellow denotes _clockwise_ rotation</li>
      <li>Volumes have some sort of "helicity"...</li>
    </ul>

    and this, of course, is taken into account by the boundary operator! A curve starts in a $-$ point and ends in a $+$ point; the spin in the surfaces must match the direction of the boundary curve...

    {{ image | boundary_operator }}

    Why is this a key fact for the boundary operator? Because this way $\partial$ works perfect when dividing objects

    {{ image | boundary_operator_division }}

    Great! Equal objects with different orientation act as opposite and cancel out. So everything works with a marvelous algebraic taste. Moreover, this clarifies the problem we had with the torus: if we cut the torus, each edge of the surface adds a boundary, but since they have opposite orientations, they cancel out!

    {{ image | cut_torus_boundary }}

    So it is true: the beforementioned loop is not the boundary of anything
  </li>
</ol>

---

So we should find objects without boundary that are not the boundary of something. We'll consider three groups:

<ul>
  <li>$C$: objects (with or without boundary)</li>
  <li>$Z$: objects without boundary</li>
  <li>$B$: objects without boundary that are also the boundary of something</li>
</ul>

And the inclusion $B\subset Z\subset C$ holds. Apparently, the set $Z\smallsetminus B$ is the interesting one. But... is this the best approach, the most "mathematical"?

Let's think for a moment in the whole numbers $\mathbb{Z}$. Among the whole numbers there is a "phenomenon", that of _being multiple of $5$_. This phenomenon is interesting precisely because the are whole numbers that are _not_ multiple of $5$. We may think of it as if $Z=\mathbb{Z}$ and $B=5\mathbb{Z}$ the multiples of $5$. One may show the fact that there are numbers that are not multiples of $5$ examining the set

$$Z\smallsetminus B=\{\cdots,-6,-4,-3,-2,-1,1,2,3,4,6,7,8,9,11,12,13,14,\cdots\}$$

But for a mathematician, working with this set is very annoying. It isn't even closed for the sum ($2$ and $3$ are in $Z\smallsetminus B$ but $2+3=5\not\in Z\smallsetminus B$), there is no interesting structure for this set. So let's consider a totally different approach

$1$ and $6$ are both non-multiples of $5$, and are distinct, but it could be said that both express the same _not-being-multiple-of-$5$_, because both are of type $5k+1$. Perhaps we could abstract the number and consider the _class_, so we'll say

$$[1]=[6]\qquad\text{ because }\qquad 1-6\in B=5\mathbb{Z}$$

In the very same spirit, we define

$$[a]=[b]\qquad\text{ if }\qquad a-b\in B=5\mathbb{Z}$$

This gives rise to five classes, making up $\mathbb{Z}_5=\{[0],[1],[2],[3],[4]\}$, which happens to be extremely rich from a structural point of view: not only is it closed for the sum and product modulus $5$, which constitutes the set as a _group_ and a _ring_, but it is also a _finite field_. And this procedure is standard in mathematics: it is the quotient $Z/B$.

So the right point of view, also for the homology, is not substraction $Z\smallsetminus B$, but quotient $Z/B$. Some examples will corroborate how useful is this procedure

---

Let $C_k(X)$ be the set of objects of dimension $k$ inside $X$. Since we are interested in an algebraic approach, we'll work with (formal) linear combinations that we may add and substact easily. That is, elements of $C_k(X)$ may be of the form

{{ image | chains }}

where $\lambda_i$, $\mu_j$, $\eta_k$ are whole numbers. These are called _chains_. We keep in mind that a negative "amount" of objects is equivalent to a change of orientation, as discussed above: swapping $-$ and $+$, inverting the direction of a curve, interchanging blue and yellow... So the boundary operator $\partial$ is better seen as a linear operator

$$\partial_k:C_k(X)\longrightarrow C_{k-1}(X)$$

which satisfies $\partial_{k-1}\circ\partial_k=0$ (or more succinctly $\partial^2=0$). This implies

$$\text{im }\partial_{k+1} \subset\text{ker }\partial_k$$

and it makes sense to define

$$Z_k(X)=\text{ker }\partial_k$$
$$B_k(X)=\text{im }\partial_{k+1}$$

(called _cycles_ and _boundaries_ respectively) and yes, $B_k(X)\subset Z_k(X)\subset C_k(X)$. And in this context, we define the **homology groups**

$$H_k(M)=\dfrac{\text{ker }\partial_k}{\text{im }\partial_{k+1}}=\dfrac{Z_k(M)}{B_k(M)}$$

Strange? Somewhat. But extremely useful. The homology groups are made up by homology classes, that merge _homologous cycles_, that is, cycles whose difference is a boundary. And, as a matter of fact, homologous cycles, those whose difference is a boundary, are precisely those that catch the same "hole". Astonishing, isn't it? So astonishing that has fascinated and keeps fascinating all sort of scientists over decades

{{ image | boundaries }}

---

Let's explore some concrete examples of homology. The simplest homology to be computed is homology of order zero, _which detects the number of (path) connected components in the space_. Why? For $k=0$, each element of $C_0(X)$ is just an integer-valued sum of points in $X$, for instance $\sigma=7p-3q$, $p$, $q\in X$. Points have no boundary, so $\partial_0:C_0(X)\longrightarrow 0$ is the null map and $Z_0(X)=C_0(X)$. On the other hand, $\partial_1:C_1(X)\longrightarrow C_0(X)$ maps each open path to a pair of points, one point with a $+$ sign and the other one with a $-$ sign. And any such pair of points belongs to the image of $\partial_1$ as long as there is some path in $X$ from the $-$ point to the $+$, that is, as long as they're in the same connected component! As a consequence, in $H_0(X)=Z_0(X)/B_0(X)$ we're free to move a point inside its component, as shown in the picture above, and we may also cancel out $+$ and $-$ points in the same component. This being so, each homological class in $H_0(X)$ assigns a net number of points to each component, and thus $H_0(X)\simeq \mathbb{Z}^n$, where $n$ is the number of connected components of the space. Fantastic, isn't it?

{{ image | homology_connected_components }}

In the very same spirit, $H_1(X)$ detects holes surrounded by a loop. The quotient ensures that different loops enclosing the same hole belong to the same class

{{ image | homologous_loops }}

Now we can reason the homology of simple spaces 

<table>
  <thead>
    <tr>
      <td c>$X$</td>
      <td c>$H_0(X)$</td>
      <td c>$H_1(X)$</td>
      <td c>$H_2(X)$</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td c>{{ image | point }}</td>
      <td c>$\mathbb{Z}$</td>
      <td c>-</td>
      <td c>-</td>
    </tr>
    <tr>
      <td c>{{ image | curve }}</td>
      <td c>$\mathbb{Z}$</td>
      <td c>0</td>
      <td c>-</td>
    </tr>
    <tr>
      <td c>{{ image | circ }}</td>
      <td c>$\mathbb{Z}$</td>
      <td c>$\mathbb{Z}$</td>
      <td c>-</td>
    </tr>
    <tr>
      <td c>{{ image | disc }}</td>
      <td c>$\mathbb{Z}$</td>
      <td c>0</td>
      <td c>0</td>
    </tr>
    <tr>
      <td c>{{ image | sphere_ep }}</td>
      <td c>$\mathbb{Z}$</td>
      <td c>0</td>
      <td c>$\mathbb{Z}$</td>
    </tr>
    <tr>
      <td c>{{ image | torus_ep }}</td>
      <td c>$\mathbb{Z}$</td>
      <td c>$\mathbb{Z}^2$</td>
      <td c>$\mathbb{Z}$</td>
    </tr>
  </tbody>
</table>

---

Even in the simplest spaces, the sets $C_k(X)$, $Z_k(X)$, $B_k(X)$ are usually extremely big. Think, for instance, that $C_1(X)$ contains all functions $f:[0,1]\longrightarrow X$ - that's _huge_. So there is a "lighter" version of homology, called _simplicial homology_ (which will be marked with a $\Delta$), that works for triangulated spaces, and that compute the very same homology groups (i.e. isomorphic). The idea is simple: use only objects of the triangulation. So $C^\Delta_0(X)$ consists of integer-valued combinations of vertices, $C^\Delta_1(X)$ consists of integer-valued combinations of oriented edges, and so on. Everything else is the same and works fine:

$$\partial^\Delta_k:C^\Delta_k(X)\longrightarrow C^\Delta_{k-1}(X)$$
$$Z^\Delta_k(X)=\text{ker }\partial^\Delta_k$$
$$B^\Delta_k(X)=\text{im }\partial^\Delta_{k+1}$$
$$H^\Delta_k(M)=\dfrac{Z^\Delta_k(M)}{B^\Delta_k(M)}$$

And yes, it computes the very same homology groups, it detects the very same holes! But now we're only working with finite dimensional spaces (provided that the triangulation is finite) which behave much better. We may _compute_ the simplicial homology groups. But since a space has many triangulations... we would like to have an "absolute" homology, which is the one described above. It is the _singular homology_, and it is one of the finest constructions in mathematics

And all this digression comes back to the Euler-Poincaré characteristic. How? Since we are now working with finite dimensional vector spaces (well, they're not vector spaces, because we're working over $\mathbb{Z}$, but it doesn't matter - we'll use rank $\text{rk}$ as the analogous of $\text{dim}$), usual linear algebra applies. In the one hand, 

$$H_k=Z_k/B_k\Longrightarrow \text{rk }H_k=\text{rk }Z_k-\text{rk }B_k$$

but on the other hand, 

$$B_{k-1}=\text{im }\partial_k\simeq C_k/\text{ker }\partial_k=C_k/Z_k$$
$$\text{rk }B_{k-1}=\text{rk }C_k-\text{rk }Z_k$$

and this necessarily holds along the whole chain

{{ image | homology_chain_dimensions }}

Plugging this into the Euler-Poincaré characteristic, we have

$$
\begin{array}{rcl}
\chi & = & \sum_i (-1)^i c_i \\
& = & \sum_i (-1)^i \text{rk }C_i \\
& = & \sum_i (-1)^i (\text{rk }Z_i + \text{rk }B_{i-1}) \\
& & \text{[index trick: \(\sum_i (-1)^i\text{rk }B_{i-1} = -\sum_i (-1)^i\text{rk }B_i\)]} \\
& = & \sum_i (-1)^i (\text{rk }Z_i - \text{rk }B_i) \\
& = & \sum_i (-1)^i \text{rk }H_i \\
\end{array}
$$

_The result above is very deep_: the quantities $c_i$ depend on the specific triangulation of the space $X$, but the Euler-Poincaré characteristic $\chi$ _does not depend_ on the triangulation, and therefore constitutes a topological invariant, because it may be expressed in terms of homology. And as a side note, it shows that homology, no matter how strange seemed at first, is of crucial importance in algebraic topology