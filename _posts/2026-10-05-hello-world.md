---
layout: post
title: "Hello, world — and a quick check that the maths renders"
date: 2026-10-05
tags: [meta]
---

This is the first post. It mainly exists to confirm that LaTeX works.

Inline maths: the Brownian motion $W_t$ satisfies $W_t - W_s \sim \mathcal{N}(0, t-s)$ for $s < t$.

Display maths, with an equation number:

$$
\begin{equation}
dS_t = \mu S_t \, dt + \sigma S_t \, dW_t
\end{equation}
$$

whose solution is

$$
S_t = S_0 \exp\!\left( \left(\mu - \tfrac{1}{2}\sigma^2\right) t + \sigma W_t \right).
$$

Code blocks are left alone by MathJax:

```python
import numpy as np
rng = np.random.default_rng(0)
W = np.cumsum(rng.normal(0, np.sqrt(1/252), 252))
```

## Writing a new post

Create a file in `_posts/` named `YYYY-MM-DD-some-title.md`, copy the header block from the top of this file, and write in Markdown.
