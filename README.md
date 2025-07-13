# IVPF-ISM-MICMAC
# IVPF-ISM-MICMAC Python Implementation

This repository provides a complete Python implementation of the **Interval-Valued Picture Fuzzy Interpretive Structural Modeling (IVPF-ISM)** and **MICMAC analysis** framework. The method is designed to model expert evaluations under uncertainty and analyze the causal relationships among factors—particularly for identifying and prioritizing socio-cultural barriers in the adoption of biomass energy technologies.

## 📌 Features

- Import expert pairwise influence judgments from Excel
- Convert linguistic terms to Interval-Valued Picture Fuzzy Numbers (IVPFNs)
- Aggregate expert opinions using the **IVPFOWIA** operator
- Calculate crisp influence matrix via score function
- Generate the Initial and Final Reachability Matrices (IRM & FRM)
- Perform **MICMAC quadrant classification**
- Construct factor level diagram (hierarchical ISM structure)
- Export all matrices and plots to Excel and image files
- Built-in validation: checks IVPF consistency and transitivity

---

## 🛠️ Requirements

- Python 3.x  
- Required packages:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `openpyxl`
  - `tkinter`

You can install the necessary packages using:

```bash
pip install numpy pandas matplotlib openpyxl
📂 Input Format
An Excel file (.xls or .xlsx) containing expert pairwise comparisons.

Each expert provides a square matrix using the following linguistic scale:

0: No influence (N)

1: Low (L)

2: Medium (M)

3: High (H)

4: Very High (VH)

'R': Refusal to judge

Each expert's matrix is stacked vertically. The number of factors is automatically detected.

🚀 How to Use
Run the script.

A file dialog will open – select your Excel file with expert judgments.

The program will:

Convert linguistic values to IVPFNs

Aggregate opinions

Calculate the crisp matrix and generate the IRM and FRM

Perform MICMAC analysis and level partitioning

Save results to:

IVPF_ISM_MICMAC_Results.xlsx

MICMAC_Results.pdf / .png

Factor_Levels.pdf / .png

All outputs are created in the current working directory.

📊 Outputs
MICMAC Plot: driving vs. dependence power, color-coded by factor type

Level Diagram: ISM structure with arrows indicating influence paths

Excel File:

Aggregated IVPF matrix

Crisp scores

Initial & final reachability matrices

MICMAC quadrant results

Factor levels and dependency sets

✅ Validation
The script includes:

Score-based defuzzification

Transitive closure algorithm

IVPF normalization checks

IVPF total membership sum control (μ + η + ν ≤ 1)

📘 Citation
If you use this code for academic work, please cite the following concept:

[Your Name], "A Novel IVPF-ISM-MICMAC Framework for Analyzing Barriers to Biomass Energy Adoption", Under Review / Submitted Journal, 2025.

📩 Contact
For questions, improvements or collaboration, feel free to open an issue or contact me directly.
