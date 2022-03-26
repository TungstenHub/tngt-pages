Let $(A|b)$ be the matrix associated to a system of linear equations with $m$ equations and $n$ unknowns, that is, $A$ has $m$ rows and $n$ columns 

<ul>
  <li>
    The system is **compatible** if and only if $\mathrm{rk}(A)=\mathrm{rk}(A|b)$

    <ul>
      <li>The system is **determinate** if and only if $\mathrm{rk}(A)=\mathrm{rk}(A|b)=n$</li>
      <li>The system is **indeterminate** if and only if $\mathrm{rk}(A)=\mathrm{rk}(A|b)\lt n$</li>
    </ul>
  </li>
  <li>The system is **incompatible** if and only if $\mathrm{rk}(A)\lt \mathrm{rk}(A|b)$</li>
</ul>

+++
Proof
+++

See the [general resolution of a system of linear equations]( exp | general_resolution_systems )

+++