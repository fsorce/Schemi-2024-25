#curves 

Suppose $k=\ol k$. The following are equivalent
1. A [[Divisors on curves|divisor]] $D$ with $\deg D=2,\ h^0(D)=2$ exists
2. There exist $p,q,p',q'\in X(k)$ such that $p+q\sim p'+q'$ but $\cpa{p,q}\cap \cpa{p',q'}=\emptyset$
3. $\div f=p+q-p'-q'$ with no cancellation for some $f\in k(X)^\times$. 
4. We can find $X\to \Pj^1$ of [[Morphisms of curves|degree]] 2 (dominant rational maps of curves extend to morphisms).

A curve $X$ over $k$ is hyperelliptic if $X_{\ol k}$ admits a degree 2 morphism to $\Pj^1_{\ol k}$ and $g(X)\geq 2$.

Note that if $\pi:X\to \Pj^1$ is of degree 2 and $X$ hyperelliptic then $\pi$ is separable
- a degree 2 extension is either separable or purely inseparable but purely inseparable morphisms preserve the genus.

All curves of [[Genus]] 2 are hyperelliptic
- By [[Riemann-Roch theorem|Riemann-Roch]], $\deg K=2$ and $h^0(K)=2$.

If $\cha k\neq 2$ and $k=\ol k$ then for all $g\geq 2$ there exists $X/k$ hyperelliptic curve with $g(X)=g$.
- Pick $a_1,\cdots, a_n\in k$ distinct and set $\vp(t)=(t-a_1)\cdots(t-a_n)$. Note that $\vp\in k[t]\bs k[t]^2$.
- Consider the field $K=\dfrac{k(t)[x]}{(x^2-\vp(t))}$ and note that it is a degree 2 extension of $k(t)=k(\Pj^1_k)$, so we get a morphism $\pi:X\to \Pj^1$ of degree 2 where $k(X)=K$.
- We have constructed an hyperelliptic curve, now we want to check that $g(X)$ can be arbitrary.
- Since $\cha k\neq 2$ and $\deg \pi=2$ the tame version of [[Riemann-Hurwitz theorem|Riemann-Hurwitz]] holds$$g(X)=\frac{\sum_{\la\in \Pj^1(k)}(2-\abs{\pi\ii(\la)})}2-1$$we want to compute the ramification.
- We have two affine charts for $X$ given by $\Spec({\ol{k[t]}^K})$ and $\Spec(\ol{k[t\ii]}^K)$. If we write $\vp(t)=t^n\psi(t\ii)$ and $y=xt^{-\ceil{n/2}}$ then these rings are$$\dfrac{k[x,t]}{(x^2-\vp(t))}\text{ and }\begin{cases}\dfrac{k[y,s]}{(y^2-\psi(s))} &\text{if $n$ even}\\\dfrac{k[y,s]}{(y^2-s\psi(s))} &\text{if $n$ odd}\end{cases}$$
- If $\vp(\la)\neq 0$, i.e. $\la\notin \cpa{a_1,\cdots, a_n}$, but $\la\neq \infty$ then $$\frac{k[t][x]}{(x^2-\vp(t),t-\la)}\cong \frac{k[x]}{(x-\sqrt{\vp(\la)})}\times \frac{k[x]}{(x+\sqrt{\vp(\la)})}$$so we have no ramification.
- If $\vp(\la)=0$ then with the same logic the fiber is given by $k[x]/(x^2)$, so we have $2-\abs{\pi\ii(\la)}=1$.
- If $\la=\infty$ then, since $\psi(0)\neq 0$ because $\vp(t)$ is monic, we get that $2-\abs{\pi\ii(\infty)}$ is $0$ for $n$ even an $1$ for $n$ odd.
- Putting everything together $g(X)=\ceil{n/2}-1$, so if we choose $n=2g+2$ then $g(X)=g$.
If $\cha k=2$ and $k=\ol k$ the proof is similar but we have to use the general version of the [[Riemann-Hurwitz theorem]] because 2 may divide the ramification. The equation is $x^2+x+\phi(t)\ii=0$ for $\phi(t)$ of degree $d>1$ and simple roots. The genus ends up being $d-1$.



If $g(X)\geq 2$ then the [[Divisors on curves|canonical map]] is an embedding if and only if $X$ is NOT hyperelliptic.
- The following are equivalences:
	- $X$ is hyperelliptic
	- there exist $p,q\in X(k)$ such that $h^0(p+q)=2$
	- By [[Riemann-Roch theorem|Riemann-Roch]] this is equivalent to $h^0(K-p-q)=g-1$ (and not $g-2$)
	- $K$ is not very ample (it still defines a morphism, so $h^0(K-p)=g-1$ anyway).


We want to understand how the [[Divisors on curves|canonical map]] behaves for hyperelliptic curves.

Since $\pi:X\to \Pj^1$ is separable the extension is Galois: $\Gal(k(X)/k(\Pj^1))\cong \znz2=\ps{\sigma}$. This is the **hyperelliptic involution**.
It is easy to see that $\pi^\ast(\pi(p))=p+\sigma(p)$ for all $p\in X(k)$.

The canonical map $f:X\to \Pj^{g-1}$ factors as $\pi:X\to \Pj^1$ followed by a Veronese embedding $\Pj^1\to \Pj^{g-1}$.
- By the [[Divisors on curves|cohomological criterion for injectivity]] of the induced map we see that $$p,q\in X(k),\ p\neq q,\ f(p)=f(q)\quad \coimplies\quad h^0(K-p-q)=g-1$$but by [[Riemann-Roch theorem|Riemann-Roch]] the second condition holds iff $h^0(p+q)=2$, thus $f=f\circ \sigma$ as a function. Since the schemes are reduced and of finite type over an algebraically closed field we actually get $f=f\circ \sigma$ as morphisms.
- We thus have a factorization $X\to \Pj^1\to \Pj^{g-1}$. Since $f$ is not [[Very ample line bundles|degenerate]], $\vp:\Pj^1\to \Pj^{g-1}$ also isn't. It must therefore be defined by $g$ linearly independent sections $s_0,\cdots, s_{g-1}\in H^0(\Pj^1,\vp^\ast\Oc_{\Pj^{g-1}}(1))$.
- Let $L=\Oc_{\Pj^1}(d)=\vp^\ast\Oc_{\Pj^{g-1}}(1)$ and note that $\pi^\ast L=\omega_X$ since $f^\ast\Oc_{\Pj^{g-1}}(1)=\omega_X$. Looking at the [[Divisors on curves|degrees]] this means that $2g-2=2d$, so $d=g-1$.
- This shows that $s_0,\cdots, s_{g-1}$ are $g$ linearly independent sections of $H^0(\Oc_{\Pj^1}(g-1))$, which has dimension $g$, so $\vp$ is defined by a basis of $H^0(\Oc_{\Pj^1}(g-1))$, which means that it is a Veronese embedding of degree $g-1$.



