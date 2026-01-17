---
layout: single
title:  "Exploring causal effects of ad campaigns during the Superbowl"
date:   2017-4-21 03:32:51 -0500
categories: jekyll update
header:
  teaser: "/images/googleresults.png"
---






One of my graduate students, Neema Aggarwal, focused her graduate thesis on an important area of research, causal inference. Neema right now is working as a consultant for the Boston Consulting Group, so we wanted to find her a thesis topic that was relevant to buisness work, but also an electrical engineering topic. Causal inference, with its roots in machine learning, was a perfect fit. 

Neema's thesis is also great example of the ingenuity of Cooper Union students. Business applications of causal inference typically focus on trying to determine whether or not a marketing campaign has an effect on sales of a product. We had a problem - no data to experiment with, as companies in general are not going to share that data. We needed two things, the obvious start of a marketing campaign, and some response variable to collect from publcally available sources to serve as a surrogate for sales data. 

The Super Bowl presented us with an opportunity, as many organizations launch marketing campaigns during this time, and it is public knowledge which ones will do so. This gave us multiple campaigns to study simultaneously. The final piece was to select data as a response variable. Instead of sales figures, we instead chose to study what we called "Digital Buzz", which we defined as the number of Google searches and Twitter mentions for the product in question. So, now we had numerous, simultaneous campaigns to study, a response variable, and some clear questions to ask:
    
- Which companies marketing campaigns caused a substantial increase in digital buzz?
- How long does this digital buzz last?
    

There was only one small problem left - Google and Twitters APIs did not allow collection of data too far in the past, meaning the data had to be collected live, especially during SuperBowl LI. Complicating matters, Neema is a Patriots fan, and her team was down 28-3 early in the 3rd quarter. As her team mounted a heroic comeback from the largest deficit in SuperBowl history, Neema mounted her own heroic data collection effort, running her scripts and collecting all the data she needed for her thesis.


The causal impact model works by tracking time series data (for example, # of hourly google searches), both before and after the event (for example the start of a marketing campaign). In order to develop a control, the model needs other, untreated markets to compare agaist. By using the time series data of both the treated and untreated markets, we can attempt to infer the causal impact. If there is a significant diverence in the response (the # of google seaches) in the treated market, then we can infer that the treatment (the marketing campaign), caused the response.

The above description is a gross over simplification, and the model Neema used is a full Bayesian treatment of this topic, and for more detail, refer to Neema's [thesis.]({{ site.url }}/assets/Neema_Thesis_vFinal.pdf)

Now, for the results, which marketing campaigns resulted in significant buzz, and which fell flat?



![google]({{ site.url }}/images/googleresults.png)

![twitter]({{ site.url }}/images/twitterresults.png)

84 lumber appears to have hit a home run with their marketing campaign. The ad depicts a mother and daughters migrant journey towards becoming legal american citizens.

<iframe width="640" height="360" src="https://www.youtube.com/embed/nPo2B-vjZ28" frameborder="0" allowfullscreen></iframe>

84 lumber's ad is quite a depature from the a more typical Superbowl ad, such as the one Avacodos from Mexico did quite well with:

<iframe width="640" height="360" src="https://www.youtube.com/embed/VneoEvAJX0g" frameborder="0" allowfullscreen></iframe>

Meanwhile Bai's ad, featuring high powered celebreties Christopher Walken and Justin Timberlake, fell decidedly flat:

<iframe width="560" height="315" src="https://www.youtube.com/embed/z-TXRa6qd7c" frameborder="0" allowfullscreen></iframe>

Another interesting aspect of the Bayesian treatment, is that it the model also determines which control markets are correlated with the market under investigation. This led to some interesting results

![budlight]({{ site.url }}/images/budlightcontrols.png)

Shock Top and Blue Moon appear to be strong controls for Bud Light, which makes sense, but why would Twix and Pringles be more relevant than Corona?

![skittles]({{ site.url }}/images/skittlessnickerscontrols.png)

Two candies have strong controls with other candies and junk foods, yet seemingly "healthy" options such as Dasani and Smart Water, also show up as strong controls for these markets.

The method Neema explored for her thesis was a lot of fun to play with. There are applications to all sort of domains, and plenty of questions left to answer.




