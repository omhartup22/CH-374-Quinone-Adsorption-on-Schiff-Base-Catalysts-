# CH-374-Quinone-Adsorption-on-Schiff-Base-Catalysts-
Structure .xyz files of different substituted Schiff-base catalysts and DTBC

# Is There a Correlation of Quinone Adsorption on Schiff-Base Catalysts With Electron Withdrawing or Electron Donating Groups?

**Author:** Olivia Hartup  
**Course:** CH 374  
**Date:** 4/27/2026

---

## Table of Contents
- [Project Overview](#project-overview)
- [Research Goal](#research-goal)
- [Methods](#methods)
- [Key Findings](#key-findings)
- [File Structure](#file-structure)
- [Navigation Guide](#navigation-guide)
- [Prerequisites](#prerequisites)
- [Software and Tools](#software-and-tools)

---

## Project Overview

This project investigates the relationship between ligand substituent electronics and quinone adsorption behavior in Schiff-base copper(II) catalysts. The goal was to determine whether electron-donating or electron-withdrawing groups influence catalytic reactivity toward 3,5-di-tert-butylcatechol (DTBC).

Understanding these effects is important for rational catalyst design in biomimetic oxidation systems.

## Research Goal

The central question of this study is:

> **Does quinone adsorption on Schiff-base catalysts correlate more strongly with electron-donating or electron-withdrawing substituents?**

This work examines how ligand modifications affect catalyst–substrate interactions and whether substituent strength plays a larger role than substituent direction alone.

## Methods

Computational modeling was performed using **ORCA** at the **PBE** level of theory with the **def2-TZVP** basis set.

The following analyses were carried out:

- Geometry optimizations.
- Adsorption energy calculations.
- Spin multiplicity analysis.
- Structural comparison across substituent types.

Initial catalyst structures were built in **Avogadro**. DTBC was positioned axially above the Cu(II) center to simulate substrate binding.

### Ligands Studied

The Schiff-base ligands were derived from salicylaldehyde and 1,3-diaminopropane and functionalized with the following substituents:

- H
- CH₃
- OCH₃
- Cl
- NO₂

## Key Findings

The copper center consistently favored a **low-spin doublet state** with multiplicity = 2, which was used for the final analysis.

Major trends observed:

- Electron-donating groups promoted closer ligand–substrate interactions.
- Electron-withdrawing groups caused greater ligand curvature around the substrate.
- Smaller bond angles were associated with the more curved structures.
- Adsorption energies depended strongly on substituent strength.

Most notably, both strong electron-donating and strong electron-withdrawing groups showed enhanced adsorption interactions relative to weaker substituents.

These results suggest that **substituent magnitude** may be more important than whether the group is donating or withdrawing. This has useful implications for catalyst design because tuning the strength of the substituent may be more effective than choosing only based on electronic direction.

## File Structure

The repository is organized into the following folders:

```text
xyz_files_OPT/
├── Optimized catalyst structures

xyz_files_metal_DTBC/
├── Optimized catalyst structures with DTBC bound

frozen_subs_xyz/
├── Catalyst structures with substituents frozen during optimization

unfrozen_subs_xyz/
├── Catalyst structures with substituents allowed to relax during optimization

log_files/
├── Log files for optimized catalyst structures

log_files_cat/
├── Log files for optimized catalyst structures with DTBC

log_file_mult4/
├── Log files for catalyst structures found using spin multiplicity 4

trj_xyz_files/
├── Trajectory files for optimized catalyst structures
```

## Navigation Guide

If you are reviewing this project, a good reading order is:

1. Start with the `log_files/` folder to examine the optimized catalyst geometries.
2. Review `xyz_files_OPT/` to inspect the final optimized structures.
3. Compare results in `frozen_subs_xyz/` and `unfrozen_subs_xyz/` to understand the effect of constraining substituents.
4. Open `xyz_files_metal_DTBC/` and `log_files_cat/` to evaluate substrate-bound catalyst structures.
5. Check `log_file_mult4/` if you want to compare the higher-spin multiplicity calculations.
6. Use `trj_xyz_files/` to follow optimization pathways and structural changes during the calculations.

### Suggested Workflow

- Begin with the optimized geometries.
- Then compare substrate-bound versus unbound systems.
- Finally, examine spin-state and substituent trends across the full dataset.

## Prerequisites

To reproduce or extend this project, you should have:

- A basic understanding of computational chemistry.
- Familiarity with density functional theory.
- Access to a molecular viewer such as **Avogadro**.
- Access to **ORCA** for quantum chemistry calculations.

## Software and Tools

- **ORCA** — quantum chemistry package used for geometry optimization and energy analysis.
- **Avogadro** — used to build and visualize molecular structures.
- **PBE functional** — density functional used in the study.
- **def2-TZVP basis set** — basis set used for electronic structure calculations.

## Notes

This project demonstrates how density functional theory can be used to study structure–property relationships in catalytic systems. It also provides insight into how ligand substituents influence adsorption behavior in Schiff-base copper catalysts.

---

If you would like, I can also turn this into a more visually polished README with badges, a short abstract, and a “How to cite this project” section.
