---
layout: single
title:  "A step towards a cohort retrieval system for EEG records"
date:   2017-12-2 03:32:51 -0500
categories: jekyll update
---
When performing cohort retrieval, the goal is to find patients who have EEGs that are similar to other patients EEGs. If such a system existed, it would enable a clinician or researcher to quickly look up patients who have EEGs similar to  each other. This could then assist them in diagnosing and treating seizures or other conditions, for example. A cohort retrieval system is a little bit different than a traditional classification method. The goal is not to classify a particular EEG, but to find other patients(i.e. the cohort), who are similar to the one in question.

My Master's Krishna Thiyagarajan student recently presented a paper we authored at the IEEE Signal Processing in Medicine and Biology Symposium. The paper was on the application of triplet loss metric to EEG signals. Our goal was to see if we could learn an embedding of EEG signals such that clustering could be performed in the embedding space.

We used the [TUH EEG corpus](https://www.isip.piconepress.com/projects/tuh_eeg/) as our dataset for this. This database contains over 30,000 EEGs and its ultimate goal is to help develop tools for the interpretation of EEGs. Our approach was to use the labeled EEGs and apply the triplet loss function to see if an embedding could be learned. If we can sucessfully learn an embedding using the labeled EEG signals, this embedding could be used in the future on un-labeled EEGs as part of a cohort retrieval system. 

We found that our method was able to learn a meaningful representation of EEGs signals in a reduced dimensional latent space, and therefore could potentially be used as part of cohort retrieval system, as a simple Euclidean(or other) distance metric could be used between patients for a rapid lookup.

For more details, please have a look at the paper, [A Learned Embedding Space for EEG Signal Clustering]({{ site.url }}/assets/EEG_Clustering.pdf).
