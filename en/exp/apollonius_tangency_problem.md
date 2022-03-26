>>> 
**Tangency Problem of Apollonius:** to draw a circle that is tangent to three given circles.
<<<

This problem, along with Gergonne's solution that will be developed here, constitutes a delicate and sublime jewel of classical geometry.

{{ image | ap }}

First things first: what are we looking for? We're looking for a circle that is tangent to the circles $A$, $B$ and $C$. But how many such circles are there?

{{ image | ap_0 }}

There are 8 of them, because for each of $A$, $B$ and $C$ we have to choose interior or exterior tangency.

Gergonne took them by pairs: in this case, we'll work with $\Gamma^+$ and $\Gamma^-$, the circles having three exterior and interior tangencies respectively.

{{ image | ap_1 }}

$A$ is bitangent to $\Gamma^+$ and $\Gamma^-$: we know that [the tangency points are aligned with the similarity point $R$ of $\Gamma^+$ and $\Gamma^-$]( exp | circle_power ), from which the power to $A$ is $\Pi_{A}(R)=\sqrt{\Pi_{\Gamma^+}(R)\Pi_{\Gamma^-}(R)}$.

{{ image | ap_2 }}

But this is true for $B$ and $C$ too, i.e. $\Pi_{A}(R)=\Pi_{B}(R)=\Pi_{C}(R)$. So $R$ is indeed the [radical center of $A$, $B$ and $C$]( app | circles_radical_center )! And we know how to draw this!

{{ image | ap_3 }}

On the other hand, having three circles, we can't help thinking of [d'Alembert Theorem]( app | circles_dalembert ): all three (exterior) similarity points $e_{BC}$, $e_{CA}$ and $e_{AB}$ are aligned in a line $l$. Is this useful? Well, it is crucial.

{{ image | ap_4 }}

The $Γ$ circles are bitangent to $B$ and $C$, so $\Pi_{\Gamma^+}(e_{BC}) = \Pi_{\Gamma^-}(e_{BC}) = \sqrt{\Pi_{B}(e_{BC})\Pi_{B}(e_{BC})}$. But in the same way $\Pi_{\Gamma^+}(e_{CA}) = \Pi_{\Gamma^-}(e_{CA})$ and $\Pi_{\Gamma^+}(e_{AB}) = \Pi_{\Gamma^-}(e_{AB})$... so $l$ must be the radical axis of $\Gamma^+$ and $\Gamma^-$!

{{ image | ap_5 }}

The tangents to $A$ drawn from the tangency points with $\Gamma^+$ and $\Gamma^-$ meet at $q$. They're of equal length, so the power of $q$ with respect to the $Γ$ circles is the same - that is, $q$ lies in the radical axis $l$.

{{ image | ap_6 }}

$q$ is the [pole]( app | circle_polar_line ) of the green line with respect to $A$, and lies in $l$. So by [polarity reciprocity]( app | circle_polar_recip ), the pole of $l$ with respect to $A$ lies in the green line. We can thus draw the green line, because we have a second anchor in $R$.

{{ image | ap_7 }}

That's Gergonne's solution!! Draw the radical center $R$, then d'Alembert line $l$, with its poles $p_A$, $p_B$ and $p_C$, and join them with $R$ - tangency points found ::heart::

{{ image | ap_label }}

Taking d'Alembert lines with pairs of internal similarity points gives rise to the other three pairs of tangent circles.