#CompactHausdorffAnalogues

A morphism is separated if the [[Diagonal morphism]] it induces is closed.
A scheme is separated if $X\to \Spec \Z$ is separated.

If $X$ is a scheme and $\cpa{U_i}$ is an affine cover then $X$ is separated iff
1. $U_i\cap U_j$ affine
2. $\Oc(U_i)\otimes \Oc(U_j)\to \Oc(U_i\cap U_j)$ surjective

Local on the base, stable under [[Base change]].

Every morphism between affine schemes is separated.
Open immersions are separated

Given $f:X\to Y,\ g:Y\to Z$ with $g$ separated, $f$ is separated iff $g\circ f$ is separated.

If $X$ is separated, $X\to Y$ is separated.

If $X\to Y$ is a [[Locally closed immersion]] then $\delta:X\to X\times_Y X$ is an isomorphism, thus locally closed immersions are separated.

If $U\subseteq X$ is [[Schematically dense]], $f,g:X\to Y$ morphisms with $Y$ separated then $\rbar f_U=\rbar g_U\implies f=g.$ (scheme analogue of $\cpa{f=g}$ is closed when codomain is $T_2$)
- We have $F:X\to Y\times Y$ given by $F=(f,g)$ and $U\to Y\to Y\times Y$ given by $\rbar f_U=\rbar g_U$ followed by the diagonal.
- $U\subseteq F\ii(\delta(Y))$ but $Y$ separated means $\delta(Y)$ closed, so $X=\ol{U}\subseteq F\ii(\delta(Y))$, i.e. $f=g$.

Valuative criterion for separatedness (uniqueness of limits in $T_2$ spaces).