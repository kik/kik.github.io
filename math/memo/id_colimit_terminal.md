---
layout: default
title: 恒等関手の余極限は終対象
---
__定理__: $$\mathscr{C}$$を圏とし、$$\mathrm{id}: \mathscr{C} \to \mathscr{C}$$を恒等関手とする。余極限

$$
(T, \theta) = \varinjlim \mathrm{id}
$$

が存在するならば、それは終対象である。

__証明__

余極限の定義より、$$\mathscr{C}$$の各対象$$X$$にたいして、$$\theta_X$$は射$$X \to T$$である。あとは、この形の射が一意であることを示せばよい。この$$\theta$$は、任意の$$\mathscr{C}$$の射$$f:X \to Y$$に対して、

$$
\theta_X = \theta_Y \circ f
$$

を満たす。すなわち、以下の図式は可換である。

$$
\begin{xy}
\xymatrix {
X \ar[rr]^f \ar[rd]_{\theta_X} &   & Y \ar[ld]^{\theta_Y} \\
  & T &
}
\end{xy}
$$

特に、$$Y$$として$$T$$を選ぶと、任意の射$$f: X \to T$$に対して、

$$
\theta_X = \theta_T \circ f
$$

が成り立つ。よって、$$\theta_T = \mathrm{id}_T$$を示せば射の一意性が得られる。

以下の２つの図式はともに可換である。

$$
\begin{xy}
\xymatrix {
X \ar[rr]^f \ar[rd]^{\theta_X} \ar@/_/[rdd]_{\theta_X} &   & Y \ar[ld]_{\theta_Y} \ar@/^/[ldd]^{\theta_Y} \\
  & T \ar[d]|{\theta_T} & \\
  & T &
}
\end{xy}
\ \ \ 
\begin{xy}
\xymatrix {
X \ar[rr]^f \ar[rd]^{\theta_X} \ar@/_/[rdd]_{\theta_X} &   & Y \ar[ld]_{\theta_Y} \ar@/^/[ldd]^{\theta_Y} \\
  & T \ar[d]|{\mathrm{id}_T} & \\
  & T &
}
\end{xy}
$$

余極限の普遍性から、射$$T \to T$$で上の形の図式を可換にするものは一意であるから、

$$
\theta_T = \mathrm{id}_T
$$

となる。証明終わり。
