#curves

A curve is a [[Smooth schemes|smooth]] [[Projective space|projective]] [[Geometrically connected]] scheme of dimension 1 over a field $k$.
Note that smooth+geometrically connected implies [[Integral schemes|integral]].
Local rings of curves are DVR.

The [[Genus]] of a curve $X$ is $h^0(\omega_X)=h^1(\Oc_X)$ where the equality is given by [[Canonical sheaf|Serre duality]].

[[Morphisms of curves]] correspond to rational functions. They have a degree which can be computed by the field of rational functions or by looking at ramification in the fibers.

Suppose $k=\ol k$. There is a contravariant equivalence of categories$$\cpa{\text{Curves,\ dominant morphisms}}\longleftrightarrow\cpa{\text{fin.gen. field extensions of $k$ with $\trdeg_k=1$}}$$We already know that dominant [[Morphisms of curves]] correspond to field extension with $\trdeg_k=1$ so we just need to find a way to construct a curve when starting from a field $K$ with $\trdeg_kK=1$.
- write $K=k(a_1,\cdots, a_n)$, set $A=k[a_1,\cdots, a_n]\subseteq K$. 
- Clearly $A$ is a domain and $\Frac A=K$. $\dim A=\trdeg_k\Frac A=\trdeg_k K=1$.
- Let $U=\Spec A\subseteq\A^n$ and let $X=\ol U\subseteq \Pj^n$ be the closure in $\Pj^n$. We know that $X$ is a projective integral scheme of dimension 1 with $k(X)=K$.
- Let $\ol X$ be the normalization of $X$. This keeps all properties we listed and adds normality, but since $\ol X$ has dimension 1 and is a scheme over $k=\ol k$, normality [[Smooth schemes|implies smoothness]] because algebraically closed fields are perfect.

[[Divisors on curves]] have a notion of degree, which passes to line bundles in a meaningful way. We can also pull back divisors.


If $f:X\to Y$ is dominant then $g(X)\geq g(Y)$.
- If $f$ is separable this follows immediately from the [[Riemann-Hurwitz theorem]] since $\deg f\geq 1$.
- Fact: if $k(X)/k(Y)$ is purely inseparable then $g(X)=g(Y)$.
- If $K\subseteq k(X)$ is the separable closure of $k(Y)$ and $Z$ is a curve such that $k(Z)=K$ then we can factorize $X\to Y$ as $X\to Z\to Y$ with $X\to Z$ purely inseparable and $Z\to Y$ separable. This gives $g(X)=g(Z)\geq g(Y)$.


If $g=g(X)=g(Y)\geq 2$ then any dominant morphism of curve $f:X\to Y$ is an isomorphism
- By the [[Riemann-Hurwitz theorem]] we have that $(1-\deg(f))(2g-2)\geq 0$ and $2g-2\geq 0$ because $g\geq 2$, so $1\geq \deg f$ and we know that [[Morphisms of curves|morphisms of degree 1 are isomorphisms]].
 


##### Cohomology of divisors:

Suppose $k=\ol k$ and pick $p\in X(k)$ and $D\in \Div(X)$. The point $p$ is a **base point** of $D$ if the map $H^0(D)\to k$ given by evaluation at $p$ is not surjective.
We can easily see with sheaf cohomology that $h^0(D)-h^0(D-p)\in \cpa{0,1}$ and it is $0$ iff $p$ is a base point of $D$.
From this we get that if $\deg D\geq 1$ and $X_{\ol k}\not\cong \Pj^1_{\ol k}$ then $h^0(D)\leq \deg D$.

The main tool at our disposal to compute cohomology of divisors is the [[Riemann-Roch theorem]].

A curve $X$ has [[Genus]] $0$ if and only if $X_{\ol k}\cong \Pj^1_{\ol k}$.
- WLOG $k=\ol k$. Just look at the [[Forms on projective schemes|canonical sheaf of P^1]]: $\omega_{\Pj^1}=\Oc_{\Pj^1}(-2)\implies g=h^0(\omega_{\Pj^1})=0$
- By [[Riemann-Roch theorem|Riemann-Roch]] $h^0(p)=1+1-0=2$ for any $p\in X(k)$, so $p\sim q$ for $p\neq q$ and thus we have $X\to \Pj^1$ of [[Morphisms of curves|degree 1, which is an isomorphism]].
If $g(X)=0$ but $X(k)=\emptyset$ then the image of $\deg:\Cl(X)\to \Z$ is $2\Z$.
- $\deg K=-2$ so $2\Z$ is in the image.
- If $\deg D=2n+1$ then $\deg(D+nK)=1$ and by [[Riemann-Roch theorem|Riemann-Roch]] we have $h^0(D+nK)=2\neq 0$, showing that $D+nK\sim E$ for $E$ effective of degree 1, i.e. $E=p\in X(k)$.  

We may try to describe curves as [[Complete intersection curves|complete intersections]] in appropriate projective spaces. 



An important type of curve are the [[Hyperelliptic curves]].










