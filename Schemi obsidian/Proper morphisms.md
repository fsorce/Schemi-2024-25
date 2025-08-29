#CompactHausdorffAnalogues

A morphism $f:X\to Y$ is proper if it is [[Finite type morphisms|of finite type]], [[Separated]] and **universally closed**.
Scheme analogue of "preimage of compact is compact".

An [[Affine morphism]] is proper iff it is [[Finite morphisms|finite]] (affine schemes are proper when they are discrete)

Since being closed is local on the base, to check that a morphism is universally closed it suffices to check the [[Base change]] to affine schemes.

Local on the base, stable under composition and [[Base change]].


If $f:X\to Y$, $g:Y\to Z$ are such that $g$ is separated and $g\circ f$ is proper then $f$ is proper. (This is the scheme analogue of $Y$ Hausdorff, $X$ compact implies that $X\to Y$ is proper)


If $\Fc$ is a [[Quasi-Coherent sheaves|coherent sheaf]] on $X$ with $X\to \Spec R$ proper, $R$ Noetherian, then $\Fc(X)$ is a finitely generated $R$-module.
- [[Pushforward]] via proper morphisms in this context preserves coherence and coherent sheaves on $\Spec R$ correspond to finitely generated modules.


Theorem(**Chevalley**) If $f:X\to Y$ is proper with finite fibers and $Y$ is locally Noetherian then $f$ is finite.



*Valuative criterion for properness* (scheme analogue of the sequence criterion for compactness):
If $f:X\to Y$ is proper then for any diagram 
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd} {\mathrm{Spec} K} & X \\ {\mathrm{Spec} R} & Y \arrow[from=1-1, to=1-2] \arrow[from=1-1, to=2-1] \arrow[from=1-2, to=2-2] \arrow[dashed, from=2-1, to=1-2] \arrow[from=2-1, to=2-2] \end{tikzcd}
\end{document}
```
with $R$ a DVR and $K=\Frac R$ there is a unique dashed arrow.
- The uniqueness follows because proper morphisms are [[Separated]].
- Consider the [[Base change]] $X_R=\Spec R\times_YX$ and call $g$ the projection to $\Spec R$. $g$ is still proper because proper morphism are stable under base change.
- Let $p\in X_R$ be the point determined by the map from $\Spec K$ and let $V=\ol{\cpa p}$. We consider $V$ with the reduced structure, so that it is an integral scheme. Note that $k(V)=K$ because $p$ is the generic point and it is $K$-rational.
- Note that $\rbar g_V:V\to \Spec R$ is closed (restriction of proper map to closed subset) and that the image contains $(0)R$, which is the generic point of $\Spec R$, so the map is surjective. 
- We can thus pick $q\in V$ such that $g(q)=\mf_R$. This gives a local homomorphism $R\to \Oc_{V,q}$.
- Note that both $R$ and $\Oc_{V,q}$ are local subrings of $K$ (here we use $K=k(V)$), which in both cases is their field of fractions. Since $R\to \Oc_{V,q}$ is local, this means that $R=\Oc_{V,q}$.
- The map $R=\Oc_{V,q}\to V\to X_R\to X$ is a valid lift.

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd} {\mathrm{Spec} K} & V & {X_R} & X \\ & {\mathrm{Spec}\ \mathcal{O}_{V,q}} & {\mathrm{Spec} R} & Y \arrow[from=1-1, to=1-2] \arrow[from=1-1, to=2-2] \arrow[hook, from=1-2, to=1-3] \arrow[from=1-2, to=2-3] \arrow[from=1-3, to=1-4] \arrow["g", from=1-3, to=2-3] \arrow["f", from=1-4, to=2-4] \arrow[from=2-2, to=1-2] \arrow["\sim", from=2-2, to=2-3] \arrow[from=2-3, to=2-4] \end{tikzcd}
\end{document}
```
