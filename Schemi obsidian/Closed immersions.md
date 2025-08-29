#Immersion

Definition for [[Locally ringed space]]: $i:Y\to X$ closed immersion topologically plus $i^\sharp$ must be surjective.
In the case of smooth manifolds $(M,C^\infty_M)$ we are saying that a function on $Y$ is smooth if and only if for every point it can be written as the restriction of a smooth function on a neighborhood of the point inside $X$, which is the classical definition.


Closed immersions into a fixed space $X$ can be considered up to isomorphism in the comma category $\LRS/X$. These classes are called **closed subspaces**.

Closed subspaces of $X$ correspond to [[Sheaves of ideals]] of $\Oc_X$.$$\correspDef{\cpa{\text{closed subspaces of }X}}{\text{Sheaves of ideals of }\Oc_X}{i:Y\to X}{\ker(\Oc_X\to i_\ast\Oc_Y)}{(\Supp (\Oc_X/\Ic),\rbar{\Oc_X/\Ic}_{\Supp})\to (X,\Oc_X)}{\Ic}$$We may define $Y_1\cap Y_2=V(\Ic_{Y_1}+\Ic_{Y_2})$. 

Closed subspaces which are compatible on an open cover can be glued to a closed subspace.

They [[Finite morphisms]], so in particular they are affine and proper.

Stable under [[Base change]] and $X'\times_X Y=f\ii(X')$ ($X$ original base, $Y$ new base). This is the schematic equivalent of "preimage of a closed subset is closed".