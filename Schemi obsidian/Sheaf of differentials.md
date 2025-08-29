#VectorBundles_and_Divisors 

We globalize the construction of the [[Kähler differentials - Algebra|module of Kähler differentials]]: let $(f:X\to S)\in \Sch/S$ and take $\Fc\in \QCoh(X)$. A map $\Oc_X\to \Fc$ is an $S$-derivation if it is additive, satisfies the Leibniz rule and "it sends constants to 0", i.e. $f\ii\Oc_S\to \Oc_X\to \Fc$ is the $0$ morphism.

There is a [[Quasi-Coherent sheaves|quasi-coherent sheaf]] $\Omega_{X/S}$ together with an $S$-derivation $d:\Oc_X\to \Omega_{X/S}$ which classifies $S$-derivations. Moreover, this sheaf satisfies the following conditions:
1. If $S=\Spec R$ and $X=\Spec A$ then $\Omega_{X/S}=\wt{\Omega_{A/R}}$. 
2. If $U\subseteq X$ open and $f(U)\subseteq V$ open in $S$ then $\rbar{\Omega_{X/S}}_U=\Omega_{U/V}$.

To construct $\Omega_{X/S}$ we could glue the sheaves given by modules of differentials, but we try instead to generalize the construction $\Omega_{A/R}=I/I^2$ with $I=\ker(A\otimes_RA\to A)$.

The analogue of that quotient of ideals is the [[Conormal sheaf]] associated to the diagonal of $X$ in $X\times_S X$. Explicitly, we set $\Omega_{X/S}=\Cc_X(X\times_S X)$ and give the $S$-derivation$$d:\funcDef{\Oc_X}{\Omega_{X/S}}{g}{[\pr_2^\ast g-\pr_1^\ast g]}$$It is easy to check that the properties we asked for hold.

If we spell out the global analogues of the properties we found for Kähler differentials we get
1. If $S\to S'$ then we get a corresponding morphism $\Omega_{X/S'}\to \Omega_{X/S}$. If $S\to S'$ is a locally closed immersion then that morphism is an isomorphism ($\Oc_{S'}\to \Oc_S$ is surjective).
2. If $Y\xrightarrow f X\to S$ morphisms then we have and exact sequence $f^\ast\Omega_{X/S}\to \Omega_{Y/S}\to \Omega_{Y/X}\to 0$
3. If $Y\to X$ is a closed immersion and $\Ic_Y$ is the sheaf of ideals then $\rbar{\Ic_Y}_Y\to \rbar{\Omega_{X/S}}_Y\to \Omega_{Y/S}\to 0$ Note that $\rbar{\Ic_Y}_Y=\Ic_Y/\Ic_Y^2=\Cc_YX$.
4. If $X\to S$ is locally of finite type and $S$ is locally Noetherian then $\Omega_{X/S}\in \Coh(X)$.
5. If $X\to\Spec k$ and $p\in X(k)$ is a **rational point** (need $\Omega_{k(p)/k}=0$) then $\Omega_{X/k}\otimes_{\Oc_X}{i_p}_\ast k\cong \mf_p/\mf_p^2$.
6. If $X\to S$, $S'\to S$ and $X'=S'\times_S X$ then $\Omega_{X'/S'}\cong \pr_2^\ast\Omega_{X/S}$.

If $X,Y\in \Sch/k$ then $\Omega_{X\times Y/k}\cong \pr_1^\ast\Omega_{X/k}\oplus \pr_2^\ast\Omega_{Y/k}$.

If $X\in\Sch/k$ is [[Smooth schemes|smooth]] of dimension $n$ then $\Omega_{X/k}$ is [[Locally free sheaves|locally free]] of rank $n$.
- It is enough to show that $\Omega_{X/k}\otimes_{\Oc_X}k(p)\cong k^n$ for all $p\in X$.  It is actually enough to check the closed points.
- First consider the case $k=\ol k$. This means that closed points are the rational, so $\dim_k\mf_p/\mf_p^2=\dim_p X=n$ by [[Points of a scheme|regularity]] and we are done.
- For general $k$ recall that $X$ is smooth over $k$ iff $X_{\ol k}$ is smooth over $\ol k$. By the special case this means that $\Omega_{X_{\ol k}/\ol k}\cong \pr^\ast\Omega_{X/k}$ is locally free of rank $n$.
- The projection $\pr:X_{\ol k}\to X$ is faithfully flat so this means that $\Omega_{X/k}$ was already locally free of rank $n$.

If $X\in \Sch/k$ is smooth we define its [[Canonical sheaf]] $\omega_{X/k}$ as the determinant of $\Omega_{X/k}$.

If $Y\subseteq X$ closed, but smooth over $k$ then $0\to\Cc_Y X\to \rbar{\Omega_{X/k}}_Y\to \Omega_{Y/k}\to 0$ is an exact sequence of vector bundles
- we are only missing the injectivity, which holds because $\Cc_Y X\to \ker(\rbar{\Omega_{X/k}}_Y\to \Omega_{Y/k})$ is surjective and both have rank $\codim_Y X$.