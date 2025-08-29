#RelativeProperties

$f:X\to Y$ is finite if
1. it is [[Affine morphism]]
2. $V\subseteq Y$ open affine then $\Oc_X(f\ii(V))$ is finite over $\Oc_Y(V)$.

Local on the base.

An *affine* morphism is finite if 2. holds for some affine cover of the base.
- $B$ finite over $A$ iff $\Spec B\to \Spec A$ finite.
- each $f\ii(V_i)\to V_i$ is affine so WLOG $V=Y$ (refine affine cover so that $V=\bigcup_{\text{some}}V_i$). 
- By quasi-compactness finite affine cover of $Y$.
- $\Oc(X)\otimes_{\Oc(Y)}\Oc(V_i)$ finite over $\Oc(V_i)$, pick some finite set of generators $S_i$ in $\Oc(X)$. Set $S=\bigcup S_i$ and $M=S\cdot \Oc(Y)\subseteq \Oc(X)$. 
- Since $M_p\subseteq\Oc(X)_p=(\Oc(X)\otimes_{\Oc(Y)}\Oc(V_{\wh i}))_p=M_p$ we have that $M=\Oc(X)$.

A finite morphism is also [[Finite type morphisms|of finite type]].

A finite morphism is closed and has finite [[Fibers]]
- WLOG affine case. $B\to A$ finite
- $I=\ker(B\to A)$ then $B/I\to A$ is a finite extension, so $\Spec A\to \Spec B/I\to \Spec B$ is a surjective map (going up theorem) followed by a closed immersion. Similar reasoning if we replace $A$ with $A/J$.
- The fiber of $\pf\in \Spec B$ is $\Spec A\otimes_B k(\pf)$ and since $A$ finite over $B$, $A\otimes_Bk(\pf)$ is a finite dimensional vector space over $k(\pf)$, so it is an Artinian ring.

Are [[Proper morphisms]].

If $f:X\to Y$ finite and $X,Y$ integral Noetherian then the degree of $f$ is $\deg f=[k(X):k(Y)]$. Moreover $\dim_{k(q)}\Oc(X_q)\geq \deg f$ for all $q\in Y$ and equality holds on an open set.
$f$ is also a [[Flat morphisms]] iff that function is constant.
