Ok, our setting is: some elements and a binary relation

<ul>
<li>A collection of elements</li>
<li>A binary relation $\in$</li>
</ul>

{{ image | set_theory_universe width = 480 }}

But what's a binary relation? In logic, a binary relation is some sort of entity that given any two elements $a$ and $b$, says whether $a\in b$ (read _$a$ in $b$_). We may imagine it as a ethereal machine with two slots, in such a way that when two elements are placed in the slot, the machine dictates 

>>>
_Yes, the first element is in the second element: $a\in b$_ 
<<<

or 

>>>
_No, the first element is not in the second element: $a\notin b$_
<<<

{{ image | set_theory_universe_comp width = 480 }}

Beware!! From the logic perspective, the two "slots" of the binary relation may be occupied by the same element, and the machine is responsible to say whether an element is in itself which, for now, is not forbidden

{{ image | set_theory_universe_comp_self width = 480 }}

The machine, or the binary relation, is unrestricted at this moment. The concept _$a$ is in $b$_ does not have any _belonging_ meaning, it simply states that the machine has declared this with a green light. So all sort of funny things may happen. For instance, it could happen that our machine always declares _true_ for any two elements, and this would be perfectly valid!

{{ image | set_theory_universe_true width = 480 }}

Or imagine that we have no elements at all. It is perfectly valid as well! We only required some elements and a machine with slots. No elements, nothing to check, everything ok

{{ image | set_theory_universe_empty width = 480 }}

Strictly speaking, one only has to "fill a table"

{{ image | set_theory_full_comp }}

%% to elaborate further %%

{{ image | set_theory_meaning width = 480 }}

We have to regulate this with axioms