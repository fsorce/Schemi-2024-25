#VectorBundles_and_Divisors #ProjectiveSchemes

On $\Pj^n_R$ we define the twisting sheaves $\Oc(d)$ for $d\in \Z$ to be the [[Quasi-Coherent sheaves]] associated to the module $R[x_0,\cdots,x_n]$ with the grading shifted by $d$. 
- They are [[Locally free sheaves|line bundles]]: $\rbar{\Oc(d)}_{U_i}\cong \rbar{\Oc_X}_{U_i}$ and the isomorphism is given by multiplying/dividing by ${x_i}^d$.
- $R[x_0,\cdots, x_n]_d=\Gamma(\Pj^n_R,\Oc(d))$.
- $\rnk_R\Gamma(\Pj^n_R,\Oc(d))=\begin{cases}0 & d<0\\ \binom{d+n}n &d\geq 0\end{cases}$
- $\Oc(d)\otimes\Oc(e)\cong \Oc(d+e)$. From this and the rank from before we get that $$\Oc(d)\cong \Oc(e)\coimplies d=e$$
Using [[(Quasi-)Coherent sheaf cohomology|Čech cohomology]] we can show that$$H^i(\Pj^n_R,\Oc(d))=\begin{cases}R^{\binom{n+d}n} &\text{if }i=0\text{ and }d\geq 0\\ R^{\binom{-d-1}n} &\text{if }i=n\text{ and }d< 0\\ 0 &\text{otherwise}\end{cases}$$From this we see that $H^1(\Pj^n,\Oc(d))=0$ when $n\geq 2$, so hypersurfaces are [[Geometrically connected]] for $n\geq 2$.

The [[(Quasi-)Coherent sheaf cohomology|Euler characteristic]] of $\Oc(d)$ is $\binom{n+d}n$ (when $d\leq -n-1$ we use $\binom{n+d}n=(-1)^n\binom{-d-1}n$).