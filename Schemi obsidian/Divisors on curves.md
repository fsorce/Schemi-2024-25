#curves 

[[Weil divisors|Divisors]] on curves have a degree. If $D=\sum_{p\in X^{(1)}} n_p p$ then $\deg D=\sum_{p\in X^{(1)}}n_p[k(p):k]$.

If $X$ is a curve and $f\in k(X)^\times$ then $\deg(\div(f))=0$.
- If $f\in k^\times$ then $\div(f)=0$ and we are done.
- Given a rational function $f\in k(X)\bs k$ we get a dominant morphism $f:X\to \Pj^1$
- Note that $p\in f\ii(0)\coimplies v_p(f)>0$ and $p\in f\ii(\infty)\coimplies v_p(f)<0$.
- Let us write $\div(f)=\div_+(f)-\div_-(f)$ with $\div_{\pm}(f)\geq 0$ and note that  $$\div_+(f)=\sum_{p\in f\ii(0)}v_p(f)p,\quad\div_+(f)=\sum_{p\in f\ii(\infty)}-v_p(f)p$$because of the previous bullet point.
- Since $k(0)=k(\infty)=k$ we have that (careful about the [[Morphisms of curves|ramification indices]])$$\deg(\div_+(f))=\sum_{p\in f\ii(0)}v_p(f)[k(p):k]\overset{f^\sharp t=f}=\sum_{p\in f\ii(0)}e_p(f)[k(p):k]=\deg(f)\overset{\text{analogous}}=\deg(\div_-(f))$$where in the last equality we used $e_p(f)=v_p(f^\sharp(t\ii))=v_p(f\ii)=-v_p(f)$ for $p\in f\ii(\infty)$.
- This shows that $\deg(\div(f))=\deg(\div_+(f))-\deg(\div_-(f))=0$.
This result shows that the degree is actually well defined on $\Cl(X)$.

Since curves are smooth, the [[Picard group]] coincides with the class group, so we can talk about the degree of a line bundle.


If $k=\ol k$ and $\deg:\Pic(X)\to \Z$ is injective then $X\cong \Pj^1$.
- This means that if $p,q\in X(k)$ are distinct rational points then $X\not\cong \Pj^1\implies [p-q]\neq 0$ in $\Cl(X)$.
- Suppose $p-q=\div(f)$ for $f\in k(X)^\times$, then $\div_+(f)=p$ and so $\deg(f)=1$, this would give an isomorphism $f:X\to \Pj^1$.

Let $j:X\to \Pj^n$ be a closed embedding and let $d=\deg X$ be the [[Hilbert polynomial|degree]] of $X$ as a closed subscheme, so that $\chi(j_\ast\Oc_X(t))=dt+1-g$ . It turns out that $d=\deg(\Oc_X(1))$ where this is the degree of the line bundle ($\Oc_X(1)=j^\ast(\Oc_{\Pj^n}(1))$).
- Let $h\in H^0(\Pj^n,\Oc(1))$ be such that $X\not\subseteq H$ where $H=V_+(h)=\div h$. Note that $s=j^\ast h\neq 0$.
- Note that $\div s=X\cap H$, so $\deg(\Oc_X(1))=\deg(\div(s))=\dim H^0(X\cap H,\Oc)$. 
- Since $\dim X\cap H=0$ we have $$\deg(\Oc_X(1))=\chi(\Oc_{X\cap H})=\chi(\Oc_X)-\chi(\Oc_X(-1))=1-g - (d(-1)+1-g)=d.$$
Since pullback of isomorphism classes of line bundles is well defined, we can define $f^\ast:\Cl(Y)\to \Cl(X)$, and this lifts to $f^\ast:\Div(Y)\to \Div(X)$ as follows:
- On a point we set $f^\ast(q)=f\ii(q)=\sum_{p\in f\ii(q)}e_pp$
- For a general divisor just extend by linearity.

If $f:X\to Y$ is a dominant morphism and $L$ is a line bundle on $Y$ then $\deg(f^\ast L)=\deg(f)\deg(L)$.
- First consider $L=\Oc_Y(q)$ for some point, then use linearity and $f^\ast(L_1\otimes L_2)=f^\ast L_1\otimes f^\ast L_2$.


##### Morphisms to projective space associated to divisors:

We call a divisor $D$ very ample when $\Oc_X(D)$ is [[Very ample line bundles|very ample]]. Note that $D$ is very ample iff $D_{\ol k}\in \Div(X_{\ol k})$ is very ample, so from now we suppose $k=\ol k$.

The sections of $H^0(D)$ define a morphism to $\Pj(H^0(D)^\vee)$ by evaluation exactly when $D$ is base point free (i.e. when any basis of $H^0(D)$ [[Morphisms to projective space|has no common zeros]]). 
This means that $D$ gives a morphism iff $h^0(D-p)=h^0(D)-1$ for all $p\in X(k)$.

The [[Canonical sheaf|canonical divisor]] defines a morphism to $\Pj^{g-1}$ when $g\geq 1$ (a dominant one when $g\geq 2$).
- By the [[Riemann-Roch theorem]] $h^0(K-p)=h^0(p)+2g-2-1+1-g=g-1$.
This morphism is called the *canonical morphism* (or canonical map).

If $D$ defines a morphism $f:X\to \Pj^n$ ($n=h^0(D)-1$) then $\Oc_X(D)=f^\ast(\Oc_{\Pj^n}(1))$, in particular $$\cpa{\text{linear forms on }\Pj^n}=H^0(\Pj^n,\Oc(1))\cong H^0(X,\Oc(D))=\cpa{E\in \Div(X)\mid E\sim D,\ E\geq 0}\cdot k^\times$$thus hyperplanes $H$ in $\Pj^n$ correspond to effective divisors on $X$ that are equivalent to $D$ and the way we translate between them is that if $H=V_+(h)$ then $E=\div(f^\ast h)=f\ii(H)$.


Theorem: The map induced by $D$ is injective iff $h^0(D-p-q)=h^0(D)-2$ for all $p,q\in X(k)$ $p\neq q$.
Theorem:  $\Oc(D)$ is very ample if and only if $h^0(D-p-q)=h^0(D)-2$ for all $p,q\in X(k)$.

This implies immediately that if $\deg D\geq 2g+1$ then $D$ is very ample.


