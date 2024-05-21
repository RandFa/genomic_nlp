# Gene Semantics Prediction Using NLP Approaches in Genomic Contexts

## Project Overview
In the post-genomic era, the volumes of genetic data are rapidly accumulating, particularly in the field of metagenomics, which involves the DNA sequencing of microbial communities directly from their ecosystems. Despite the vast amounts of data available, the function of a significant portion of genes encoded by these microbes remains unknown. Understanding these uncharacterized genes is a major challenge in microbial genomics and has immense potential value in biotechnology and medicine.

This project reworks the analysis done in the paper "Deciphering microbial gene function using natural language processing" to explore the application of Natural Language Processing (NLP) techniques on genomic data to predict gene functions. The focus is on using the genomic context—the set of genes residing near a given gene—to infer gene function, drawing parallels with how context is used in NLP to understand word meanings.

## Background
Experimental and computational studies have shown that the genomic context provides important information regarding gene function. This phenomenon is particularly evident in prokaryotes, where co-functioning genes are often organized in clusters. An example is the CRISPR-Cas systems, which encode a series of genes that confer resistance to foreign genetic elements.

NLP models use the context of words in a sentence to learn semantics. Modern NLP approaches train deep learning algorithms on large corpora of text to provide meaningful numerical representations of words, which can then be used in various downstream applications. Similar techniques have been applied to model "protein languages" and predict properties of amino acids based on their context within a corpus of sequences.

In this project, I extend the application of NLP to a higher level of representation, creating a universal model of "gene semantics". Gene families are treated as "words" that comprise "genomic sentences". By analyzing an extensive dataset of publicly available genomes and metagenomes, we transform genetic data into a corpus and model gene families based on their genomic context.

## Methodology

### Data Collection and Preprocessing:
* Re-annotate and analyze a large dataset of genomes and metagenomes.
* Transform genetic data into a corpus by clustering genes into families.
* Add a layer of abstraction by treating gene families as words in genomic sentences.
* 
### Model Building:
* Word embedding with word2vec
* Claasification based on embeddings

### Validation and Discovery:
Validate the approach by demonstrating its ability to correctly identify recently discovered systems.
Assess the discovery potential of different functional categories.

## Repository Contents
notebooks/: Jupyter notebooks containing the reworked analysis and code implementation, in addition to results.
data/: functuons to scrape the data are available.


## References
Miller, D., Stern, A. & Burstein, D. Deciphering microbial gene function using natural language processing. Nat Commun 13, 5731 (2022). https://doi.org/10.1038/s41467-022-33397-4
## Acknowledgements
The authors of the original paper for their groundbreaking work in applying NLP techniques to genomic data.
The contributors to the publicly available genomic datasets and bioinformatics tools used in this project.
