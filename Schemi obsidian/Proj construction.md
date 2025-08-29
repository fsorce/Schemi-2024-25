#LocallyRingedSpace #ProjectiveSchemes

[[Graded commutative algebra]]

Analogous construction to [[Affine schemes]].

Set: $\Proj A=\cpa{\pf\in \Spec A\mid \pf\text{ homogeneous, }A_+\not\subseteq \pf}$ (for all points, some positive degree homog. form doesn't vanish on it).
Topology: Zariski 
- if $I$ homog., $\sqrt I=\bigcap_{\smat{I\subseteq\pf\\\pf\in \Proj A}}\pf$
- $V_+(I)\subseteq V_+(J)\coimplies \sqrt I\cap A_+\supseteq \sqrt J\cap A_+$.
- $(\Proj A)_f=\cpa{\pf\in \Proj A\mid f\notin \pf}\cong \Spec A_{(f)}$ (homeomorphism which becomes isomorphism once the structure sheaf is defined).
Sheaf: Same as affine case, stalks are supposed to be $A_{(\pf)}$.

If $A,B$ graded, $\vp:A\to B$ of degree $d$ ($\vp(A_i)\subseteq B_{i\cdot d}$) then we get a morphism$$\Proj B\bs V_+(A_+B)\to \Proj A.$$If degree 1 and surjective then $B=A/I$ for some homogeneous ideal (the kernel), giving $\Proj B\to \Proj A$ which is a closed embedding onto $V_+(I)$.

All [[Closed subschemes]] are given by $\Proj A/I$ for $I$ homogeneous ideal.


