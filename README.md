# PINNs for Option Pricing

**From Black-Scholes to Stochastic Volatility Calibration**

Semester project for FYS5429 — Advanced Machine Learning and Data Analysis for the Physical Sciences, University of Oslo.

## About

This project investigates Physics-Informed Neural Networks (PINNs) as mesh-free solvers for financial PDEs. The core idea: embed the governing differential equation directly into the neural network loss, so the model learns to price options while respecting the underlying physics.

The project progresses in three steps:

1. **Black-Scholes PINN** — solve the 1D BS PDE, validate against the analytical formula, compute Greeks via automatic differentiation
2. **Heston PINN** — extend to the 2D stochastic volatility PDE with a mixed derivative term
3. **Calibration** — use PINNs for the inverse problem: recover Heston parameters from observed option prices

## Structure

The paper is written in LaTeX and synced with Overleaf via this repo.

| File | Content |
|---|---|
| `00 MAIN.tex` | Root document |
| `01 FRONTMATTER.tex` | Title and abstract |
| `10 INTRO.tex` | Introduction |
| `11 METHOD.tex` | Methods |
| `12 RESULT.tex` | Results |
| `13 CONCLUSION.tex` | Conclusion and roadmap |
| `bib.bib` | Bibliography |

## Author

Egil Furnes — [egilsf@uio.no](mailto:egilsf@uio.no)
