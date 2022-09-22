# test_data_distribution
test data distribution

# Tutorial

## Pre-Requisites
Clone the Repository and install the required packages. Please refer to this section in the README for [instructions](https://github.com/sabiqali/strcount#installation-instructions) on how to install all the required packages.

## Reproducible Example

### Initial Steps:
* ```cd /path/to/cloned/repository```
* ```mkdir test && cd test```
* Download the test dataset:
  ```
  wget https://github.com/sabiqali/test_data_distribution/releases/download/0.1.0/na12878_loci_nanopore.tar.gz
  tar -xvf na12878_loci_nanopore.tar.gz
  ```
  
### For chr6:145272942-145273029 with AGAT repeats
```
mkdir AGAT_chr6_145272942-145273029
python ../src/STRcount/create_config.py --ref /path/to/hg38_reference --motif AGAT --start 145272942 --end 145273029 --chr chr6 --name AGAT > ./AGAT_chr6_145272942-145273029/AGAT_chr6_145272942-145273029.strcount.config.tsv
python ../src/STRcount/STRcount.py --reference /path/to/hg38_reference --fastq ./na12878_loci/AGAT_chr6_145272942-145273029/AGAT_chr6_145272942-145273029.fastq --config ./AGAT_chr6_145272942-145273029/AGAT_chr6_145272942-145273029.strcount.config.tsv --output AGAT_chr6_145272942-145273029.strcount.output.tsv --output_directory ./AGAT_chr6_145272942-145273029/
```
