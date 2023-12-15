# co_expression_analysis


Data Wrangling and Exploration (data_wrangling_exploration.Rmd)

The data_wrangling_exploration.Rmd script is designed to handle the initial steps of processing and exploring count data in a systematic and reproducible manner. Below is an overview of the key functionalities it performs:

1. Filtering Count Data
The script reads raw count data and employs a two-step filtering process:

Gene Filtering: Genes with low expression levels are removed from the dataset to ensure a focus on biologically relevant signals.
Sample Filtering: Samples with low read counts are excluded to enhance the overall quality of the dataset.
2. Merging Count Data with Sample Information
The filtered count data is merged with sample information, providing a comprehensive dataset that includes both expression values and relevant sample metadata.

3. Gene of Interest Extraction
The script extracts genes of interest based on specific categories:

Protein-Coding Genes
Long Non-Coding RNAs (lncRNAs)
Pseudogenes
This step narrows down the dataset to genes of particular biological relevance.

4. Writing Filtered Count Data to a File
The resulting filtered count data is written to a file, ensuring that the processed dataset is easily accessible for downstream analyses.

5. Gene Annotation Retrieval
The script connects to the Ensembl BioMart database for bovine genes, obtaining comprehensive gene annotations.

6. Writing Annotation Data to Files
The retrieved gene annotation data is written to files, facilitating subsequent analyses that require detailed information about the genes in the dataset.

These steps collectively contribute to a well-curated and annotated dataset, laying the foundation for further exploration and analysis of biological insights.
