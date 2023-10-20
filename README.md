# Brooks_Capstone
This code takes tab deliminated BED files from promoter region coverage data and creates
a file for each promoter defined by its: 

- Number (in the order that it was found in the BED file) 
- Chromosome it was located on 
- Start/Stop locations 
- Length in BP
- Average Coverage across its region
- Median Coverage across its region
- Maximum Coverage value

Inputs: 
- Tab-delimited .bedgraph file
