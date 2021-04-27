# Datasets for Girls Who Code visualization

Datasets from three different studies: 

## Demo data

`clinical.csv`

## COVID-19 immunological data

`covid19_immunology.csv`

  This includes demographic and biological data from patients with COVID-19 and healthy patients. The biological data is from 3 different experiments on the same blood samples, across multiple timepoints. This is from SDY1655 in ImmuneSpace (https://www.immunespace.org/project/Studies/SDY1655/begin.view?), and is published here: https://pubmed.ncbi.nlm.nih.gov/32717743/ 
  
  Columns of interest: 
  * IgG_OD450: IgG is a type of antibody. This number is the result of the ELISA assay, which measures the amount of IgG antibody present. Higher numbers mean that the patient's immune system is responding more strongly. 
  
  * virus_copies_per_ml: This is the result from a PCR test, which amplifies a particular DNA or RNA fragment by forcing it to copy itself. A type of PCR test is used for COVID testing. Higher numbers here mean that the patient is more likely to have active SARS-CoV-2 (COVID-19 virus) in their system. 
  
  * _percent: There are a lot of columns with <something>_ percent. These are the results from the flow cytometry assay. Flow cytometry is used for determining the type of individual cells. These columns tell you the percent of each cell type in the sample. 

## Flu vaccination response data

  There are two datasets from a flu vaccination study. One includes gene expression data for one cohort across time. The other contains immune response data for two cohorts across time. In this study, participants were vaccinated with a flu shot, and researchers took blood samples across different timepoints. This is from SDY1276 in ImmuneSpace (https://www.immunespace.org/project/Studies/SDY1276/begin.view?) and is in this publication: https://pubmed.ncbi.nlm.nih.gov/21357945/
  
  1. `flu_vaccination_gene_expression.csv` 
  
  This csv file contains some demographic information about each sample, and columns for each gene (it has > 6,000 columns!). 
      
        
  2. `flu_vaccination_hai.csv`

  This file contians immune response data from the HAI assay. HAI tests how well a sample will bind to a virus, and can give you an idea of how well the patient's immune system is responding to the vaccine. Higher numbers correspond to a stronger response. 
    
    
    
    
    
