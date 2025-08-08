git clone https://github.com/ldutoit/RAD_snakemake.git

Show the config file:

....

module load cutadapt FastQC BWA SAMtools Stacks snakemake


snakemake --dag filtered.recode.vcf | dot -Tsvg > dag.svg # create the graph of rules 
snakemake --cores all filtered.recode.vcf
