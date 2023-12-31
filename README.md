# QuantAge

This research project aims to investigate the relationship between epigenetic marks and chronological age. By studying known epigenetic blocks, we aim to develop a method to accurately determine ages based on these marks. Epigenetic marks are modifications to DNA that can provide insights into an individual's biological age, which may differ from their chronological age. Understanding the connection between epigenetic marks and age can have significant implications for various fields, including aging research, forensic science, and personalized medicine.

Through extensive analysis and data collection, we will explore the patterns and correlations between epigenetic marks and chronological age. By examining a diverse range of samples and utilizing advanced computational techniques, we aim to develop a robust model that can accurately predict ages based on epigenetic marks. This research project has the potential to contribute to our understanding of the aging process and open up new avenues for age-related studies and applications.

Please note that the findings and results of this research project are preliminary and subject to further verification and validation.

## Remote Servers

<details>
<summary> [DNAm age calculator](https://dnamage.genetics.ucla.edu/), Horvath (updated: 2014) </summary>
   
   Based on [the seminal Horvath paper in 2013](https://genomebiology.biomedcentral.com/articles/10.1186/gb-2013-14-10-r115). Replaced by an improved online calculator at [clockfoundation.org](https://dnamage.clockfoundation.org). A tutorial and example data files are provided.

   * Measurement platform: Illumina Infinium (EPIC, 450K, or 27K)
</details>

<details>
<summary>[Clock Foundation](https://dnamage.clockfoundation.org/user/login), (not yet registered)</summary>
</details>

<details>
<summary>[ClockBase](https://www.clockbase.org/), Ying et al. (updated: 2023)</summary>

   Eleven aging clock models in total, not yet open-sourced. [preprint](https://doi.org/10.1101/2023.02.28.530532)
</details>

<details>
<summary>[Aging.AI](http://www.aging.ai/) Deep Biomarkers of aging from basic blood test, by Insilico Medicine.</summary>
</details>

## Databases

## Downloadable Softwares
<details>
<summary>[Mammalian Methylation Assortium](https://github.com/shorvath/MammalianMethylationConsortium), Horvath et al. (updated: 2023)</summary>
   
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
</details>

<details>
<summary>[Mammalian Methylation Clocks](https://github.com/jazoller96/mammalian-methyl-clocks), Zoller and Horvath (updated: 2023)</summary>

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

</details>

<details>
<summary>[AltumAge](https://github.com/rsinghlab/AltumAge/tree/main), [Camillo et al., Nature Aging, 2022](https://www.nature.com/articles/s41514-022-00085-y), (updated: April 2022)</summary>

   A pan-tissue DNA methylation epigenetic clock based on deep learning. 

   #### Problems
      * Missing my_functions.py
      * Missing gold_standards.csv
      * Missing data_pkl/*.pkl
      * Who knows what!

</details>

## Helper Packages
<details>
<summary>[GEOparse](https://github.com/guma44/GEOparse), (updated: August 2021)</summary>
Python library to access Gene Expression Omnibus Database (GEO).

GEOparse is python package that can be used to query and retrieve data from Gene Expression Omnibus database (GEO). The inspiration and the base for it is great R library GEOquery.

   #### Problems
      * Lack documentation
      * Lack features
</details>