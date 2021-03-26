# Single Cell RNA-Seq analysis with Seurat

*Waldeyr Mendes Cordeiro da Silva; compiled on Mar-2021*

### Case Study
This R notebook is the code used in a case study of the Chapter "Transcriptome Analysis Throughout RNA-seq" by Brigido et al.

The basic environment is a Linux with R version 4.x. 
I recomend to setup the environment and run it using anaconda by following the steps:

1. Download and install anaconda [anaconda](https://www.anaconda.com/products/individual)
2. Create a conda environment with R version > 4
`conda create --name r4-base`
3. Activate the r4-base environment to use it
`conda activate r4-base`
4. Install R v4.x and the jupyter notebook
`conda install -c conda-forge r-base jupyter git`
5. Open the R console and install/configure

`install.packages('IRkernel')`

`IRkernel::installspec()`

`if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install(version = "3.12")`

`BiocManager::install('limma')`

`BiocManager::install('calibrate')`

`BiocManager::install('dplyr')`

`BiocManager::install('Matrix')`

`BiocManager::install('Seurat') # It requires R version 4.x`

`quit()`

6. Clone this repository

`git clone https://github.com/waldeyr/single_cell_analysis.git`

7. Run the notebook server

`jupyter-notebook`
