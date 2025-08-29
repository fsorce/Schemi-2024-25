#Cohomology 

Given an indexed open cover $\Uc=\cpa{U_\al}_{\al\in I}$ of $X$ with $I$ ordered and $\Fc\in \Pre(X)$ we can define$$Č^p(\Uc,\Fc)=\prod_{\al_0<\cdots<\al_p}\Fc(U_{\al_0,\cdots,\al_p})$$We can define a differential by$$\delta:\funcDef{Č^p(\Uc,\Fc)}{Č^{p+1}(\Uc,\Fc)}{s}{\pa{\sum_{i=0}^{p+1}(-1)^i\rbar{s_{\al_0,\cdots,\wh{\al_i},\cdots,\al_{p+1}}}_{U_{\al_0,\cdots,\al_{p+1}}}}_{\al_0,\cdots, \al_{p+1}}}$$We define the Čech cohomology of $\Fc$ as $Ȟ^p(\Uc,\Fc)=H^p(Č^\bullet(\Uc,\Fc))$.

If $\Fc$ is a sheaf then we have a natural map $Ȟ^\bullet(\Uc,\Fc)\to H^\bullet(X,\Fc)$, moreover, if $H^i(U_{\al_0,\cdots, \al_p},\rbar\Fc_{U_{\al_0,\cdots, \al_p}})=0$  for all $\al_0,\cdots, \al_p\in I$ then this is an isomorphism.


If $X$ is a Noetherian topological space $H^i(X,\Fc)=0$ for all $i>\dim X$.