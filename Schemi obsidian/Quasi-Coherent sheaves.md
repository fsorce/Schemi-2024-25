#Sheaves 

[[Quasi-Coherent sheaves affine case|In the affine case]], quasi-coherent sheaves are the essential image of the category of $A$-modules in the category of $\Oc_{\Spec A}$-modules. They are denoted $\QCoh(X)$.

Since being Quasi-coherent can be checked on an open cover, we can define quasi-coherent sheaves for arbitrary schemes.

Given a graded ring $A$ and a graded module $M$ we can define a quasi-coherent sheaf on [[Proj construction|Proj(A)]] in the same way we defined the structure sheaf of $\Proj A$. We get an exact sheafification functor.

In the [[Noetherian schemes|locally Noetherian]] case we may consider **Coherent sheaves**, which correspond to finitely generated modules.


Exact sequences:
- If $X$ affine and $0\to \Fc'\to \Fc\to \Fc''\to 0$ exact with $\Fc'\in \QCoh(X)$ then $0\to \Fc'(X)\to \Fc(X)\to \Fc''(X)\to 0$  is also exact.
- For general schemes, if $0\to \Fc'\to \Fc\to \Fc''\to 0$ exact and any two are $\QCoh$ then the third sheaf is also quasi-coherent
	- Since $\QCoh$ is abelian the cases where $\Fc$ is quasi-coherent are known, we are just left with the case where we know that $\Fc'$ and $\Fc''$ are $\QCoh$.
	- WLOG $X$ affine since being quasi-coherent is a local property.
	- From previous proposition we have that $0\to \Fc'(X)\to \Fc(X)\to \Fc''(X)\to 0$  is also exact
	- Sheafify and take the maps to the original exact sequence of sheaves. We are in a 5 lemma situation.

[[Locally free sheaves]] on schemes are quasi-coherent.


