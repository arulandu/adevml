# Notes on ADEV Paper
A summary of this [paper](https://dl.acm.org/doi/pdf/10.1145/3571198).

## Outline
Given f : params -> (probabilistic) real, build semantics such that "diff f" is a g : params -> (prob) real s.t. g(param) = d/d(param) E[f(param)]. Use case for ML, optimization, applications that need to AD EVs of PPLs.

Problem is that current approaches ignore probabilistic effects and simply AD branches. Even if d/dt E[f] is hard, semantics give unbiased estimator. Respects composition, modularity, etc. 



## References
```
@article{lew2023adev,
  title={ADEV: Sound automatic differentiation of expected values of probabilistic programs},
  author={Lew, Alexander K and Huot, Mathieu and Staton, Sam and Mansinghka, Vikash K},
  journal={Proceedings of the ACM on Programming Languages},
  volume={7},
  number={POPL},
  pages={121--153},
  year={2023},
  publisher={ACM New York, NY, USA}
}
```
