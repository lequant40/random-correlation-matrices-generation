# Description

Random correlation matrices can be generated using an algorithm due to Pourahmadi and Wang [1] based on the hyperspherical parametrization.

This algorithm relies internally on a procedure to generate random samples from a specific probability density, for which Makalic and Schmidt [2] initially proposed an efficient rejection sampling algorithm.

Later, Opdyke [3] introduced an analytical expression for the c.d.f. of this probability density as well as an analytical expression for its inverse function. This allows in particular 
to use the inverse transform method instead of the rejection sampling algorithm, thus improving the performances of Pourahmadi and Wang's algorithm to generate random correlation matrices.

This repository contains a Jupyter notebook comparing the practical performances of these two sampling algorithms.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lequant40/random-correlation-matrices-generation/HEAD?labpath=random_correlation_matrices_generation.ipynb)

To be noted, though, that Opdyke's derivation of the inverse c.d.f. of Makalic and Schmidt's probability density allows for much more advanced use-cases, detailled in his presentation.

# References

[1] - [Pourahmadi, M., and X. Wang. 2015. Distribution of random correlation matrices: Hyperspherical parameterization of the Cholesky factor. Statistics & Probability Letters 106: 5–12. doi:10.1016/j.spl.2015.06.015.](https://www.sciencedirect.com/science/article/abs/pii/S0167715215002011?via%3Dihub)

[2] - [Enes Makalic & Daniel F. Schmidt (2022) "An efficient algorithm for sampling from sink(x) for generating random correlation matrices", Communications in Statistics - Simulation and Computation, 51:5, 2731-2735](https://www.tandfonline.com/doi/abs/10.1080/03610918.2019.1700277?journalCode=lssp20)

[3] - [Opdyke, JD, "Beating the Correlation Breakdown (for Pearsons', Kendall's, Spearman's, and MORE!): Robust Inference and Flexible Scenarios and Stress Testing for Financial Portfolios"](https://ssrn.com/abstract=4056268)     
