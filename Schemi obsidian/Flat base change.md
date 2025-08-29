#Sheaves  #Cohomology 

Let $X\in \Sch/R$ be a [[Separated]] and [[Quasi-compact]], $R\to R'$ is flat then$$R'\otimes_R\Gamma(X,\Oc_X)\cong \Gamma(X_{R'},\Oc_{X_{R'}})$$   - If $X=\Spec A$ then both rings are clearly $R'\otimes_R A$ (didn't use flatness).
- In general take $\Uc=\cpa{U_i}$ finite affine cover, $\cpa{(U_i)_{R'}}$ is an affine cover of the [[Base change]] $X_{R'}$.
- By separatedness $U_{\al\beta}$ is also affine.
- Consider $0\to \Oc(X)\to \bigoplus \Oc(U_\al)\to \bigoplus \Oc(U_{\al,\beta})$ and tensor with $R'$ (stays exact because of flatness), we get a diagram with exact rows
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd} 0 & {R'\otimes\mathcal{O}(X)} & {\bigoplus_\alpha R'\otimes\mathcal{O}(U_\alpha)} & {\bigoplus_{\alpha,\beta}R'\otimes\mathcal{O}(U_{\alpha,\beta})} \\ 0 & {\mathcal{O}(X_{R'})} & {\bigoplus_\alpha\mathcal{O}((U_\alpha)_{R'})} & {\bigoplus_{\alpha,\beta}\mathcal{O}((U_{\alpha,\beta})_{R'})} \arrow[from=1-1, to=1-2] \arrow[from=1-2, to=1-3] \arrow[from=1-2, to=2-2] \arrow[from=1-3, to=1-4] \arrow[from=1-3, to=2-3] \arrow[from=1-4, to=2-4] \arrow[from=2-1, to=2-2] \arrow[from=2-2, to=2-3] \arrow[from=2-3, to=2-4] \end{tikzcd}
\end{document}
```
- by the affine case we can now apply the 5 lemma to conclude


Let $X\in \Sch/R$ be a [[Separated]] and [[Quasi-compact]], $\Fc\in \QCoh(X)$, $R\to R'$ flat. Then$$R'\otimes_RH^i(X,\Fc)\cong H^i(X_{R'},\Fc_{R'})$$   - if $X=\Spec A$ then $\Fc=\wt M$, $\Fc_{R'}=\wt{M\otimes_R R'}$ and so the theorem holds (without using flatness).
- In general take $\Uc=\cpa{U_i}$ finite affine cover, $\cpa{(U_i)_{R'}}$ is an affine cover of $X_{R'}$ and we have the isomorphism$$Č^\bullet(\Uc,\Fc)\otimes_R R'\cong Č^\bullet(\Uc_{R'},\Fc_{R'})$$If $R\to R'$ is flat then $R'\otimes_R$ commutes with computing the [[Čech cohomology]].