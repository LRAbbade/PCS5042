# PCS-5042

Trabalhos da disciplina PCS5042 (Inteligência Artificial Informada por Leis Físicas e Modelos de Ordem Reduzida para Engenharia) do PPGEE

---

1.

a)

> Replicate figure 3 in [Fuks and Tchelepi, 2020](10.1615/JMachLearnModelComput.2020033905) using an analytical solution to the Buckley–Leverett equation, non-convex flux problem (equation 21)

b)

> Discretize and numerically solve the Kuramoto–Sivashinsky equation, using the same parameters as [Vlachas et. al](https://doi.org/10.1016/j.neunet.2020.02.016), section 5.3. Option: Fourier transform. Solution should be similar to figure 14

---

2.

> Solve 1a (Buckley–Leverett) using PINN. Setup only initial condition and boundary countitions, not to use generated data on training. PINN will not be able to learn due to discontinuity in function, train again using diffusive term `epsilon = 0.0025` and `epsilon = 0.01`, this will smooth out discontinuity and allow PINN to learn

---

3.

> Using the data generated in 1b make a model of reduced order using PCA to estimate `qhat`. Use `qhat` to estimate train matrices and validation lambdas. Using estimated matrices, rebuild `q` using `t` larger than in training data. Compare `q` with 1b solution. Use OpInf to evolve this model in time, then move back to original domain
