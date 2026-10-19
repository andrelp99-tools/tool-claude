# Biologia e genomica (30 skill)

Ogni skill: `library/<nome>/SKILL.md`.

- **bulk-rnaseq**: Prepares bulk RNA-seq FASTQ, Salmon, STAR or featureCounts output for gene-level differential expression.
- **biopython**: Provides Biopython workflows for sequence manipulation, file parsing (FASTA/GenBank/PDB), phylogenetics, and programmatic NCBI/PubMed access (Bio.Entrez).
- **pysam**: Provides Python/HTSlib workflows for genomic files.
- **scikit-bio**: Biological data toolkit.
- **bioservices**: Provides a Python interface to bioinformatics services including UniProt, KEGG, ChEMBL, Reactome, QuickGO, and UniChem.
- **primer-design**: Designs and audits PCR and RT-qPCR primers with Primer3, explicit thermodynamic conditions, reference-based off-target amplification searches, and traceable sequence coordinates.
- **scanpy**: Performs Scanpy single-cell RNA-seq QC, normalization, HVG selection, PCA/UMAP/t-SNE, clustering, exploratory marker ranking, pseudobulk preparation, visualization, and Seurat or SingleCellExperiment RDS conversion to h5…
- **anndata**: Handles annotated matrices in single-cell analysis, .h5ad and Zarr files, and integration with the scverse ecosystem.
- **scvi-tools**: Fits probabilistic models for single-cell omics, including scVI batch integration, scANVI annotation, totalVI CITE-seq, MultiVI RNA/ATAC integration, and posterior differential expression.
- **scvelo**: Performs RNA velocity analysis with scVelo from spliced and unspliced single-cell RNA counts.
- **arboreto**: Infers candidate gene regulatory networks from bulk or single-cell expression data using AertsLab Arboreto GRNBoost2 and GENIE3.
- **cellxgene-census**: Queries the CZ CELLxGENE Census programmatically for versioned public single-cell and spatial transcriptomics data.
- **gget**: Queries 20+ bioinformatics resources through CLI/Python.
- **geniml**: Supports audited local Geniml genomic-interval workflows: validate BED and universe contracts, plan Region2Vec or scEmbed runs, inspect model/tokenizer compatibility, and assess consensus universes.
- **gtars**: Supports Gtars for local genomic interval models and set algebra, overlaps and counts, consensus and coverage, tokenization, fragment processing, and refget/BEDbase planning across Python, Rust, and the CLI.
- **deeptools**: NGS analysis toolkit.
- **polars-bio**: Performs genomic interval overlap, nearest, merge, coverage, complement and subtraction on Polars DataFrames, and reads or writes BED, VCF, BCF, BAM, CRAM, GFF, GTF, FASTA and FASTQ data.
- **zarr-python**: Stores and queries chunked N-D scientific arrays with Zarr-Python 3, including codecs, sharding, S3/GCS storage, and NumPy/Dask/Xarray integration.
- **tiledbvcf**: Stores and retrieves genomic variant calls with TileDB-VCF.
- **flowio**: Reads, inspects, and writes Flow Cytometry Standard (FCS) 2.0, 3.0, and 3.1 files with FlowIO.
- **flowkit**: Analyzes flow cytometry data with FlowKit, including spillover compensation, logicle and biexponential transforms, hierarchical gating, GatingML strategies, and supported FlowJo 10 workspaces.
- **genomic-coordinates**: Converts genomic intervals between coordinate conventions, normalises and compares variant representations, and detects assembly or contig-naming mismatches before they corrupt an analysis.
- **onekgpd**: Queries the 1000 Genomes Project dataset (3,202 whole-genome-sequenced individuals, GRCh38) at the level of individual participants.
- **pydeseq2**: Performs bulk RNA-seq differential expression analysis with PyDESeq2, including count validation, formula designs, explicit contrasts, Wald tests, FDR correction, coefficient-matched LFC shrinkage, and result visualizati…
- **mageck**: Analyzes pooled CRISPR screen FASTQ reads and guide-count matrices with MAGeCK, validates guide libraries and contrasts, measures replicate and library QC, and produces gene hit rankings with effect sizes and FDR.
- **qiime2-amplicon**: Processes paired-end 16S amplicon reads into QIIME 2 ASVs and taxonomy with retained artifact provenance.
- **pathway-enrichment**: Performs pathway and gene-set enrichment analysis on gene lists or ranked gene data and interprets the results.
- **etetoolkit**: Analyzes, manipulates, compares, annotates, and visualizes phylogenetic or other hierarchical trees with ETE 4.
- **phylogenetics**: Builds and analyzes phylogenetic trees using MAFFT multiple sequence alignment, IQ-TREE maximum likelihood with ModelFinder and branch support, and FastTree approximate inference.
- **waypoint-bio**: Supports work with Outpost Bio's open microbiome foundation models - the Waypoint checkpoints (Waypoint-6m, Waypoint-45m, Waypoint-170m), the Atlas pretraining corpus, the Compass eight-task benchmark, or the `waypoint` …
