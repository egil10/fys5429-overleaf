# PINNs for Option Pricing

Can a neural network learn to price options by understanding the physics?

This is the LaTeX source for my FYS5429 semester project at the University of Oslo. The core idea: embed the Black-Scholes and Heston PDEs directly into the neural network loss, so the model satisfies the governing equations by construction — no grid, no finite differences, no closed-form required.

The companion code lives at [github.com/egil10/fys5429](https://github.com/egil10/fys5429).

## Roadmap

1. **Black-Scholes** — solve the 1D PDE, validate against the analytical formula, compute Greeks via autodiff
2. **Heston** — extend to 2D stochastic volatility with a mixed derivative term
3. **Calibration** — use the PINN as a differentiable solver to recover Heston parameters from market prices

## Files

| File | Content |
|---|---|
| `00 MAIN.tex` | Root document |
| `10 INTRO.tex` | Introduction |
| `11 METHOD.tex` | Methods |
| `12 RESULT.tex` | Results |
| `13 CONCLUSION.tex` | Conclusion |
| `bib.bib` | Bibliography |

Compiled on Overleaf; synced here via git.

---

Egil Furnes · [egilsf@uio.no](mailto:egilsf@uio.no)
