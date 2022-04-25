# replication-materials-jiehanL
## Purpose
The repertoire of autocratic regimes surviving strategies has greatly extended with the development of modern information and communications technology (ICT). Currently, the relationship between these current digital tools and established, traditional autocratic survival strategies is under-studied. This project aims at using computational methods to depict the use of pro-regime social bots in the events of social movements and using causal inference methods to study its relations with, and effect on, repression and co-optation. 

The code and data in this repository is used for producing reproducible results pertains to the study, it is also in partial fulfillment of the requirements for MACS 30200 "Perspectives on Computational Research" at the University of Chicago.

## Dependencies
The code is written in Python 3.9.7 and R 3.6.1. All of the Python packages can be installed by running the following in the terminal (with the requirements.txt file included in this repository):

```
pip install -r requirements.txt
```
For R packages, you might need to run the following in the terminal (with requirements_r.txt file included in this repository ):
```
#!/usr/bin/bash
while IFS=" " read -r package version; 
do 
  Rscript -e "devtools::install_version('"$package"', version='"$version"')"; 
done < "requirements_r.txt"
```

## Workflow and preliminary results


P.W.D. Charles, Project Title, (2013), GitHub repository, https://github.com/charlespwd/project-title
