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
  
### For chr6:145272942-145273029 with AGAT repeats:
```
mkdir AGAT_chr6_145272942-145273029

python ../src/STRcount/create_config.py --ref /path/to/hg38_reference --motif AGAT --start 145272942 --end 145273029 --chr chr6 --name AGAT > ./AGAT_chr6_145272942-145273029/AGAT_chr6_145272942-145273029.strcount.config.tsv

python ../src/STRcount/STRcount.py --reference /path/to/hg38_reference --fastq ./na12878_loci/AGAT_chr6_145272942-145273029/AGAT_chr6_145272942-145273029.fastq --config ./AGAT_chr6_145272942-145273029/AGAT_chr6_145272942-145273029.strcount.config.tsv --output AGAT_chr6_145272942-145273029.strcount.output.tsv --output_directory ./AGAT_chr6_145272942-145273029/
```

### For chr16:73546662-73546736 with TGC repeats:
```
mkdir TGC_chr16_73546662-73546736

python ../src/STRcount/create_config.py --ref /path/to/hg38_reference --motif TGC --start 73546662 --end 73546736 --chr chr16 --name TGC > ./TGC_chr16_73546662-73546736/TGC_chr16_73546662-73546736.strcount.config.tsv

python ../src/STRcount/STRcount.py --reference /path/to/hg38_reference --fastq ./na12878_loci/TGC_chr16_73546662-73546736/TGC_chr16_73546662-73546736.fastq --config ./TGC_chr16_73546662-73546736/TGC_chr16_73546662-73546736.strcount.config.tsv --output TGC_chr16_73546662-73546736.strcount.output.tsv --output_directory ./TGC_chr16_73546662-73546736/
```

### For chrX:55366379-55366473 with TATC repeats:
```
mkdir TATC_chrX_55366379-55366473

python ../src/STRcount/create_config.py --ref /path/to/hg38_reference --motif TATC --start 55366379 --end 55366473 --chr chrX --name TATC > ./TATC_chrX_55366379-55366473/TATC_chrX_55366379-55366473.strcount.config.tsv

python ../src/STRcount/STRcount.py --reference /path/to/hg38_reference --fastq ./na12878_loci/TATC_chrX_55366379-55366473/TATC_chrX_55366379-55366473.fastq --config ./TATC_chrX_55366379-55366473/TATC_chrX_55366379-55366473.strcount.config.tsv --output TATC_chrX_55366379-55366473.strcount.output.tsv --output_directory ./TATC_chrX_55366379-55366473/
```

### For chr10:107609688-107609784 with ATCT repeats:
```
mkdir ATCT_chr10_107609688-107609784

python ../src/STRcount/create_config.py --ref /path/to/hg38_reference --motif ATCT --start 107609688 --end 107609784 --chr chr10 --name ATCT > ./ATCT_chr10_107609688-107609784/ATCT_chr10_107609688-107609784.strcount.config.tsv

python ../src/STRcount/STRcount.py --reference /path/to/hg38_reference --fastq ./na12878_loci/ATCT_chr10_107609688-107609784/ATCT_chr10_107609688-107609784.fastq --config ./ATCT_chr10_107609688-107609784/ATCT_chr10_107609688-107609784.strcount.config.tsv --output ATCT_chr10_107609688-107609784.strcount.output.tsv --output_directory ./ATCT_chr10_107609688-107609784/
```

### For chr7:152384548-152384614 with CAC repeats:
```
mkdir CAC_chr7_152384548-152384614

python ../src/STRcount/create_config.py --ref /path/to/hg38_reference --motif CAC --start 152384548 --end 152384614 --chr chr7 --name CAC > ./CAC_chr7_152384548-152384614/CAC_chr7_152384548-152384614.strcount.config.tsv

python ../src/STRcount/STRcount.py --reference /path/to/hg38_reference --fastq ./na12878_loci/CAC_chr7_152384548-152384614/CAC_chr7_152384548-152384614.fastq --config ./CAC_chr7_152384548-152384614/CAC_chr7_152384548-152384614.strcount.config.tsv --output CAC_chr7_152384548-152384614.strcount.output.tsv --output_directory ./CAC_chr7_152384548-152384614/
```

### For chr4:42555085-42555198 with TATC repeats:
```
mkdir TATC_chr4_42555085-42555198

python ../src/STRcount/create_config.py --ref /path/to/hg38_reference --motif TATC --start 42555085 --end 42555198 --chr chr4 --name TATC > ./TATC_chr4_42555085-42555198/TATC_chr4_42555085-42555198.strcount.config.tsv

python ../src/STRcount/STRcount.py --reference /path/to/hg38_reference --fastq ./na12878_loci/TATC_chr4_42555085-42555198/TATC_chr4_42555085-42555198.fastq --config ./TATC_chr4_42555085-42555198/TATC_chr4_42555085-42555198.strcount.config.tsv --output TATC_chr4_42555085-42555198.strcount.output.tsv --output_directory ./TATC_chr4_42555085-42555198/
```

### For chr1:161051967-161052060 with CAC repeats:
```
mkdir CAC_chr1_161051967-161052060

python ../src/STRcount/create_config.py --ref /path/to/hg38_reference --motif CAC --start 161051967 --end 161052060 --chr chr1 --name CAC > ./CAC_chr1_161051967-161052060/CAC_chr1_161051967-161052060.strcount.config.tsv

python ../src/STRcount/STRcount.py --reference /path/to/hg38_reference --fastq ./na12878_loci/CAC_chr1_161051967-161052060/CAC_chr1_161051967-161052060.fastq --config ./CAC_chr1_161051967-161052060/CAC_chr1_161051967-161052060.strcount.config.tsv --output CAC_chr1_161051967-161052060.strcount.output.tsv --output_directory ./CAC_chr1_161051967-161052060/
```

### For chr12:4702128-4702202 with CCA repeats
```
mkdir CCA_chr12_4702128-4702202

python ../src/STRcount/create_config.py --ref /path/to/hg38_reference --motif CCA --start 4702128 --end 4702202 --chr chr12 --name CCA > ./CCA_chr12_4702128-4702202/CCA_chr12_4702128-4702202.strcount.config.tsv

python ../src/STRcount/STRcount.py --reference /path/to/hg38_reference --fastq ./na12878_loci/CCA_chr12_4702128-4702202/CCA_chr12_4702128-4702202.fastq --config ./CCA_chr12_4702128-4702202/CCA_chr12_4702128-4702202.strcount.config.tsv --output CCA_chr12_4702128-4702202.strcount.output.tsv --output_directory ./CCA_chr12_4702128-4702202/
```

### For chr17:10995712-10995775 with CTG repeats
```
mkdir CTG_chr17_10995712-10995775

python ../src/STRcount/create_config.py --ref /path/to/hg38_reference --motif CTG --start 10995712 --end 10995775 --chr chr17 --name CTG > ./CTG_chr17_10995712-10995775/CTG_chr17_10995712-10995775.strcount.config.tsv

python ../src/STRcount/STRcount.py --reference /path/to/hg38_reference --fastq ./na12878_loci/CTG_chr17_10995712-10995775/CTG_chr17_10995712-10995775.fastq --config ./CTG_chr17_10995712-10995775/CTG_chr17_10995712-10995775.strcount.config.tsv --output CTG_chr17_10995712-10995775.strcount.output.tsv --output_directory ./CTG_chr17_10995712-10995775/
```

Here the options ```--min-identity```, ```--min-aligned-fraction```, ```--write-non-spanned```, ```--repeat_orientation```, ```--prefix_orientation```. ```--suffix_orientation```, ```--multiseed-DP```, and ```--precise-clipping``` have not been entered as they have default values and they do not need to be added for this particular dataset and the config combination. But, depending on your dataset, you might want to set these parameters to the required value. 

If you do not have a config file created, you may use the provided create config utility to create one. 
