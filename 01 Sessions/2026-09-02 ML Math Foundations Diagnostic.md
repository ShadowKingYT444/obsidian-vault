---
type: learning-session
date: 2026-09-02
topic: Mathematical foundations for machine learning
goal: Build rigorous mathematical foundations, then reconnect them to familiar model mechanisms.
status: active
---

# Mathematical Foundations for Machine Learning

## Target capability

Derive, interpret, and connect the mathematical machinery behind modern ML rather than merely execute formulas. Identify hidden gaps efficiently, repair them from first principles, and transfer the resulting understanding back to models and training systems.

## Diagnostic model

### Reported strengths

- Transformer mechanisms and systems-level performance techniques
- Training precision and quantization
- Inference serving and attention optimization
- On-policy/off-policy reinforcement learning, PPO, and GRPO
- Harness engineering

These are useful priors, not yet assessment evidence.

### Mathematical strands to locate

- Linear algebra as geometry and operators: subspaces, projections, eigendecomposition, SVD, PCA
- Multivariable calculus: differentials, gradients, Jacobians, Hessians, constrained optimization
- Probability and statistics: random variables, expectation, covariance, conditioning, estimation
- Information theory: entropy, cross-entropy, KL divergence, likelihood
- Optimization: curvature, conditioning, stochastic gradients, regularization, convergence intuition

### Remaining uncertainty

Current depth in each strand and whether knowledge transfers between equations, geometry, and ML mechanisms.

## Plan

Begin with one integrated diagnostic. Branch only where its answer changes the learning route. Build the dependency DAG after locating the frontier.

## Evidence checkpoints

| Concept | Question type | What it discriminated | Result | Interpretation |
|---|---|---|---|---|
| Dot product / projection | Geometric interpretation | Scalar contraction versus vector projection | Gap | Treated $v^\top x$ as a matrix transformation and gave $vv^\top x$ as its result; non-unit scaling also confused with direction. |
| Linear transformations / eigenvectors | Mechanism and definition | Operator geometry versus invariant directions | Partial | Correctly described axis scaling and essentially stated $Av=\lambda v$, but could not identify eigenpairs. |
| Covariance / PCA | Mechanistic explanation | Variance direction and covariance eigensystem | Frontier | Correct long-axis intuition; covariance treated as a scalar and eigenvector mechanism remained unclear. |
| Multivariable gradient | Meaning and calculation | Directional derivative structure | Frontier | Knows local rate-of-change role; missing partial-derivative calculation and conflates steepest descent with pointing to the origin. |
| Negative log-likelihood | Explanation | Probability semantics and logarithmic penalty | Mostly pass | Good qualitative penalty intuition; probability value misstated as 0.9 rather than 0.8. |
| Curvature / optimization | Contrast | Scale, derivatives, curvature, and stable step size | Gap | Noticed magnitude difference; missing derivative/Hessian account of update dynamics. |
| Inner product | Calculation and interpretation | Scalar result and geometric similarity | Partial pass | Correct calculation and useful similarity intuition; needs separation from cosine similarity. |
| Outer product / shapes | Shape discrimination | Inner versus outer dimensions and result types | Gap | Believed $ab^\top$ was invalid or equivalent to the inner product. |
| Projection | Geometric reconstruction | Scalar coordinate versus vector reconstruction | Unclear | Did not clearly state the projected vector $[1,1]^\top$. |
| Diagonal eigenpairs | Direct application | Invariant directions and scale factors | Pass | Correctly identified both eigenvalues and axis behavior. |
| Partial derivatives | Calculation | Holding other variables constant | Gap | Left the differentiated variable in each cross term. |
| Gradient descent scale | Worked step | Effect of slope scale under a fixed learning rate | Pass | Correctly obtained $0.8$ and $-19$. |
| Log-loss ordering | Contrast | Monotonic nonlinear probability penalty | Pass | Correct ordering and recognized unequal loss changes. |
| Matrix-product shapes | Transfer calculation | Compatibility and output dimensions | Pass | Correctly classified all three products and shapes. |
| Orthogonality | Mechanistic interpretation | Zero dot product versus opposite direction | Partial | Calculation correct; described an orthogonal vector as nearly opposite. |
| Unit-vector projection | Reconstruction | Scalar coordinate followed by vector reconstruction | Partial | Coordinate correct; lost the $\sqrt{2}$ cancellation and returned $[0.5,0.5]^\top$. |
| Non-unit projection | Invariance explanation | Normalization against arbitrary direction-vector scale | Partial | Correct qualitative purpose; calculation omitted. |
| Multivariable gradient | Novel calculation | Cross-term partial derivatives | Partial | Correct negative-gradient principle, but dropped cross-term coefficients. |
| Attention product shapes | ML transfer | Individual-vector versus batched-matrix products | Partial | Correctly described $QK^\top$ but substituted it for $q^\top k$ and $qk^\top$. |

## Parking lot

### Checkpoint 2 evidence

- Matrix multiplication shapes: pass.
- Orthogonal versus opposite: partial pass; geometry correct, raw dot product confused with cosine similarity.
- Non-unit projection invariance: pass.
- Attention object shapes: partial pass; $q^\top k$ and $QK^\top$ correct, but $qk^\top$ interpreted as token-to-token rather than feature-to-feature.
- Partial derivatives and gradient evaluation: pass.
- Unit steepest-descent direction: partial; negative-gradient principle correct, normalization not operational.

The root skills are sufficient to advance to covariance and PCA while repairing normalization and object semantics in context.

- Revisit familiar model mechanisms after the mathematical foundation is secure.

## Next step

- Derive the PCA mechanism and complete the PCA Checkpoint in `[[2026-09-02]]`.
