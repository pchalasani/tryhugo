---
title: Hugo Post
date: '2018-02-12 16:09:45 -0500'
published: true
---


With forestry when editing inline math equations we need to carefully watch for the rich-text editor inserting extra backslashes, munging underscores, etc.



Inline math with double-backslash-parens:  \\( E = mc^2 - a_i + \\sum_i y_i \\) works just fine.

Weirdly, inline math within dollar signs $ E = mc^2 - a_i + \sum_i y_i $ also works but the fonts are subtly different.

Normal display math enclosed in double-dollar signs:

<div>

    $$
    E = \sum_i m_i c_i^2
    $$

</div>

display math with equation aligned (note we don't need the double-dollar sign, since the `align` environment triggers MathJax.

<div>

    \begin{align}
    x &= \sum_{i=1}^n x_i \\
    &= \int_0^1 \exp(-\beta x_i)
    \end{align}

</div>

Try in Typora: $e = mc^2 - x_i - z_i \sum_k u_k$ and display math:


$$
\begin{align}
a &= u_i - z_i \\
  &= z_i + \sum_i u_i
 \end{align}
$$
