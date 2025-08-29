#Sheaves 

We want the left-adjoint of [[Pushforward]].

For [[Presheaves]] we set $f\ii G(U)=\displaystyle \varinjlim_{f(U)\subseteq V}G(V)$ and get a valid presheaf functorially.
***
For [[Sheaves]] we just sheafify and we still have an adjoint by the universal property.

If we have $f:X\to Y$, $g:Y\to Z$ then we have a canonical isomorphism $(g\circ f)\ii\cong f\ii\circ g\ii:\Sh(Z)\to \Sh(X)$.
- Use Yoneda lemma.

If $f:p\to Y$ is the inclusion of a point then $f\ii G(p)=G_{f(p)},\ f\ii G(\emptyset)=0$. 
It follows that $(f\ii G)_p=G_{f(p)}$.

If $j:U\inj X$ [[Open immersion]] then $j\ii \Fc=\rbar\Fc_U$.

***
In the case of [[(Pre-)Sheaves of O_X-modules|O_X-modules]], pullback $f:X\to Y$ does not yield $\Oc_X$-modules but $f\ii\Oc_Y$-modules. By the adjuction, $f^\sharp:\Oc_Y\to f_\ast\Oc_X$ gives a homomorphism $f\ii\Oc_Y\to \Oc_X$, so we can consider$$f^\ast G=\Oc_X\otimes_{f\ii\Oc_Y}f\ii G.$$Note that $f^\ast\Oc_Y=\Oc_X\otimes_{f\ii\Oc_Y}f\ii\Oc_Y=\Oc_X$.

In the case of open immersions we still get restriction, more precises $\Oc_U\otimes_{\Oc_U}\rbar\Fc U\cong \rbar\Fc_U$ canonically.

Pullback preserves [[Quasi-Coherent sheaves]]. This follows from this affine case:
If $X=\Spec A, Y=\Spec B$, $N\in \Mod_B$ and $f:X\to Y$ comes from $\vp:B\to A$ then we have $f^\ast\wt N\cong \wt{N\otimes_B A}$.
- Use Yoneda lemma and adjunctions.

In the spirit of the Yoneda lemma, if $\Fc\in \Sh(\Oc_X)$ then $\Fc(X)=\Hom_{\Sh(\Oc_X)}(\Oc_X,\Fc)$. This means that the pullback homomorphism $f^\ast:\Gc(Y)\to f^\ast\Gc(X)$ can be interpreted as a map$$\Hom_{\Sh(\Oc_Y)}(\Oc_Y,\Gc)\to \Hom_{\Sh(\Oc_X)}(\Oc_X,f^\ast\Gc)$$
