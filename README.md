# Platinum-Pedigree-Datasets


Platinum Pedigree Consortium includes whole genome sequencing using five technologies on a 4-generation family. This is the CEPH-Utah (CEU) family 1463 and includes 4 grandparents from 1st generation, 2 parents from 2nd generation, 5 children from 3rd generation, 9 individuals from the 4th generation representing 2 branches of the 3rd generation, and their 2 additional parents. Family was not selected for disease, rather large size to study genetic transmission and human variation. 

<p align="center">
<img src="https://github.com/Platinum-Pedigree-Consortium/Platinum-Pedigree-Datasets/blob/main/images/CEPH_pedigree_github.png" width="500">
</p>



## Accessing the Amazon Open Data

To access the S3 bucket use the amazon awscli:
```
aws s3 ls --no-sign-request s3://platinum-pedigree-data/data
```
## Accessing controlled samples
Not all samples described in Porubsky et al. 2024 are consented for open access. In the third generation NA12883 (2298), NA12884 (2215), and NA12887 (2187) are restricted.
Controlled access samples can be found at dbgap:
```
https://www.ncbi.nlm.nih.gov/gap/
```

## datasets
```
Mapped Element data:
data/element/

Mapped HiFi data:
data/hifi/

Mapped Illumina data:
data/illumina

Mapped ONT data:
data/ont

Mapped and raw Strand-seq data:
data/strandseq
```

## variants
```
Pedigree consistent merged structural variant calls:
variants/merged_sv_truthset/GRCh38/merged_hg38.svs.sort.oa.vcf.gz

Pedigree consistent merged structural variant calls removing overlapping TRs:
variants/merged_sv_truthset/GRCh38/merged_hg38.svs.TRexclusion.sort.oa.vcf.gz

Pedigree consistent tandem repeats:
variants/tr_truthset/GRCh38/ceph_1463_tandem_repeats.oa.vcf.gz

Pedigree consistent merged small variant calls (truthset):
  variants/small_variant_truthset/GRCh38/CEPH1463.GRCh38.family-truthset.ov.vcf.gz
  variants/small_variant_truthset/GRCh38/hq_regions_final.bed.gz

DeepVariant (HiFi) calls:
variants/small_variants/(GRCh38|CHM13)/CEPH1463.GRCh38.deepvariant.glnexus.oa.vcf.gz

Dragen (Illumina) calls:
variants/small_variants/(GRCh38|CHM13)/CEPH1463.GRCh38.illumina-dragen.oa.vcf.gz

Clair3 (ONT) calls:
variants/small_variants/(GRCh38|CHM13)/CEPH1463.GRCh38.ont-clair3.glnexus.oa.vcf.gz

Assembly-based variant calls with respect to both GRCh38 and T2T-CHM13 (CHM13) human references reported by dipcall variant caller:
variants/assembly-based/dipcall

Reported by PAV variant caller:
variants/assembly-based/pav
 
```
---
<p align="center">
  Thanks to Amazon Open Data for sponsorship 
</p>

<p align="center">
<a href="https://aws.amazon.com/what-is-cloud-computing"><img src="https://d0.awsstatic.com/logos/powered-by-aws.png" alt="Powered by AWS Cloud Computing"></a>
</p>


