#Sheaves  

The associated sheaf to $M\in \Mod_A$ is defined like the structure sheaf of an [[Affine schemes|affine scheme]]. We also have $$\Hom_{\Sh(\Oc_{\Spec A})}(\wt M,\Fc)\cong \Hom_A(M,\Fc(\Spec A)).$$
We can restrict to open affine $\Spec B\subseteq \Spec A$ by tensoring the module:$$\wt{\pa{M\otimes_A B}}\cong \rbar{\wt M}_{\Spec B}$$- We have $M\otimes_A B\to \wt M(\Spec B)$ induced by the universal property of tensor product, finish the isomorphism by looking at stalks.

TFAE:
1. $\Fc\in \Sh(\Oc_X)$ is quasi-coherent
2. $\Fc\cong \wt{\Fc(X)}$.
3. for all $U\subseteq X$ open affine, $\Oc(U)\otimes_A\Fc(X)\to \Fc(U)$ isomorphism
4. for all $f\in A$, $\Fc(X)_f\to \Fc(X_f)$ isomorphism
5. for all $p\in X$, $\Fc(X)_p\to \Fc_p$ is an isomorphism

Direct sum of quasi-coherent is quasi-coherent, but not direct products.

If $M,N\in \Mod_A$ then $\wt{\pa{N\otimes_A M}}\cong \wt N\otimes_{\Oc_{\Spec A}}\wt M$.

Being quasi-coherent is a local property, it can be checked on an affine cover.
- WLOG finite affine cover $\cpa{X_\al}$. We want to prove $\Oc(U)\otimes_A\Fc(X)\cong \Fc(U)$ for all open affine $U$.
- Note that $\Oc(U)$ is flat over $\Oc(X)$ because [[Open immersion]] are flat.
- From $0\to \Fc(X)\to \bigoplus_\al\Fc(X_\al)\to\bigoplus_{\al,\beta}\Fc(X_{\al,\beta})$ (exact because it is a sheaf) we get diagram with exact rows
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd} 0 & {\mathcal{F}(X)\otimes\mathcal{O}(U)} & {\bigoplus_\alpha\mathcal{F}(X_\alpha)\otimes\mathcal{O}(U)} & {\bigoplus_{\alpha,\beta}\mathcal{F}(U\cap X_{\alpha,\beta})\otimes\mathcal{O}(U)} \\ 0 & {\mathcal{F}(U)} & {\bigoplus_\alpha\mathcal{F}(U\cap X_\alpha)} & {\bigoplus_{\alpha,\beta}\mathcal{F}(U\cap X_{\alpha,\beta})} \arrow[from=1-1, to=1-2] \arrow[from=1-2, to=1-3] \arrow[from=1-2, to=2-2] \arrow[from=1-3, to=1-4] \arrow[from=1-3, to=2-3] \arrow[from=1-4, to=2-4] \arrow[from=2-1, to=2-2] \arrow[from=2-2, to=2-3] \arrow[from=2-3, to=2-4] \end{tikzcd}
\end{document}
```
- note that the last two vertical arrows are isomorphisms, so the first one is also.
