#Cohomology 

We define the sheaf cohomology of $\Fc\in \Sh(X)$ to be the cohomology of the global sections of the [[Flabby sheaves and Godement resolution|Godement resolution]] of $\Fc$.
From the definition we immediately get the long exact sequence in cohomology.

[[Flabby sheaves and Godement resolution|Flabby]] sheaves are acyclic with respect to sheaf cohomology
- Split into short exact sequences of sheaves
- Use the flabbiness of the first sheaf to prove recursively that every sheaf that shows up is flabby and take global sections
- Put the short exact sequences back together, this shows that $\Gc^\bullet\Fc(X)$ is exact, like we wanted.

If $i:Y\to X$ with $Y$ closed then $H^j(X,i_\ast \Fc)=H^j(Y,\Fc)$ because $i_\ast$ commutes with $\Gc^\bullet$.

If $\Fc$ is a sheaf of $R$-modules on $X$ then $\Gc^\bullet\Fc$ is a complex of sheaves of $R$-modules, so $H^i(X,\Fc)$ is an $R$-module.
***

How do we compute sheaf cohomology?
- Acyclic resolutions: dimension shifting argument.
- [[Čech cohomology]]

We are mostly concerned with [[(Quasi-)Coherent sheaf cohomology]].

