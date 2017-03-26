# WSMD
Discovery motifs on ChIP-seq datasets with WSMD
=================================================

Dependencies:
-------
  * R ( ≥ 3.2.5 )
  * Matrix ( ≥ 1.2-6 )
  * Rcpp( ≥ 0.12.6 ）
  * Rmosek（≥ 7.1.2 ）
  * seqLogo（≥ 1.36.0 ）
  * ChIPpeakAnno（≥ 3.4.6 ）
  * BSgenome.Hsapiens.UCSC.hg19（≥ 1.4.0 ）

R packages:
-------------------------
  * Linux binary package: WSMD_0.1.1_R_x86_64-pc-linux-gnu.tar.gz
  * Windows binary package: WSMD_0.1.1_windows_binary.zip
  * Source package: WSMD_0.1.1.tar.gz
  
Installation guides:
-------------------------
  * Dowload mosek 7 from https://mosek.com/resources/downloads/legacy/version-7-1, unpack and install it following the MOSEK Quickstart Guide which can be found in the unpacked directory.
  * Install Rmosek for mosek 7 and other dependencies following http://rmosek.r-forge.r-project.org/.
  * Download and install WSMD R package.
    
Usage guides:
-------------------------
  * Load WSMD package before using it.
  * WSMD offers a function named 'WSMD' to apply de novo motif discovery or motif optimization.
  * WSMD offers a function named 'peak2seq' to Extract foreground and background sequences from ChIP-seq peak file.
  * WSMD offers three evaluate functions named 'evaluate_PWM_AUC', 'evaluate_PWM_fishers_exact_test_P_value' and 'evaluate_PWM_MHG_P_value' to help users to assess the reported motifs.
  * Details on using each function are given in the help documents of WSMD package. After successfully installing, users can access the help documents by running following scripts in R:

```r
# Get all the help documents of WSMD package by running
library("WSMD")
help(package = "WSMD")
# Or get the Description, Usage and Arguments information of each funciton directly by running
library("WSMD")
?WSMD
?peak2seq
?evaluate_PWM_AUC
?evaluate_PWM_fishers_exact_test_P_value
?evaluate_PWM_MHG_P_value
```
 
Input and output examples:
-------------------------
  * Inout sequence files: input_foreground_sequences.fasta, input_background_sequences.fasta
  * Output motif file: output_motif.txt
  
If having any questions about WSMD packages, please feel free to contact hongbozhang0808@163.com
