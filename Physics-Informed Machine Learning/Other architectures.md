There is a wide array of literature on architectures and methods that try to embed ideas from classical mechanics to target nicher, more specific problems with the tools of physics-informed neural networks. We will discuss in what follows some of those contributions.

In the study of [[Liouville integrable systems]], systems with "enough" conserved quantities, Daigavane et al. introduce [[Action-Angle Networks]] for temporally evolving these systems using the concept of [[Action-Angle coordinates]][^1]. Also, Ishikawa et al. introduce a data-driven approach to learn the Hamiltonian of integrable systems (tested in the paper on the Toda lattice problem)[^2].

Another interesting method is [[Generating Function Neural Network]], introduced by Chen and Tao[^3]. 

Karniadakis's group has published two papers on the use of the [[Hamilton-Jacobi equation]] in neural networks in application to optimal control problems[^4] <sup>and</sup> [^5]. See [[The Hamilton-Jacobi Equation in Optimal Control Setting]].

[^1]:  Daigavane, A., Kosmala, A., Cranmer, M., Smidt, T., & Ho, S. (2022). Learning Integrable Dynamics with Action-Angle Networks. [https://arxiv.org/abs/2211.15338](https://arxiv.org/abs/2211.15338)

[^2]:  Ishikawa, F., Suwa, H., & Todo, S. (2021). Neural Network Approach to Construction of Classical Integrable Systems. Journal of the Physical Society of Japan, 90(9), 093001. [https://doi.org/10.7566/jpsj.90.093001](https://doi.org/10.7566/jpsj.90.093001)

[^3]:  Chen, R., & Tao, M. (2021). Data-driven Prediction of General Hamiltonian Dynamics via Learning Exactly-Symplectic Maps. [https://arxiv.org/abs/2103.05632](https://arxiv.org/abs/2103.05632)

[^4]:  Meng, T., Zhang, Z., Darbon, J., & Karniadakis, G. E. (2022). SympOCnet: Solving optimal control problems with applications to high-dimensional multi-agent path planning problems. [https://arxiv.org/abs/2201.05475](https://arxiv.org/abs/2201.05475)

[^5]:  Zhang, Z., Wang, C., Liu, S., Darbon, J., & Karniadakis, G. (2024). A time-dependent symplectic network for non-convex path planning problems with linear and nonlinear dynamics. [https://arxiv.org/abs/2408.03785](https://arxiv.org/abs/2408.03785)