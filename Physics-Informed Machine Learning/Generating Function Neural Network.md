## Physics Insight
The authors use the idea that the flow of the Hamiltonian systems can be thought of as a canonical transformation from time $t_i$ to $t_{i+h}$; we obviously know that the systems at both time points will obey Hamilton's equations of motion. Thus, the underlying concept is to try to discover this canonical transformation that gives us the flow of the systems. 

We can think of canonical transformations, a change of coordinates from $(q, p)$ to another set of canonically conjugate coordinates $(Q, P)$, as arising from a generating function $F$. There are four types of generating functions, each using a different combination of old and new coordinates, that allow us to define the transformation between the canonical coordinates. For derivations and more detailed explanations, check out [^1], [^2], or [^3].

Although not explicitly stated in the paper, the authors are trying to discover what are called "infinitesimal canonical transformations", which consist of a type-2 generating function and is close to the identity transformation. It can be used to evolve the system. Check p. 216 of Hand and Finch's Analytical Mechanics[^3] and p. 269-270 of Arnold's Mathematical Methods of Classical Mechanics[^1]. Also check [[Infinitesimal Canonical Transformation]] for my concise explanation of the physics behind it.

## Architecture
Based on the explanation in [[Infinitesimal Canonical Transformation]], the authors aim to discover the function $G$ (they call it $S_h$) that predicts the time flow of the system, given a dataset of $q$ and $p$. 
The loss function they aim to minimize is:


[^1]:  Arnold, V. I. (1989). Mathematical Methods of Classical Mechanics. In Graduate Texts in Mathematics. Springer New York. [https://doi.org/10.1007/978-1-4757-2063-1](https://doi.org/10.1007/978-1-4757-2063-1) [[arnold1989 Mathematical Methods for Classical Mechanics]]

[^2]:  Goldstein, H. (2011). Classical Mechanics. Pearson.

[^3]:  Hand, L. N., & Finch, J. D. (1998). Analytical Mechanics. Cambridge University Press.