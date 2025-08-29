Jacobson rings
- DVR is not Jacobson.
- Ring with $\Spec_mA$ dense but not very dense ($R[x]$ with $R$ a DVR)

Sheaves and Presheaves:
- Small base space:
	- $\Pre(\emptyset)=\Ab$, $\Sh(\emptyset)=\cpa0$. 
	- $\Pre(pt)=\Arr(\Ab)$, $\Sh(pt)=\Ab$.
	- $X$ discrete, $\Sh(X)=\prod_{x\in X}\Ab$.
- If $f:X\to pt$ then $f_\ast\Fc=\Fc(X)$.
- If $Y$ is a point then the pullback via $f:X\to Y$ as presheaf of some sheaf on $Y$ may not be a sheaf on $X$ (for example for $X$ disconnected).
- Consider a scheme morphism $f:X\to \Spec k$. The pullback as a sheaf of $\Oc_{\Spec k}$ are the locally constant functions on $X$ with values in $k$, and this is certainly not a $\Oc_X$-module in general.

Morphism of ringed spaces but not of locally ringed spaces
- Let $A$ be a local domain, $K=\Frac A\neq A$, consider $(f,f^\sharp):\Spec K\to \Spec A$ with $f(\eta)=s$ where $\Spec K=\cpa{\eta}$ and $s$ is the only closed point of $A$. We then set $f^\sharp_U=0$ is $U\neq X$ and $f^\sharp_X:A\to K$ is the inclusion.

Non-affine schemes: $\A^2\bs \cpa{(0,0)}$, $\Pj^1$...
The line with two origins is not affine and cannot be an open subset of an affine.

Projective stuff:
- In general $\Gamma(\Proj A,\Oc_{\Proj A})\neq A_0$, for example $\Proj R=\emptyset$ when $R=R_0$.
- $\Proj R[x]\cong \Spec R$ with standard grading.
- $A_0\to \Gamma(\Proj A,\Oc)$ gives $\Proj A$ a structure of $A_0$-scheme.

Closed subspace of a scheme which is not a closed subscheme:
- $X=\A^1_k$, $Y=(\cpa{(x)}, \Jc)$ with $\Jc(U)=\bigcap I_{Y_n}(U)$, $Y_n=\Spec k[x]/(x^{n+1})$.

$\Spec A$ Noetherian topological space does not imply $A$ Noetherian.
- $k$ field, $V$ an infinite dimensional vector space over $k$, $A=k\oplus V$ with the product $$(\la,v)\cdot (\mu,w)=(\la\mu,\la w+\mu v).$$Note that all vector subspaces of $V$ become ideals in $A$, so $A$ is not Noetherian. However $\sqrt{(0)A}=V$ (all elements $(0,v)$ square to $0$ and $(\la,v)^n=(\la^n,n\la v)$ so if $\la\neq 0$ then the first entry is never $0$) so $\Spec A$ and $\Spec A/V=\Spec k$ have the same underlying topological space, a point, which is a Noetherian topological space.

Quasi-compact morphisms:
- NOT local on the domain: Take $X\to \Spec k$ with $X$ not q.c.. Since $X$ is covered by affine open, which are q.c., we fail the "check the property locally" condition.
- There exists $f:X\to Y$ with $X,Y$ quasi-compact but $f$ not quasi-compact: Let $X$ be affine that has some non-q.c. open subset. Set $Y=X\amalg_U X=X_1\cup X_2$ fibered coproduct. $Y$ is q.c. because it is the union of two q.c. spaces but the inclusion $f:X\equiv X_1\inj Y$ is such that $U=f\ii(X_2)$.

Affine morphisms:
- Open immersions are not always affine: $U\inj X$ with $X$ affine and $U\subseteq X$ open but not affine.
- The $\G_m$-projection of $\Proj$ is affine: If $A$ graded, the projection $\Spec A\bs V_+(A_+)\to \Proj A$ is affine.

Dimension:
- There exists $A$ Noetherian domain such that $\codim_p \Spec A=\dim A_p$ is not $\dim A$ even when $p$ is a closed point. Take $R$ a DVR and $A=R[x]$. The point $(xt-1)$ is closed but has height 1 when $\dim R[x]=2$.

Smoothness:
- The Jacobian criterion can fail for non-rational points: take $k$ with $\cha k=p$ not perfect and $X=k[x]/(x^p-a)$ with $a\in k\bs k^p$. $X$ is a point and it is regular but the rank of the Jacobian matrix is 0 instead of 1 ($n=1$ in this case).

Flatness:
- Locally constant dimension of fibers but module not flat: $A=k[x]/(x^2)$, $M=A/(x)=k$ is not free (and so not flat since $A$ local) but the dimension of fibers is constant because $\Spec A=\cpa{(x)}$ is just a point.
- The ideal $(x,y)$ is a module over $k[x,y]$ and it is not flat.
- Even if $p\mapsto \dim_pf\ii(f(p))$ is constant there is no guarantee that $f$ is flat: $\Spec k\to \Spec k[\e]$.

Dense but not schematically dense:
- Consider $X=\Spec\dfrac{k[x,y]}{(y^2,xy)}$ (line with thick origin). If we take $U=X_x=\A^1\nz$ then $\ol U=\A^1\subsetneq X$, so $U$ is not schematically dense in $X$.

Quasi-coherent sheaves:
- Direct product of $\QCoh$ is not always $\QCoh$: 
	- $X=\A^1_k$, $\Fc=\Oc_X^\N$ is not quasi-coherent
	- the ideal sheaf in the example of closed subspace which isn't a closed subscheme

Not geometrically connected:
- $\Spec\C\to \Spec \R$ is not geometrically connected, the base change to $\C/\R$ consists of two disjoint points.

Cohomology of some sheaves on $\Pj^1_k$:
- Consider $k=\ol k$, we want to compute $H^1(\Pj^1_k,\Oc_{\Pj^1_k}^\times)$.
	- Set $K=k(\Pj^1_k)=k(t)$ and note that $\Oc_{\Pj^1_k}^\times\subseteq K_{\Pj^1_k}^\times$, we thus get $0\to \Oc_{\Pj^1_k}^\times\to K_{\Pj^1_k}^\times\to Q\to 0$ for some quotient $Q$.
	- It turns out that $Q=\bigoplus_{p\in \Pj^1_k(k)}\Z$ with the map given by taking the valuation of a rational function at the point $p$ (we have $(K^\times/\Oc_{\Pj^1_k,p}^\times,\cdot)\cong (\Z,+)$).
	- This is a flabby resolution: $K_{\Pj^1_k}^\times$ is flabby because $\Pj^1_k$ is irreducible and $\bigoplus_{p\in \Pj^1_k(k)}\Z$ is flabby because $\Pj^1$ is Noetherian (so all open are quasi-compact and thus $(\bigoplus_{p\in \Pj^1_k(k)}\Z)(U)=\bigoplus_{p\in \Pj^1_k(k)}\Z(U)=\bigoplus_{p\in U(k)}\Z$.
	- So $H^1(\Pj^1_k,\Oc_{\Pj^1_k}^\times)=\coker(k(t)^\times\to \bigoplus_{p\in \Pj^1_k(k)}\Z)$ and this is isomorphic to $\Z$ because the image of $k(t)^\times$ yield exactly all collections that sum to $0$.
- We may proceed analogously for $H^1(\Pj^1_k,\Oc_{\Pj^1_k})$, but in this case we have $K/\Oc_{\Pj^1_k,p}$ (additive), which amounts to specifying a Laurent tail. 

Class group
- If $f\in k[x_0,\cdots, x_n]_d\nz$ irreducible then $\Cl(k[x_0,\cdots, x_n]_{(f)})=\Cl((\Pj^n_k)_f)=\dfrac{\Cl(\Pj^n_k)}{\ps{[V_+(f)]}}=\znz d$, so the ring $k[x_0,\cdots, x_n]_{(f)}$ is regular but not a UFD.

Curves:
- If $g(X)=0$ then $\deg K=-2$ so $-K$ is very ample and so $X\inj \Pj^2$ injection of degree 2. This means that every genus 0 curve is realized as a plane conic.