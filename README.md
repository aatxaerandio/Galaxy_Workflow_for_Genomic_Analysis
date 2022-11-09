[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)


# Galaxy Workflow for Genomic Analysis
Galaxy Workflow to perform an automated and complete characterization of bacterial genomes

# After your analysis
Check your history to see if your analysis went well. It will go through different statuses before is completed. 

 
| Extension | Description | Description |
| --------- | ----------- |
| Color | Icon | Meaning |
| Color | Icon | Meaning |
| Color | Icon | Meaning |
| Color | Icon | Meaning |
| Color | Icon | Meaning |
| .gff | This is the master annotation in GFF3 format, containing both sequences and annotations. It can be viewed directly in Artemis or IGV. |
| .gbk | This is a standard Genbank file derived from the master .gff. If the input to prokka was a multi-FASTA, then this will be a multi-Genbank, with one record for each sequence. |
| .fna | Nucleotide FASTA file of the input contig sequences. |
| .faa | Protein FASTA file of the translated CDS sequences. |
| .ffn | Nucleotide FASTA file of all the prediction transcripts (CDS, rRNA, tRNA, tmRNA, misc_RNA) |
| .sqn | An ASN1 format "Sequin" file for submission to Genbank. It needs to be edited to set the correct taxonomy, authors, related publication etc. |
