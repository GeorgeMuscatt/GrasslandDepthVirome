# README

This repository contains the data and code used in Muscatt et al. (on [bioRxiv](https://www.biorxiv.org)). 
-   The metagenomic data set, generated previously by Sharrar et al. (DOI: 10.1128/mBio.00416-20), can be accessed from NCBI under project accession PRJNA577476 (sample accessions SAMN13153360-SAMN13153383). 
-   dsDNA vOTU genome sequences can be accessed from NCBI under project accession PRJEB57765 (sample accession SAMEA112154074). 
-   vOTU prediction stats, FASTA nucleotide files (containing vOTU genomes, MAG bins, and rpS3 sequences), FASTA amino acid files (containing vOTU genes and DNA polymerase genes), Newick tree file containing jumbo phage phylogeny, and vConTACT2 network input and output files are available from [figshare](https://figshare.com).

------------------------------------------------------------------------

The R markdown script `figures_and_tables.Rmd` can be used to generate all the main and supplementary figures and tables in the above publication. Each figure/table is contained within chunks which are intended to be run sequentially i.e., later chunks may require the supplementary tables to have been loaded into the R environment at the beginning. The script is not intended to be knitted, rather each figure/table will be saved to file within the `Figures` or `Tables` directory, respectively.

Note: **Table 1** is not generated within R.

The `Data` directory holds the raw and processed data files to be loaded into the R environment by `figures_and_tables.Rmd`:

-	`AMG_annotations.csv` = functional annotations for putative viral-encoded auxiliary metabolic genes
-	`defense_finder_genes.tsv` = anti-phage defence system genes detected on microbial scaffolds
-	`defense_finder_systems.tsv` = anti-phage defence systems detected on microbial scaffolds
-	`DNA_vOTU_gene_annotations.csv` = functional annotations for all viral genes
-	`DNA_vOTU_reads` = vOTU data including read counts
-	`DNAP_tree` = tree file for jumbo phage phylogenetic tree based on DNA polymerase gene
-	`edges.csv` = edges for drawing vConTACT2 network 
-	`genome_by_genome.csv` = viral cluster statuses outputted by vConTACT2
-	`green_genes.tsv` = Greengenes bacterial taxonomy list
-	`inphared_data_1Aug2022.tsv` = metadata on viral genomes from INfrastructure for a PHAge REference Database (INPHARED) repository
-	`instrainComparer_comparisonsTable.tsv` = consensus ANI output from instrain
-	`local_contig_microdiversity.tsv` = micro diversity estimates at contig-level outputted by metapop
-	`local_gene_microdiversity.tsv` = micro diversity estimates at gene-level outputted by metapop
-	`lysogeny_gene_hits.tsv` = viral gene hits to lysogenic PFAM modules
-	`MAG_bin_index.csv` = index to connect 285 microbial MAG bins to 337 microbial MAGs
-	`MAG_metadata.xlsx` = metadata of 337 microbial MAGs provided by Sharrar et al. 2020
-	`MAG_normalised_coverage.csv` = MAG data including normalised coverage values
-	`nodes.csv` = nodes for drawing vConTACT2 network
-	`OTU_normalised_coverage.csv` = OTU data including normalised coverage values
-	`PhageClouds_hits_sources.csv` = sources of viral genomes from PhageClouds database
-	`scaffold_bin_index.csv` = index to connect 285 microbial MAG bins to 120,665 scaffolds

The `Figures` directory serves as a location for main and supplementary figures created by the script `figures_and_tables.Rmd` to be saved into.

The `Tables` directory serves as a location for supplementary tables created by the script `figures_and_tables.Rmd` to be saved into.

This README and `figures_and_tables.Rmd` was written by George Muscatt (g.s.muscatt(at)warwick.ac.uk).
