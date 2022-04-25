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

### collected tweets around election and protest 
1. collected tweets around 2011 Russian Duma Election and protest
![tweets_around_election_2011](https://user-images.githubusercontent.com/65253017/165016966-800b721c-e3e3-431e-8fb1-a439d4629026.png)
2. collected tweets around 2016 Russian Duma Election and protest
![tweets_around_election_2016](https://user-images.githubusercontent.com/65253017/165016970-26b68e88-3f59-4472-82b1-0b02db94b18d.png)

The above plots show the number of tweets before and after Russian Duma elections in 2011 and 2016. All the tweets were collected through *twint* package through searching hashtag:
#путин, #владимир, #крым, #стpaна, #Украина, #новый, #президент, #Навальный, #сша, #россия, #медведев, #заявлять
(#putin, #vladimir, #Crimea, #country, #Ukraine, #new, #the president, #Navalny, #USA, #Russia, #medvedev, #declare). 
The results show 

To replicate these results, you can use the data from  ```2011_tweets.zip``` and ```2016_tweets.zip``` data and run the 

### detected social bots tweets around election and protest 
1. detected social bots tweets around 2011 Russian Duma Election and protest
![bots_around_election_2011](https://user-images.githubusercontent.com/65253017/165017137-72dc3c73-5033-49ca-84b6-80938350263f.png)

2. detected social bots tweets around 2016 Russian Duma Election and protest
![bots_around_election_2016](https://user-images.githubusercontent.com/65253017/165017168-c15e37c8-44b0-41b4-9098-45e3b14e277e.png)

P.W.D. Charles, Project Title, (2013), GitHub repository, https://github.com/charlespwd/project-title
