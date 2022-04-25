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
There is often a spike in tweet counts after elections. Considering that all the tweet data is collected according to the above hashtag, it can be derived that these tweets are related to the election and the protest。

To replicate these results, you can use the data from  ```2011_tweets.zip``` and ```2016_tweets.zip``` data and run the the chuck of code ```twitter data visualization``` at the ```data visualization.Rmd`` file. 

### detected social bots tweets around election and protest 
1. detected social bots tweets around 2011 Russian Duma Election and protest
![bots_around_election_2011](https://user-images.githubusercontent.com/65253017/165017137-72dc3c73-5033-49ca-84b6-80938350263f.png)

2. detected social bots tweets around 2016 Russian Duma Election and protest
![bots_around_election_2016](https://user-images.githubusercontent.com/65253017/165017168-c15e37c8-44b0-41b4-9098-45e3b14e277e.png)

The above plots show the social bots tweets before and after Russian Duma elections in 2011 and 2016. 
From the 2011 figure, we can see that the number of social bots tweets was high before the election and dropped on the Election Day. With the start of the first round of social protests, the number of social bots grew and fell between the two protests, until the second round of protests on December 24th they increased again. 
In the 2016 figure, the number of social bots is low before the election and on election day, and the number of social bots does not increase until the protest starts. 

To replicate these results, you can use the data from  ```classification_result.csv``` and run the the chuck of code ```classification result visualization``` at the ```data visualization.Rmd`` file. 

## What do we know so far? 
The above results suggest that the social bots has been used to meddle with election and social protests in Russia: along with the social protests, there are usually a surge in pro-regime social bots deployment. It is also worth noticing that the percentage of social bots in 2011 protest is higher than in 2016 protest, but social bots depoyment in 2016 protest is more timely and prompt, indicating that the government is more experienced in information manipulation online. The next step would be looking into the interaction among social bots deployment, repression, and co-optation. 

If you use this repository for a scientific publication, you can cite the following GitHub repository URL as it is just preliminary result:
L. Jiehan, Russia Social Bots and Autocrats' Surviving Strategies, (2021), GitHub repository, https://github.com/macs30200-s22/replication-materials-jiehanL/edit/main/README.md
