# Platinum-Pedigree-Datasets

Platinum Pedigree Consortium includes whole genome sequencing using five technologies on a 4-generation family. This is the CEPH-Utah (CEU) family 1463 and includes 4 grandparents from 1st generation, 2 parents from 2nd generation, 5 children from 3rd generation, 9 individuals from the 4th generation representing 2 branches of the 3rd generation, and their 2 additional parents. Family was not selected for disease, rather large size to study genetic transmission and human variation. 


## Accessing the Amazon Open Data

You will need the AWS command line interface for large transfers:
```https://aws.amazon.com/cli/```

Example of using the awscli 
```
aws s3 ls --no-sign-request s3://platinum-pedigree-data/data
```
