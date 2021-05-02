For all set $A$, there is no bijective map from $A$ to $\mathcal{P}(A)$. Therefore $A\preccurlyeq\mathcal{P}(A)$ and $A\not\approx\mathcal{P}(A)$ (also denoted $A\prec\mathcal{P}(A)$). In other words, $\mathcal{P}(A)$ is strictly bigger that $A$

+++
Proof
+++

First of all, $A\preccurlyeq\mathcal{P}(A)$ because the map $f:A\longrightarrow\mathcal{P}(A)$ defined by $f(a)={a}$ is clearly injective.

Now suppose we have some $g:A\longrightarrow\mathcal{P}(A)$; we'll find an element in $\mathcal{P}(A)$ not contained in $\mathrm{im}(g)$, so $g$ will never be surjective.

For each $a\in A$, $g(a)$ is a subset of $A$. And $a$ may or may not be an element of this subset. This depends on $a$. So we'll take those $a$ that are not an element of the associated subset: 

$$B={a\in A|a\not\in g(a)}$$

This set $B$ is a subset of $A$ and therefore an element of $\mathcal{P}(A)$, and we claim that it is not covered by $\mathrm{im}(g)$. In fact, suppose that there exists some $b\in A$ satisfying $g(b)=B$. May it happen that $b\in B$? This would imply, by the definition of $B$, that $b\not\in g(b)=B$. This is nonsense! But the other way is nonsense too, because $b\not\in B=g(b)$ directly implies that $b$ is among those having the property of not belonging to its associated subset, that is, $b\in B$. So there is no such $g(b)=B$ and thus $g$ is not surjective.

+++