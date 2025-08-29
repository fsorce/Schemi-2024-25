#Sheaves 

Theorem (Projection formula) Let $X,Y$ be [[Noetherian schemes]] and $f:X\to Y$. Let $E$ be a [[Locally free sheaves|locally free sheaf]] on $Y$ and $F\in \QCoh(X)$. In $\QCoh(Y)$ we have a canonical isomorphism$$E\otimes_{\Oc_Y}f_\ast F\cong f_\ast(f^\ast E\otimes_{\Oc_X} F)$$   - If $E\cong {\Oc_Y}^r$ then both sheaves are $(f_\ast F)^r$ in a canonical way:
	- choose a basis for $E$ and give the obvious isomorphisms in that basis
	- if we change basis of $E$, we do it on both sides and so the resulting isomorphism is actually the same.
- Do the above on a trivializing neighborhood for $E$ and then glue, which we can do because the isomorphism was base-independent.