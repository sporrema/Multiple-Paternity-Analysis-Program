# Multiple-Paternity-Analysis-Program
An R package modeled off of the C++ Program, FMM

Description:
This program is based off of FMM, a C++ Program created by Neff et al. (2002). Which calculates the frequency of multiple mating within a population based on a sample of broods. 

**Objectives:**
1. Model an R package off of the C++ Program, FMM (Neff et al., 2002).
2. Improve rigid data structure of original FMM program
3. Allow for data sets with more than 20 loci or 40 alleles

**Directions:**

Before running the program four data files must be set-up and saved into your working directory. These files must be saved as .csv files. The following data must be entered in each spreadsheet and read into R as follows:

(1) maternal.csv
Read into R as:

 > maternal <- read.csv("../Data/kichler_maternal.csv", as.is = T)
 
a data frame with columns that include:
an individual ID for each mother (or father) and is labelled "Indiv_ID"
a brood ID that is the same for a mother and all her offspring and is labelled "Brood_ID"
a column of each allele at a locus labelled loc1.1 and loc1.2, etc

Indiv_ID   Brood_ID  loc1.1  loc1.2 

Notes:

(2) offspring.csv
Read into R as:

> offspring <- read.csv("../Data/kichler_offspring.csv", as.is = T)

a data frame with columns that include:

an individual ID for each offspring and is labelled "Indiv_ID"
a brood ID that corresponds to the offspring mother and all her other offspring and is labelled "Brood_ID"
a clutch ID that differentiates between different clutches layed by the same mother and is labelled "Clutch_Num"
a column of each allele at a locus labelled loc1.1 and loc1.2, etc and should be the same number of allele columns as "maternal.csv"

Indiv_ID  Brood_ID  Clutch_Num  loc1.1  loc1.2


(3) paternal.csv
Read into R as:
> paternal <- read.csv("../Data/kichler_paternal.csv", as.is = T)
 
