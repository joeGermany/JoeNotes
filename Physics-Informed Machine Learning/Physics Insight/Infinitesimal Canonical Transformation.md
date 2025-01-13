Let us consider the generating function (of type-2): $$F (q, P) = qP + \epsilon G(q, P) \tag{1}$$
Notice that this is very close to the identity transformation since $F = qP$ gives us $p = \dfrac{\partial F}{\partial q} = P$ and $Q = \dfrac{\partial F}{\partial P} = q$, which corresponds to the identity transformation, and $\epsilon$, as we shall see, must be very small.

From (1), we get that $p = P + \epsilon \dfrac{\partial G}{\partial q}$ and $Q = q + \epsilon \dfrac{\partial G}{\partial P}$.
Let as consider, as Hand and Finch do in[^1], that $\epsilon = dt$ is a small time step. 
Thus, we get $Q = q + dt \dfrac{\partial G}{\partial P}$ and $P = p - dt \dfrac{\partial G}{\partial q}$.
We see that if $G(q, P) \approx H(q, p)$ as $dt \to 0$, then we recover Hamilton's canonical equations. We thus interpret $Q$ and $P$ as $q_{t+h}$ and $p_{t+h}$, and the old $q$ and $p$ as $q_t$ and $p_t$. 

Hence, from a machine-learning standpoint, if we can learn such a function $G$ close to $H$, we can evolve the system with time. This is the idea behind [[Generating Function Neural Network]]. 

[^1]:  Hand, L. N., & Finch, J. D. (1998). Analytical Mechanics. Cambridge University Press.