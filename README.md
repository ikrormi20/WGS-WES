# WGS-WES
GATK pipeline for germline variant calling in whole genome sequencing and whole exome sequencing 
This pipeline takes fastq files, preprocesses and maps to human hg19 genome, runs GATK pipeline for germline variant calling and annotates the variants with Annovar software. Adds population databases, prediction tools for variants such as gnomad_exome, gnomad_genome, clinvar databases, OMIM_gene_id and OMIM_phenotypes. This pipeline also generates both unfilter annovar file and filtered annovar file at MAF <= 0.01

Note: Input files are fastq files, and specify respective bed file for whole exome. Bed is not required for WGS.

Usage:
#Execute the job in background#
nohup sh filename.sh &
