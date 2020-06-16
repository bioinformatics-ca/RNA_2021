---
layout: workshop_main_3day
permalink: /RNAseq_2020_CC_cloud
title: RNA-Seq CC Cloud
header1: Workshop Pages for Students
header2: Informatics for RNA-Seq Analysis 2020
image: /site_images/CBW_RNA_seq_icon.jpg
keywords: RNA-seq data, differential expression analysis, assemble transcripts
description: Course providing an introduction to RNA-seq data analysis followed by integrated tutorials demonstrating the use of popular RNA-seq analysis packages.
instructors: Malachi Griffith, Obi Griffith, Allegra Petti, Kelsy Cotto, Huiming  Xia, Saad Khan
length: 3 days
---
# Compute Canada Virtual Cluster
We have set up a virtual cluster at Compute Canada cloud environment. Each student will have up to 8 cores and 60G memory.
## Access the cluster
### linux/mac user: use "terminal"

```bash
ssh <your username>@login1.CBW.calculquebec.cloud
```
### Windows user: use putty

- Session->hostname: login1.CBW.calculquebec.cloud</br>
![](https://github.com/bioinformatics-ca/RNAseq_2020/blob/master/putty_host.png)
- Connection->Data->Auto-login username: your username</br>
![](https://github.com/bioinformatics-ca/RNAseq_2020/blob/master/putty_user.png)

**Please accept the server's fingerprint if you connect for the first time.** After you sucessfully log into the cluster, you will see a window like:</br>
![](https://github.com/bioinformatics-ca/RNAseq_2020/blob/master/putty_login.png)

## Use the cluster

### Interactive job

After you log into the cluster, you will be on the login node. There are only 2 cores and 2G memory on the login node, so please do NOT run anything here. You can access a compute node with an interactive session using "salloc" command. For example:

```bash
salloc --mem 640M -c 1 -t 1:0:0
```

- --mem: the real memory required per node.
- -c | --cpus-per-task: number of processors required.
- -t | --time: limit on the total run time of the job allocation.
- The command requests an interactive session with 1 core and 640M memory for 1 hour. Once the job is allocated, you will be on one of the compute nodes.

### Software

Compute Canada software stack is mounted on the cluster. It uses limux *module* to manage the software. 

- module available: list all the available modules
- module show <module/version>: show the details of the module
- module load <module/version>: load module for certain version of software
- module unload <module/version>: remove the module settings from system

## Jupyter Hub

Jupyter Hub is available at [https://jupyter.cbw.calculquebec.cloud](https://jupyter.cbw.calculquebec.cloud/). You should be able to use the cluster through your browser. Please use your username and password to login. You will be asked to request resources after you log in and then you will be on one of the compute nodes. You can also download/upload files through jupyter hub.</br>
![](https://github.com/bioinformatics-ca/RNAseq_2020/blob/master/jupyter.png)</br>
**It is important to __*log out*__ once you finish jupyter hub to release the resources. If you only close the browser window, your jupyter hub is still running and using the resources.**