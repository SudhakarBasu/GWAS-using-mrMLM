# GWAS Analysis Using mrMLM

[![R](https://img.shields.io/badge/R-276DC3?style=flat&logo=r&logoColor=white)](https://www.r-project.org/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## 📋 Overview

This repository contains a Genome-Wide Association Study (GWAS) analysis pipeline using the **mrMLM (multi-locus random-SNP-effect Mixed Linear Model)** approach. The mrMLM method is designed to identify quantitative trait nucleotides (QTNs) associated with complex traits by implementing multiple multi-locus GWAS methods simultaneously.

## 🎯 Features

- **Multi-locus GWAS**: Implements mrMLM methodology for robust QTN detection
- **Interactive GUI**: User-friendly graphical interface via `mrMLM.GUI` package
- **Comprehensive Outputs**: Generates Manhattan plots, Q-Q plots, and detailed result tables
- **Sample Data Included**: Example genotype and phenotype data for testing

## 📁 Repository Structure

```
GWAS_mrMLM/
├── MrMLM.R                    # Main R script to launch mrMLM GUI
├── mdp_genotype.hmp.txt       # Genotype data in HapMap format
├── mdp_traits.txt             # Phenotype/trait data
├── 1_Final result.csv         # Final GWAS results with significant SNPs
├── 1_intermediate result.csv  # Intermediate analysis results
├── 1_Manhattan plot.png       # Manhattan plot visualization
└── 1_qq plot.png              # Q-Q plot for p-value distribution
```

## 🚀 Getting Started

### Prerequisites

- **R** (version ≥ 4.0.0 recommended)
- **mrMLM.GUI** package

### Installation

1. **Clone this repository**:
   ```bash
   git clone https://github.com/SudhakarBasu/GWAS-using-mrMLM.git
   cd GWAS-using-mrMLM
   ```

2. **Install required R package**:
   ```r
   install.packages("mrMLM.GUI")
   ```

### Usage

1. **Launch the mrMLM GUI**:
   ```r
   # Run the provided R script
   source("MrMLM.R")
   
   # Or manually execute:
   library(mrMLM.GUI)
   mrMLM.GUI()
   ```

2. **Load your data**:
   - **Genotype file**: `mdp_genotype.hmp.txt` (HapMap format)
   - **Phenotype file**: `mdp_traits.txt` (trait measurements)

3. **Configure analysis parameters** through the GUI interface

4. **Run the analysis** and view results

## 📊 Input Data Format

### Genotype Data (`mdp_genotype.hmp.txt`)
- Format: HapMap format
- Contains SNP markers across the genome
- Includes chromosome positions and allele information

### Phenotype Data (`mdp_traits.txt`)
- Tab-delimited text file
- First column: Sample IDs
- Subsequent columns: Trait measurements

## 📈 Output Files

| File | Description |
|------|-------------|
| `1_Final result.csv` | Significant SNPs with effect sizes, p-values, and LOD scores |
| `1_intermediate result.csv` | Detailed intermediate calculations and statistics |
| `1_Manhattan plot.png` | Genome-wide visualization of SNP associations |
| `1_qq plot.png` | Q-Q plot showing observed vs. expected p-values |

### Example Output Visualizations

**Manhattan Plot**: Shows the -log10(p-value) of SNPs across chromosomes
![Manhattan Plot](1_Manhattan%20plot.png)

**Q-Q Plot**: Validates the statistical model and identifies true associations
![Q-Q Plot](1_qq%20plot.png)

## 🔬 Methods

The mrMLM package implements six multi-locus GWAS methods:

1. **mrMLM** - Multi-locus random-SNP-effect MLM
2. **FASTmrMLM** - Fast multi-locus random-SNP-effect MLM
3. **FASTmrEMMA** - Fast multi-locus random-SNP-effect EMMA
4. **pLARmEB** - Polygenic-background-control-based least angle regression plus empirical Bayes
5. **pKWmEB** - Polygenic-background-control-based Kruskal-Wallis test plus empirical Bayes
6. **ISIS EM-BLASSO** - Iterative modified-sure independence screening EM-Bayesian LASSO

## 📚 References

- Wang, S. B., et al. (2016). Improving power and accuracy of genome-wide association studies via a multi-locus mixed linear model methodology. *Scientific Reports*, 6, 19444.
- Zhang, J., et al. (2020). mrMLM v4.0: An R platform for multi-locus genome-wide association studies. *Genomics, Proteomics & Bioinformatics*, 18(4), 481-487.

## 📝 Citation

If you use this pipeline in your research, please cite:

```
Basu, S. (2026). GWAS Analysis Using mrMLM. 
GitHub repository: https://github.com/SudhakarBasu/GWAS-using-mrMLM
```

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/SudhakarBasu/GWAS-using-mrMLM/issues).

## 📧 Contact

**Sudhakar Basu**
- GitHub: [@SudhakarBasu](https://github.com/SudhakarBasu)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

⭐ **Star this repository** if you find it helpful!
