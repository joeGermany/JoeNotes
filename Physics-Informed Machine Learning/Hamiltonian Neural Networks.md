Hamiltonian Neural Networks, introduced in 2019 by Greydanus et al. in this paper[^1], build upon the idea of adding physics-informed soft constraints in the loss function of the neural network (based on [[raissi2017 Physics-Informed Deep Learning]]).
## Physics Insight
Hamiltonian neural networks target a class of physical systems called [[Hamiltonian system]]s, which are endowed by a specific structure.
## Architecture
The Hamiltonian neural network (HNN) aims to approximate the Hamiltonian quantity $H$ by using a feedforward neural networks whose objective is to match Hamilton's canonical equations, so as to preserve the "structure" of the Hamiltonian system.

The authors generate a dataset of position and momentum values (along with their derivatives) by using the fourth-order Runge-Kutta integrator. The loss function used in HNN is:
$L = \lVert \dfrac{\partial \hat{\mathcal{H}}_{\theta}}{\partial \mathbf{p}} - \dfrac{d \mathbf{q}}{d t} \rVert ^2 + \lVert \dfrac{\partial \hat{\mathcal{H}}_{\theta}}{\partial \mathbf{q}} + \dfrac{d \mathbf{p}}{d t} \rVert ^2,$
where the $\dfrac{d \mathbf{q}}{dt}$ and $\dfrac{d \mathbf{p}}{dt}$ are calculated in the data generation phase (by finding slope of the $q(t)$ and $p(t)$ graphs using finite-difference) and the $\dfrac{\partial \hat{\mathcal{H}}_{\theta}}{\partial \mathbf{q}}$  

and  $\dfrac{\partial \hat{\mathcal{H}}_{\theta}}{\partial \mathbf{p}}$ are computed using auto-differentiation[^2] of the output of the HNN with respect to the input.

## A Few Notes
- The use of a non-structure preserving integrator has an effect on the accuracy and validity of the results. This deficiency led to the introduction of [[Symplectic Recurrent Neural Networks]].

[^1]:  Greydanus, S., Dzamba, M., & Yosinski, J. (2019). Hamiltonian Neural Networks. [https://arxiv.org/abs/1906.01563](https://arxiv.org/abs/1906.01563)

[^2]:  