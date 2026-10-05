---
type: learner-model
updated: 2026-09-02
---

# Learner Model

This page changes only when a session produces evidence. Empty sections mean unknown, not weak.

## Current goals

- Build a rigorous, connected command of the mathematics underlying machine learning, then reinterpret familiar model mechanisms using that foundation.

## Stable foundations

- Self-reported: transformer architecture end to end; sparse attention; mixed-precision training; NVFP4 quantization; speculative decoding; dynamic batching; FlashAttention; on-policy versus off-policy RL; PPO; GRPO; and harness engineering. These remain unverified until relevant reasoning or transfer demonstrates them.
- Demonstrated matrix-product shape checking, diagonal eigenpair identification, partial differentiation of polynomial cross-terms, gradient assembly, non-unit projection invariance, and one-step scalar gradient descent.

## Active frontier

- Diagnose mathematical depth across linear algebra, multivariable calculus, probability/information theory, and optimization.
- Repair matrix-product shape reasoning, inner/outer products, vector projection, and partial derivatives before advancing to PCA and curvature.

## Fragile knowledge and misconceptions

- Dot products, vector projections, and general linear transformations are currently conflated.
- Covariance has been treated as a scalar rather than a direction-sensitive matrix.
- Gradient is understood as local change but not yet as a vector of partial derivatives; steepest direction is conflated with direction toward the origin.
- Optimization scale is noticed qualitatively, but slope and curvature are not yet distinguished.
- Frequently preserves the high-level mechanism while losing an object's type, shape, normalization factor, or cross-term coefficient during algebra.
- Distinguishes matrix shapes successfully when prompted explicitly; needs this discipline to transfer automatically to attention and projection expressions.
- Raw dot products and cosine similarity still require deliberate separation.
- Single-vector outer products need feature-by-feature interpretation rather than token-by-token interpretation.

## Useful learning patterns

- Prefer first-principles derivation and visible motivation.
- Concentrate depth on generating ideas; compress secure prerequisites.
- Use discriminative questions and novel transfer before marking a target secure.
- Present diagnostic questions in compact batches of at least five when practical.
- Put substantial mathematical prompts in Obsidian notes so MathJax renders cleanly.

## Next review

-
