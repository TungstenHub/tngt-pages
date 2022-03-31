Sometimes a space $X$ is mapped over another space $Y$ by two maps that are different, but that are in some way compatible, in the sense that "one map may be continuously deformed to match the another map"

{{ image | homotopic_maps }}

How to formally describe this property?

---

Let $X$, $Y$ be two topological spaces, $f$ and $g:X\longrightarrow Y$ two maps. We say that $f$ and $g$ are **homotopic maps** if there exists $H:X\times [0,1]\longrightarrow Y$ such that $H(x,0)=f(x)$, $H(x,1)=g(x)$, for all $x\in X$.

We denote $f\sim g$ (or $f\sim_H g$ if $H$ is wanted to be explicit). $H$ is called the _homotopy_ (between $f$ and $g$).

---

It also may happen that we want to describe the previous phenomenon but stressing at the same time that the image of some subset of $X$ remains the same all over the deformation

{{ image | homotopic_maps_relative }}

---

Let $A\subset X$, $f$, $g:X\longrightarrow Y$ with $f\vert_A=g\vert_A$. We say that $f$ and $g$ are **homotopic maps relative to $A$** if there exists $H:X\times [0,1]\longrightarrow Y$ such that $H(x,0)=f(x)$, $H(x,1)=g(x)$, for all $x\in X$, and $H(a,s)=f(a)=g(a)$, for all $a\in A$, $s\in [0,1]$. It is denoted $f\sim g (A)$.