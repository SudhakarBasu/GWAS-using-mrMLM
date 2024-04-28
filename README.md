# GWAS-using-mrMLM
# Multi-Locus Genetic Analysis Tool

## Description

This repository hosts an R-based tool that utilizes the `mrMLM.GUI` package for multi-locus random-SNP-effect mixed linear model analysis. The tool is designed to provide a user-friendly graphical interface to facilitate the analysis of genetic data, making it accessible to geneticists and researchers with varying levels of computational expertise.

The GUI simplifies the complex process of configuring and running genetic models, thereby improving the efficiency and effectiveness of genetic data analysis.

## Features

- **Easy-to-use graphical user interface:** Streamlines the input of data and setting of analysis parameters.
- **Implementation of advanced genetic models:** Leverages the `mrMLM.GUI` for rigorous analysis.
- **Adaptable to various genetic datasets:** Suitable for a wide range of genetic research purposes.

## Installation

To get started with this tool, follow these steps to set up your environment:

1. **Install R:**
   Ensure that you have R installed on your computer. You can download and install it from [CRAN](https://cran.r-project.org).

2. **Install the `mrMLM.GUI` package:**
   Open R and run the following command to install the `mrMLM.GUI` package:

   ```R
   install.packages("mrMLM.GUI")
   
3. **Load the package:**
   Use the following command in R to load the package:
   ```R
   library(mrMLM.GUI)
   
4. **Launch the GUI:**
   Start the graphical interface by executing:
   ```R
    mrMLM.GUI()

## Usage

After launching the mrMLM.GUI, the graphical interface will guide you through the process of loading your data and setting up the analysis. Follow the on-screen instructions to configure the analysis parameters and execute the model.

**Data Input:** Use the GUI to input your data files.

**Parameter Settings:** Adjust the analysis settings as necessary for your specific dataset.

**Run Analysis:** Execute the analysis and view the results directly through the GUI.
