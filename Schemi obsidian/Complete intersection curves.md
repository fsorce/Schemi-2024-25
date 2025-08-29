#curves

If a curve $X\subseteq \Pj^{r+1}$ can be expressed as $X=\Proj\dfrac{k[x_0,\cdots, x_{r+1}]}{(f_1,\cdots, f_r)}$ then $X$ is called a complete intersection.

If $\deg f_i=d_i$ then $\deg X=d_1\cdots d_r$ (as a subscheme of $\Pj^{r+1}$). 

If $X$ is a complete intersection like above then $\omega_X=\Oc_X(d_1+\cdots+d_r -r-2).$
- By definition we have a surjective map $\Oc_{\Pj^{r+1}}(-d_1)\oplus\cdots\oplus\Oc_{\Pj^{n+1}}(-d_r)\onto \Ic_X$. If we restrict to $X$ we get $\Oc_{X}(-d_1)\oplus\cdots\oplus\Oc_{X}(-d_r)\onto \Ic_X/\Ic_X^2=\Cc_X\Pj^{r+1}$. 
- Note that since $X$ and $\Pj^{r+1}$ are smooth we have that both [[Conormal sheaf|are vector bundles]] on $X$, the first of rank $r$ and the second of rank $\codim_X\Pj^{r+1}=r+1-1=r$. 
- Since the homomorphism is surjective this proves that we have an isomorphism and so taking the dual $\Nc_X\Pj^{r+1}\cong \Oc_X(d_1)\oplus\cdots\oplus \Oc_X(d_r)$.
- By the [[Canonical sheaf|Adjunction formula]] this yields $$\omega_X=\det(\Oc_X(d_1)\oplus\cdots\oplus \Oc_X(d_r))\otimes \rbar{\omega_{\Pj^{r+1}}}_X=\Oc_X(d_1+\cdots+d_r -r-2).$$
From this we get that the [[Genus]] of $X$ is ($j:X\subseteq \Pj^{r+1}$, recall that [[Divisors on curves|pullback commutes with degree]])$$\begin{align}g(X)=&\dfrac{2+\deg \omega_X}2=\dfrac{2+\deg (j^\ast\Oc_{\Pj^{r+1}}(d_1+\cdots+d_r-r-2))}2=\\=&\dfrac{2+\deg X\deg(\Oc_{\Pj^{r+1}}(d_1+\cdots+d_r-r-2))}2=\\=&\dfrac{2+d_1\cdots d_r(d_1+\cdots+d_r-r-2)}2.\end{align}$$ 