---
layout: single
title:  "Projections"
date:   2017-6-3 03:32:51 -0500
categories: jekyll update
header:
  teaser: "/images/stairs.jpg"

---



This semester, I advised a collaborative project between an electrical engineering student (Jessica Marshall)  and an art student (Emily Adamo). The goal of this project was to get an engineer and an artist talking about algorithms and data, and how they are applied and interpreted. 

We quickly focused on a unique dataset that we had at Cooper  - the results from alumni survey. Of the most interest to us was the free form text answers to the question:

 "From the perspective you have gained since graduation, what do you especially value about your undergraduate experience at this institution?"

We had nearly 20 pages, and dozens of individual responses to this question, and we decided to apply a machine learning method, Latent Dirichlet Allocation(LDA), to this data. LDA is a method that attempts to learn and group topics from free form text like this.

Applying LDA to this data produced clusters of topics that echoed the typical buzzwords we've all grown to hear about Cooper, "Rigor", "Free", "Critical Thinking"  etc...

So, LDA told us what we already knew, but this is where the collaboration gets interesting. As Jess and Emily discussed how the algorithm works, and how to interpret and communicate the results, Emily questioned a basic assumption of how the LDA algorithm works. She questioned something that I, as an engineer, wouldn?t have given a second thought to.

One of the first steps in preparing data for LDA is to give the algorithm a set of stop words. This list of stop words instructs the algorithm to ignore certain words, words like "the", "of" , "to", etc... These words while frequent in text, do not necessarily contribute to any underlying topics or meaning.

Emily postulated: What would happen if we remove all the buzzwords about Cooper that we have come to accept? What would the algorithm tell us is left? So, they added all the buzzwords to the stop word list, and re-ran LDA. Naturally, the resulting topics were quite different, and were more about relationships and experiences.

Finally, they wanted some way to visualize these results. This was another moment where I really came to appreciate the value of this collaboration. As an engineering professor, I would have expected an accepted a report with some sort of charts and graphs and been very happy. That is not at all what they chose to do. Instead, they associated the resulting topics with images and locations around Cooper, and made a series of projection drawings all over campus, as well as a [map]({{ site.url }}/images/map.pdf) so people can explore the work.


<link rel="stylesheet" href="/assets/css/colorbox.css" />
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
<script>window.jQuery || document.write('<script src="_/js/libs/jquery-1.9.1.min.js"><\/script>')</script>


## Mapping values to projections in the spatial domain via the application of Latent Dirichlet Allocation to text data from the time domain"


<center>
    <div class="photoset-grid-lightbox" data-layout="213">
        <img src="/images/stairs.jpg">
        <img src="/images/clock.jpg">
        <img src="/images/clock2.jpg">
        <img src="/images/lincoln.jpg">
        <img src="/images/deal.jpg">
        <img src="/images/elevator.jpg">
    </div>
</center>

<script src="/assets/js/jquery.photoset-grid.js"></script>


<script src="/assets/js/jquery.photoset-grid.js"></script>

<script src="/assets/js/jquery.colorbox.js"></script>

<script type="text/javascript">
$('.photoset-grid-lightbox').photosetGrid({
  highresLinks: true,
  rel: 'withhearts-gallery',
  gutter: '5px',

  onComplete: function(){
    $('.photoset-grid-lightbox').attr('style', '');
    $('.photoset-grid-lightbox a').colorbox({
      photo: true,
      scalePhotos: true,
      maxHeight:'90%',
      maxWidth:'90%'
    });
  }
});
</script>



<!--
<script type="text/javascript">
    $('.photoset-grid-custom').photosetGrid({
    // Set the gutter between columns and rows
    gutter: '5px',
  
    // Wrap the images in links
    highresLinks: true,
  
    // Asign a common rel attribute
    rel: 'print-gallery',

    onInit: function(){},
    
    onComplete: function(){
        // Show the grid after it renders
        $('.photoset-grid-custom').attr('style', '');
    }
});
</script>
-->
