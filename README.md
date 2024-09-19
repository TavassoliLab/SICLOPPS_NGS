# SICLOPPS_NGS

Data analysis pipeline to complement the paper: 
Next Generation SICLOPPS Screening for the Identification of inhibitors of the HIF-1a/HIF-1b protein-protein interaction 

DOI: https://doi.org/10.1021/acschembio.4c00494

Alexander McDermott,1,# Leonie Windeln,1,# Jacob Valentine,1 Leonardo Baldassarre,2 Andrew Foster,1 and Ali Tavassoli1,* 
1School of Chemistry, University of Southampton, Southampton, SO17 1BJ, U.K. 
2Curve Therapeutics, Delta House, Southampton Science Park, Southampton, SO16 7NS, U.K.

#authors contributed equally to this work 

*e-mail: ali1@soton.ac.uk 

Jupyter notebooks:

Process_raw_sequencing_data: Reads in the FASTA file and performs some initial analysis. This is mainly raw data processing and can be adjusted for other sequencing setups by changing the writefiles function. This mainly relies on biopython for parsing the Fastq files.

Analyse_enrichment: Takes dataframes of cleaned data and does some further enrichment analysis. This also contains the clustering code. Scipy, sklearn, and radialtree are used here.

Scan peptides: Creates sequence logos from the saved dataframe - using the logomaker package. (Tareen A, Kinney JB (2019) Logomaker: beautiful sequence logos in Python. Bioinformatics btz921. bioRxiv doi:10.1101/635029.)
