# Effect of Digoxin on clusters of circulating tumor cells in patients with metastatic breast cancer: a phase 1 trial

A [workflowr][] project.

[workflowr]: https://github.com/workflowr/workflowr



## Data pre-processing

Raw data is available at Gene Expression Omnibus (GEO, NCBI; accession number [XXXXX](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE180097)). Data processing is computationally expensive and is not covered in this repository. We provide description of the data pre-processing workflow together with software version in the original publication. Processed data, large result files, additional functions, references and metadata are were archived at [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1021505.svg)](https://doi.org/10.5281/zenodo.1021505)


##  Data and code availability

To reproduce our analysis, first clone source code from the [GitHub repository](https://github.com/TheAcetoLab/dicct-trial). This repository is also archived at [![DOI](https://zenodo.org/badge/DOI/XXX/XXXX.svg)](https://doi.org/XXXX/XXXX)

    git clone https://github.com/TheAcetoLab/dicct-trial

Next, download processed data deposited in [Zenodo](https://doi.org/10.5281/zenodo.1021505) into the cloned project folder ./data directory and untar the files.

    for file in *.tar.gz; do tar xzvf "${file}" && rm "${file}"; done
    
## Reproducibility

The results form our analyses are listed below in webpage format. They were generated from R Markdown documents deposited in the [GitHub repository](https://github.com/TheAcetoLab/dicct-trial). The workflow of the analysis was created using the [workflowr](https://cran.r-project.org/web/packages/workflowr/index.html) R package and can be reproduced in its totality using [workflowr](https://cran.r-project.org/web/packages/workflowr/index.html) [wflow_build](https://jdblischak.github.io/workflowrBeta/reference/wflow_build.html) command after the installation of the proper R packages. Session info, including R and package versions, was automatically included at the end of each analysis file.

Files containing pre-computed results from differential expression or gene-set enrichment analyses were deposited in [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1021505.svg)](https://doi.org/10.5281/zenodo.1021505). In order to generate those files again change the option `eval = FALSE` to `eval = TRUE` in the specific code chunk from the R Markdown file.
