The condition on a linear order to be a well-order is very restrictive. Informally stated, all well-ordered sets begin the same way when arranged with respect to this order, and any two of them are sort of comparable. But why?

Suppose $\langle A, <\rangle$ is a non-empty well-ordered set. Then it has a minimal element, say $a_0$, because $A\subset A$ is a non-empty subset. We have $a_0 < a$ for all $a\in A$, $a\neq a_0$. But if $A\smallsetminus \{a_0\}$ is non-empty, then it has again a minimal element $a_1$, and $a_0 < a_1 < a$ for all $a\in A$, $a\neq a_0$, $a_1$. Can you see the pattern? If $A$ is big enough, we would have $a_2$ the minimal element of $A\smallsetminus \{a_0,a_1\}$, $a_3$ the minimal element of $A\smallsetminus \{a_0,a_1,a_2\}$, and so on. This process may eventually terminate

{{ image | ordinals_order_init_1 }}

or it may become infinite

{{ image | ordinals_order_init_2 }}

But even if it is infinite, it may not contain all the elements in $A$: think of $\mathbb{N}\times \mathbb{N}$ with the lexicographical order for instance. So we have to go on. How? Well, one could define _the set of elements of $A$ that do not belong to the previous row_. This property can be formalized into a logical formula (the set of elements $b$ for which there is no finite sequence $a_0,a_1,\dots,a_n$ such that $a_0 < a_1 < \cdots < a_n < b < a$ for all $a\in A\smallsetminus \{a_0,a_1,\dots,a_n,b\}$, and so on) in order to apply the [Axiom of Specification]( def | axiom_schema_specification ). And now: this subset has a minimal element! And when this element is removed, we get another one! So a new thread starts

{{ image | ordinals_order_init_3 }}

Provided $A$ is not completely exhausted by this procedure, we would have more and more threads

{{ image | ordinals_order_init_4 }}

Even infinite threads!

{{ image | ordinals_order_init_5 }}

And after all those infinite threads... one could look at the remaining elements and start again! It would look like... a three-dimensional arrangement?

{{ image | ordinals_order_init_6 }}

That's why all the well-ordered sets "begin the same way". And this pattern will be capture by the _ordinal numbers_: the examples above would be represented by the ordinals $4$, $\omega$, $\omega+4$, $\omega\times 4 + 4$, $\omega^2$ and $\omega^2\times 4$ respectively.

This may seem terribly intricate... but it is just the beginning. If you look carefully, all the sets above are numerable, and indeed all the well-ordered sets we can "describe in a plain language" are numerable. Then, how would a non-numerable well-ordered set look like? What if we could define a well-order in $\R$? Its inner structure would be enormous. For instance, think that there would be a _first_ element (for the minimal element property) whose section is non-numerable, all previous elements having numerable section (just like the first element of the second "thread", which gives rise to non-finite sections). Can you imagine it?

Finally, this discussion is closely related to the more than controversial [Axiom of Choice]( def | axiom_choice ). This axiom seems rather stupid at first; it says that for any set $A$, there is a function that assigns any non-empty subset of $A$ an element that belongs to this subset. It sounds obvious: if the subset is non-empty, we can choose an element in it! The hot point is that we need to have all this choices _beforehand, all at once_, like some sort of criteria. Could you describe some criteria that assigns every non-empty subset of $\R$ an element in it? (Beware, there are very weird subsets of $\R$!)

In fact, one cannot describe such criteria (try as hard as you want). And if such function-criteria existed, the construction above could be replicated. Suppose we have a function of choice in $\R$:

$$f:\mathcal{P}(\R)\longrightarrow \R\qquad f(a)\in a\,\forall a\subset \R$$

Ok, now we define

$$
\begin{array}{rcl}
a_0 & = & f(\R) \\ 
a_1 & = & f(\R\smallsetminus\{a_0\}) \\ 
a_2 & = & f(\R\smallsetminus\{a_0,a_1\}) \\ 
a_3 & = & f(\R\smallsetminus\{a_0,a_1,a_2\}) \\ 
a_4 & = & f(\R\smallsetminus\{a_0,a_1,a_2,a_3\}) \\ 
& \vdots & \\
\end{array}
$$

See? And after one thread, we may start another one... it is as if there was a well-order in $\R$. How long can we proceed as above? Well, forever, and it is always the same principle: if there are elements of $\R$ which can't be put into this well-order, which is $f$ of this subset? So it is equivalent: having all these choices _beforehand, all at once_, and such huge non-numerable well-order existing. Mind-blowing, isn't it? More on that later