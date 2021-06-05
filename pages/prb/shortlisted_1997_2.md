**[CAN]** Let $R_1$, $R_2$ ... be the family of finite sequences of positive integers defined by the following rules: $R_1 = (1)$, and if $R_{n−1} = (x_1,\cdots,x_s)$, then

$$R_n = (1, 2,\cdots,x_1, 1, 2,\cdots,x_2,\cdots, 1, 2,\cdots,x_s, n)$$

For example, $R_2 = (1, 2)$, $R_3 = (1, 1, 2, 3)$, $R_4 = (1, 1, 1, 2, 1, 2, 3, 4)$.

Prove that if $n > 1$, then the $k$th term from the left in $R_n$ is equal to $1$ if and only if the $k$th term from the right in $R_n$ is different from $1$.

{{ image | shortlisted_1997_2 }}

+++
Solution
+++

The solution to this incredibly beautiful problem is based upon an equivalent construction that leads to the property asked to prove and to other remarkable ones, for instance, that the sequence $R_n$ has $2^{n-1}$ elements, which is also not obvious from the initial definition.

The equivalent construction resembles the Pascal Triangle: each slot is built upon the concatenation of the two slots above. The left side is filled with ones and the right side is filled with the number of the row. Each sequence $R_n$ is just the concatenation of all the slots in the $n$-th row.

{{ image | shortlisted_1997_2_res_0 }}

In this equivalent construction it is almost trivial to prove the antisymmetry of the terms, since it is a property naturally inherited from row to row. It is also trivial that the sequences have $2^{n-1}$ elements, since the cardinality of the slots match the binomial coefficients in the Pascal Triangle, whose sum in a row is known to lead to powers of 2.

So the key is to prove that both constructions are equivalent, which is not so obvious.

To ease the notation, let's introduce the _expansion_ operation: given a sequence, we return another sequence in which each number $k$ is replaced by $1,2,3,\cdots,k$, and we denote it with a bar, that is,

$$\overline{(4,7,5)} = (1,2,3,4,1,2,3,4,5,6,7,1,2,3,4,5)$$

This operation commutes well with the concatenation, for instance

$$\overline{(4,7)}\,\overline{(5)} = (1,2,3,4,1,2,3,4,5,6,7)(1,2,3,4,5) = (1,2,3,4,1,2,3,4,5,6,7,1,2,3,4,5) = \overline{(4,7,5)}$$

In this notation, our sequences are just $R_n = \overline{R_{n-1}}n$

And the trick is to realize that, in our Pascal Triangle arrangement, each slot is the expansion of the slot above to the right. If this is true, then each row is the expansion of the previous one plus a final number $n$, just like the original definition!

In the left side of the tringle, this expansion property holds, since $\overline{(1)}=(1)$

{{ image | shortlisted_1997_2_res_1 }}

In the right side, it holds too: the upper diagonal contains the sequences $(n)$, the lower one contains their expansions $(1,2,3,\cdots,n)$, and this pattern is preserved when concatenating.

{{ image | shortlisted_1997_2_res_2 }}

And last but not least, if the two "arrows" above satisfy this expansion property, then the lower one satisfies it too: in the diagram, $C$ is the concatenation of $\overline{A}$ and $\overline{B}$, which come from $A$ and $B$, but on the other hand $\overline{B}$ comes also from the concatenation of $A$ and $B$, so 

$$C = \overline{A}\,\overline{B} = \overline{AB} = \overline{(\overline{B})}$$

{{ image | shortlisted_1997_2_res_3 }}

This way, this property holds in all the triangle: each slot is the expansion of the slot above to the right. So both constructions are equivalent and our solution is finished.

+++