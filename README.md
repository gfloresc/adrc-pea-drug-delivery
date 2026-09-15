# Adaptive Saturated ADRC of a Piezoelectric Drug-Delivery Actuator

Manuscript and supplementary material for

> G. Flores and M. Rakotondrabe, *Adaptive Saturated ADRC of a Piezoelectric
> Drug-Delivery Actuator with Cubic Damping and Dahl Hysteresis*,
> submitted to **IEEE Control Systems Letters (L-CSS)**, submission 26-1103.

The letter develops an adaptive saturated output-feedback ADRC scheme for
position tracking of a piezoelectric actuator (PEA) delivering liquid drug.
The actuator combines cubic viscous damping with Dahl hysteresis, its effective
input gain is unknown within a known interval, and the driving voltage
saturates. The control law uses position measurements only.

## Contents

| File | Description |
|---|---|
| `paper.pdf` | The letter, six pages. Changes with respect to the first submitted version are typeset in blue. |
| `supplementary.pdf` | Supplementary material: proofs of Lemmas 1–5 (Section S-I), of Proposition 1 (S-II) and of Proposition 2 (S-III), and the complete simulation study (S-IV). |

Equation, lemma and figure numbers in the supplementary material follow those of
the letter; its own displayed equations, figures and tables are prefixed with S.

## Summary of the contribution

- The position and velocity envelopes are **derived** rather than assumed: the
  saturated input and the quartic dissipation of the cubic damping confine the
  trajectories to a computable region.
- The bounded-disturbance-rate condition customary in ADRC is **derived** from
  plant data alone, so no closed-loop signal enters the hypothesis.
- **No lower bound on the observer bandwidth** is required, because the
  monotonicity of the cubic damping, and not only a Lipschitz estimate, is used
  in the observer-error analysis.
- The unknown input gain is handled by a projection-based adaptive law whose
  estimation error enters the Lyapunov function, and the saturation residual
  enters the tracking analysis explicitly.

The tracking and observer errors are proved semiglobally uniformly ultimately
bounded.

## Note

This repository hosts the two documents for convenience. The submitted package,
including the response to the reviewers, is handled through the journal
submission system.
