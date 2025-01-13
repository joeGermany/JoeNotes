There is a wide array of literature on architectures and methods that try to embed ideas from classical mechanics to target nicher, more specific problems with the tools of physics-informed neural networks. We will discuss in what follows some of those contributions.

In the study of [[Liouville integrable systems]], systems with "enough" conserved quantities, Daigavane et al. introduce [[Action-Angle Networks]] for temporally evolving these systems using the concept of [[Action-Angle coordinates]][^1]. Also, Ishikawa et al. introduce a data-driven approach to learn the Hamiltonian of integrable systems (tested in the paper on the Toda lattice problem)[^3].

Another interesting method is [[Generating Function Neural Network]], introduced by Chen and Tao[^2]. 

The use of Hamilton-Jacobi equation in neural networks:
- [[The Hamilton-Jacobi Equation in Optimal Control Setting]]

Karniadakis's two papers 

[^1]:  Daigavane, A., Kosmala, A., Cranmer, M., Smidt, T., & Ho, S. (2022). Learning Integrable Dynamics with Action-Angle Networks. [https://arxiv.org/abs/2211.15338](https://arxiv.org/abs/2211.15338)

[^2]:  Chen, R., & Tao, M. (2021). Data-driven Prediction of General Hamiltonian Dynamics via Learning Exactly-Symplectic Maps. [https://arxiv.org/abs/2103.05632](https://arxiv.org/abs/2103.05632)

[^3]: 