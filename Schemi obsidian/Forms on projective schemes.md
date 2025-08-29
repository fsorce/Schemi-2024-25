#VectorBundles_and_Divisors #ProjectiveSchemes

It is useful to study the [[Sheaf of differentials]] on [[Projective space|projective schemes]].

Theorem(**Euler sequence**) we have an exact sequence $0\to \Omega_{\Pj^n_R/R}\to \Oc_{\Pj^n_R}(-1)^{n+1}\to \Oc_{\Pj^n_R}\to 0$.
- For simplicity we assume $R=k$ field.
- We construct the first map by considering the derivation $$\funcDef{\Oc_{\Pj^n}}{\Oc_{\Pj^n}(-1)^{n+1}}{f}{\pa{\pp{x_0}f,\cdots,\pp{x_n}f}}$$while the second is given by $(g_0,\cdots, g_n)\mapsto \sum_{i=0}^n g_i x_i$, which is clearly surjective.
- If $f$ is homogeneous of degree $0$ we know (Euler property) that $\sum x_i\pp{x_i}f=0\cdot f=0$, so the composition $\Omega_{\Pj^n/k}\to \Oc(-1)^{n+1}\to \Oc$ is $0$.
- Let us now check exactness locally: pick a chart $U_i$ (WLOG $i=0$), set $t_j=x_j/x_0$.
- $\rbar{\Omega_{\Pj^n/k}}_{U_i}=\wt{\Omega_{A/k}}\cong \wt{\bigoplus_{j=1}^nA dt_j}$ where $A=k[t_1,\cdots,t_n]$. The maps become $$Adt_1\oplus\cdots\oplus A dt_n\to (x_0\ii A)^{n+1}\to A$$where the last map is $$(x_0\ii g_0(t_1,\cdots, t_n),\cdots, x_0\ii g_n(t_1,\cdots, t_n))\mapsto g_0(t_1,\cdots, t_n)+\sum_{i=1}^nt_ig_i(t_1,\cdots, t_n)$$and the first is given by $$dt_j\mapsto \pa{\pp{x_0}{t_j},\cdots, \pp{x_n}{t_j}}=\pa{-\frac{t_j}{x_0},0,\cdots, 0, \frac1{x_0},0,\cdots, 0}=x_0\ii(e_j-t_ie_0).$$It is now easy to check exactness.

Thanks to the Euler sequence we see that after taking the [[Locally free sheaves|determinant of the exact sequence]] we are left with $\Oc(-n-1)=\Oc(-1)^{\otimes(n+1)}=\det(\Oc(-1)^{n+1})=\omega_{\Pj^n_k/k}\otimes_\Oc\Oc=\omega_{\Pj^n_k/k}$.

This is enough to show that $\Omega_{\Pj^n_k/k}$ is not a direct sum of [[Twisting sheaves]] when $n\geq 2$.
- Suppose that $\Omega_{\Pj^n/k}=\Oc(a_1)\oplus\cdots\oplus \Oc(a_n)$. This implies that $\omega_{\Pj^n/k}=\Oc(a_1+\cdots+a_n)$.
- Consider the Euler sequence $0\to \Omega_{\Pj^n}\to \Oc(-1)^{n+1}\to \Oc\to0$ and twist it so that it becomes$$0\to \Omega_{\Pj^n}(1)\to \Oc^{n+1}\to \Oc(1)\to0$$This means that $H^0(\Omega_{\Pj^n}(1))\subseteq \ker(k^{n+1}\to H^0(\Oc(1)))$ (the global sections functor is exact on the right). The map $k^{n+1}\to H^0(\Oc(1))$ maps the basis vectors $e_i$ to the linear form $x_i$, in particular it is injective so $H^0(\Omega_{\Pj^n}(1))\subseteq 0$, showing that $a_i\leq -2$ for all $1\leq i\leq n$.
- The two conditions on the numbers $a_i$ are incompatible because $-n-1\leq n(-2)\coimplies n\leq 1$. 