# Multimodal profiling of the transcriptional landscape of developing mouse striatal tissue 

# Description of Scripts + Analysis. 
snRNA1-QC

snRNA2-UMAP

snRNA3-DE

snRNA4-monocle3


# snATAC-seq Analyses
snATAC1-QC => Quality control of snATAC data based on number of fragments and TSS enrichment.

snATAC2-aggregateBin => Final QC and code for generating count matrices based on genomic bins (for initial clustering), gene bodies and promoters.

snATAC3-normalization => Code for initial clustering based on fragments  from fixed-size genome wide bins.

snATAC4-peakNormalization => Final peak calling based on initial clusters to generate high quality peak set, used for final clustering and visualization.

snATAC5-chromVAR_motifs => Computing motif accessibility deviations using chromVAR (Schep et al., 2017) implemented in Signac.

snATAC6-Compute_Gene_Scores => Computing gene activity scores using Cicero, used for subsequent integraton analyses. 

snATAC7-Cluster_Unique_Peaks => Identification of cluster specific peaks.

# Integration Analyses of snRNA & snATAC
snRNA_snATAC_Integration_01_Align_snATAC_snRNA => Integration of snRNA and snATAC data using nearest neighbor information.

snRNA_snATAC_Integration_02_Create_Aggregate_snATAC_snRNA => Aggregate snRNA and snATAC data using nearest neighbor information.

snRNA_snATAC_Integration_03_Compute_Peak_to_Gene_Links => Identification of enhancer-gene pairs by correlating each pair of distal snATAC peak and gene promoter.

snRNA_snATAC_Integration_04_P2G_Analysis => Further characterization of identified enhancer-gene pairs.

snRNA_snATAC_Integration_05_P2G_Monocle => Pseudotime analysis on integrated snRNA-snATAC object using Monocle3. Analyses also include model fitting to identify changes of accessibility and motif deviations as a function of pseudotime.

snRNA_snATAC_Integration__06_chromVAR => Motif analysis for integrated object using chromVAR.


# List of Figures

