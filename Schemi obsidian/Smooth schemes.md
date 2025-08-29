#PropertiesSchemes 

Locally Noetherian schemes locally of finite type over a field.

We want to extend the [[Regular schemes|Jacobian criterion]] to [[Points of a scheme|points]] that may not be rational.

Note that $\mat{\displaystyle \pp{x_j}{f_i}(p)}_{i,j}\in \Mc(n,r,k(p))$ in general.

A smooth point is regular:
- It is enough to show that $A_{p}\to A'_{p'}$ is flat (see Com.Alg.).
- $A'=k(p)\otimes_k A$ is flat over $A$, so $A'\otimes A_p$ is flat over $A_p$
- $A'_{p'}=(A'\otimes_k A_p)\otimes A_{p'}$ is flat over $A'\otimes A_p$ because $p'$ is a prime ideal of $A'\otimes A_p$. (think  $k(p)\otimes_k A_p\to k(p)\otimes_k k(p)\to k(p)$)

If $k(p)/k$ is separable then $p$ is regular if and only if it is smooth.
- set $k'=k(p)$ and note $k'=k[t]/(f(t))$ with $f$ irred. with simple roots.
- Fix an isomorphism $k'=k[t]/(f(t))$ so that $k'\ni\al=[t]$, then $$k'\otimes_k k'\cong \frac{k'[t]}{(t-\al)}\times \frac{k'[t]}{g(t)}\cong k'\times(something),$$ so $p'$ is isolated in the fiber of $p$ in $X_{k'}$.
- From $0\to \mf_p\to A_p\to k'\to 0$ tensor with $A'_{p'}$ to get $0\to \mf_p\otimes A'_{p'}\to A'_{p'}\to k'\to 0$ (I used step above). This shows $\mf_p\otimes A'_{p'}=\mf_{p'}$.
- This means that $\mf_{p'}/\mf_{p'}^2\cong \mf_p/\mf_p^2$. Since $\dim A_p=\dim A'_{p'}$ we are done.

Smooth = geometrically regular.