En una variedad riemanniana hay una conexión canónica, la conexión de Levi-Civita, que impone una compatibilidad con respecto a la métrica y a la simetría. Si la métrica riemanniana viene de una métrica hermítica en una variedad compleja, nos gustaría también cierta compatibilidad con respecto a la estructura compleja. Más concretamente, buscamos una conexión $\nabla$ que sea compatible con la métrica riemanniana ($\nabla g=0$) y con la métrica hermítica ($\nabla \tilde{h}=0$), lo que necesariamente implica $\nabla\omega=0$.

Sin embargo, como $\omega(u,v)=g(Ju,v)$, se cumple la siguiente relación:

$$
\begin{array}{rcl}
(\nabla_w\omega)(u,v) & = & w[\omega(u,v)]-\omega(\nabla_w u,v)-\omega(u,\nabla_w v)\\
& = & w[g(Ju,v)]-g(J(\nabla_w u),v)-g(Ju,\nabla_w v)\\
& = & g(\nabla_w(Ju),v)+g(Ju,\nabla_wv)-g(J(\nabla_w u),v)-g(Ju,\nabla_w v)\\
& = & g(\nabla_w(Ju)-J(\nabla_w u),v)=g((\nabla_w J)(u),v)\\
\end{array}
$$

y esta relación implica que para una variedad hermítica $(M,J,h)$ son equivalentes

<ol>
<li>$\nabla J=0$</li>
<li>$\nabla \omega=0$</li>
<li>$\mathrm{d} \omega=0$</li>
</ol>

Una **variedad de Kähler** es una variedad hermítica satisfaciendo las condiciones equivalentes anteriores, en cuyo caso la conexión de Levi-Civita es compatible con la métrica hermítica.