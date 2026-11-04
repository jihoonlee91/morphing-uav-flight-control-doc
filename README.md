<div align="center">

# Flight Control System Design for a Morphing-Wing UAV

**LQR and nonlinear dynamic inversion for an aircraft with an SMPC (shape-memory polymer composite) flap module.**

![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=flat-square&logo=latex&logoColor=white)
![Project](https://img.shields.io/badge/MOTIE%20project-2016%E2%80%932020-1d4ed8?style=flat-square)
![Overleaf](https://img.shields.io/badge/Overleaf-ready-47A141?style=flat-square&logo=overleaf&logoColor=white)

<img src="resources/pdf/lqr.png" width="640" alt="Longitudinal and lateral LQR control structure">

<sub>Longitudinal and lateral LQR control structure for the morphing aircraft</sub>

</div>

## About

Technical design document (written in Korean) from the Ministry of Trade, Industry and Energy project **"Development of an SMPC Flap Module for Morphing Wings"** (2016–2020), with collaborators at Korea Aerospace University and Chungnam National University — the project behind my morphing-wing aircraft control research. It treats span and sweep morphing generically, following Seigler and Neal's modeling approach, and assumes an aerodynamic model is given.

## Contents

1. **Introduction**
2. **Modeling** — force and moment derivation, nonlinear model, linear model
3. **Linear Quadratic Regulator** — optimal control law, application to the morphing aircraft
4. **Nonlinear Dynamic Inversion** — general theory, longitudinal control, issues specific to morphing aircraft
5. **Conclusion**
6. **Appendices** — MATLAB listings for the LQR and NDI controllers

<div align="center">
<img src="resources/pdf/rolling.png" width="640" alt="Roll-angle step response">

<sub>Roll-angle step response from the document</sub>
</div>

## Read or build

**Read:** download the compiled PDF from the [latest release](https://github.com/jihoonlee91/morphing-uav-flight-control-doc/releases/latest) (`morphing-fcs-design.pdf`, built by GitHub Actions from `main.tex`).

**Build:** `latexmk -pdf main.tex` (needs a TeX distribution with `kotex` for the Korean text), or open the repository in Overleaf. Sources: `main.tex`, figures in `resources/`, template in `packages/`.

## Related publications

| | Publication | Aircraft model |
|---|---|---|
| Same project | [Flight Control of a Variable Span Morphing Wing UAV](https://jihoonlee91.github.io/papers/2017-variable-span-morphing-flight-control-design-ko.html) — *KSAS Spring 2017 (in Korean)* | variable-span morphing UAV |
| Same project | [Hierarchical Flight Control System for Morphing Aircraft](https://jihoonlee91.github.io/papers/2018-hierarchical-flight-control-morphing-ko.html) — *SASE Fall 2018 (in Korean)* | overview of the group's morphing control work |
| NDI, journal | [Neural network-based nonlinear dynamic inversion control of variable-span morphing aircraft](https://jihoonlee91.github.io/papers/2020-nn-nonlinear-dynamic-inversion-morphing.html) — *Proc. IMechE Part G, 2020* | F-18 HARV with variable span |
| NDI | [Neural network-based nonlinear dynamic inversion control of variable-span morphing aircraft](https://jihoonlee91.github.io/papers/2017-nn-nonlinear-dynamic-inversion-conf.html) — *EUCASS 2017* | F-18 HARV with variable span |
| NDI, Gold Award | [Flight control of asymmetric variable-span morphing aircraft using nonlinear dynamic inversion](https://jihoonlee91.github.io/papers/2019-flight-control-nonlinear-dynamic-inversion-gold.html) — *APISAT 2019* | NASA GTM-T2 |

## Credits

Typeset with the [Sleek LaTeX template](https://github.com/francois-rozet/sleek-template) by François Rozet (MIT — see [`packages/LICENSE-sleek-template`](packages/LICENSE-sleek-template); that license covers the template files in `packages/`, not the document). Document text and figures © Jihoon Lee and the project collaborators.

<sub>Part of my morphing-aircraft control research at the Seoul National University Flight Dynamics and Control Lab — more at <a href="https://jihoonlee91.github.io/">jihoonlee91.github.io</a>.</sub>
