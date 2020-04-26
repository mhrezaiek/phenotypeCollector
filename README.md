# phenotypeCollector
Collecting phenotypes from ENA and make their SNPs

## dataCollector.py
In this code by using the phenotypes id in the "FILE_NAME".txt file we will download its .fastq files from ENA databese

## SNP.py
In this code by using the phenotypes id in the "FILE_NAME".txt file and its .fastq files we will make its SNP using bwa and samtools and GATK and get the common SNP of both files and store in ("Final_" + id + ".vcf")

If the code fail in make SNP of special phenotype, the id will be write in the "missIdForSNP.txt"

By calling preprocessing() function you will get the ( "Final_" + id + "_table.csv" ) file which contatin "pos, ref, alt" for each SNP

