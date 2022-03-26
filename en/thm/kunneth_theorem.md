The map

$$
\bigoplus_{a+b=k} H^a(M)\otimes H^b(N)\longrightarrow H^k(M\times N)
$$

is an isomorphism for each $k$, inducing altogether

$$
H^*(M\times N)\simeq H^*(M)\otimes H^*(N),
$$

isomorphism of exterior algebras

+++
Proof
+++

The term _exterior algebra_ refers to the fact that, besides the usual sum, there is a product $\wedge$ mapping a pair of forms into another form, even when the orders differ

This theorem is very useful because it explicitely describes the cohomology of the product space in terms of the cohomology of the factors. For instance, it is now straightforward that $H^0(\T)=\langle[1]\rangle$, $H^1(\T)=\langle[\d \alpha],[\d \beta]\rangle$ and $H^2(\T)=\langle[\d \alpha\wedge\d \beta]\rangle$

A chart of $(p,q)\in M\times N$ may be taken of the form $U\times V \xrightarrow{\varphi\times\psi} M\times N$ with $\varphi$ chart of $p$ in $M$ and $\psi$ chart of $q$ in $N$. Along with this chart we have the base $\{\d x_1,...,\d x_m,\d y_1,...,\d y_n\}$ with which built all the other forms. Then, when a $k$-form in $(\varphi\times\psi)(U\times V)\subset M\times N$ is expressed with respect to this base, each sumand has $a$ components of type $\d x_i$ and $b$ components of type $\d y_j$, where $a+b=k$

All these reasonings may convince ourselves that there is some relation between $\Omega^k(M\times N)$ and $\bigoplus_{a+b=k} \Omega^a(M)\otimes \Omega^b(N)$, and it's true that they're related (they're not equal, though! Just like a function of two variables $f(x,y)$ is not always a product $g(x)h(y)$). Perhaps we may proceed further as in the Poincaré Lemma? Maybe, but look: we now have more powerful tools with which to get a far simpler and smarter solution. It has three steps

<ol>
  <li>
  Let $U\subset M$ be an open set diffeomorphic to $\R ^n$ (and therefore with its same cohomology)

  {{ image | open_sets_induction_1 }}

  Due to the [Poincaré Lemma]( lem | poincare_lemma ),

  $$
  H^k(U\times N) \xrightarrow{s^\ast} H^k(N) \qquad\qquad 
  H^k(U\times N) \xleftarrow{p^\ast} H^k(N)
  $$

  are inverse isomorphisms. But that's equivalent to say that for the manifolds $U$ and $N$ the Künneth Theorem holds

  $$
  \bigoplus_{a+b=k} H^a(U)\otimes H^b(N)\xrightarrow{\simeq}H^k(U\times N)
  $$ 

  since $H^0(U)\simeq\R$, $H^a(U)=0$ for $a>0$

  </li>
  <li>
  This step sounds somewhat strange. We'll prove that whenever for any open sets $U$ and $V$ of $M$, if for $U$, $V$ and $U\cap V$ Künneth Theorem holds (when considering the product with $N$), then it also holds for $U\cup V$

  {{ image | open_sets_induction_2 }}

  The key is the [Mayer-Vietoris sequence]( cor | mayer_vietoris_sequence ). In one hand, we take the Mayer-Vietoris sequence associated to $U$ and $V$, multiply each factor by $H^b(N)$ and perform a direct sum over $a+b=k$. In the other hand, we take the Mayer-Vietoris sequence associated to the open sets $U\times N$ and $V\times N$. Altogether we get the (quite intimidating) diagram:

  {{ image | kunneth_form_five_lemma }}

  The maps $i^*$, $j^*$ and $\d ^*$ are extended in the natural way, and $\Psi$ is the Künneth map. It seems plausible that the rows are still exact and that the diagram is commutative, and it is indeed the case; one should check all the nitty-gritty details, but they're somewhat easy and systematic. 

  Now, the diagram is commutative and its two rows are exact; furthermore, by hypothesis, $\Psi$ is an isomorphism in the first, second, fourth and fifth columns. Applying the [Five Lemma]( lem | five_lemma ), we get that $\Psi$ is an isomorphism in the third column too. That is, the Künneth Theorem holds for the pair $U\cup V$ and $N$
  </li>
  <li>
  In the last step we perform something similar to an induction over open sets. This needs a _good cover_ in our manifold $M$

  {{ image | open_sets_induction_3 }}

  A good cover is an open cover whose open sets are diffeomorphic to $\R ^m$ and such that finite intersections among open sets are diffeomorphic too. At first sight, it seems reasonable that such cover exists (just pick "small and round" open sets), and it is true, but to prove it rigorously is quite complex and technical. If the manifold is compact, a finite open cover exists; the most usual manifolds have a finite good cover too, and only the weirdest need countably many open sets to form a good cover (for instance, the connected sum of infinite tori). Even for these there is a trick: the admit a finite good cover if we let the open sets being diffeomorphic to the (possibly numerable) union of balls in $\R ^m$, that is, the infinite open sets that cover $M$ may be distributed into $l$ grups such that open sets in the same group do not overlap. In these conditions, the argument that follows (with some little nuances) also works

  Our induction will be over the number of open sets in the good cover of $M$

  <ul>
    <li>
    If $M$ is the only open set of the covering, then $M$ is diffeomorphic to $\R^m$ and the Künneth Theorem holds
    </li>
    <li>
    Suppose that we have shown the validity of the Künneth Theorem for manifold with good covers of $l-1$ open sets, and let 

    $$\{U_1, U_2, ... , U_l\}$$ 

    be a good cover of $M$. For

    $$U=U_1\cup U_2\cup ... \cup U_{l-1}$$

    and 

    $$V=U_{l}$$

    the Künneth Theorem holds by hypothesis, because $\{U_1, U_2, ... , U_{l-1}\}$ is a good cover for $U$. And it also holds for $U\cap V$, for which 

    $$\{U_1\cup U_l, U_2\cup U_l, ... , U_{l-1}\cup U_l\}$$

    is a good cover of $l-1$ open sets (this is the step where it's crucial that the finite intersections are also diffeomorphic to $\R^m$!). So the Künneth Theorem is valid for $M=U\cup V$ too
    </li>
  </ul>
  </li>
</ol> 

+++