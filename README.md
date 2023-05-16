# Background

We are looking for students that can successfully train machine learning models on limited and complex biological data.
This will require experience/familiarity with ML models and some amount of biological knowledge to be able to work with the data.

# Task - A-domain specificity
Not all peptides are constructed by ribosomes.
Instead, a large enzyme called a non-ribosomal peptide synthetase (NRPS) builds these non-ribosomal peptides.
While heavily modified post-assembly, the NRP backbones are constructed of proteinogenic and non-proteinogenic amino acids.
The regions of NRPSs that select for the backbone amino acids are the adenylation domains.
More specifically, a select set of amino acids in adenylation domains are local to the binding pocket and confer specificity.

We have provided a two-column TSV in `data/a_domains.tsv`.
The first column is the specificity-conferring amino acids of an adenylation domain.
This consists of the 20 proteinogenic amino acids and `-` for gaps in the alignment.
The second column is a three letter code for the amino acid it binds to.
More information can be found about amino acids in `data/amino_acid_codes.tsv`.

Your task is to predict the recruited amino acid from the A-domain sequence.
You are free to use any model, any data featurization, and any data splitting you like.
However, one of the models is required to be a neural network built using PyTorch.
A previously successful method is described [in this paper](https://academic.oup.com/nar/article/39/suppl_2/W362/2506164).
All attempted models should be documented along with their results.

In your fork of the repository please include:
1. All of your code
2. A markdown document that explains how to compile and run your to train and evaluate the model
3. A presentation or PDF containing a summary of model architectures attempted and their results
