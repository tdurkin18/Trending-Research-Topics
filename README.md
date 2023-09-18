
# Determine Trending Research Topics Through Grant Abstracts

## Abstract

This study investigates data extracted from Dimensions in order to produce topic models from grant abstracts. Models were built for the University of Rochester as well as R1 Research Universities. Our approach includes creating models using both Latent Dirichlet Allocation and BERTopic to analyze research topic trends. It was determined that the foremost topics for the University of Rochester consist of Clinical Sciences, Physical Sciences, Cell Biology, and Brain & Cognitive Sciences. R1 institutions had 15 topics which mapped to several categories relating to AI, Systems, Theory and Interdisciplinary Areas in CS Rankings, with an additional topic focused on conferences, education and workshop.

## Dataset
Consists of 51,000 grants from Research 1 Universities from the period 2000-2020. The abstract and year from each grant was used to build the topic models.

## Data Cleaning
Numerous NLP techniques were utilized to clean the dataset in order to build distinguishable topics.

- Removing stop words
- Constructing bigrams and trigrams
- Applying lemmatization to convert common words to their root word
- Removable of words with a high TF-IDF

## Modeling
Two different modeling techniques were used: Latent Dirichlet Allocation and BERTopic. Models were created for 5 year period from 2000 to 2020. Additional models were made only using data from the University of Rochester. LDA models were evaluated based on the Coherence Score to make sure the topics had little overlap. The BERTopic models allowed us to create similarity matrices and see how a topic changes over time.
</br></br>
![](https://github.com/thomasdurkin/Trending-Research-Topics/blob/master/Word%20Cloud%20Example.PNG)
## Results
For each 5 year period model, word cloud were created allowing us to construct self-labelled topics. Our topics were mapped to those listed on CSrankings.org. Concluded that the four major topics over all years were Clinical Sciences, Applied Phyiscs, Genomics, and Brain Sciences. Shift towards patient care and Psychology was seen between 2010-2020.
