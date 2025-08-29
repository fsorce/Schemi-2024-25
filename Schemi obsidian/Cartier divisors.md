#VectorBundles_and_Divisors

Let $X$ be a Noetherian, integral and normal scheme. A [[Weil divisors|divisor]] on $X$ is called Cartier when it is locally principal, that is, when there is an open cover $\cpa{U_i}$ of $X$ such that $\rbar D_{U_i}=\div(f_i)$ for some $f_i\in k(U_i)^\times=k(X)^\times$. We denote Cartier divisors by $\CDiv(X)\subseteq \Div(X)$.

From Cartier divisors we can construct line bundles as follows: $$\Oc_X(D)(U)=\cpa{f\in k(X)^\times\mid \rbar{(\div f+D)}_U\geq 0}\cup \cpa0.$$This is a line bundle:
- $\Oc_X(D)$ is a sheaf of $\Oc_X$-modules
- If $D=\div f$ for $f\in k(X)^\times$ then $\Oc_X(D)(U)=\cpa{g\in k(X)^\times\mid \rbar{\div(fg)}_U\geq 0}\cup \cpa0$ and this ring is isomorphic to $\Oc_X(U)$ under the map $$\funcDef{\Oc_X(D)(U)}{\Oc_X(U)}{g}{fg}$$This shows that $\Oc_X(\div f)\cong \Oc_X$.
- If $D$ is locally principal and we fix a cover over which $D$ becomes principal then that cover trivializes $\Oc_X(D)$, showing that $\Oc_X(D)$ is indeed invertible.

Cartier divisors are exactly the image of the map $\wt \Pic(X)\to \Div(X)$, so the [[Picard group]] of $X$ is isomorphic to $\frac{\CDiv(X)}{\imm(\div)}\subseteq \Cl(X)$.
- If $D=\div s$ for some rational section $s$ of $L$ then $D$ is locally principal, simply take a trivializing cover for $L$. If instead we start with a locally principal divisor, consider the pair $(\Oc_X(D),1)$.
- If $t\in L_\xi\nz$ with $t\in L(U)$ then $\rbar{\div t}_U\geq 0$. Note that $\div(t)=\div(t/s)+\div(s)=\div(t/s)+D$, so we have an isomorphism $L(U)\to \cpa{f\in k(X)^\times\mid \rbar{(\div f+\div s)}_U\geq0}=\Oc_X(\div s)$ given by sending $t$ to $t/s$ (in particular $s\mapsto 1$). Therefore $[(L,s)]=[(\Oc_X(\div s),1)]$.
- If we view $1$ as a rational section of $\Oc_X(D)$ then $\div 1=D$.


From this description it follows that [[Effective Cartier Divisors]] come as divisors of global sections of line bundles.