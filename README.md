# Brooks_Capstone

README: 
Author: Brooks Baay

Bed_2_Prom:

This code takes tab-delimited BED files from 
promoter region coverage data and creates
a pandas DataFrame for each promoter and a
matching text file: 

Inputs: 
- Tab-delimited .bedgraph file of promoters

Outputs: 
- A DataFrame with the following columns:
  - Number (in the order that it was found in the BED file) 
  - Chromosome it was located on 
  - Start/Stop locations 
  - Length in BP
  - Average Coverage across its region
  - Median Coverage across its region
  - Maximum Coverage value

- A histogram of the promoter lengths

- A histogram with the average coverage 

- A text file copy of the promoter data frame named “Promoters.txt”


Promoter_2_Gene:

This Code takes in a pandas DataFrame of defined promoters, 
a GFF file with the locations of genes documented, 
and a text file with chromosome ID to chromosome number conversions 
and produces a text file of promoter-gene pairs. 

Inputs:
- The promoter data frame must include the following columns in order: 
  - Number (in the order that it was found in the BED file) 
  - Chromosome it was located on 
  - Start/Stop locations 
  - Length in BP
  - Average Coverage across its region
  - Median Coverage across its region
  - Maximum Coverage value

- GFF File of desired reference genome 

- A chromosome ID conversion text file

Outputs:
A DataFrame and matching text file labeled “Prom_2_Gene”
separated into columns by: 
- Promoter Number
- Chromosome Number 
- PROM Start
- PROM Stop
- Strand (designated by "+"/"-")
- GENE Start
- GENE Stop
- GENE ID
