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
Not all samples described in Porubsky et al. 2024 are consented for open access. Controlled access samples can be found at dbgap:
```
https://www.ncbi.nlm.nih.gov/gap/
```


---
<p align="center">
  Thanks to Amazon Open Data for sponsorship 
</p>

<p align="center">
<a href="https://aws.amazon.com/what-is-cloud-computing"><img src="https://d0.awsstatic.com/logos/powered-by-aws.png" alt="Powered by AWS Cloud Computing"></a>
</p>
