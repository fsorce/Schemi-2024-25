#PropertiesSchemes 

If $X$ scheme and $p\in X$ then $p\in U$ with $U=\Spec A$. $$k(p)=\Oc_{X,p}/\mf_p=A_p/pA_p=\Frac(A/p).$$Moreover we have a projection $A\to A/p\to k(p)$, so $\Spec k(p)\to \Spec A=U$ that maps $(0)$ to $p$. This yields $\Spec k(p)\to X$. Conversely, if we have $\Spec K\to X$ we find that $K=k(p)$ where $p$ is the image of $\Spec K$.

If $T$ is a [[Reduced schemes|reduced scheme]] and $f:T\to X$ has image $p\in X$ then $f$ factors through $p\to X$.

The natural morphism $\Spec \Oc_{X,p}\to X$ is universal among the morphisms $T\to X$ such that the image is contained in every open subset of $X$ that contains $p$.

Generic points
- [[Irreducible]] components correspond to points, their generic points
- If $X$ [[Integral schemes|integral]] then we can define the field of [[Rational functions]] as $k(\xi)$ where $\xi$ is the generic point.


Field extensions:
- If $X\to \Spec k$ then we get $\Spec k(p)\to X\to \Spec k$, so $k(p)$ is an extension of $k$. 
- If $X$ [[Finite type morphisms|of finite type]] over $k$ and $p$ closed then $k(p)$ is a **finite** extension.
- If $k=k(p)$ then $p$ is a **rational point**.
- Rational points are closed.
- If $X$ [[Finite type morphisms|of finite type]] over $k$ and $k$ algebraically closed, all closed points are rational, thus $X(k)$ is [[Very dense - Jacobson rings|very dense]].


Regular and smooth points (Noetherian schemes):
- Regular if $\Oc_{X,p}$ is a regular local ring
- Smooth if $\Oc_{X_{k(p)},p'}$ is a regular local ring ($p'$ is the point in $p\times p$ which corresponds to multiplication $k(p)\otimes_k k(p)\to k(p)$)


Associated points (Noetherian)
- For affine schemes they are the associated primes. In general $p$ is associated if $\mf_p\in \Ass(\Oc_{X,p})$.
- The closures of non-minimal associated points are called embedded components.
- Reduced schemes have no embedded components.
- Hypersurfaces have no embedded components (Hauptidealsatz) 