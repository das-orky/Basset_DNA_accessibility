### Effort to re-implement Basset with Pytorch

<br/>

Basset[1] is one of seminal work done in the field of DNA accessibility with the help of the deep learning networks. Most of the available code for this technique is implemented with tensorflow. This repo try to re-implement the technique using Pytorch. 


The aim is **not to re-implement it with Pytorch but to learn the basic structure of the technique and to understand how DNA accessibility can be implemented via deep networks**

The learning process is broken down into various steps. 


**Step-1**: Basset_raw_data_to_fastq_1cell.ipynb: This Notebook converts the raw data downloaded from the human genome project to a fasta file. For single cell type or for multiple cell types. For this experiment only considering CD4+ T cell. Convert fastq to bed file. 


**Step-2**: Basset_raw_data_to_fastq_multiple_cell.ipynb: Same as the above step but for multiple cell types not only CD4+ T cell. 



**Step-3**: Basset_fasta_to_matrix.ipynb: Converts the bed file into a matrix. 


**Step-4**: Basset_matrix_to_hdf5: the matrix will be converted into a hdf5 type file which helps in loading huge data files into the memory.


**Step-5**: Basset_CNN: it contains the Convolutional Neural Network for classifying accessible genomic sites of a cell. It can be for a single cell or multiple cells.


1. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4937568/