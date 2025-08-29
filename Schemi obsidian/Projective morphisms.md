#Immersion #ProjectiveSchemes

[[Closed immersions]] into a [[Projective space]] followed by the projection to the base.

Stable under [[Base change]] because closed immersions are and $\Pj^n_{Y'}\overset{def}=Y'\times_Y\Pj^n_Y$.

[[Morphisms to projective space|Segre embedding]] for stability under composition.


Projective morphisms are [[Proper morphisms|proper]]
- Since closed embeddings are proper it is enough to check that $\Pj^n_Y\to Y$ is proper and by the base change property we may just check $\Pj^n_\Z\to \Spec \Z$. 
- This is clearly finite type and separated so we just need universally closed, which we can check on affine bases so we just need to show that $\Pj_R^n\to \Spec R$ is closed. 
- The [[Proj construction|closed subschemes of projective space]] are given by homogeneous ideals, so we need to check that $\pi:X=\Proj\dfrac{R[x_0,\cdots, x_n]}{I}=\Proj A\to \Spec R$ has closed image, i.e. that $\Spec R\bs \pi(X)$ is open.
- The fiber over $p\in \Spec R$ is $p\times_{\Spec R}X=\Proj(k(p)\otimes_R A)$ and we want see when this is empty, i.e. when $\pa{k(p)\otimes_R A}_+$ is a nilpotent ideal.
- $\pa{k(p)\otimes_R A}_+^r=(0)\coimplies 0=\pa{k(p)\otimes_R A}_r=k(p)\otimes_R A_r$.
- By Nakayama, if we fix $r$, we see that $\cpa{p\in\Spec R\mid k(p)\otimes_R A_r=0}$ is open, so $\Spec R\bs \pi(X)$ is given by a union of open sets.
