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

## sample meta data 

|ped |id    |father|mother|sex|sec.id |primary.id|Generation|
|----|------|------|------|---|-------|----------|----------|
|1463|2281  |0     |0     |1  |GM12889|NA12889   |G1        |
|1463|2280  |0     |0     |2  |GM12890|NA12890   |G1        |
|1463|2214  |0     |0     |1  |GM12891|NA12891   |G1        |
|1463|2213  |0     |0     |2  |GM12892|NA12892   |G1        |
|1463|2209  |2281  |2280  |1  |GM12877|NA12877   |G2        |
|1463|2188  |2214  |2213  |2  |GM12878|NA12878   |G2        |
|1463|2216  |2209  |2188  |2  |GM12879|NA12879   |G3        |
|1463|2211  |2209  |2188  |2  |GM12881|NA12881   |G3        |
|1463|2212  |2209  |2188  |1  |GM12882|NA12882   |G3        |
|1463|2298  |2209  |2188  |1  |GM12883|NA12883   |G3        |
|1463|2215  |2209  |2188  |1  |GM12884|NA12884   |G3        |
|1463|2217  |2209  |2188  |2  |GM12885|NA12885   |G3        |
|1463|2189  |2209  |2188  |1  |GM12886|NA12886   |G3        |
|1463|2187  |2209  |2188  |2  |GM12887|NA12887   |G3        |
|1463|200080|      |      |1  |NA     |200080    |Spouse    |
|1463|200081|      |      |2  |NA     |200081    |G4        |
|1463|200082|      |      |2  |NA     |200082    |G4        |
|1463|200084|      |      |1  |NA     |200084    |G4        |
|1463|200085|      |      |1  |NA     |200085    |G4        |
|1463|200086|      |      |2  |NA     |200086    |G4        |
|1463|200087|      |      |1  |NA     |200087    |G4        |
|1463|200100|      |      |2  |NA     |200100    |Spouse    |
|1463|200101|      |      |1  |NA     |200101    |G4        |
|1463|200102|      |      |1  |NA     |200102    |G4        |
|1463|200103|      |      |2  |NA     |200103    |G4        |
|1463|200104|      |      |2  |NA     |200104    |G4        |
|1463|200105|      |      |1  |NA     |200105    |G4        |
|1463|200106|      |      |2  |NA     |200106    |G4        |



## Ethics declarations
Human subjects: Informed consent was obtained from the CEPH/Utah individuals, and the University of Utah Institutional Review Board approved the study (University of Utah IRB reference IRB_00065564).



---
<p align="center">
  Thanks to Amazon Open Data for sponsorship 
</p>

<p align="center">
<a href="https://aws.amazon.com/what-is-cloud-computing"><img src="https://d0.awsstatic.com/logos/powered-by-aws.png" alt="Powered by AWS Cloud Computing"></a>
</p>


