#VectorBundles_and_Divisors

If $X\in \Sch/k$ is smooth of dimension $n$ then its [[Sheaf of differentials]] is locally free of rank $n$. We define the canonical sheaf of $X$ as the  $\omega_{X/k}=\det \Omega_{X/k}$.

Theorem(**Adjunction formula**) Let $X$ be a smooth scheme over $k$ and $Y$ a smooth closed subscheme. We have that $\omega_Y\cong(\rbar{\omega_X}_Y)\otimes\det(\Nc_Y X)$.
- Consider the exact sequence $0\to\Cc_Y X\to \rbar{\Omega_{X/k}}_Y\to \Omega_{Y/k}\to 0$ and take the [[Locally free sheaves|determinant]] to get $\rbar{\omega_X}_Y\cong \omega_Y\otimes_{\Oc_Y} \det(\Cc_Y X)$.
- Tensor with the determinant of the [[Tangent and normal sheaves|normal bundle]], which is the dual of $\det(\Cc_Y X)$, to conclude.

Theorem (**Serre Duality**) Let $X\in \Sch/k$ be a smooth, projective and connected scheme of dimension $n$. If $E$ is [[Locally free sheaves|locally free]] on $X$ then there is a canonical isomorphism$$H^i(X,E)\cong H^{n-i}(X,E^\vee\otimes\omega_X)^\vee.$$
