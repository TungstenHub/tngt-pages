To represent the usual natural numbers, one could use the following sets

$$
\begin{array}{rcl}
0 & = & \varnothing\\ 
1 & = & \{\varnothing\}\\ 
2 & = & \{\{\varnothing\}\}\\ 
3 & = & \{\{\{\varnothing\}\}\}\\ 
4 & = & \{\{\{\{\varnothing\}\}\}\}\\
& \vdots & \\
\end{array}
$$

At first, this seems quite sensible. But it turns out to be very akward. For instance, how could we define $n < m$ for $n$ and $m$ natural numbers defined as above? Perhaps saying that one has more curly braces than the other one? That's no good. Instead, we'll proceed as follows:

$$
\begin{array}{rclcl}
0 & = & \varnothing & = & \{\} \\ 
1 & = & \{\varnothing\} & = & \{0\}\\ 
2 & = & \{\varnothing,\{\varnothing\}\} & = & \{0,1\}\\ 
3 & = & \{\varnothing,\{\varnothing\},\{\varnothing,\{\varnothing\}\}\} & = & \{0,1,2\}\\ 
4 & = & \{\varnothing,\{\varnothing\},\{\varnothing,\{\varnothing\}\},\{\varnothing,\{\varnothing\},\{\varnothing,\{\varnothing\}\}\}\} & = & \{0,1,2,3\}\\
& \vdots & & & \\
\end{array}
$$

Clever, isn't it? Now we would have $n < m$ if and only if $n\in m$. But in fact, it's more than that, because this pattern will appear again with ordinal numbers