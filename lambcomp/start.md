# Using Lambowitz lab server #

The Lambowitz lab server (*lambcomp*) is managed by Center for [Biomedical Research Support](https://sites.cns.utexas.edu/cbrs/cbrs-administration).

## Requesting an account  ##

To request an account, you will need to visit the [account managment system](https://rctf-account-request.icmb.utexas.edu/cqb), and make sure to select **Lambowitz Alan** as your affiliation.


## Basics ##

Everytime you need to get on *lambcomp*, you will do this in terminal:

```	
ssh {username}@lambcomp01.ccbb.utexas.edu
```

If you need to download something from *lambcomp* to you local machine (e.g. the lab mac), you will do:

```
scp {username}@lambcomp01.ccbb.utexas.edu:(full path to your file, starts with /stor) (where you want it to be on your computer)
```

### Organization of the lab storage space ###

Below is the directory tree on *lambcomp* that you may find helpful:

```
/stor
├── home 
  	└── {username}      <———————— (your home directory, everything is backed up, 100GB limits)
            ├── {project 1 scripts}
            └── {project 2 scripts}
├── scratch 
	└── Lambowitz
		    └── {username}   <———————— (your SCARTCH directory, everything is not backed up)
├── work
 	└── Lambowitz		
            ├── {username} <———————— (your WORK directory, everything is backed up)
                    └── {project 1 data and results}     
		    ├── Data
                └── NGS		<———— (shared within lab, folder storing all the NGS data we have)
                    ├── JA1?????  <—— (project number from GSAF)
                    └── md_anderson_Sequencing <—— (sequencing jobs from md anderson, very disorganized now)
		    └── ref     <———— (shared within lab, reference genome)     
                ├── Ecoli
                    └── k12_mg1655.fa   <—— (this is mg1655 reference fasta)
                └── hg19                <—— human genome reference 
```

- home directory is the place that I put my scripts/codes.  
    - **backed up**
    - 100 GB limits
- work directory is the place to put all the result/data in  
    - **backed up**
    - up to 60TB for the whole lab)
- scratch directory, you can ignore it, or if you are trying something out, you can use it 
    - not being backed up)
    

## More ##

For more information, you can visit the [user page](https://wikis.utexas.edu/display/RCTFusers/POD+Accounts) for Research Computing Task Force Users.