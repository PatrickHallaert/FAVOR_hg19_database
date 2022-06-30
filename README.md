# A FAVOR-inspired Back-end Functional Annotation Database for the hg19 Reference Genome

## A Short Synopsis

 This repository outlines the code employed in the construction of a back-end database inspired by the FAVOR Project.
FAVOR, short for *Functional Annotation of Variants - Online Resource*, is a portal that efficiently dispenses functional annotation data acquired from a large assemblage of distinct databases.

 To learn more about FAVOR, I highly recommend visiting [this website](https://favor.genohub.org/) and [this repository](https://github.com/zhouhufeng/FAVORannotator).

 Over the past month, I've had the pleasure of working with some of the highly-skilled and knowledgable scientists that developed this unique resource. This repository is a culmination of my work building an unofficial back-end functional annotation database for FAVOR. More specifically, this project involves the python-based manipulation of data needed to combine and organize functional annotation information from a wide variety of sources. It is worth mentioning that only single nucleotide variants are included in this database. However, I hope to incorporate other genomic variations in the near future.

 ## Details
 
 ### Organization 
 
This repository's files are organized by chromosome. For instance, the *Chr1_Database.ipynb* file includes all the code needed to generate the section of the database corresponding to Chromosome 1 functional annotations and variants.

There is also the *Truncated_Chr22_Database.ipynb* file. This is not part of the database code: it is a "toy" project using a shortened version of Chr22.

### Libraries

The *Dask* python library is integral to the data manipulation used in my code. Thanks to its lazy loading capabilities, it has allowed me to work with massive amounts of data from a computer with minimal RAM.

The *Pandas* library was also useful in my *Truncated_Chr22_Database.ipynb* project; however, due to file sizes and memory issues, it was not employed in the final whole-chromosome code. Nonetheless, it is a great asset.

### Footnotes
Note that replicating this code on your end may lead to a different result. The files and data used in my programs were often manipulated in the command line prior to use in Python. They are not necessarily identical to their "source". 
