singularity exec –bind /scratch/trampush/GWAS:/mount /scratch/…/gatk_latest.sif
gatk CNNScoreVariants -R /mnt/ref/Homo_sapiens_assembly19.fasta -V
/mnt/vcfs/g94982_b37_chr20_1m_15871.vcf.gz -O /mnt/sandbox/my_1d_cnn_scored.vcf

singularity exec\
–bind /scratch1/trampush/GWAS:/mount\
/scratch1/…/verse_latest.sif

gatk CNNScoreVariants -R /mnt/ref/Homo_sapiens_assembly19.fasta -V
/mnt/vcfs/g94982_b37_chr20_1m_15871.vcf.gz -O /mnt/sandbox/my_1d_cnn_scored.vcf
