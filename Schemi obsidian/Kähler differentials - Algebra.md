#Algebra

Let $A$ be an $R$ algebra, $M\in \Mod_A$. An $A$-derivation is an $R$-linear map $D:A\to M$ such that (Leibniz rule) $D(fg)=fD(g)+gD(f)$.
- If $D$ is an abelian group homomorphism and respects the Leibniz rule then it is a derivation iff it maps constants (elements of $R$) to 0.

We can consider the endofunctor of $\Mod_A$ given by $M\mapsto \Der_R(A,M)$. This functor is representable by the $A$-module $\Omega_{A/R}$.
- We quotient a free module by $R$-linearity and Leibniz rule:$$\Omega_{A/R}:=\dfrac{\bigoplus_{f\in A}\ol f A}{\ps{\forall r,s\in R\ \ \ol{rf+sg}-r\ol f-s\ol g,\ \ol{fg}-f\ol g-g\ol f}}$$The bar denotes that it is a basis element of the free group.
- For $f\in A$ we set $df=[\ol f]\in \Omega_{A/R}$.

Given $M\in\Mod_A$ we can define an algebra $A\oplus M$. We have bijections $$\Hom_A(\Omega_{A/R},M)\cong \Der_R(A,M)\cong \Hom_{R-alg}(A,A\oplus M)$$where the derivation $D:A\to M$ is identified with the map $A\to A\oplus M$ given by $a\mapsto (a,D(a))$.


Let $I$ be the kernel of the multiplication map $A\otimes_R A\to A$, i.e. the ideal that cuts out the diagonal in $\Spec A\times_R \Spec A$. We have that $I/I^2\cong \Omega_{A/R}$ and one such isomorphism is defined by sending $df$ to $[1\otimes f-f\otimes 1]$.
- By the second isomorphism theorem $0\to I/I^2\to \frac{A\otimes_R A}{I^2}\to A\to 0$. This sequence splits if we consider the section $A\to \frac{A\otimes_RA}{I^2}$ given by $a\mapsto [a\otimes 1]$.
- This yields an $R$-algebra isomorphism $\frac{A\otimes_R A}{I^2}\cong A\oplus I/I^2$ (the algebra structure on the direct sum is the one we gave above for arbitrary modules). The isomorphism as $R$-modules is given by the splitting of the sequence. This is also a ring homomorphism: 
	- In $A\otimes_R A$ we can rewrite elementary tensors as follows: $$a\otimes b=(a\otimes 1)(1\otimes b)=(a\otimes 1)(b\otimes 1+(1\otimes b-b\otimes 1))=ab\otimes 1+(a\otimes b-ab\otimes 1)$$Note that $a\otimes b-ab\otimes 1\in I$. This means that under the isomorphism above this elementary tensor maps to $(ab,[a\otimes b-ab\otimes 1])\in A\oplus I/I^2$. 
	- We now check that it is a ring homomorphism:$$\begin{align}\vp(a\otimes b)\vp(c\otimes d)&=(ab,[a\otimes b-ab\otimes 1])(cd,[c\otimes d-cd\otimes 1])\\&=(abcd,[acd\otimes b-abcd\otimes 1+abc\otimes d-abcd\otimes 1])=\\
	&=(acbd,[ac\otimes bd-abcd\otimes 1+acd\otimes b-abcd\otimes 1+abc\otimes d-ac\otimes bd])=\\
	&=(acbd,[ac\otimes bd-abcd\otimes 1+\under{\in I^2}{(ad\otimes 1- a\otimes d)(c\otimes b - cd\otimes 1)}])=\\
	&=(acbd,[ac\otimes bd-abcd\otimes 1])=\\&=\vp(ac\otimes bd)=\vp((a\otimes b)(c\otimes d)).\end{align}$$Since the elementary tensors generate we are done ($1\otimes 1\mapsto (1,0)$).
- Consider now the $R$-algebra homomorphism given by the other section: $a\mapsto [1\otimes a]\in \frac{A\otimes_R A}{I^2}$, which in the ring $A\oplus I/I^2$ is $(a,[1\otimes a-a\otimes 1])$. This defines a derivation $A\to I/I^2$ given by $a\mapsto [1\otimes a-a\otimes 1]$.
- We now verify that $I/I^2$ with this derivation represents $\Der_R(A,\bullet)$: 
	- Let $D:A\to M$ be any derivation and consider the unique $R$-algebra homomorphism $A\otimes_R A\to A\oplus M$ given by $a\otimes 1\mapsto (a,0)$ and $1\otimes a\mapsto (a,D(a))$. The assignment $1\otimes a\mapsto (a,D(a))$ is forced because we want to factorize $A\to A\oplus M,a\mapsto (a,D(a))$.
	- By definition of $I$, the restriction $I\to A\oplus M$ factors through $M$ and since for all $m,n\in M$ we have $(0,m)(0,n)=0$ we have that $I^2$ is in the kernel of the map.
	- This induces a map $I/I^2\to M$ that sends $[1\otimes a-a\otimes 1]$ to $D(a)$.

We now want to understand how the module $\Omega_{A/R}$ changes under common algebraic constructions:

It's easy to see by the universal property that $\Omega_{S\ii A/R}=S\ii \Omega_{A/R}$.

If $R\to A\to B$ are ring homomorphisms then we have an exact sequence $$B\otimes \Omega_{A/R}\to \Omega_{B/R}\to \Omega_{B/A}\to 0$$   - Note that $\Der_A(B,M)\subseteq \Der_R(B,M)$, so we have an induced map $\Omega_{B/R}\to\Omega_{B/A}$.
- Since $A\to B\to \Omega_{B/R}$ is a derivation we have an induced map $\Omega_{A/R}\to \Omega_{B/R}$. Since  $\Omega_{B/R}$ is a $B$-module this gives $B\otimes \Omega_{A/R}\to \Omega_{B/R}$.
- Now we simply check that applying $\Hom_B(\bullet,M)$ always yields exact sequences.

If $B=A/I$ and $A$ is an $R$-algebra then we have an exact sequence ($I$ is an ideal of $A$, not $A\otimes_R A$)$$I/I^2\to B\otimes_A\Omega_{A/R}\to \Omega_{B/R}\to 0$$   - In this case $\Omega_{B/A}=0$: derivations send constants to $0$ but $A\to B=A/I$ is also surjective
- We build the last part of the sequence like before. $I/I^2=I\otimes B$ and so the first map is given by $I\subseteq A\to \Omega_{A/R}$.
- Now we simply check that applying $\Hom_B(\bullet,M)$ always yields exact sequences.

If $A=R[x_1,\cdots, x_n]$, $I=(f_1,\cdots,f_r)$ then $\Omega_{(A/I)/R}=\dfrac{Adx_1\oplus \cdots\oplus Adx_n}{\ps{df_1,\cdots, df_r}}$. 
Stated another way, if $B$ is an $R$-algebra of finite type then $\Omega_{B/R}$ is a finite $B$-module.

In the case where $R=k$ and $I=p$ is a prime ideal that corresponds to a $k$-rational point $p$ we actually get an isomorphism $\mf_p/\mf_p^2=I/I^2\to k\otimes\Omega_{A/k}$.
- $B=A/I=k$ because $p$ is $k$-rational, so $\Omega_{B/R}=\Omega_{k/k}=0$ and we get surjectivity immediately.
- We now show that this map is invertible. The derivation $A\to I/I^2$ given by $f\mapsto [f-f(p)]$ induces a map $\Omega_{A/k}\to I/I^2$. 
- Since $I/I^2=I\otimes_A A/I=I\otimes_A k$ we indeed get a map $k\otimes \Omega_{A/k}\to I/I^2$. This map sends $1\otimes df$ to $[f-f(p)]$ and it is easy to see that this is indeed the inverse of the map $[g]\mapsto 1\otimes dg$ from before.
The proof also works for any point such that $\Omega_{k(p)/k}=0$, not necessarily rational points.

If $R\to R'$ and $A$ is an $R$-algebra (set $A'=R'\otimes_R A$) then $\Omega_{A'/R'}\cong R'\otimes_R\Omega_{A/R}$.
- Yoneda lemma 


If $L/K$ is a finite and separable field extension then $\Omega_{L/K}=0$.
- By the primitive element theorem $L=K(\theta)$ for some $\theta\in L$. 
- We may write $K(\theta)=\frac{K[x]}{(f(x))}$ with $f(x)\in K[x]$ and $\gcd(f(x),f'(x))=1$.
- Consider the exact sequence we get for quotients$$\frac{(f)}{(f)^2}\to \under{=L\otimes_KKdx=Ldx}{L\otimes_K \Omega_{K[x]/K}}\to \Omega_{L/K}\to 0$$where the first map is given by $[f]\mapsto f'(x)dx$.
- This means that $\Omega_{L/K}\cong\dfrac{Ldx}{(f'dx)}=\dfrac{K[x]/(f)}{(f')}=\dfrac{K[x]}{(f,f')}=0$.