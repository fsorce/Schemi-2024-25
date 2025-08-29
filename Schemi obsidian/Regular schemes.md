#PropertiesSchemes 

Only for locally [[Noetherian schemes]].
A scheme is regular if $\Oc_{X,p}$ is regular for all points. It suffices to check closed points.

A regular scheme is also [[Normal schemes|normal]] because regular local Noetherian rings are UFD and so integrally closed.

(For locally of finite type over a field)

Jacobian criterion: $X=\Spec\dfrac{k[x_1,\cdots, x_n]}{(f_1,\cdots, f_r)}$. Fix a [[Points of a scheme|rational point]] $p\in X(k)$, then $$\dim_k\frac{\mf_p}{\mf_p^2}=n-\rnk\mat{\displaystyle \pp{x_j}{f_i}(p)}_{i,j}.$$So a rational point is regular iff the rank of the Jacobian matrix is maximal ($n-\dim\Oc_{X,p}$).
(Intuitively, we have an equality of [[Tangent and normal sheaves|tangent spaces]] $\ker \mat{\pp{x_j}{f_i}(p)}_{i,j}=T_pX$ and we take dimensions)
- Let $R=k[x_1,\cdots, x_n]$, $A=R/(f_1,\cdots,f_r)$. We have $R^r\to R\to A\to 0$ exact. 
- From this we get $R^r\to M_p\to \mf_p\to 0$ where $\mf_p$ and $M_p$ are the maximal of $\Oc_{X,p}$ and $\Oc_{\A^n_k,p}$.
- Tensor with $k$ and we get (it's a rational point) $k^r\to k^n\to \mf_p/\mf_p\to 0$, moreover, the first linear map is represented by the Jacobian matrix. Conclude by exactness.

If $k=\ol k$ then we can use the Jacobian criterion to check regularity.