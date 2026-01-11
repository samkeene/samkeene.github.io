---
layout: post
title:  "Data Science Projects for Social Good, Spring 2018, Eviction Prevention"
date:   2016-6-3 03:32:51 -0500
categories: jekyll update
permalink: dspEvic2018.html
---

Dash Chrisner (Arch '18), Mary Dwyer(mechE '19), Eva Gabrielson (Art '19), Nicole Lindner (Art '20) worked with the [Coalition for the Homeless](http://www.coalitionforthehomeless.org), to analyze a dataset on an eviction prevention program. This program provides people who are on the verge of eviction with a one time grant of up to $1000. 

The student team examined two things related to this dataset. First, they tried to build a predictive model and determine if there were any major predictors such as age, race, gender, etc... that influenced whether or not someone would receive the grant. They found that the biggest predictors were the amount of money owed, and the neighborhood the person at risk of eviction lived in. The fact that no other demographic information had a large influence on the prediction indicated that there appears to be little to no bias in the Coalition for the Homeless selection of grant awardees.

The other aspect examined was to overlay the locations of grant awardees with a dataset of [bad landlords](https://advocate.nyc.gov/landlord-watchlist/worst-landlords), as provided by the NYC public advocate. By comparign these locations, there are some obvious areas of overlap as would be expected. Neighborhoods with many 'bad landlords' in general seem to have a higher amount of people at risk of eviction. However, there were some neighborhoods, with a high amount of 'bad landlords', that currently do not have a high amount of evictions. Further investigation will study what is different about these neighborhoods, and perhaps an intervention strategy can be developed to prevent future evictions in those areas.

See the gallery below for some of their visualizations, and pdf versions of the maps are [here]({{ site.url }}/assets/DC_CFH_AmountCases_01.pdf) and [here]({{ site.url }}/assets/DC_CFH_LandlordFollowup_02.pdf). To read more details, have a look at their [final report](https://docs.google.com/document/d/1wKUZoMTeDdwQj50NUd_zV2UrE_ZsMljG6Fpsd1-L-jw/edit?usp=sharing)

## Gallery

<link rel="stylesheet" href="/assets/css/colorbox.css" />
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
<script>window.jQuery || document.write('<script src="_/js/libs/jquery-1.9.1.min.js"><\/script>')</script>



<center>
    <div class="photoset-grid-lightbox" data-layout="21">
        <img src="/images/dataSci/Eva_DWM_36x24_RGB1024_1.jpg">
        <img src="/images/dataSci/DC_CFH_AmountCases_01.jpg">
        <img src="/images/dataSci/DC_CFH_LandlordFollowup_02.jpg">       
    </div>
</center>



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
