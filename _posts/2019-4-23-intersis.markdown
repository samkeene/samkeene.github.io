---
layout: single
title:  "Interstice"
date:   2019-4-23 03:32:51 -0500
categories: jekyll update
header:
  teaser: "/images/intersis/P1022285.jpg"
---

Graduating art student Aden Bailey held her senior show, Interstice, on April 23rd. As part of this show, Aden curated many pieces that students have done in a couple of my interdisciplinary courses this year. Below are some pieces from the [Data Science and Design Projects for Social Good]({{site.url}}/images/intersis/Syllabus_DataScience&DesignForSocialGood_2019.pdf) course, (co-intructor [Taylor Woods](https://www.taylorwoods.me/)), and the [Generative Machine Learning for Architecture](https://docs.google.com/document/d/1aRgETbX_IjhJSH7hlOZwHqhf1osZfUHpRg391f7JBbQ/edit?usp=sharing) course (co-instructor [Ben Aranda](http://arandalasch.com/work/featured/)). 


## **Center for Employment Opportunities**

This piece formed the centerpiece of the show, as it covered nearly 1/3 of the gallery. The work was inspired by a dataset shared with us by the Center for Employment Opportunties. At its core, the work is a flowchart, that walks the viewer through the challenges one experiences while reintegrating into society after being incarcerated. The layout of this forces the viewer into uncomfortable, difficult positions, where they must squat, or strain in order to navigate the various obstacles.

<link rel="stylesheet" href="/assets/css/colorbox.css" />
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
<script>window.jQuery || document.write('<script src="_/js/libs/jquery-1.9.1.min.js"><\/script>')</script>



<center>
    <div class="photoset-grid-lightbox" data-layout="122">
        <img src="/images/intersis/P1022285.jpg">
        <img src="/images/intersis/P1022341.jpg">
        <img src="/images/intersis/P1022359.jpg">
        <img src="/images/intersis/P1022360.jpg">
        <img src="/images/intersis/P1022567.jpg">
    </div>
</center>
Students: Aden Bailey, Ariana Freitag, Sophie Schneider




## **Olmsted Park Generation**
This group digitized numerous drawings of parks by Frederick Olmsted, such as Central Park and Prospect Park. The groups goal was to apply generative machine learning algorithms in an attempt to recreate Olmsted's design style. They did this by using an evolutionary algorithm to optimize a heuristic mathematical function that attempts to capture some of the style aspects. For more details, see their [report](https://docs.google.com/document/d/1XVQzZ1pOgOMI7aYa6F5_ZzZmAa659TTZ-2bX1cxbWok/edit?usp=sharing), or their [Github](https://github.com/jbentivegna15/ML-ARCH). Some images of the results are below.


<link rel="stylesheet" href="/assets/css/colorbox.css" />
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
<script>window.jQuery || document.write('<script src="_/js/libs/jquery-1.9.1.min.js"><\/script>')</script>



<center>
    <div class="photoset-grid-lightbox" data-layout="12">
        <img src="/images/intersis/olmsted1.jpg">
        <img src="/images/intersis/olmsted5.jpg">
        <img src="/images/intersis/olmsted7.jpg">
   </div>
</center>
Students: Joseph Bentivegna, Frank Zhang, Jacob Maarek, Danny Smith


## **AnimAIte**

This group chose to build a tool that would animate simple motion graphic GIFs using generative machine learning. The student scraped the GIPHY website for motion graphic GIFs to create their training set, and used a generative machine learning image interpolation algorithm to create the motion graphics from two images provided by the user. The first image serves as the starting point, and the second as the endpoint. Below are examples of the results. For more details, see the [booklet]({{site.url}}/images/intersis/Animaite Booklet.pdf) the made to accompany this work.


<iframe width="560" height="315" src="https://www.youtube.com/embed/p4KngbVx5xY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
Students: Isaac Alboucai, Dylan Dewald, Dongkyu Kim, Tandis Shoushtary, Yvette Wang, Will Chen

## **eMotion**

This project creates a visual representation of Twitter emotional sentiments depicted in a physical environment– demonstrating the effect of a crowd from an online sphere into a public space.

After gathering Twitter sentiment analysis/topic modeling data, they created a  digital animation; its motion is determined based on factors including the amount of tweets written at any given time, the type of emotional sentiment the tweet demonstrates (categorized by joy, anger, and fear), and the intensity of that emotion. In this video, walking speed is the main distinguisher within the crowd: fear is represented as the fastest walking speed, joy as intermediate, and anger as static.

They then used Pix2Pix to transform the Processing animation into a more photorealistic video using the Cityscape dataset— translating the flat colors into people walking through a public square, evolving based off the real-time Twitter data. The resulting video is below.

<iframe width="560" height="315" src="https://www.youtube.com/embed/WUzPt4-TfSE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
Students: Anna Burholt, Liao Hu, Zhekai Jin, Natain Yan, Camille Chow

## **Object Creation**

This group was inspired by The Design of Everyday Things by Donald Norman, a book that discusses how design serves as the communication mechanism between an object and its user. They sought out to explore the space of everyday, utilitarian objects, such as lamps, forks and tea kettles. We were interested in what a computer would consider such an object to look like, what purpose they might serve, and how useful they would actually end up being.

To this, they scraped a dataset of objects from [Bloomingdales](https://www.bloomingdales.com), because of the wide range of objects, the high quality images, and the fact that the objects were uniformly photographed against a white background. They used a [progressive GAN](https://arxiv.org/abs/1710.10196) approach in an attempt to generate new images of everyday objects. Unfortunately, they were unable to get the training to converge in time for this show. However they did produce a compelling video that illustrates the outputs of the GAN as it trains. Work on this project is ongoing, and the code is availble on [GitHub](https://github.com/ostapstephan/MachineLearningAndArchitecture).

<iframe width="560" height="315" src="https://www.youtube.com/embed/Dx34MqIsrP0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
Students: Ostap Voynarovskiy, Shifra Abittan, Stephen Brett, Aden Bailey

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



