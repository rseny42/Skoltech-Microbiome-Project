HMP.zip contains the original database, containing .biom files. It includes 14102 items:
AGP database, 9511 items
IBD database, 86 items
PTB databse, 3462 items, including 5 empty folders (probably an error of data acquiring)
T2D database, 1043 items

AGP database is normalized to 1, every other databse is not.

AGP database is also the only database that was corrected by the blooming procedure. Citation:
"An important practical question is whether selfcollected microbiome samples can match those from better-controlled studies. Most AGP samples are stools collected on dry swabs and shipped without preservative to minimize costs and avoid exposure to toxic preservatives. Escherichia coli and a few other taxa grow in transit, so based on data from controlled-storage studies as previously described (15), we removed sub-operational taxonomic units (sOTUs) (16) (median of 7.9% of sequences removed per sample) shown to bloom." for more details look the articles from Bloom Analyses Directory.

HMP_1.zip contains the same database, but every directory has also a table-format .txt file converted from biom format. It contains the whole taxonomic information and OTU IDs (for all databases),  and nucleotide chains (for AGP database). Every directory contains bash scripts for converting biom data to table format.

HMP_2.zip also contains 3 tables - pivot for the taxonomy levels o, f and g and scripts for the splitting the tabular data. As a result of conversion 5 empty folders in ptb database were found and also cut tails in the same database. In the other 3 databases if any taxonomy level was not presented, there was a s__ empty marker (or other letter indicating taxonomy level instead of s). And in the ptb database for some reason to be investigated, in some positions in some files there were just empty fields. The script is working in such a manner that it replaces empty fields with the s__ (or other letter indicating taxonomy level instead of s) marker. Also the script checks the sum of the whole file bacteria quantity before and after the splitting.

5 empty folders for PTB database are:
EP038468_K40_MV1D.otu_table.biom
EP216429_K130_BRCD.otu_table.biom
EP261740_K30_MCKD.otu_table.biom
EP407012_K70_BCKD.otu_table.biom
EP970774_K20_MV1D.otu_table.biom
