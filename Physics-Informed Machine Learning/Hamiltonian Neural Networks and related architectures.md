There is a wide range of proposed methods to predict the evolution of a Hamiltonian system.
There are methods that directly try to learn the phase flow (the vector field of the Hamiltonian system) in a "graybox" manner with the help of physics-influenced inductive biases, or that try to learn the Hamiltonian quantity first and then use an integrator to evolve the system relying on [[Hamilton's equations]].

Let's start by exploring both camps of thought!
## 1. Learning the Hamiltonian quantity
The "canonical" paper on Hamiltonian dynamics and machine learning by Greydanus et al. on [[Hamiltonian Neural Networks]] (HNNs) was one of the first that explored the idea of evolving the Hamiltonian system by using a neural network to learn the Hamiltonian quantity (by minimizing [[Hamilton's equations]]) and using that to integrate the system with time. Many refinements, additions, and changes have been suggested since its publication. Prominently, [[Symplectic Recurrent Neural Networks]] also adopted a similar strategy, but mended some of the weaknesses of HNNs by using a symplectic integrator to preserve the structure of the Hamiltonian.
## 2. Learning the phase flow / vector field
Some of the papers that try to learn the phase flow of the Hamiltonian system through a neural network architecture (which typically conserves some sort of intrinsic property of the system like symplecticity) include [[SympNet]].

<hr>

In physics, it is often quite helpful to employ a change of coordinates, which can sometimes help in reducing the difficulty of the problem; some problems that seem intractable in one set of coordinates can be easily solved in another. [[Canonical transformation]]s and [[Action-Angle coordinates]] can often be helpful in that aim.

There has been a few papers that try to use machine learning to learn a transformation to "easier" coordinates with the hypothesis that evolving the system in those coordinates and then transforming back to the original coordinates can be more accurate. 
This technique has been especially used in the literature when dealing with [[Liouville integrable systems]] since they are guaranteed, by the [[Liouville-Arnold theorem]], to have [[Action-Angle coordinates]], which "linearize" the phase-space diagram. This leads to easier, more accurate evolution using the Euler method. This is the basic premise of [[Action-Angle Networks]].
An earlier work by Bondesan and Lamacraft also targets [[Liouville integrable systems]] in the paper "[[Learning Symmetries of Classical Integrable Systems]]".
Also, Ishikawa et al. in "[[Neural Network Approach to Construction of Classical Integrable Systems]]" use [[Action-Angle coordinates]] to temporally evolve [[Liouville integrable systems]] by imposing (in a loss function) the constancy of the action coordinate and total energy of the system.

- [[Hamiltonian Neural Networks]]
- [[Symplectic Recurrent Neural Networks]]
- [[Hamiltonian Generative Networks]]
- [[Symplectic ODE-Net]]
- [[Hamiltonian Graph Networks with ODE Integrators]]
- [[Nonseparable Symplectic Neural Networks]]
- [[Taylor-Net]]
- [[Simplifying Hamiltonian and Lagrangian Neural Networks via Explicit Constraints]]
- 

## Lagrangian-related Neural Network Architectures
- [[Lagrangian Neural Networks]]
- [[Deep Lagrangian Networks]]

## Port-Hamiltonian Networks
- 

# References
- [[greydanus2019 Hamiltonian Neural Networks]]
- 
