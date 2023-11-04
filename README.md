# QuantAge

## Remote Servers
1. [DNAm age calculator](https://dnamage.genetics.ucla.edu/), Horvath (updated: 2014)
   
   Based on [the seminal Horvath paper in 2013](https://genomebiology.biomedcentral.com/articles/10.1186/gb-2013-14-10-r115). Replaced by an improved online calculator at [clockfoundation.org](https://dnamage.clockfoundation.org). A tutorial and example data files are provided.

   * Measurement platform: Illumina Infinium (EPIC, 450K, or 27K)

2. [Clock Foundation](https://dnamage.clockfoundation.org/user/login), (not yet registered)

3. [ClockBase](https://www.clockbase.org/), Ying et al. (updated: 2023)

   Eleven aging clock models in total, not yet open-sourced. [preprint](https://doi.org/10.1101/2023.02.28.530532)

4. [Aging.AI](http://www.aging.ai/) Deep Biomarkers of aging from basic blood test, by Insilico Medicine.

## Databases

## Downloable Softwares
1. [Mammalian Methylation Assortium](https://github.com/shorvath/MammalianMethylationConsortium), Horvath et al. (updated: 2023)
   
   Contains various data files, clock coefficiencts, and source R codes, including universal mammalian clock and network analysis
   #### Data files
      * An example dataset
      * Genome coordinates for different species
      * The array manifest (names and locations of probes)
      * Probe design details

   #### Measurement platform

   #### Source codes
      * Alignment and annotation
      * Sesame normalization
      * Universal pan-mammalian epigenetic clocks
      * universal blood epigenetic clocks
      * universal skin epigenetic clocks
      * adaptations to Illumina 450K/EPIC array
      * various tissue, sex, and species predictors for mammalian species
      * mammalian network analysis in Haghani et al., Science 2023

   #### Binary codes


2. [Mammalian Methylation Clocks](https://github.com/jazoller96/mammalian-methyl-clocks), Zoller and Horvath (updated: 2023)

   Contains various clock coefficients, and binary R codes. Publishes [A companion paper on biorxiv](https://www.biorxiv.org/content/10.1101/2023.09.06.556506v1) and references to all R functions.

   Over twenty clock coefficients are provided for various species, as well as the Universal Clock (Lu, 2023, Nature Aging). Different reverse age transformations may be required for different clocks.

   In principle, one can write corresponding code in python based on the descriptions?

   * Data normalization. Process raw data wiht Sesame normalization.
   * Data imputation. All clocks are based on Horvath 40K methylation datta. Imputation was only done with Mouse by simply taking mean methylation across all of their mouse data. The standard 320K, 800K, or EPIC array was not tried previously. One last resort is to replace all NAs with 0.5

   #### Data files
      * Over 30 clock coefficients files
      * AnAge table (not sure what it is yet)
   #### Source codes
      * Age transformations (R)
   #### Binary codes
      * The entire MammalMethylClock package is in compiled R binaries only!
      * 
3. [AltumAge](https://github.com/rsinghlab/AltumAge/tree/main), [Camillo et al., Nature Aging, 2022](https://www.nature.com/articles/s41514-022-00085-y), (updated: April 2022)

   A pan-tissue DNA methylation epigenetic clock based on deep learning. 

   #### Problems
      * Missing provide my_functions.py
      * Missing gold_standards.csv
      * Missing data_pkl/*.pkl
      * Who knows what!