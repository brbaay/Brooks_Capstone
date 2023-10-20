# Brooks_Capstone
This code takes tab deliminated txt files from promoter region coverage data and creates
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

Included in this folder are: 
- The BED_2_Promoter code 
- 4 sets of coverage text files
- A smaller "Test" text file that is a smaller version of the "MSp134.bedgrapgh" file
- A text file including the promoter data
