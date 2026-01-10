---
layout: post
title:  "Data Science Projects for Social Good, Spring 2018, Impact of charities"
date:   2016-6-3 03:32:51 -0500
categories: jekyll update
permalink: dspCN2018.html
---

Ross Kaplan(EE '18), Anusrhree Sreedhar(chemE '18) and Yvette Wang(EE '19), worked on a dataset provided to us by [Charity Navigator](https://www.charitynavigator.org/). Charity Navigator is a non-profit that ranks charities, so that people can make informed donations to them.

As part of a new program they are developing, Charity Navigator has been asking charities to fill out a survey answering the following questions:

* What is the organization aiming to accomplish?
* What are the organization key strategies to make this happen?
* What are the organization’s capabilities for doing this?
* How will they know if they are making progress?
* What have and haven’t they accomplished so far?

The goal of the student team was to analyze this dataset and provide Charity Navigator with some new insights about how charities talk about themselves. This gives insight as to how charities want themselves to be viewed by the outside world. Furthermore, by grouping charities together based on how they speak about themselves, in contrast to hand-sorting, it might lead to a new method of categorization. In the long term, this new categorization method could help build a system to recommend similar charities. 

The team analyzed this dataset using a technique called Latent Dirichlet Allocation[(LDA)](https://en.wikipedia.org/wiki/Latent_Dirichlet_allocation), which is a method for organizing large corpora of documents. LDA postualtes that a document is made up of a mixture of hidden, or latent, topics. When presented with a large corpora of data, LDA can learn the underlying topics that exist in the dataset, and additionally indicate a percentage of how much each topic contributes to a particular document.

Much more details about this are presented in their [final report]({{ site.url }}/~keene/assets/Charity_Navigator_Final_Paper.pdf). For an interactive data visualization that shows the document clustering, have a look [here](https://yucy96.github.io/Charity_Navi/).

