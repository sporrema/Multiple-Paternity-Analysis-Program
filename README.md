# Multiple-Paternity-Analysis-Program
An R package modeled off of the C++ Program, FMM

Description:
This program is based off of FMM, a C++ Program created by Neff et al. (2002). Which calculates the frequency of multiple mating within a population based on a sample of broods. 

Objectives:
1. Model an R package off of the C++ Program, FMM (Neff et al., 2002).
2. Improve rigid data structure of original FMM program
3. Allow for data sets with more than 20 loci or 40 alleles

Directions:

Before running the program four data files must be set-up. These files must be saved as .csv files. The following data must be entered in each spreadsheet and read into R as follows:

(1) maternal.csv
Read into R as:

 > maternal <- read.csv("../Data/kichler_maternal.csv",as.is=T)
 
a data frame with columns that include:
an individual ID for each mother (or father) and is labelled "Indiv_ID"
a brood ID that is the same for a mother and all her offspring and is labelled "Brood_ID"
a column of each allele at a locus labelled loc1.1 and loc1.2, etc

Indiv_ID   Brood_ID  loc1.1  loc1.2 

Notes:




 
 
