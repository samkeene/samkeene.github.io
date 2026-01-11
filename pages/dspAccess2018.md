---
layout: post
title:  "Data Science Projects for Social Good, Spring 2018, Access to Services"
date:   2016-6-3 03:32:51 -0500
categories: jekyll update
permalink: dspAccess2018.html
---

Joseph Bentivegna(EE '19), Yonatan Katzelnik(Art '19), Jeremiah Pratt(EE '19) and Zhenia Dementyeva(Arch '20) worked on a dataset provided to us by [SingleStop](http://singlestopusa.org/). SingleStop is an organization dedicated to providing coordinated access to the safety net and connect people with the resources they need to attain higher education, obtain good jobs, and achieve financial self-sufficiency. They do this through a unique, one-stop-shop, where they meet with people indivdually to guide them through the process of applying for aid.

SingleStop provided us with a dataset about the applicants to their program, and our student group investigated several questions:

* Are there certain characteristics that make a particular applicant a better candidate to receive government aid?
* How long do it take to receive government aid? Does this vary by program?
* Which New York City neighborhoods are most in need of government aid? Are different boroughs in need of different kinds of aid?
* What kinds of  benefits are most likely to be received together?
* Is it possible to qualify the amount of time an applicant must wait for their aid?

The answers to these questions are found in their [final report](https://docs.google.com/document/d/1U-1GBPGm_MpWBM52V-1ltm4H6nQOaqYkdYxuvITZM_4/edit?usp=sharing). Some of their visualizations are shown in the gallery below. The team also created an [interactive visualization](https://public.tableau.com/views/SSviz3/CountofHouseholds?:embed=y&:display_count=yes) in Tableau.


## Gallery

<link rel="stylesheet" href="/assets/css/colorbox.css" />
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
<script>window.jQuery || document.write('<script src="_/js/libs/jquery-1.9.1.min.js"><\/script>')</script>




<center>
    <div class="photoset-grid-lightbox" data-layout="22">
        <img src="/images/dataSci/Zhenia_24x2480x80_RGB_031024_1.jpg">
        <img src="/images/dataSci/Zhenia_24x2480x80_RGB_031024_2.jpg">
               <img src="/images/dataSci/Zhenia_24x2480x80_RGB_031024_3.jpg">
        <img src="/images/dataSci/Zhenia_24x2480x80_RGB_031024_4.jpg">
 
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

