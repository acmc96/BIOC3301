# BIOC3301 report codes

This folder contains the codes used for Metagenomic analysis of the soil micrbiome.

Each of these scrips were run with each year's dataset, form 2016-2018, except Join Paired Ends in 2016 and 2017 according to the weaker quality of data. 

Order of the codes used:

###### *1. Join Pair Ends*

This script takes the forward and reverse Illumina reads and joins them using SeqPrep (method chosen). Index file containing barcodes were included to match the surviving joined pairs to the barcodes.

###### *2. Splitting Libraries*

This script performs demultiplexing of Fastq sequence data where barcodes and sequences are contained in two separate fastq which are present on Illumina runs. The reference database used was Greengenes. 

###### *3. Picking OTUs*

Scripts picks OTUs in closed reference method; and constructs an OTU table. The table is in a biom format that can be made human readable with the command: biom summarize -i /path/to/table. Default clustering tool was used, uclust.

###### *4. Core Diversity*

Scripts generates analysis of alpha diversity, beta diversity and taxanomy data. 

###### *5. Plot Summary*

Script used to create pie charts of OTU percentage abundence.

###### *6. Summarize Taxa*

Used to create a biom table with phylum abundence only. Permits further analysis at phylum level only. 

###### *7. Heatmap*

Generated heatmaps of phyulm abundence in each sample, within each dataset for each year. 

###### *8. Make OTU Network*

Script creates network text files demonstrating links between sampleID and phylum presence, to be used in Cytoscape. 


Spearman's rank statistical analysis was carried out in Excel. 

