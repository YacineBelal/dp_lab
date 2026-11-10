# dp_lab

A hands-on workspace for learning and demonstrating differential privacy (DP).
It combines exercises from *Hands-On Differential Privacy* (OpenDP) with
from-scratch implementations, experiments, and short write-ups on the theory
behind them.

> Status: work in progress. I'm filling this in as I go through the material.

## Goals

- Connect theory (Dwork & Roth, papers) to practice (real libraries, real pitfalls).
- Keep a record of lessons learned.

## Repository structure

| Folder | Contents | Status |
|---|---|---|
| `01-foundations/` | Neighboring datasets, sensitivity, the formal (ε, δ)-DP definition | 🚧 |
| `02-mechanisms/` | Laplace, Gaussian, exponential, randomized response (from scratch + OpenDP) | 🚧 |
| `03-composition/` | Basic/advanced composition, zCDP, RDP, privacy accounting | ⏳ |
| `04-pitfalls/` | Floating-point attacks, bad sensitivity bounds, post-processing misconceptions | ⏳ |
| `05-private-ml/` | DP-SGD, private statistics and queries | ⏳ |
| `notes/` | Short write-ups: paper summaries, open questions | 🚧 |

(🚧 in progress, ⏳ planned)

## Highlights

*To be filled in as the repo grows. Planned examples:*

- Privacy-utility tradeoff plots for different mechanisms
- Empirical check that mechanism outputs on neighboring datasets are statistically close
- Reproduction of a result from a paper

## Getting started

This project uses [uv](https://docs.astral.sh/uv/) for dependency management.

```bash
git clone https://github.com/YacineBelal/dp-lab.git
cd dp-lab
uv sync
...
```

## References

- Dwork & Roth, *The Algorithmic Foundations of Differential Privacy*
- *Hands-On Differential Privacy: Introduction to the Theory and Practice Using OpenDP*
- [OpenDP library](https://opendp.org)
- Mironov, *On Significance of the Least Significant Bits for Differential Privacy*

## Open questions

- How should ε actually be chosen in practice?
- Where do theoretical guarantees break down in real implementations?

*(Updated as I go.)*
