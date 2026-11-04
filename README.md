# ChemEdu-Acidity-Visualization

[![DOI](https://img.shields.io/badge/DOI-10.1021%2Facs.jchemed.6c00581-blue.svg)](https://doi.org/10.1021/acs.jchemed.6c00581)
[![Journal](https://img.shields.io/badge/Journal-J._Chem._Educ.-orange.svg)](https://pubs.acs.org/journal/jceda8)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

Official open-access computational dataset and visualization resources supporting the research article:  
**"Visualization-Guided Teaching of Organic Acid Acidity via Computational Chemistry: Bridging Electronic Structure and Acid–Base Reasoning"**, published in the *Journal of Chemical Education* (ACS Publications).

---

## 📖 Overview

Understanding organic acid acidity can be challenging for undergraduate students because conventional instruction frequently relies on qualitative rules and memorized $pK_a$ trends. When inductive and resonance effects operate simultaneously or appear contradictory, students often struggle to formulate causal mechanistic explanations.

This repository provides open-access quantum chemical visualization assets, wave function analysis outputs, and coordinate datasets designed to scaffold **Evidence-Based Reasoning (EBR)** through cognitive conflict and guided inquiry across three core instructional contexts:

1. **Carbonic Acid Anomaly (Intrinsic vs. Apparent Acidity)**: Resolves the discrepancy where reported aqueous $pK_a$ (∼6.35) suggests a weak acid, but computed intrinsic deprotonation free energy ($\Delta G_{\text{deprot}}$) reveals an intrinsic proton-release tendency stronger than acetic acid, distinguishing macroscopic hydration equilibria ($CO_2(aq) + H_2O \rightleftharpoons H_2CO_3$) from microscopic ionization.
2. **Complementary Reactant and Product Evidence**: Combines reactant-side electrostatic potential (ESP) and intrinsic bond strength (IBSI) with conjugate-base average local ionization energy (ALIE) to evaluate proton release and conjugate-base stabilization holistically.
3. **Aromaticity Loss vs. Resonance (Phenol vs. Acetic Acid)**: Demonstrates why greater $\pi$-delocalization does not necessarily yield higher acidity, highlighting the significant loss of aromatic stabilization (HOMA decrease) in phenoxide upon deprotonation.

---

## 🔬 Computational Methodology

All quantum chemical computations and wave function analyses were performed with reproducible open-science protocols:

- **Electronic Structure & Geometry Optimization**: ORCA and Gaussian 16
- **Density Functional & Basis Set**: Range-separated hybrid meta-GGA $\omega\text{B97M-V}$ / def2-TZVPP and B3LYP / 6-311++G(d,p)
- **Solvation Model**: Universal Solvation Model Based on Solute Electron Density (SMD, aqueous phase, $\varepsilon = 78.4$)
- **Wave Function Analysis & Descriptors**: Multiwfn 3.8
- **Molecular Graphics**: VMD and GaussView

---

## 📂 Repository Structure & Descriptors

The repository organizes computational outputs and visualization resources by theoretical analysis method:

| Directory | Theoretical Descriptor / Method | Pedagogical & Chemical Role |
| :--- | :--- | :--- |
| **`ALIE/`** | Average Local Ionization Energy | Evaluates conjugate-base oxygen electron-binding capability; unifies inductive and conjugative stabilization as a quantitative benchmark for acidity. |
| **`CDFT/`** | Conceptual DFT & Dual Descriptors | Includes Fukui functions ($f^+$, $f^-$, $f^0$) and condensation dual descriptor (CDD) grids showing closed-loop vs. open-leak charge delocalization. |
| **`ESP/`** | Electrostatic Potential Surfaces | Illustrates molecular polarity, surface extremes ($V_{\text{min}}$, $V_{\text{max}}$), and substituent-induced O–H polarization on the reactant side. |
| **`HOMA/`** | Harmonic Oscillator Model of Aromaticity | Quantifies aromaticity preservation in neutral phenols and aromaticity loss in phenoxide anions (∼11.7% disruption). |
| **`IBSI/`** | Intrinsic Bond Strength Index | Evaluates covalent O–H bond strength and polarization across substituted acids and phenols. |
| **`NICS/`** | Nucleus-Independent Chemical Shift | Evaluates magnetic shielding and ring-current modulation across substituted phenol derivatives. |
| **`Frequency_visualization/`** | Vibrational Mode Animations | Animated GIFs depicting lowest-frequency vibrational normal modes to assist 3D dynamic understanding. |
| **`ORCA_calculate/`** | DFT Coordinates & Wave Functions | Optimized Cartesian coordinates, ORCA input files, and formatted wave function files for both neutral acids and conjugate bases. |

---

## 🎓 Classroom Implementation & Supporting Information

The instructional activity is designed as a 45-minute modular classroom case featuring a three-phase progression:
- **Phase 1: Cognitive Conflict Elicitation** (10 min)
- **Phase 2: Multi-Descriptor Visualization Exploration** (20 min)
- **Phase 3: Guided Inquiry & Mechanism Construction** (15 min)

For instructors seeking classroom materials, refer to the Supporting Information published alongside the paper:
- **SI-A (Computational Methods & Assessment Instruments)**: ORCA inputs, Multiwfn scripts, optimized coordinates, and three bilingual (English/Chinese) diagnostic and survey instruments.
- **SI-B (Instructional Interpretation of Acidity Evidence)**: In-depth thermodynamic data, descriptor correlation plots ($\Delta G_{\text{deprot}}$ vs. ALIE), and pedagogical interpretation guidelines.

---

## 📜 License

The materials in this repository (computational data, wave function outputs, and visualization images) are licensed under the **[Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)**.

### Specific Attribution Requirements
If you reuse or adapt any data, scripts, or figures from this repository in slides, publications, course syllabi, or educational software, please provide a clear citation to the original research article.

---

## 📚 Citation

If you use any data, workflows, or visualizations from this project, please cite the following article:

> **Tianzhu Yu, Kejia Li, Lin Gao, Shuyi Wei, Zhaoxiong Yan,\* and Zhihua Xu.\***  
> *"Visualization-Guided Teaching of Organic Acid Acidity via Computational Chemistry: Bridging Electronic Structure and Acid–Base Reasoning."*  
> **Journal of Chemical Education**, 2026.  
> DOI: [10.1021/acs.jchemed.6c00581](https://doi.org/10.1021/acs.jchemed.6c00581)

📖 **Read the Full Article:**  
Access the complete paper online via ACS Publications: [https://doi.org/10.1021/acs.jchemed.6c00581](https://doi.org/10.1021/acs.jchemed.6c00581)

### BibTeX
```bibtex
@article{Yu2026ChemEduAcidity,
  author    = {Yu, Tianzhu and Li, Kejia and Gao, Lin and Wei, Shuyi and Yan, Zhaoxiong and Xu, Zhihua},
  title     = {Visualization-Guided Teaching of Organic Acid Acidity via Computational Chemistry: Bridging Electronic Structure and Acid–Base Reasoning},
  journal   = {Journal of Chemical Education},
  year      = {2026},
  doi       = {10.1021/acs.jchemed.6c00581},
  url       = {https://doi.org/10.1021/acs.jchemed.6c00581}
}
```

### Institutional Affiliation
Key Laboratory of Flexible Optoelectronic Materials and Technology, Ministry of Education and School of Optoelectronic Materials and Technology, Jianghan University, Wuhan 430056, PR China.  
*Corresponding Authors*: Zhaoxiong Yan (`zhaoxiongyan@jhun.edu.cn`), Zhihua Xu (`zhihuaxu@jhun.edu.cn`).
