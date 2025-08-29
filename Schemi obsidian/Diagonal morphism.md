#CompactHausdorffAnalogues

If $f:X\to Y$ is a morphism, the diagonal morphism it induces is $X\to X\times_Y X$ given by the two identities.

The diagonal is always a [[Locally closed immersion]].
- In the affine case it is actually closed (multiplication $A\otimes_B A\to A$ is clearly surjective).
- We have $X\times_Y X\to Y$ so up to pulling back an affine cover of $Y$ WLOG $Y$ affine.
- Cover $X$ with affine $U_i$. Note that $U_i=\delta\ii(U_i\times)Y U_i)$ and so by the affine case $U_i$ closed in $U_i\times_Y U_i$.
- Set $U=\bigcup U_i\times_Y U_i$ and see that $X\subseteq U$ is closed ([[Closed immersions]] are local on the base) while $U\subseteq X\times_YX$ is open.

Note that $\delta\ii(U_i\times_Y U_j)=U_i\cap U_j$ so $\delta$ is a closed immersion when $U_i\cap U_j$ is closed in $U_i\times_Y U_j$.
If $Y$ is affine this means that when we take an affine cover, the intersection of two elements of the cover needs to still be affine