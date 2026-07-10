# Flight Control System Design for Morphing Aircraft

*Development of an SMPC Flap Module for Morphing Wings*

Technical document (LaTeX) for the morphing aircraft project, funded by the Ministry of Trade, Industry and Energy (2016–2020).

## Content

Describes the design of the flight control system for a morphing-wing aircraft equipped with an SMPC (shape memory polymer composite) flap module. Document structure:

1. **Introduction**
2. **Modeling** — force and moment derivation, nonlinear model, linear model
3. **Linear Quadratic Regulator** — derivation of the optimal control law, application to the morphing aircraft
4. **Nonlinear Dynamic Inversion** — general NDI theory, application to longitudinal control, issues specific to applying NDI to a morphing aircraft
5. **Conclusion**
6. **Appendices** — MATLAB code listings for the LQR and NDI controllers

## Repository Structure

- `main.tex`: document source
- `resources/`: figures and other resources
- `packages/`: [Sleek LaTeX Template](https://github.com/francois-rozet/sleek-template) (François Rozet), used to typeset the document

## How to Build

Compile with `pdflatex main.tex` (or open in Overleaf) from the repository root.
