---
layout: tutorial_page
permalink: /RNAseq_laptop_setup_instructions
title: RNAseq
header1: Workshop Pages for Students
header2: Informatics for RNAseq Analysis 2020
image: /site_images/CBW_RNA_seq_icon.jpg
home: https://bioinformaticsdotca.github.io/RNAseq_2020
---

1) Install latest version of R which can be downloaded from http://probability.ca/cran/.

1b) Download and install the most recent version of [R Studio desktop](http://www.rstudio.com/).  If prompted to install git, select yes.

2) Install the BioConductor core packages. If you have installed R version 3.5.0 or higher, open R and at the '>' prompt, paste the commands:
 
```
install.packages("BiocManager");
library(BiocManager);
BiocManager::install();
```

If you already have an older version of R installed (3.4.4 or lower), open R and at the '>' prompt, paste the commands:

```
source("http://bioconductor.org/biocLite.R");
biocLite();
```

If you are unsure which version you have installed, open R and at the '>' prompt, enter the command:

```
version
```

3) Install Java. The visualization program that we will be using (IGV) requires Java version 11. First check if you have it installed ([instructions](https://www.java.com/en/download/help/version_manual.xml)). [Install Java 11](https://java.com/en/download/help/download_options.xml) if needed. 

4) Install the Integrative Genomics Viewer 2.8.3 (IGV). Follow the [IGV Install Instructions](http://software.broadinstitute.org/software/igv/download) for your operating system.

5) Install an SSH client if needed. Mac users already have a command line ssh program that can be run from the terminal. For Windows users, please download [PuTTY](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html).  

6). Install the Loupe browser.  First go to the [10x download pages](https://support.10xgenomics.com/single-cell-gene-expression/software/downloads/latest). Enter your info and selectthe Loupe Browser 4.0.0 download for your operating system.

7.) Download the example scRNA loupe files from our [course server](http://genomedata.org/rnaseq-tutorial/scrna/).

