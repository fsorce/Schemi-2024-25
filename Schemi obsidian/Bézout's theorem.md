#Cohomology 

Let $f_1,f_2\in k[x_0,x_1,x_2]\nz$ be two homogeneous polynomials of degree $d_1,d_2$ with no common factors. Let $C_1=V_+(f_1),C_2=V_+(f_2)$ be the associated curves. 
Since they have no common components, $\dim C_1\cap C_2=0$, so all cohomology of the intersection lives in $H^0$. 
The rank of $H^0(\Pj^2_k,i_\ast\Oc_{C_1\cap C_2})$ is the number of points of $C_1\cap C_2$ counted with multiplicity.

Theorem(Bézout's) $H^0(\Pj^2_k,i_\ast\Oc_{C_1\cap C_2})=d_1d_2$.
- Take a free resolution of $A=\dfrac{k[x_0,x_1,x_2]}{(f_1,f_2)}$.
- If we sheafify that resolution we get $$0\to \Oc(-d_1-d_2)\to \Oc(-d_1)\oplus \Oc(-d_2)\to \Oc_{\Pj^2_k}\to i_\ast\Oc_{C_1\cap C_2}\to 0$$and this concludes because we know the Euler characteristic of the [[Twisting sheaves]].