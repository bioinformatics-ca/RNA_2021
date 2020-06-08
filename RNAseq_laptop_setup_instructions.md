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

3) Java -The visualization program that we will be using (IGV) requires Java. Check if you have Java installed: https://www.java.com/verify/ and download Java 11 if you do not have it installed.

4) Integrative Genomics Viewer 2.8.3 (IGV) - Once java is installed, go to http://www.broadinstitute.org/igv/ and register in order to get access to the downloads page. Once you have gained access to the download page, click on the appropriate launch button that matches your computer's operating system   

5) SSH client - Mac and Linux users already have a command line ssh program that can be run from the terminal. For Windows users, please download [PuTTY](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html).  

6). Loupe browser ...

7.) scRNA example loupe files ..

