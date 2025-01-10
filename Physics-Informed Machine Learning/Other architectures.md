## Action-Angle Networks
### Physics Insight
There is a subclass of Hamiltonian systems called [[Liouville integrable systems]].
The [[Liouville-Arnold theorem]] guarantees that for these systems, there exists a canonical transformation to a set of coordinates called [[Action-Angle coordinates]].
### The Architecture
Daigavane et al.[^1] introduce Action-Angle networks, an architecture that takes advantage of the linear evolution of the angle variable to evolve the system forward in time. The paper adopts an autoencoder-type architecture

This is the schematic of the architecture (image taken from [^1]):
![[ActionAngleNetworkArchitecture.png]]

The loss function of the action-angle network has the following two terms:
- $L_{\text{predict}} = \frac{1}{1 + \Delta t} \sum_{t_0 \in Tr} ||\mathcal{M} - u(t_0 + \Delta t)||^2$
- 
where $Tr$ is the training data composed of position $q(t)$ and momentum $p(t)$ data for a number of time steps.

[^1]: Daigavane, A., Kosmala, A., Cranmer, M., Smidt, T., & Ho, S. (2022). Learning Integrable Dynamics with Action-Angle Networks. https://arxiv.org/abs/2211.15338