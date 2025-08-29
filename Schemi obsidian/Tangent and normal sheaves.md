#VectorBundles_and_Divisors

Let $X\in \Sch/k$ be a smooth scheme and $Y\subseteq X$ a closed subscheme which is also smooth, then the [[Conormal sheaf]] $\Cc_YX$ is locally free of rank $\dim X-\dim Y$.

We define the normal sheaf of $Y\subseteq X$ as $\Nc_Y X=(\Cc_Y X)^\vee$, which is still locally free of rank $\dim X-\dim Y$.

We define the dual of the [[Sheaf of differentials]] to be the tangent sheaf $T_X=\Omega_{X/k}^\vee$.
We call the tangent space to $X$ at $p$ the *fiber* (not stalk) of $T_X$ at $p$, i.e. $T_{X,p}:=T_X\otimes_{\Oc_X} k(p)$.

Taking the dual of the exact sequence $0\to\Cc_Y X\to \rbar{\Omega_{X/S}}_Y\to \Omega_{Y/S}\to 0$ yields $$0\to T_Y\to \rbar{T_X}_Y\to \Nc_Y X\to 0$$which is in a sense the geometrically intuitive definition of the normal sheaf.


Recall that [[Sheaf of differentials|if p is a rational point then]] $T_{X,p}\cong (\mf_p/\mf_p^2)^\vee$. There is a natural bijection$$\Hom_{\Sch/k}(\Spec k[\e],X)\longleftrightarrow\cpa{(p,v)\mid p\in X(k),\ v\in T_{X,p}}$$The latter is the classical notion of the *tangent bundle*.