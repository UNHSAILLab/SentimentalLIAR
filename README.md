# Sentimental LIAR: Extended Corpus and Deep Learning Models for Fake Claim Classification
Our Sentimental LIAR dataset is a modified and further extended version of the LIAR extension introduced by Kirilin et al. In our dataset, the multi-class labeling of LIAR is converted to a binary annotation by changing half-true, false, barely-true and pants-fire labels to False, and the remaining labels to True. Furthermore, we convert the speaker names to numerical IDs in order to avoid bias with regards to the textual representation of names. The binary-label dataset is then extended by adding sentiments derived using the Google NLP API . Sentiment analysis determines the overall attitude of the text (i.e., whether it is positive or negative), and is quantified by a numerical score. If the sentiment score is positive, then we assign Positive for the sentiment attribute, otherwise Negative is assigned. We also introduced a further extension by adding emotion scores extracted using the IBM NLP API for each claim, which determine the detected level of 6 emotional states namely anger, sadness, disgust, fear and joy. The score for each emotion is between the range of 0 and 1. Below demonstrates a sample record in Sentimental LIAR for a short claim in the LIAR dataset.

statement="McCain opposed a requirement that the government buy American-made motorcycles. And he said all buy-American provisions were quote ’disgraceful.’ "  
subject: federal-budget  
speaker id: 2  
speaker job: President  
state info: Illinois  
party affiliation: democrat  
sentiment: NEGATIVE  
anger: 0.1353  
disgust: 0.8253  
sad: 0.1419  
fear: 0.0157  
joy: 0.0236  
barely true counts: 70  
false counts: 71  
half true counts: 160  
mostly true counts: 163  
pants on fire counts: 9  
SEN sentiment score: -0.7  



This repository contains the dataset for this paper: https://arxiv.org/abs/2009.01047
