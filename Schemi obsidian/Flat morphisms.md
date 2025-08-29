#RelativeProperties

A morphism $f:X\to Y$ is flat if $f^\sharp_p:\Oc_{Y,f(p)}\to \Oc_{X,p}$ is flat for all $p\in X$.
A morphism is faithfully flat if it is flat and surjective (faithfully flat $\coimplies$ flat with non-empty fibers).

Local on the base and stable under [[Base change]].

If $S$ integral Noetherian, $f:X\to S$ flat such that $X$ Noetherian then every irreducible component of $X$ dominates $S$.
- WLOG X irreducible and both affine
- $\Oc(S)\to \Oc(X)$ flat means torsion free and both are domains so $\Oc(S)\to \Oc(X)$ injective.

**Slogan**: flatness has something to do with continuity of the [[Fibers]].

Let $f:X\to Y$ be a [[Finite morphisms|finite morphism]] of [[Noetherian schemes]].
- If $q\in Y$ and $q\in V\subseteq Y$ open affine, $U=f\ii(V)$ is also open affine and $f\ii(q)=\Spec(k(q)\otimes_{\Oc_Y(V)}\Oc_X(U))$.
- If we view $\Oc_X(U)$ as a $\Oc_Y(V)$-module we get the function $$\funcDef{V}{\N}q{\dim_{k(q)}k(q)\otimes_{\Oc_Y(V)}\Oc_X(U)}$$which is locally constant when $f$ is flat.
- Putting everything together, if $f$ is finite and flat the function $$\funcDef{Y}{\N}{q}{\dim_{k(q)}\Oc_{f\ii(q)}(f\ii(q))}$$is locally constant. 

If $f:X\to S$ is [[Finite type morphisms|of finite type]] consider$$\funcDef{X}\N p{\dim_pf\ii(f(p))}$$This function is upper-semicontinuous and if $f$ is flat it is locally constant.

Suppose $f:X\to Y$ is a morphism between schemes of finite type over $k$.
- If $p\in X$ closed point, $\dim_p X\leq \dim_{f(p)}Y+\dim_pf\ii(f(p))$.
- If $f$ is flat we have equality
- **Miracle flatness**: If $X,Y$ are regular and we have equality for all closed points then $f$ is flat.
- If $f$ is a finite and surjective morphism between regular schemes of finite type over a field then $f$ is flat ($\dim_p f\ii(f(p))=0$ so it is constant).

If $f:X\to Y$ is faithfully flat and $X,Y$ are locally Noetherian then
- $X$ regular $\implies$ $Y$ regular
- $X$ integral and normal $\implies$ $Y$ integral and normal.

If $S$ regular Noetherian integral of dimension 1, $f:X\to S$ with $X$ Noetherian reduced. Then $$\text{flat}\coimplies\text{irreducible components of $X$ dominate }S$$
If $f:X\to S$ flat of finite type and $S$ locally Noetherian then $f$ is an open map.


