#VectorBundles_and_Divisors

We develop the theory of divisors in the case of schemes that are [[Integral+Noetherian+Normal|Noetherian, integral  and normal]].

Set $X^{(1)}=\cpa{p\in X\mid \dim\Oc_{X,p}=1}=\cpa{V\subseteq X\mid \text{closed irred. of codimension }1}$. 
Because of the assumed properties  $\Oc_{X,p}\subseteq k(X)$ is a DVR for all $p\in X^{(1)}$, so we can define$$\ord_p(f)=v_p(f)\quad\text{where }v_p:k(X)^\times\to \Z\text{ the discrete valuation.}$$Because of an algebra result for normal rings we have that$$\Oc_X(U)=\cpa{f\in k(X)^\times\mid \forall p\in U^{(1)},\ \ord_p(f)\geq 0}\cup\cpa0.$$We define the group of divisors on $X$ as $\Div(X)=\bigoplus_{p\in X^{(1)}}\Z$. 

If $f\in k(X)^\times$ we can define $\div(f)=\sum_{p\in X^{(1)}}v_p(f)p$ and it is a divisor because this sum is finite:
- Let $U$ be an open such that $f\in \Oc_X(U)^\times$. This means that $v_p(f)=0$ for all $p\in U^{(1)}$.
- It follows that $\cpa{p\in X^{(1)}\mid v_p(f)\neq 0}\subseteq X^{(1)}\bs U\leftrightarrow\cpa{\text{irr.comp. of }X\bs U}$.
- Since $X$ is Noetherian, $X\bs U$ has a finite number of irreducible components.
Note that $\div(f)=0$ exactly when $f\in \Oc(X)^\times$. 

We define the [[Class group]] of $X$ as $\Cl(X)=\coker\div$.


If $\xi$ is the generic point of $X$ and $L$ is a [[Locally free sheaves|line bundle]] we can define a **rational section** of $L$ to be an element of $L_\xi\nz$ in analogy with [[Rational functions]].
We can associate a divisor to a rational section: if $p\in X^{(1)}$, $p\in U$ for some $U$ open that trivializes $L$ and $\vp:\rbar L_U\to \Oc_U$ is an isomorphism then for $s\in L_\xi\nz$ we set $v_p(s):=v_p(\vp(s))$. 
- This definition does not depend on $U$ of $\vp$ since changing them only serves to multiply $\vp(s)$ by an invertible rational function, so the divisor doesn't change.
We define $\div(s)=\sum_{p\in X^{(1)}}v_p(s)p\in \Div(X)$.

Note that like for rational functions, $v_p(s)\geq 0\coimplies s\in L_p$.

Divisors obtained from rational sections are called [[Cartier divisors]].

If $s\in L(X)$ then the $\div(s)\in \Div(X)$ give [[Effective Cartier Divisors]].