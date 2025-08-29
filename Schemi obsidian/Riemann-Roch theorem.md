#curves 

Any divisor that has the [[Canonical sheaf]] $\omega_X$ as its associated sheaf is called a canonical divisor, denoted $K$.

We can rewrite [[Canonical sheaf|Serre duality]] for curves with the language of divisors as $h^1(D)=h^0(K-D)$ or $\chi(\Oc(D))=h^0(D)-h^0(K-D)$.

Theorem(Riemann-Roch) $\chi(\Oc(D))=h^0(D)-h^0(K-D)=\deg D+1-g$.
- The theorem clearly holds for $D=0$.
- Let us prove that if the theorem works for $D$ then it works for $D-p$ where $p\in X^{(1)}$:
	- Consider $0\to \Oc_X(D-p)\to \Oc_X(D)\to \Oc_p\otimes\Oc_X(D)\to 0$. 
	- Since $p$ is a point  $\Oc_p\otimes\Oc_X(D)\cong \Oc_p$, which is a skyscraper sheaf with ring $k(p)$ at $p$.
	- Taking the Euler characteristic we get $$\chi(\Oc(D-p))=\chi(\Oc(D))-\deg p=\deg D-\deg p+1-g=\deg(D-p)+1-g.$$ which is what we wanted.
- The case of $D+p$ follows from the formula above if we substitute $D$ with $D+p$.
It follows immediately that $\deg K=2g-2$.

