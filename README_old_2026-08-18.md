# Near-Optimal Stochastic Autoregression from Full Traces

## Abstract

How many full trajectories are needed to learn an autoregressive generator whose parameters are shared across time? For unrestricted $d$-dimensional logistic generators, the best known chain-of-thought bound is roughly $d^2\log M/\epsilon$ trajectories at horizon $M$. Whether the natural $d$-dimensional rate is possible was left open. We answer this question affirmatively, up to logarithmic factors. A proper information-theoretic learner achieves trajectory Hellinger risk and final-token squared error at most $\epsilon$ from 

$$O\\\\\\!\left(\frac{d\log(Md)\log(1/\epsilon)+\log(1/\delta)}{\epsilon}\right)$$

 full trajectories, with no norm, margin, mixing, or prompt-distribution assumption. A matching $\Omega((d+\log(1/\delta))/\epsilon)$ lower bound holds already at one step. The proof identifies an observed-path dimension that is much smaller than the complexity of the marginalized final-token map. After exponentiating the logistic weights, the likelihood of one revealed path is a rational function of $d$ positive parameters with degree at most $Md$. A sign-pattern argument gives VC-subgraph dimension $O(d\log(Md))$. A conditional rho-estimator then converts this dimension into a proper Hellinger oracle inequality while canceling the unknown prompt marginal. The argument extends to misspecification, every bounded trajectory statistic, unrestricted multiclass softmax generators, and model selection over unknown memory orders. It also yields a general theorem for shared-parameter autoregressive models with rational local probabilities.

## Contributions

- We prove an observed-path theorem: if local probabilities are degree-$D$ rational functions of $p$ shared parameters, length-$M$ path densities have VC-subgraph dimension $O(p\log(MD))$.
- We combine this theorem with conditional rho-estimation to obtain a proper, high-probability, misspecified trajectory-Hellinger oracle inequality under an arbitrary and unknown prompt distribution.
- For unrestricted $d$-dimensional logistic autoregression, we obtain a $\widetilde O(d/\epsilon)$ full-trace upper bound and a matching $\Omega(d/\epsilon)$ lower bound. This resolves the chain-of-thought side of the open problem of.
- We derive norm-free multiclass softmax rates, guarantees for every bounded trajectory statistic, and adaptation to unknown memory.

## Keywords

autoregressive learning, chain-of-thought, sample complexity, Hellinger risk, VC-subgraph dimension, rho-estimation, logistic generators, trajectory learning

## Files

- `main.pdf`
- `main.tex`
- `references.bib`
- `iclr2027_conference.sty`, `iclr2027_conference.bst`, `natbib.sty`, `fancyhdr.sty`
- `main.pdf.ots`, `README.md.ots` OpenTimestamps priority proofs
