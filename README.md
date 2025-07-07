# CSAMA_annotation

This repository begins with notes on an evening meeting at CSAMA 2025.  If you
were present please add your github id to the issue #1.

# Some key annotation resources

- BSgenome, BSgenome.Hsapiens.UCSC.hg38, other reference genomes; TxDb packages for gene models
- GENCODE models in AnnotationHub
- rtracklayer for obtaining computable representations of UCSC genome browser tracks
- ensembldb and EnsDb packages
- ontologies available through ontoProc include cell ontology, human phenotype ontology
- celldex as a collection of transcriptomes of specific cell types used for annotating transcriptomes in single cell RNA-seq
- SingleR book

# Resources for model organisms mentioned in the meeting

## Medaka (Oryzias latipes)

```
library(AnnotationHub)
ah = AnnotationHub()
med = query(ah, "Oryzias")  # returns AH119390
med = ah[["AH119390"]]
```
The `med` report is:
```
EnsDb for Ensembl:
|Backend: SQLite
|Db type: EnsDb
|Type of Gene ID: Ensembl Gene ID
|Supporting package: ensembldb
|Db created by: ensembldb package from Bioconductor
|script_version: 0.3.10
|Creation time: Sun Oct 27 16:27:31 2024
|ensembl_version: 113
|ensembl_host: 127.0.0.1
|Organism: Oryzias latipes
|taxonomy_id: 8090
|genome_build: ASM223467v1
|DBSCHEMAVERSION: 2.2
|common_name: Japanese medaka HdrR
|species: oryzias_latipes
| No. of genes: 24365.
| No. of transcripts: 38211.
|Protein data available.
```
- 

