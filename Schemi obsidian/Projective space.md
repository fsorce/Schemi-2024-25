#ProjectiveSchemes

We define projective space over $\Z$ with the [[Proj construction]] $\Pj^n_\Z=\Proj\Z[x_0,\cdots, x_n]$. For arbitrary base just [[Base change]].

[[Closed subschemes]] of a projective space are called projective schemes.

With standard grading, $\Gamma(\Pj^n_R, \Oc_{\Pj^n_R})=R$.

Weighted projective space is $\Proj R[x_0,\cdots, x_n]=\Proj A$ but with possibly non-standard grading. Weighted projective spaces are projective:
- If $\deg x_i=d_i$ and $d=\mcm\cpa{d_0,\cdots, d_n}$ then $A^{(d)}=\bigoplus_{i\in\N} A_{d\cdot i}$ is generated in degree 1.
- $\sqrt{A^{(d)}_+ A}=\sqrt{A_+}$, so $\Proj A\cong \Proj A^{(d)}$, the latter being some graded $R$-algebra with standard grading, i.e. a projective scheme.


On $\Pj^n_R$ we can define very natural [[Locally free sheaves|line bundles]] $\Oc(d)$ for $d\in \Z$ by taking the [[Quasi-Coherent sheaves]] associated to the module $R[x_0,\cdots,x_n]$ with the grading shifted by $d$. They are called [[Twisting sheaves]].
