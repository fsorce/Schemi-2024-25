#RelativeProperties

Intersection of open subschemes:
- $f:X\to S,g:Y\to S$, $U\subseteq X,V\subseteq Y,W\subseteq S$ open such that $f(U)\subseteq W,g(V)\subseteq W$, then $$U\times_W V=\pr_1\ii(U)\cap\pr_2\ii(V)\subseteq X\times_S Y$$This is because $U\times_W V=U\times_S V$ and the following diagram is cartesian
```tikz 
\usepackage{tikz-cd} 
\begin{document}
\begin{tikzcd} {\mathrm{pr}_1^{-1}(U)\cap\mathrm{pr}_2^{-1}(V)} & {\mathrm{pr}_2^{-1}(V)} & V \\ {\mathrm{pr}_1^{-1}(U)} & {X\times_SY} & Y \\ U & X & S \arrow[from=1-1, to=1-2] \arrow[from=1-1, to=2-1] \arrow[from=1-2, to=1-3] \arrow[from=1-2, to=2-2] \arrow[from=1-3, to=2-3] \arrow[from=2-1, to=2-2] \arrow[from=2-1, to=3-1] \arrow["{\mathrm{pr}_2}"', from=2-2, to=2-3] \arrow["{\mathrm{pr}_1}"', from=2-2, to=3-2] \arrow[from=2-3, to=3-3] \arrow[from=3-1, to=3-2] \arrow[from=3-2, to=3-3] \end{tikzcd}
\end{document}
```

The category of schemes has fibered products (affine cover of everything, use stuff above and glue).






