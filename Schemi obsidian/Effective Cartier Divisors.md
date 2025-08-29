#VectorBundles_and_Divisors 

Let $L$ be a [[Locally free sheaves|line bundle]] on $X$ and $s$ a global section of $L$. We can define the closed subscheme $Z(s)$ by the following universal property:
1. If $L\cong \Oc_X$ then $Z(s)$ is the [[Closed subschemes|closed subscheme]] associated to the [[Sheaves of ideals|sheaf of ideals]] $(s)\Oc_X$ (the isomorphism is irrelevant because it amounts to multiplying the generator by a unit locally).
2. If $f:X'\to X$ and $L$ is a line bundle on $X$ with section $s$ then $Z(s')=f\ii(Z(s))=Z(s)\times_X X'$ for $s'=f^\ast s\in f^\ast L$.

A section $s\in L(X)$ is called **regular** if for all $U\subseteq X$ we have that $f\cdot \rbar s_U=0\implies f=0$ for all $f\in \Oc_X(U)$.

Consider a closed subscheme $Y\subseteq X$. TFAE
1. $Y=Z(s)$ for some line bundle $L$ and $s\in L(X)$ regular section.
2. $\Ic_Y$ is a line bundle
3. There is an affine cover where $Y\cap U_i=\Spec \Oc_X(U_i)/(f_i)$ for $f_i\in \Oc_X(U_i)$ not a zero divisor.
It turns out that the $L$ is 1. must be $\Ic_Y^\vee$ and that the section $s$ is just the inclusion $\Ic_Y\to \Oc_X$.
By the Hauptidealsatz, these $Y$ have pure codimension $1$.

These $Y$ are called **hypersurfaces**. 

There is a natural correspondence between hypersurfaces and effective Cartier divisors (when the latter make sense). To $Z(s)$ we associate $\div(s)$ and viceversa. The effectiveness corresponds to the fact that $s$ is indeed a global section, so $Z(s)$ makes sense. 