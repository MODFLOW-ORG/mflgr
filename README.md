# MODFLOW-LGR

[![mflgr CI/CD](https://github.com/MODFLOW-ORG/mflgr/actions/workflows/ci.yml/badge.svg)](https://github.com/MODFLOW-ORG/mflgr/actions/workflows/ci.yml)

## Overview of MODFLOW-LGR

LGR2 provides the capability to simulate groundwater flow using multiple block-shaped higher-resolution local grids (a child model) within a coarser-grid parent model. LGR2 accomplishes this by iteratively coupling separate MODFLOW-2005 models such that heads and fluxes are balanced across the grid-refinement interface boundary. LGR2 can be used in two-and three-dimensional, steady-state and transient simulations and for simulations of confined and unconfined groundwater systems. Traditional one-way coupled telescopic mesh refinement methods can have large, often undetected, inconsistencies in heads and fluxes across the interface between two model grids. The iteratively coupled ghost-node method of LGR2 provides a more rigorous coupling in which the solution accuracy is controlled by convergence criteria defined by the user. In realistic problems, this can result in substantially more accurate solutions and require an increase in computer processing time. The rigorous coupling enables sensitivity analysis, parameter estimation, and uncertainty analysis that reflects conditions in both model grids. This report describes the method used by LGR2, evaluates accuracy and performance for two-and three-dimensional test cases, provides input instructions, and lists selected input and output files for an example problem. It also presents the Boundary Flow and Head (BFH2) Package, which allows the child and parent models to be simulated independently using the boundary conditions obtained through the iterative process of LGR2.


## How to Cite MODFLOW-LGR

### Report Citation

Mehl, Steffen, and Hill, M.C., 2013, MODFLOW-LGR--Documentation of ghost node local grid refinement (LGR2) for multiple areas and the boundary flow and head (BFH2) package: U.S. Geological Survey Techniques and Methods, book 6, chap. A44, 43 p., https://doi.org/10.3133/tm6A44

## Source

Source code retrieved from https://water.usgs.gov/ogw/modflow-lgr/modflow-lgr-v2.0.0/mflgrv2_0_00.zip.

## Disclaimer

This repository is provided as a courtesy and is not actively maintained. Modifications to the original source may have been made. Use this resource at your own risk; it should be regarded as provisional and not as an authoritative substitute for the official software release by the original authors.
