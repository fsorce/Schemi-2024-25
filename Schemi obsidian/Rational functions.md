#PropertiesSchemes 

Consider [[Separated]] and [[Integral schemes]] of [[Finite type morphisms|finite type]] over a field $k$.
In this context open subschemes are always [[Schematically dense]].

A rational function $f:X\dashrightarrow Y$is a pair $(U,f)$ with $f:U\to Y$ morphism up to the equivalence $(U,f)\sim (V,g)\coimplies \exists W\subseteq U\cap V\ s.t.\ \rbar f_ W=\rbar g_W$.

There is a unique maximal domain for a rational function because of [[Separated|how separated schemes and schematically dense open subsets behave]].

If $\xi$ is the generic point of $X$, the field of rational functions on $X$ is $k(X)=\Oc_{X,\xi}$.

There is a bijective correspondence$$\cpa{\text{Rational functions }X\dashrightarrow Y}\longleftrightarrow\Hom_{\Sch}(\Spec k(X),Y)$$
We would like to make these the arrows is a category, the issue is that we can't define composition yet (the image may not contain an open subset of the target).

A rational function $f:X\dashrightarrow Y$ is **dominant** if $f(\xi_X)=\xi_Y$. These correspond to those morphisms $\Spec k(X)\to Y$ such that the image set-theoretically is $\xi_Y$, which correspond to the morphisms $\Spec k(X)\to k(Y)$. We thus have$$\cpa{\text{Dominant rational functions }X\dashrightarrow Y}\longleftrightarrow\cpa{\text{Field extensions }k(Y)\inj k(X)}$$

If $f:X\dashrightarrow Y$ with $Y$ [[Proper morphisms|proper]] over $k$ field and $X$ [[Regular schemes|regular scheme]] over $k$, then the maximal domain of $f$ contains all points of codimension 1.
- Let $p\in X$ be a point of codimension 1. Since $X$ is regular we have that $\Oc_{X,p}$ is a DVR. Since $X$ and $Y$ are over $k$ we have $\Spec\Oc_{X,p}\to \Spec k$.
```tikz 
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd} {\mathrm{Spec}(k(X))} & Y \\ {\mathrm{Spec}(\mathcal{O}_{X,p})} & {\mathrm{Spec}\ k} \arrow[from=1-1, to=1-2] \arrow[from=1-1, to=2-1] \arrow[from=1-2, to=2-2] \arrow[dashed, from=2-1, to=1-2] \arrow[from=2-1, to=2-2] \end{tikzcd}
\end{document}
```
- By the valuative criterion for properness we get a map $\Spec(\Oc_{X,p})\to Y$, which yields a map $V\to Y$ for some open neighborhood $V$ of $p$. 
- This map is compatible with $f$ because of the diagram, so $p$ must lie in the maximal domain.