Genomic Data Analytics (GDA)
================
Giulio Caravagna (<gcaravagna@units.it>)
3/5/2021

*MSc program in Data Science and Scientific Computing. University of
Trieste, Italy*

-   3CFU - 24h, 12 lecture, 2 hours each. 50% theoretical lecture, 50%
    practical session (40’ each).
-   GitHub: <https://github.com/caravagn/GDA>

### Lecturers:

-   Giulio x 3 + 1 +2
-   Alex x 1
-   Daniele x 1
-   Salvatore/Riccardo x 1
-   Riccardo x 1
-   Salvatore x 1

—————

# Part 1 - Somatic calling from bulk

Lecture (FORSE TOGLIERE)

-   (Theory) Introduction to the course:
    -   Cancer Evolution,
    -   Modern Genomics,
    -   Single-cell.
    -   Research at the CDSLab.
-   (Theory) Mutation calling:
    -   tumour-matched-normal design,
    -   intuition on Binomial testing,
    -   panel of normals
-   (Practice) Tidyverse
-   (Practice) VCF manipulation

Readings

-   Strelka2
-   Mutect2
-   Platypus
-   GTK

Lecture

    - (Theory) Aneuploidy and Copy Number calling 
        - CBS, ASCAT model, Sequenza
        - Subclonal CNA from Battenberg

    - (Practice) Example runs with ASCAT, Sequenza (inspection of alternative solutions) and playing with CBS. Cohort-level distribution of CNAs per chromosome (length, percentage, copy state).

Readings

-   (tool) Favero, Francesco, et al. “Sequenza: allele-specific copy
    number and mutation profiles from tumor sequencing data.” Annals of
    Oncology 26.1 (2015): 64-70.
-   (tool) Van Loo, Peter, et al. “Allele-specific copy number analysis
    of tumors.” Proceedings of the National Academy of Sciences 107.39
    (2010): 16910-1691
-   (tool) Ross, Edith M., et al. “Allele-specific multi-sample copy
    number segmentation in ASCAT.” Bioinformatics (2020).
-   (tool) Olshen, Adam B., et al. “Circular binary segmentation for the
    analysis of array‐based DNA copy number data.” Biostatistics 5.4
    (2004): 557-572.
-   (Review) Ben-David, Uri, and Angelika Amon. “Context is everything:
    aneuploidy in cancer.” Nature Reviews Genetics 21.1 (2020): 44-62
-   (Review) Weaver, Beth AA, and Don W. Cleveland. “Does aneuploidy
    cause cancer?.” Current opinion in cell biology 18.6 (2006):
    658-667.
-   (In vivo measurements) Bolhaqueiro, Ana CF, et al. “Ongoing
    chromosomal instability and karyotype evolution in human colorectal
    cancer organoids.” Nature Genetics 51.5 (2019): 824-834.
-   (coding) DNAcopy: A Package for Analyzing DNA Copy Data
    <https://bioconductor.org/packages/release/bioc/vignettes/DNAcopy/inst/doc/DNAcopy.pdf>
-   (coding)Total copy-number segmentation using CBS.
    <https://cran.r-project.org/web/packages/PSCBS/vignettes/CBS.pdf>

Lecture

    - (Theory) Quality check somatic calls with CNAqc, and CCFs
    - (Practice) Implement mapping of SNVs to CNA segments, validate MSeq calls, identify good and bad samples from PCAWG

—————

# Parte 2 - mathematical modelling e inference from bulk

Lecture

    - (Theory) Branching process modelling (Riccardo)
    - Synthetic tumour generation with TEMULATOR (https://t-heide.github.io/TEMULATOR/), inspecting VAF distributions for subclones that are about to sweep, or too small to detect), and example tumours from CHESS (https://github.com/sottorivalab/CHESS.cpp)

Lecture

    - (Theory) Subclonal deconvolution with Pyclone e MOBSTER
    - (Practice) Implementation of a Binomial mixture model in R, playing around with MOBSTER single-sample data and BMix.

Lecture

    - (Theory) Phylogenetic inference {Neighbour joining, clones trees, mutation trees, SCITE}
    - Sample trees for MSeq
    - Full subclonal deconvolution with multi-region data

Lecture

    - (Theory) Mutational signatures (Daniele)

—————

# Part 3 - Single-cell genomics transcriptomics

Lecture

    - (Theory) Single-cell RNA analysis (Riccardo/Salvatore) {Seurat,Scanpy}
    - Tutorial vignettes from the tools for scRNAseq

Lecture

    - (Theory) Longitudinal evolution single cell (Alex) {SCITE longitudinal, LACE}
    - Longitudinal evolution from scRNAseq

Lecture

    - (Theory) Count-based modelling single-cell RNA (Salvatore) {clone align, CONGAS}
    - CONGAS vignette from scRNAseq

—————

# Part 4 - Population-level inference

Lecture

    - (Theory) Repeated evolution {REVOLVER}
    - Analysis of TRACERx data and MSeq adenocarcinomas

Lecture

    - (Theory) Population-level models {Bayesian Networks models}
    - Analysis of CODREAD with PICNIC
    - Analysis of other cbio/TCGA datasets

—————
