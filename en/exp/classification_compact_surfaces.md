A surface is a manifold of dimension 2. For example:

<ul>
<li>The sphere $\S^2=\{(x,y,z)\in \mathbb{R}^3 \, \vert \,x^2+y^2+z^2=1\}$</li>
<li>The torus $\T^2=\{(x,y,z)\in \mathbb{R}^3 \, \vert \, (\sqrt{x^2+y^2}-2)^2+z^2=1\}$</li>
</ul>

{{ image | sphere_torus }}

In fact, from a regular equation $S=\{(x,y,z) \, \vert \, F(x,y,z)=0\}$ in $\mathbb{R}^3$ we always get a surface. Being regular means that $\nabla F(x,y,z) \neq 0$, $\forall (x,y,z)\in S$.

Given two surfaces $M_1$ and $M_2$, we may build their connected sum: just make two holes and glue the boundaries. We call it $M_1 \# M_2$

{{ image | connected_sum }}

Of course, the connected sum of two surfaces is a surface again!

{{ image | connected_sum_local }}

So we have double torus, triple torus... in general we speak about tori of genus $g$ (and we denote them by $\Sigma_g$)

{{ image | g_torus }}

Are these all the possibilities for surfaces? Let's see

To warm-up, let's see other surfaces, some of them with boundary. Sometimes we can get it by gluing the sides of some polygons.

When gluing two sides of a square with the same orientation, we get a cylinder

{{ image | square_cylinder }}

But if we change the orientation of one of the sides, we get a Möbius strip

{{ image | square_mobius }}

The cylinder and the Möbius strip cannot be the same surface, because the cylinder has two circles as boundary, whereas the Möbius strip has only one.

By gluing polygons we may also create closed surfaces. The torus for example

{{ image | square_torus }}

And soon we come to know a more complex surface: the Klein bottle

{{ image | square_klein }}

We cannot take it into space without crossings! But there are no boundaries nor breaks, so this is a fledged closed surface.

An even stranger surface: the projective plane

{{ image | projective_plane_manifold width = 480 }}

We get it by identifying the opposite points in a sphere, or when identifying the points in the boundary of a disc like in the figure

{{ image | sphere_opposite_identification }}

In fact, all the surfaces we come across may be obtained by gluing the sides of a polygon. For instance, the connected sum of two surfaces made with one polygon each is also made with another polygon

{{ image | connected_sum_polygon }}

This is the case of the double torus

{{ image | double_torus_polygon }}

When dealing with the pasting of the sides of a polygon, we use 'words'

{{ image | polygon_word }}

Just by taking the sides of the polygon in the right order; wrong direction arrows are signed with a $-1$

Now we know lots of surfaces made up by gluing polygons

<ul>
<li>The torus $\T^2$: $aba^{-1}b^{-1}$</li>
<li>The double torus $\T^2 \# \T^2$: $aba^{-1}b^{-1}cdc^{-1}d^{-1}$</li>
<li>The torus of genus $g$ $\Sigma_g$: $a_1 b_1 a_1^ {-1}b_1^{-1}\cdots a_gb_ga_g^{-1}b_g^{-1}$</li>
<li>The Klein bottle $Kl$: $abab^{-1}$</li>
<li>The projective plane $\mathbb{R}P^2$: $aa$</li>
</ul>

And symbolically $S^2$: $aa^{-1}$

{{ image | sphere_planar_representation }}

Before computing and proving that the word method is useful for classifying the compact surfaces, we need some remarks.

<ol>
<li>
The projective plane is the union along the boundary of a Möbius band and a disc 

{{ image | projective_plane_mobius_disc }}

Indeed, we remove a disc and glue...

{{ image | projective_plane_mobius_disc_decomposition }}
</li>
<li>
The Klein bottle is the union of two Möbius bands along the boundary, and hence the connected sum of two projective planes

{{ image | klein_bottle_halves width = 480 }}

We also may check it with cut-and-paste diagrams

{{ image | klein_bottle_two_mobius_strips_decomposition }}
</li>
<li>
The connected sum of a torus and a projective plane is the same as the connected sum of a Klein bottle and a projective plane. But since the Klein bottle is equal to the connected sum of two projective planes, both of the previous objects are equal to the connected sum of three projective planes
    
But why? First of all, making a connected sum with a torus is like attaching a 'handle'

{{ image | torus_handle }}

And making a connected sum with a Klein bottle is also like attaching a 'handle', but with reversal directions!

{{ image | klein_bottle_handle }}

And when working with a projective plane... then everything is the same, because inside the projective plane there is a Möbius strip

{{ image | mobius_strip_handle }}
</li>
</ol>

Altogether we may think the following: we make connected sums of tori, connected sums of projective planes... but with the connected sums of tori and projective planes there is nothing new, because it is a connected sum of projective planes again! This inspires us to conjecture the

**Theorem of Classification of Compact Surfaces**

Any compact and connected surface belongs to one these three groups:

<ul>
<li>The sphere $S^2$</li>
<li>The connected sum of $g$ tori (or torus of genus $g$) $\Sigma_g$</li>
<li>The connected sum of $k$ projective planes (called $X_k$)</li>
</ul>

and all these surfaces are mutually different, having therefore a complete classification

**Proof**

At this moment we will not prove that all these surfaces are inequivalent; this requires more powerful tools and we will come back when studying the foundamental group (it is not enough to say that these surfaces 'look' different: the connected sums of a projective plane and a torus and of a projective plane and a Klein bottle are equal!)

First step: a surface may be always divided into tiny polygons that reconstruct the surface when suitably glued, like in the following torus

{{ image | torus_triangulation width = 480 }}

(Be careful! It may seem simple, and with surfaces it is, but to do something similar in higher dimensions is difficult... and even may be impossible!) We would have something like this

{{ image | surface_polygons_decomposition }}

Perhaps we have many little pieces... if we have two different polygons with an edge to be glued, we may glue it and reduce the number of pieces

In the end, if we have done everything ok... we should have only one polygon. If we have more than one polygon with no edges to be glued in different polygons, then when we glue everything each polygon makes its own surface... but our surface is connected, isn't it?!

And when we have our polygon, is every gluing possible? Well, the sides have to be paired. A side without pair means a border in the surface, and if we glue more than two edges together, we would end up with something like

{{ image | surface_multiple_gluing width = 480 }}

That's no surface at all!

Having all these things in mind, we proceed by steps

**STEP 1:** We have to look for letters that appear twice in the same sense, that is, something like $ap_1ap_2$. Then there is some Möbius strip... it looks like we were going to be able to extract a projective plane as connected sum... exactly! Just some cut-and-paste

{{ image | projective_plane_cut_and_paste }}

By repeating this process if necessary, we 'isolate' the projective planes and we get a word like $a_1a_1\cdots a_ka_kp$, where in $p$ each pair of edges has opposite orientation

**STEP 2:** Now we choose (if we have not finished) a pair of opposite-directed edges, $ap_1a^{-1}p_2$. We will choose them to be the nearest possible. They may even be adjacent! But then we are very lucky, because we may simplify the gluing and get rid of a letter

{{ image | simplify_words }}

In the extreme case, our surface may be $aa^{-1}$. That's a sphere! But suposing the general case that the $a$ sides are not adjacent, we will find some other $b$ inbetween. Its pair $b^{-1}$ must be located in the other side between $a$ and $a^{-1}$, because those were chosen to be the nearest possible. So we have four edges that resemble those of a torus... and we may isolate it again

{{ image | torus_cut_and_paste }}

Finally, repeating the process, we isolate all the tori until there remains nothing. So we have: our surface is a sphere, or the connected sum of projective planes, or the connected sum of tori, or the connected sum of both projective planes and tori, which we know to be in fact a connected sum of projective planes. So endly we may conclude that our classification is true.