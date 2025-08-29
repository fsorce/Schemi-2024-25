#VectorBundles_and_Divisors

Isomorphism classes of line bundles together with the following unit and operations$$0=[\Oc_X],\ [L_1]+[L_2]=[L_1\otimes_{\Oc_X}L_2],\ -[L]=[L^\vee]$$form a group, called Picard group and denoted $\Pic(X)$.

If $X=\Spec A$ with $A$ a PID then $\Pic(X)=0$ (projective modules over PID are free).

The Picard group is functorial because [[Pullback]] preserves isomorphism classes and tensor products, i.e. $L_1\cong T_1$, $L_2\cong T_2\implies f^\ast(L_1\otimes L_2)\cong f^\ast T_1\otimes f^\ast T_2$.


(From now on $X$ is Noetherian, normal and integral so that divisors make sense)

The Picard group admits a canonical injection in the [[Class group]]
- Let $\wt\Pic(X)$ be the group of isomorphism classes of pairs $(L,s)$ with $L$ line bundle and $s\in L_\xi\nz$. Operations extend in the obvious way ($s^\vee\in L^\vee_\xi=\Hom_{k(X)}(L_\xi,k(X))$ is the functional defined by $s^\vee(s)=1$ and the identity is given by $[(\Oc_X,1)]$ now).
- We can define $\div:\wt\Pic(X)\to \Div(X)$ by taking the [[Weil divisors|divisor of the rational section]]. 
- We also have a "forgetful" map $\wt \Pic(X)\to \Pic(X)$, whose kernel is given by the different choices of rational section up to isomorphism, that is, $L_\xi^\times /\Oc(X)^\times\cong k(X)^\times/\Oc(X)^\times$.
- We have a commutative diagram with exact rows
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd} 1 & {\mathcal{O}(X)^\times} & {k(X)^\times} & {\widetilde{\mathrm{Pic}}(X)} & {\mathrm{Pic}(X)} & 0 \\ 1 & {\mathcal{O}(X)^\times} & {k(X)^\times} & {\mathrm{Div}(X)} & {\mathrm{Cl}(X)} & 0 \arrow[from=1-1, to=1-2] \arrow[from=1-2, to=1-3] \arrow["{=}"{marking, allow upside down}, draw=none, from=1-2, to=2-2] \arrow["\alpha", from=1-3, to=1-4] \arrow["{=}"{marking, allow upside down}, draw=none, from=1-3, to=2-3] \arrow[from=1-4, to=1-5] \arrow["{\mathrm{div}}", from=1-4, to=2-4] \arrow[from=1-5, to=1-6] \arrow[from=2-1, to=2-2] \arrow[from=2-2, to=2-3] \arrow["{\mathrm{div}}", from=2-3, to=2-4] \arrow[from=2-4, to=2-5] \arrow[from=2-5, to=2-6] \end{tikzcd}
\end{document}
```
- the second row is exact by definition of [[Class group]]. We just checked that the first row is exact ($\al(f)=[(\Oc_X,f)]$). Because of this we have an induced map $\Pic(X)\to \Cl(X)$ given by choosing an arbitrary rational section and taking the class of [[Weil divisors|its divisor]].
- This map is injective exactly when $\wt\Pic(X)\to \Div(X)$ is injective by diagram chasing. If $(L,s)$ is such that $\div s=0$ then $s\in L(X)^\times\subseteq L(X)$ and so the map $\Oc_X\to L$ it induces is an isomorphism, meaning that $[(L,s)]=[(\Oc_X,1)]$.

The image of this injection are the [[Cartier divisors]].

Notice also that $\Pic(X)=\Cl(X)$ if and only if $\CDiv(X)=\Div(X)$. This condition is equivalent to requiring that all divisors that consist only of a single point are locally principal. If $V=\ol{\cpa{p}}$ for $p\in X^{(1)}$ then this translates to requiring that the [[Sheaves of ideals|sheaf of ideals]] $\Ic_V$ is locally principal or, equivalently, that it is a line bundle (one of the exercises).

From commutative algebra we see that if $\Ic_V$ is locally principal and $p\in V$ is such that $V$ is regular at $p$ then $X$ must also be regular at $p$.


$\Pic(X)=\Cl(X)$ if and only if $X$ is locally factorial
- $\Pic(X)=\Cl(X)$ is equivalent to $\Ic_{V,p}\subseteq \Oc_{X,p}$ principal for all $p\in V$ and all $V\in X^{(1)}$
- The condition above means that all primes of height 1 in $\Oc_{X,p}$ are principal
- Since $\Oc_{X,p}$ is a normal Noetherian domain, that condition [[Class group|means]] that $\Oc_{X,p}$ is UFD.