#VectorBundles_and_Divisors 

A locally free sheaf (or vector bundle) $E$ on a locally ringed space $X$ is an $\Oc_X$-module such that there exists an open cover $\cpa{U_i}$ of $X$ such that $\rbar E_{U_i}\cong \Oc_{U_i}^{\oplus r}$ for some natural number $r$. 
If $r$ is consistent for the entire sheaf we call this the **rank** of $E$.

Locally free sheaves of rank 1 are called line bundles.
Isomorphism classes of line bundles together with tensor product form the [[Picard group]].


If $E$ is a locally free sheaf of rank $r$ on $X$ locally ringed space we can define the exterior powers $\bw^dE$ as the alternating quotient of $E^{\otimes d}$. The rank of $\bw^d E$ is $\binom rd$ and it is trivialized by any cover that trivializes $E$.
We define the **determinant** of a vector bundle $E$ of rank $r$ to be $\det E:=\bw^r E$. 
If $f:E\to E$ is a homomorphism then the induced map $\det E\to \det E$ corresponds to multiplication by $\det(f)$ fiber wise.
Exterior powers and restricting to a closed subspace commute with taking the dual (the second does not hold if we are not dealing with vector bundles).


If $0\to E'\to E\to E''\to 0$ is an exact sequence of vector bundles then $\det E\cong \det(E')\otimes \det(E'')$.
- (A lot of boring linear algebra on trivializing neighborhoods)
- If $r'=\rnk E',\ r''=\rnk E'',\ r=\rnk E$ (and so $r=r'+r''$) then we first want a map $\bw^{r'}E'\otimes \bw^{r''}E''\to \bw^r E$, that is, an $r$-multilinear map $$\under{r'\text{ times}}{E'\times\cdots\times E'}\times \under{r''\text{ times}}{E''\times\cdots\times E''}\to \bw^rE$$which is also alternating in the first $r'$ entries and in the last $r''$.
- We actually construct $\under{r'\text{ times}}{E'\times\cdots\times E'}\times \under{r''\text{ times}}{E\times\cdots\times E}\to \bw^rE$ and then verify that choosing a different preimage of an element in $E''$ for the last entries does not change the map.
- We choose a frame for $E'$, send it to $E$ and complete it to a frame of that, show that this yields a frame of $E''$. Now just prove that the natural expressions for a basis of domain and codomain correspond under this map.