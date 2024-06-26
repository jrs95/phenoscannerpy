# phenoscannerpy <img src="logo.png" align="right" height="139"/>
**The PhenoScanner database is no longer maintained.**  

## Introduction
Python 3 tool to query the PhenoScanner database of human genotype-phenotype associations from a terminal.  

## Installation
* Download the [phenoscanner.py](https://raw.githubusercontent.com/phenoscanner/phenoscannerpy/master/phenoscanner.py) file.  
* Download the test files.  

## Usage

### Single query  
A single SNP, gene or region can be queried on the command line using the snp, gene or region flag respectively (see examples below).  

### Multiple queries  
Multiple queries can be performed by using inputting a file containing the SNPs/genes/regions to be queried. Input files have to be tab-delimited text files (without a header) with one SNP, gene or genomic region per line (max 100 SNPs, 10 genes or 10 regions) depending on the query. These files are loaded into the program using the infile option (file prefix only, i.e. no .txt) and by setting the relevant query type to True (see examples below).  

## Examples
```
# Help  
python3 phenoscanner.py --help

# SNP  
python3 phenoscanner.py --snp=rs10840293
python3 phenoscanner.py --snp=True --infile=test_snp

# Gene  
python3 phenoscanner.py --gene=SWAP70
python3 phenoscanner.py --gene=True --infile=test_gene

# Region
python3 phenoscanner.py --region=chr11:9500000-10500000 
python3 phenoscanner.py --region=True --infile=test_region
```

## Citations
* Staley JR, *et al.* PhenoScanner: a database of human genotype-phenotype associations. [Bioinformatics](https://pubmed.ncbi.nlm.nih.gov/27318201/) 2016;32(20):3207-3209.  
* Kamat MA, *et al.* PhenoScanner V2: an expanded tool for searching human genotype-phenotype associations. [Bioinformatics](https://pubmed.ncbi.nlm.nih.gov/31233103/) 2019;35(22):4851-4853.  

## Terms of use
Please abide by the [terms of use](http://www.phenoscanner.medschl.cam.ac.uk/about/#terms) of PhenoScanner when using this R package.  

