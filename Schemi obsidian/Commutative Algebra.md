Jacobson rings

Dimension theory:
- Going up
- Hauptidealsatz

Graded commutative algebra

Finite, finite type, integral

Noether normalization

*Nakayama* to say $M_p=0\coimplies M\otimes k(p)=0$ and thus $M_p\otimes N_p=0\coimplies M_p=0$ or $N_p=0$ because of dimension.

Normal:
- UFD implies Normal
- Noeth+Int.dom then $A_\pf$ is DVR if $\mathrm{ht}(\pf)=1$ and $A=\bigcap_{\mathrm{ht}(\pf)=1}A_{\pf}$.
- If $A$ is fin.type $k$-alg. then integral closure is finite over $A$.
	- $K=\Frac A$, If $L/K$ finite extension we claim that $\ol{A}^L$ is finite over $A$ (the thesis is $K=L$).
	- By Noether normalization $R=k[x_1,\cdots,x_r]\subseteq A$ finite, so $\ol A^L=\ol R^L$ so for the stronger thesis WLOG $A\cong k[x_1,\cdots, x_r]$.
	- $L/K$ separable
	- $L/K$ purely inseparable
	- $L/K$ finite, up to extending $L$ assume $L/K$ normal. $L^{\Aut(L/K)}/K$ is purely inseparable and $L/L^{\Aut(L/K)}$ is separable.

Regularity:
- $A$ local Noetherian is regular if $\dim_{A/\mf}\mf/\mf^2=\dim A$.
- Auslander-Buchsbaum-Serre: regular iff finite global dimension, so can check regularity only on maximals.
- Local regular implies UFD
- If $A\to B$ is local, flat, both rings are Noetherian and $B$ is regular then $A$ is also regular. 
	- Use global dimension argument
- If $R$ is a local Noeth. domain, $f\in\mf\nz$ and $R/(f)$ is regular then $R$ is also regular.


Flatness:
- Field extensions are flat.
- If $A$ Noeth. and $M$ finite, $M$ is flat iff it is projective iff $M_\pf$ free for all $\pf\in \Spec A$.
- If $A$ Noeth., $M$ finite and flat then $\pf\mapsto \dim_{k(\pf)}M\otimes k(\pf)$ is locally constant on $\Spec A$.
- $A$ **reduced** Noeth, $M$ finite, $\pf\mapsto \dim_{k(\pf)}M\otimes k(\pf)$ loc. cost. then $M$ is flat.
- Inductive limit (colimit with indices) of flat modules is flat
- $M$ faithfully flat iff flat and no empty fibers ($M\otimes k(p)\neq 0$ for all $p\in \Spec_m A$)
- flat + local homomorphism $\implies$ faithfully flat homomorphism
- Let $A\to B$ be local, $A,B$ Noetherian, $C=B\otimes_A k(A)$.
	- $\dim B\leq \dim A+\dim C$
	- If $A\to B$ is flat we have equality
	- **Miracle flatness**: If $A,B$ are regular then equality implies flatness
- If $A\to B$ local and flat, $A,B$ Noetherian then
	- $B$ regular $\implies$ $A$ regular (use $\gldim$)
	- $B$ normal domain $\implies$ $A$ normal domain
- $A$ regular domain, $\dim A=1$, then $M$ flat iff torsion free


Associated primes (Noetherian rings)
- $\Ass_A(M)=\cpa{\pf\in \Spec A\mid \exists m\in A\ s.t.\ \pf=\Ann_A(m)}$.
- $\Ass_A(M)=\cpa{\pf\in \Spec A\mid \exists A/\pf\inj M}$ (take the immersion given by $[1]\mapsto m$ from above).
- If $M$ finite over $A$, $\Ass_A(M)$ is finite.
- Associated prime behave well with localization.
- $\pf\in \Ass_A(M)$ iff $\pf A_\pf\in \Ass_{A_\pf}(M_\pf)$.


Given $A\to B,\ M\in \Mod_A,\ N\in \Mod_B$ we have an adjunction$$\Hom_B(M\otimes_A B, N)\cong \Hom_A(M,N).$$

