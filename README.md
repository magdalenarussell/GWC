# Datasets for Girls Who Code visualization

Datasets from three different studies: 

## Demo data

`clinical.csv`

## COVID-19 immunological data

`covid19_immunology.csv`

  This includes demographic and biological data from patients with COVID-19 and healthy patients. The `cohort` column tells you which patients are healthy controls and which are COVID-19 patients. The biological data is from 3 different experiments on the same blood samples. 
  
  Some COVID-19 patients were sampled more than once, on different days. For these samples, the `study_time_collected` column will be greater than 0, and indicates the number of days since the initial sample. You can use this information to see how some patients' immune systems change over time. 
  
  This is from SDY1655 in ImmuneSpace (https://www.immunespace.org/project/Studies/SDY1655/begin.view?), and is published here: https://pubmed.ncbi.nlm.nih.gov/32717743/ 
  
  Columns of interest: 

  * `IgG_OD450`: IgG is a type of antibody. This number is the result of the ELISA assay, which measures the amount of IgG antibody present. Higher numbers mean that the patient is producing more antibodies, indicating that their immune system is responding more strongly. 
  
  * `virus_copies_per_ml`: This is the result from a PCR test, which amplifies a particular DNA or RNA fragment by forcing it to copy itself, so you can more easily detect that particular fragment. This test measures the amount of SARS-CoV-2 (COVID-19 virus) present in the blood sample. 
  
  * `_percent`: There are a lot of columns with `<something>_ percent`. These are the results from the flow cytometry assay. Flow cytometry is used for determining the type of individual cells. These columns tell you the percent of each cell type in the sample. 

## Flu vaccination response data

  There are two datasets from a flu vaccination study. One includes gene expression data for one cohort across time. The other contains immune response data for two cohorts across time. 
  
  In this study, participants were vaccinated with a flu shot, and researchers took blood samples across different timepoints. Samples where `study_time_collected` is 0 are baseline samples, meaning they were taken before the vaccine was given. There are two cohorts, one is all female, and the other is all male.
  
  This is from SDY1276 in ImmuneSpace (https://www.immunespace.org/project/Studies/SDY1276/begin.view?) and is in this publication: https://pubmed.ncbi.nlm.nih.gov/21357945/
  
  1. `flu_vaccination_gene_expression.csv` 
  
  This csv file contains some demographic information about each sample, and columns for each gene (it has > 6,000 columns!). 
      
        
  2. `flu_vaccination_hai.csv`

  This file contians immune response data from the HAI assay. HAI tests how well antibodies in a blood sample will bind to a virus, and can give you an idea of how well the patient's immune system is responding to the vaccine. For each patient, a blood sample was taken before vaccination, and at several different timepoints after being vaccinated. Each blood sample was tested against several different flu viruses to see how well the patient's antibodies can respond to that virus.
  
  Columns of interest: 
  
  * `virus`: This indicates which virus the sample was tested against
  
  * `value_preferred`: This is the result of the HAI assay. Higher numbers mean that the blood sample has more antibodies which bind to the virus, indicating that that patient had stronger response to the vaccine. 
  