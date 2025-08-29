#Cohomology 

Let $X_1,X_2\subseteq \Pj^n_k$ be hypersurfaces with no common components with equations $f_1,f_2$ and degrees $d_1,d_2$. 
Suppose $f$ is a non-zero homogeneous polynomial of degree $d$ such that $f=g_1f_1+g_2f_2$ with $g_1,g_2$ homogeneous of degrees $d-d_1$ and $d-d_2$. In this case $X=V_+(f)\supseteq X_1\cap X_2$.

Theorem(AF+BG) if $n\geq 2$ and $X_1\cap X_2\subseteq X$ then $f\in (f_1,f_2)$.
- If $I=\ker(\Oc_{\Pj^n_k}\to \Oc_{X_1\cap X_2})$ then by tensoring with $\Oc(d)$ we get$$0\to I(d)\to \Oc(d)\to \Oc_{X_1\cap X_2}(d)\to 0$$Taking global sections and noting that $f\in H^0(\Oc(d))$ we see that $f$ goes to $0$ in $H^0(\Oc_{X_1\cap X_2}(d))$ exactly when $f\in H^0(I(d))$, i.e. when $X_1\cap X_2\subseteq X$
- Now note that from $0\to \Oc(-d_1-d_2)\to \Oc(-d_1)\oplus\Oc(-d_2)\to \Oc_{\Pj^n}\to \Oc_{X_1\cap X_2}\to 0$ we can extract the first short exact sequence and then twist by $d$ to get$$0\to \Oc(d-d_1-d_2)\to \Oc(d-d_1)\oplus\Oc(d-d_2)\to I(d)\to 0$$
- Now take the associated long exact sequence and see that what we want holds if $H^1(\Oc(d-d_1-d_2))=0$, which is true because $n\geq 2$.