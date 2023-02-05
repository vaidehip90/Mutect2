# Mutect2

Mutect2 is a variant calling tools that calls the somatic short mutations. Mutect2 is part of gatk(genomic Analysis toolkit) and can be used when gatk is installed in linux.Mutect2 can be used to call viral variants or tumor samples variants.The three modes of mutect2 can be included; 1)tumor-normal mode which is tumor samples are matched with normal sample. 2) tumor mode where single tumor sample aligment are used in analysis 3) Mitochondrial mode where sensitive calling are done. For this analysis, mutect2 was used to call viral variants for identity testing to find variants present in the samples.

https://gatk.broadinstitute.org/hc/en-us/articles/360037593851-Mutect2

# Installation 

conda install -c bioconda gatk

conda install -c bioconda picard

# Usuage(Command line)

time gatk mutect2 -R ref.fasta -I VCA-test.bam -O VCA-test-mutect2.vcf.gz


-I = -- input

-O = --output

-R = --reference

#reference file = ref.fasta

#Input file = VCA-test.bam

#output file = VCA-test-mutect2.vcf.gz



