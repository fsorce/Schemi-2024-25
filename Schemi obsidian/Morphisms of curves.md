#curves 

Let $X,Y$ be curves and $f:X\to Y$ a morphism of $k$-schemes, then we have two possibilities:
1. $f$ is constant and the image is a rational point of $Y$.
2. $f$ is surjective, finite and flat.
Proof:
- If $f$ is constant with image $p$ then $X\to Y$ factors through $X\to\Spec k(p)$. Taking global sections of this we get $k(p)\to H^0(X,\Oc_X)=k$, but $k(p)$ was already an extension of $k$, so $p$ is rational. 
- If $f$ is not constant it is surjective and has finite fibers
	- surjective: image is irreducible closed, not a point and target is irreducible of dimension 1
	- finite fibers: same reasoning because proper implies that the fibers are closed and a single fiber can't be the whole of $X$ because $f$ is not constant. 
- Since $X$ is proper, by [[Proper morphisms|Chevalley's theorem]] we have that $f$ is finite. 
- Since $X$ and $Y$ are smooth of dimension 1, by [[Flat morphisms|miracle flatness]] this means that $f$ is also flat, thus $X$ dominates $Y$ because curves are integral.
We define the [[Finite morphisms|degree]] of a dominant morphism of curves $X\to Y$ to be $[k(X):k(Y)]$.

If $f:X\to Y$ is a dominant morphism then for all closed point $q\in Y$ we have that $$\deg f=\sum_{p\in f\ii(q)}[k(p):k(q)]e_p(f)$$where $e_p(f)=v_p(f^\sharp t_q)$ is the **ramification index** of $f$ at $p$.
- If $q\in Y$ closed, $\deg f=\dim_{k(q)}H^0(f\ii(q),\Oc_{f\ii(q)})$. Note that we have a decomposition $H^0(f\ii(q),\Oc_{f\ii(q)})=\bigoplus_{p\in f\ii(q)}\Oc_{f\ii(q),p}$.
- If $t_q\in \Oc_{Y,q}$ is a uniformizing parameter we can write $\Oc_{f\ii(q),p}=\dfrac{\Oc_{X,p}}{(f^\sharp t_q)}$
- Since $\Oc_{X,p}$ is also a DVR, we have that $(f^\sharp t_q)=(t_p^{v_p(f^\sharp t_q)})=\mf_p^{e_p(f)}$. This shows that$$\dim_{k(q)}\Oc_{f\ii(q),p}=[k(p):k(q)]\dim_{k(p)}\Oc_{f\ii(q),p}=[k(p):k(q)]\cdot e_p(f).$$
Note that since [[Rational functions|any rational map extends to codimension 1 points]] we have that rational maps between curves extend to morphisms. 
This means that dominant morphisms between curves correspond to extensions of the fields of rational functions. In particular a morphism of curves is an *isomorphism iff it has degree 1*.

Dominant morphisms $\Pj^1\to \Pj^1$ correspond to $f\in k(x)\bs k$. If we write $f=p/q$ with $p,q\in k[x]\nz$ not both constants and relatively prime then the degree of the induced morphism $F$ is $\max\cpa{\deg p,\deg q}$.
- If $\deg p\geq \deg q$ then $F\ii([1:0])=\Spec \dfrac{k[x]}{(p(x))}$ and this has $\deg p$ points counted with multiplicity
- If $\deg p<\deg q$ consider the map induced by $1/f$ and note that both have the same degree because we can switch between them via an automorphism of the codomain.


