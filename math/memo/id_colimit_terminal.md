---
layout: default
title: 恒等関手の余極限は終対象
---
__定理__: $$\mathcal{C}$$を圏とし、$$\mathrm{id}: \mathcal{C} \to \mathcal{C}$$を恒等関手とする。余極限

$$
(T, \theta) = \varinjlim \mathrm{id}
$$

が存在するならば、それは終対象である。

__証明__

余極限の定義より、$$\mathcal{C}$$の各対象$$X$$にたいして、$$\theta_X$$は射$$X \to T$$である。あとは、この形の射が一意であることを示せばよい。この$$\theta$$は、任意の$$\mathcal{C}$$の射$$f:X \to Y$$に対して、

$$
\theta_X = \theta_Y \circ f
$$

を満たす。特に、$$Y$$として$$T$$を選ぶと、任意の射$$f: X \to T$$に対して、

$$
\theta_X = \theta_T \circ f
$$

が成り立つ。よって、$$\theta_T = \mathrm{id}_T$$を示せば射の一意性が得られる。まず、$$f$$として$$\theta_X$$を選ぶことで次を得る。

$$
\theta_X = \theta_T \circ \theta_X
$$

余極限の普遍性から、射$$u: T \to T$$のうち次を満たすものは一意である: 「任意の$$\mathcal{C}$$の対象$$X$$について

$$
\theta_X = u \circ \theta_X
$$

を満たす」

$$\mathrm{id}_T$$と$$\theta_T$$はともにこの性質を満たすので等しい。証明終わり。





