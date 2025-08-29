#Immersion

$U\subseteq X$ [[Open immersion|open subscheme]] is schematically dense if the only [[Closed subschemes|closed subscheme]] that contains $U$ (as a scheme) is $X$.

If $X$ is [[Reduced schemes|reduced]] and $U\subseteq X$ is open dense then it is schematically dense
- Topologically $Y=X$. If $Y$ did not have the reduced structure we would have $U\subseteq X\subsetneq Y$ scheme theoretically, which is not how a closure works, so $X=Y$ as a scheme.

Let $X$ be Noetherian.
- $U\subseteq X$ is dense iff it contains the generic points of the irreducible components
- $U\subseteq X$ is schematically dense iff it contains all [[Points of a scheme|associated points]].
	- Reduce to affine case
	- $U\subseteq X=\Spec A$ is NOT schematically dense iff $\exists I\nor A$ with $I\neq 0$ and $\Supp I\cap U=\emptyset$.
	- If $\pf\in \Ass(A)$ then $A/\pf$ can be identified with an ideal of $A$ and $\Supp(A/\pf)=V(\pf)$.