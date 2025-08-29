#Cohomology 

Flabby = all restrictions are surjective.

Every sheaf lives inside a flabby sheaf: $\Fc\inj \Gc^0\Fc$ (sheaf of discontinuous sections).

If the first sheaf in an exact sequence is flabby then the global sections form an exact sequence.
- Just need to check surjectivity, take a Zorn system of preimages when restricted to open subsets, prove that a maximal element must be defined on the whole of $X$.
This lets us prove that if $\Fc$ is flabby then $(\Gc^0\Fc)/\Fc$ is also flabby.

The canonical flabby resolution (or Godement resolution) of a sheaf $\Fc$ is$$0\to \Gc^0\Fc\to \Gc^1\Fc\to \Gc^2\Fc\to\cdots\qquad \Gc^1\Fc=\Gc^0\pa{\frac{\Gc^0\Fc}\Fc},\quad  \Gc^i\Fc=\Gc^0(\coker(\Gc^{i-2}\Fc\to \Gc^{i-1}\Fc))$$The Godement resolution is functorial with respect to $\Fc$
If $0\to \Fc'\to \Fc\to \Fc''\to 0$ is exact then $0\to \Gc^\bullet\Fc'\to \Gc^\bullet\Fc\to \Gc^\bullet\Fc''\to 0$ is also exact (of complexes). Moreover, since the sheaves are flabby, we also have the exactness of $0\to \Gc^\bullet\Fc'(X)\to \Gc^\bullet\Fc(X)\to \Gc^\bullet\Fc''(X)\to 0$.


If $i:Y\inj X$ closed, $\Fc\in \Sh(Y)$ then $\Gc^\bullet(i_\ast \Fc)=i_\ast\Gc^\bullet\Fc$.
