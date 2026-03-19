# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

FYS5429 semester project at University of Oslo — "PINNs for Option Pricing: From Black-Scholes to Stochastic Volatility Calibration". The paper is compiled on Overleaf; this repo is the git-synced mirror.

## File Structure

| File | Purpose |
|---|---|
| `00 MAIN.tex` | Root document — sets up packages, geometry, and inputs all sections |
| `01 FRONTMATTER.tex` | Title block and abstract (two-column-false wrapper) |
| `10 INTRO.tex` | Introduction: heat equation → Black-Scholes → Heston motivation |
| `11 METHOD.tex` | Methods: MLE→MSE derivation, PINN loss formulation, activation functions |
| `12 RESULT.tex` | Results (to be filled) |
| `13 CONCLUSION.tex` | Conclusion + Progress & Roadmap section |
| `98 BIB.tex` | Just calls `\printbibliography` |
| `99 APPENDIX.tex` | Appendix (to be filled) |
| `bib.bib` | Bibliography entries (biblatex/biber format) |
| `99 GRAVEYARD.tex` | Old discarded document skeleton — not compiled |
| `99 NOTES.tex` | Scratch notes — not compiled |

## LaTeX Setup

- **Compiler**: pdflatex + biber (biblatex with `authoryear` style)
- **Layout**: `twocolumn`, 10pt, 0.7in margins
- **Font**: lmodern
- **Refs**: `\textcite{}` for inline, `\parencite{}` for parenthetical; `\cref{}` for cross-references (cleveref)
- **Figures**: `\captionsetup{figurename=Figure}`, bold labels

To add a new reference: add an entry to `bib.bib` and cite with `\textcite` or `\parencite`.

## Project Roadmap (due June 1 2026)

- **Phase 1** (→ Apr 4): BS-PINN implementation, validate against analytical Black-Scholes
- **Phase 2** (→ Apr 18): Activation function comparison (tanh, Swish, GELU, Softplus, SIREN)
- **Phase 3** (→ May 9): Heston PINN (2D PDE, mixed derivative)
- **Phase 4** (→ May 23): Heston calibration (inverse problem)
- **Phase 5** (→ Jun 1): Write-up and submission
