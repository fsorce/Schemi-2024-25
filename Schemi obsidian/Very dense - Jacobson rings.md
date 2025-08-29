#Algebra 

$Y\subseteq X$ is Jacobson (Very dense) if for all closed $Z\subseteq X$ we have $Z\cap Y$ dense in $Z$.
Equivalently, open subsets of $Y$ correspond UNIQUELY to open subset of $X$ by intersection.


A ring is *Jacobson* if $\Spec_mA$ is Jacobson in $\Spec A$. 

TFAE (Varieties are specified by their closed points basically)
1. Jacobson
2. every prime is the intersection of some maximal ideals
3. every radical ideal is the intersection of some maximal ideals

**Thm** (NSS) If $R$ is Jacobson, $A$ is a f.t. $R$-algebra via $\vp:R\to A$ then $A$ is also Jacobson and if $\mf$ is maximal in $A$ then $\vp^\ast(\mf)$ is maximal in $R$ and $[k(\mf):k(\vp^\ast(\mf))]$ is finite.

(If $R=k=\ol k$ then we get that if $I\subseteq A$ proper ideal, $I\subseteq \mf$ and $k(\mf)$ finite extension of $k$, so $k=k(\mf)$. $A=k[a_1,\cdots, a_n]\to k(\mf)=k$ means that $(a_1-b_1,\cdots, a_n-b_n)=\mf$ is maximal in $A$ and contains $I$ where $b_i$ is the image of $a_i$ in $k(\mf)=k$)


Example:
Note that $\ol{\Spec_m A}=V(J(A))$ where $J(A)=\bigcap \mf$ is the Jacobson radical, so 
		$\Spec_m A$ is dense in $\Spec A$ when $J(A)=\Nc(A)=\sqrt{0}$.

If $R$ is a DVR with uniformizer $t$ and $A=R[x]$ then $J(A)=\sqrt0$ but $A$ is not Jacobson.
**pf**: 
- recall that $J(A)=\cpa{f\in A\mid 1-af\in A^\ast\ \forall a\in A}$ and that in our case $A^\ast=R$. If $f\neq0$ then we can find $a$ such that $1-af\notin R$, so $J(A)=0$.
- $V(x)=\Spec R[x]/(x)=\Spec R$ is a closed subset of $\Spec A$ and in this closed subset we have only one closed point, which is not dense. (if $R[x]$ was Jacobson then $R=R[x]/(x)$ would also be Jacobson by the NSS, but it isn't).
