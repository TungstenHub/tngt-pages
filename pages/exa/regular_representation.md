[{z_5}]

Let's find the regular representation of $\Z_5=\{[0],[1],[2],[3],[4]\}$. The effect of each element on the vector space of formal sums would be

$$[0](a[0]+b[1]+c[2]+d[3]+e[4]) = a[0]+b[1]+c[2]+d[3]+e[4]$$
$$[1](a[0]+b[1]+c[2]+d[3]+e[4]) = a[1]+b[2]+c[3]+d[4]+e[0]$$
$$[2](a[0]+b[1]+c[2]+d[3]+e[4]) = a[2]+b[3]+c[4]+d[0]+e[1]$$
$$[3](a[0]+b[1]+c[2]+d[3]+e[4]) = a[3]+b[4]+c[0]+d[1]+e[2]$$
$$[4](a[0]+b[1]+c[2]+d[3]+e[4]) = a[4]+b[0]+c[1]+d[2]+e[3]$$

which is represented by the matrices

$$
[0] \maps
\begin{pmatrix}
1 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 1 
\end{pmatrix}
$$

$$
[1] \maps
\begin{pmatrix}
0 & 0 & 0 & 0 & 1 \\
1 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 & 0 
\end{pmatrix}
$$

$$
[2] \maps
\begin{pmatrix}
0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 1 \\
1 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 
\end{pmatrix}
$$

$$
[3] \maps
\begin{pmatrix}
0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 1 \\
1 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 
\end{pmatrix}
$$

$$
[4] \maps
\begin{pmatrix}
0 & 1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 1 \\
1 & 0 & 0 & 0 & 0 
\end{pmatrix}
$$

---

[{s_3}]

Now it's time for $S_3=\{e,(123),(132),(12),(13),(13)\}$. Taking into account the rules of multiplication of this group, we would have

$$
\begin{array}{rcl}
e & \maps &
\begin{pmatrix}
1 & 0 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 0 & 1 \\
\end{pmatrix}
\\[4em]
(123) & \maps &
\begin{pmatrix}
0 & 0 & 1 & 0 & 0 & 0 \\
1 & 0 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 0 & 1 \\
0 & 0 & 0 & 1 & 0 & 0 \\
\end{pmatrix}
\\[4em]
(132) & \maps &
\begin{pmatrix}
0 & 1 & 0 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 & 0 \\
1 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 1 \\
0 & 0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 0 & 1 & 0 \\
\end{pmatrix}
\\[4em]
(12) & \maps &
\begin{pmatrix}
0 & 0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 0 & 1 \\
1 & 0 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 & 0 \\
\end{pmatrix}
\\[4em]
(23) & \maps &
\begin{pmatrix}
0 & 0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 0 & 1 \\
0 & 0 & 0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 & 0 \\
1 & 0 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 & 0 \\
\end{pmatrix}
\\[4em]
(13) & \maps &
\begin{pmatrix}
0 & 0 & 0 & 0 & 0 & 1 \\
0 & 0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 0 & 1 & 0 \\
0 & 1 & 0 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 & 0 \\
1 & 0 & 0 & 0 & 0 & 0 \\
\end{pmatrix}
\end{array}
$$