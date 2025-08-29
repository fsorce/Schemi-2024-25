#LocallyRingedSpace

$(X,\Oc_X)$ with $\Oc_X$ [[Sheaves|sheaf]] of rings such that $\Oc_{X,p}$ local. Set $k(p)=\Oc_{X,p}/\mf_p$.
If $\phi\in \Oc_X(U)$ and $p\in U$ then we set $\phi(p)=[\phi_p]\in k(p)$.

Morphisms: $(f,f^\sharp)$ with $f$ continuous and $f^\sharp:\Oc_Y\to f_\ast\Oc_X$ such that the composition $$f^\sharp_p:\Oc_{Y,f(p)}\to(f_\ast\Oc_X)_{f(p)}\to\Oc_{X,p}$$is local, that is, $f^\sharp\vp(p)=0\coimplies \vp(f(p))=0$ for any $\vp$ defined near $f(p)$. 
This recovers the classical definition: if $\vp$ is regular on $U\ni f(p)$ open then the pullback defined by $(f^\sharp\vp)(p):=\vp(f(p))$ is regular on $f\ii(U)$.

A morphism factors through an open subspace iff it factors topologically.

If $\phi\in \Oc_X(U)$ for some open $U$ the set $\cpa{p\in U\mid \phi(p)=0}$ is closed.

Relative POV:
- If $A$ is a ring, a structure of sheaf of $A$-algebras on $\Oc_X$ is uniquely given by the homomorphism $A\to \Gamma(X,\Oc_X)$. 
- The functor $\Spec:\Ring\op\to \LRS$ is fully faithful, indeed we actually have $$\Hom_\Ring(A, \Gamma(X,\Oc_X))=\Hom_{\LRS}(X,\Spec A).$$Giving an $A$-scheme structure corresponds to giving a morphism to the [[Affine schemes|affine scheme]] $\Spec A$.
- As a continuous function, the $X\to \Spec A$ that corresponds to $\vp:A\to \Gamma(X,\Oc_X)$ is the map that sends $x\in X$ to $\ker(A\xrightarrow\vp\Gamma(X,\Oc_X)\to k(x))\in \Spec A$.


If $G$ is a group that acts on $(X,\Oc_X)\in \LRS$ then there exists a categorical quotient $Y$, i.e.
1. fix $\pi:(X,\Oc_X)\to (Y,\Oc_Y)$
2. $\pi$ is $G$-invariant, i.e. if $\phi_g\in \Aut((X,\Oc_X))$ comes from $g\in G$ then $\pi\circ \phi_g=\pi$.
3. Every $G$-invariant $f:(X,\Oc_X)\to (Z,\Oc_Z)$ factors through $\pi:X\to Y$.
It turns out that $\Oc_Y(V)=\Oc_X(\pi\ii(V))^G$.

