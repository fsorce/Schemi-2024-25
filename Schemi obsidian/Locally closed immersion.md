#Immersion

[[Closed immersions]] followed by an open immersion.
Equivalently we can ask that topologically it is locally closed immersion and we still have surjectivity of the sheaf morphism.

If a locally closed immersion has **closed image** then it is a [[Closed immersions]].

If $X$ is a scheme we can define locally closed subschemes in the natural way. 
We can define the **schematic closure** of a locally closed subscheme $Y\inj U\subseteq X$ as the intersection of the closed subschemes that contain it, i.e.$$\Ic_{\ol Y}=\sum_{\smat{Z\inj X\text{ closed subscheme}\\\\ Y\inj Z\cap U\text{ closed subscheme}}}\Ic_Z$$Note that $\Ic_{\ol Y}$ is [[Quasi-Coherent sheaves|quasi-coherent]] since it is $\imm(+:\bigoplus I_Z\to \Oc_X)$, so it defines a [[Closed subschemes]].

If $X$ is reduced **or** [[Noetherian schemes|Noetherian]] then $\ol Y\cap U=Y$.
- If $X$ reduced everything restricts to the topological case and it works
- If $X$ is Noetherian then $U$ is also Noetherian. We have $0\to \Ic_Y\to \Oc_U\to \Oc_Y\to 0$ and we know that $j_\ast\Ic_Y,\ j_\ast \Oc_U$ are quasi-coherent (because $X$ Noetherian).
- Let $J=(j^\sharp)\ii(j_\ast \Ic_Y)=\cpa{s\in \Oc_X\mid \rbar{(\rbar s_U)}_Y=0}$. Note that $J$ is quasi-coherent because it is$$J=\ker\pa{\Oc_X\overset{j^\sharp}\to j_\ast \Oc_U\to \frac{j_\ast \Oc_U}{j_\ast \Ic_Y}}$$so $J=\Ic_Z$ for some closed subscheme $Z$ of $X$. 
- This $Z$ must be $\ol Y$ and by construction $Z\cap U=Y$.


Local on the base, stable under [[Base change]]

