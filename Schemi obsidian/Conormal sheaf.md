#VectorBundles_and_Divisors 

Let $i:Y\to X$ be a [[Locally closed immersion]] that factors as a closed immersion in the open $U\subseteq X$ (let $j:Y\to U$ be the closed immersion). We define the conormal sheaf of this immersion as $$\Cc_YX=\Ic/\Ic^2=j^\ast\Ic\in \QCoh(Y)$$where $\Ic$ is the [[Sheaves of ideals|sheaf of ideals]] that cuts out $Y$ in $U$. The definition is actually independent of the choice of $U$ (if $V$ another open see that both sheaves coincide with the one given by $U\cap V$).

If $X$ and $Y$ are regular then $\Cc_YX$ is locally free of rank $\codim_Y X$.
- This is a local property so WLOG $X=\Spec A$, $Y=\Spec B$ with $B=A/I$. Thus $\Cc_YX=\wt{I/I^2}$. Let $\vp:A\to B$ be the projection.
- If $q\in Y=\Spec B$ and $p=\vp\ii(q)$ then $B_q=A_p/I_p$.
- Since $A_p$ and $B_q$ are both regular by assumption, there is a system of parameters $a_1,\cdots, a_m\in \mf_p$ such that the images $\ol{a_1},\cdots, \ol{a_n}\in \mf_q$ are a system of parameters for $B_q$ and $I_p=(a_{n+1},\cdots, a_m)$.
- $I_p/I_p^2=I_p\otimes_A B_q$ is a free $B_q$-module with basis $[a_{n+1}],\cdots, [a_m]$. They clearly generate. We now show linear independence:
	- Suppose they have a non-trivial $B_q$-relation $b_{n+1}a_{n+1}+\cdots + b_m a_m\in I_p^2$. If we quotient by $(a_{n+1},\cdots, a_{m-1})$ then we get that $b_ma_m\in I_p^2/(a_{n+1},\cdots, a_{m-1})=(a_m^2)$. 
	- Since $a_m$ is not a zero divisor modulo $(a_{n+1},\cdots, a_{m-1})$, $b_m\in (a_m)\subseteq I$ and since $B=A/I$ this means that $b_m=0$ in $B_q$. 
	- Iterating the argument we show that $b_{m-1}=0$ and so on until $b_{n+1}=0$, showing that the relation was actually trivial.
