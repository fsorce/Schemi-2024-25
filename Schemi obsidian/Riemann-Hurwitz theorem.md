#curves

A [[Morphisms of curves]] is called **separable** if $k(X)/k(Y)$ is a separable extension.
If $\cha k\nmid \deg f$ then $f$ is separable.

Throughout this file we assume $k=\ol k$.

Consider a **separable** morphism of curves $f:X\to Y$. There exists a **ramification divisor** $R$ on $X$ such that$$2(X)-2=(\deg f)(2g(Y)-2)+\deg R.$$   - Looking at the statement, we have to relate $\omega_X$ and $f^\ast\omega_Y$ in some way.
- Consider the exact sequence of [[Sheaf of differentials]] ${f^\ast\Omega_{Y/k}}\to {\Omega_{X/k}}\to \Omega_{X/Y}\to 0$. In terms of the [[Canonical sheaf]] this is$$f^\ast\omega_Y\to \omega_X\to \Omega_{X/Y}\to 0$$We would like to show injectivity of the first map so that this becomes a short exact sequence.
- Since $X$ and $Y$ are smooth, the canonical sheaves are line bundles, so the first map is either injective or the zero map. 
- We just need to check one stalk so consider $\Spec k(X)=\xi$ generic point of $X$. Since $\omega_X$ is a line bundle, the stalk is not 0, so if we can show surjectivity we have that the map is not zero and therefore injective. We thus want to show that $\pa{\Omega_{X/Y}}_\xi=0$.
- [[Sheaf of differentials|Recall]] that if $X\to Y$, $Y'\to Y$ and $X'=Y'\times_Y X$ then $\Omega_{X'/Y'}\cong \pr_2^\ast\Omega_{X/Y}$.
- Let $\eta$ be the generic point of $Y$ and note that $f(\xi)=\eta$, i.e. $\eta\times_Y X=\xi$. Combining with the above$$\Omega_{k(X)/k(Y)}=\Omega_{\xi/\eta}\cong (\xi\to X)^\ast\Omega_{X/Y}=(\Omega_{X/Y})_\xi$$so the stalk we are interested in is $\Omega_{k(X)/k(Y)}$.
- Since $f$ is separable, $k(X)/k(Y)$ is a [[Kähler differentials - Algebra|separable extension and so]] $\Omega_{k(X)/k(Y)}=0$.
- We now have $0\to f^\ast\omega_Y\to \omega_X\to \Omega_{X/Y}\to 0$, so by tensoring with $\omega_X^\vee$ we get$$0\to f^\ast\omega_Y\otimes\omega_X^\vee\to \Oc_X\to \Omega_{X/Y}\otimes\omega_X^\vee\to 0$$showing that $\Omega_{X/Y}\otimes \omega_X^\vee$ is a quotient of $\Oc_X$ with kernel given by a line bundle, thus$$\Omega_{X/Y}\otimes\omega_X^\vee\cong \Oc_R,\qquad f^\ast\omega_Y\otimes\omega_X^\vee\cong \Oc_X(-R)$$for some [[Cartier divisors|Cartier divisor]] $R$ in $X$.
- Taking the [[Divisors on curves|degree]] on both sides of $f^\ast\omega_Y\otimes\omega_X^\vee\cong \Oc_X(-R)$ we get the desired result.

Note that, since $\Oc_R$ is a skyscraper sheaf, $\Oc_R\cong \Omega_{X/Y}$. This means that if $R=\sum_{p\in X^{(1)}} e_p'(f)p$ then $e_p'(f)=\dim_k(\Omega_{X/Y})_p$. Let's relate $e_p'(f)$ with the [[Morphisms of curves|ramification index]] $e_p(f)$:

If $q\in Y$, $p\in f\ii(q)$, $t_p,t_q$ are uniformizers of $\Oc_{X,p}$ and $\Oc_{Y,q}$ respectively and $f^\ast t_q=ut_p^{e_p(f)}$ for some $u\in \Oc_{X,p}^\times$ then we have that$$e_p'(f)=e_p(f)-1+v_p\pa{e_p(f)u+t_p\dd{t_p}u}$$so in particular $e_p'(f)\geq e_p(f)-1$ and equality holds exactly when $\cha k\nmid e_p(f)$.
- Let us write $f^\ast(dt_q)=\vp dt_p$ for some $\vp\in \Omega_{X,p}$. 
- Note that $\displaystyle e_p'(f)=\dim_k(\Omega_{X/Y})_p=\dim_k\frac{\Omega_{X,p}}{f^\ast\Omega_{Y,q}}=\dim_k\frac{\Oc_{X,p}dt_p}{(f^\ast(dt_q))}=\dim_k\frac{\Omega_{X,p}}{(\vp)}=v_p(\vp)$.
- Note that $\vp dt_p=f^\ast(dt_q)=d(f^\ast t_q)=d(ut_p^{e_p(f)})=du t_p^{e_p(f)}+ue_p(f)t_p^{e_p(f)-1}dt_p$ so $$\vp=\dd{t_p}ut_p^{e_p(f)}+ue_p(f)t^{e_p(f)-1}\implies v_p(\vp)=e_p(f)-1+v_p\pa{\dd{t_p}{u}t_p+ue_p(f)}.$$
Theorem (**Riemann-Hurwitz**) Let $f:X\to Y$ a dominant [[Morphisms of curves]] such that $\cha k\nmid e_p(f)$ (for example $\cha k=0$ or $\cha k>\deg f$), then$$2g(X)-2-(\deg f)(2g(Y)-2)=\sum_{p\in X(k)}(e_p(f)-1)=\sum_{q\in Y(k)}(\deg f-\abs{f\ii(q)})$$where $\abs{f\ii(q)}$ is the number of distinct points in the [[Fibers|fiber]] of $f$ over $q$.





