---
layout: post
title:  "Test Page"
permalink: testpage.html
---



<script src="//ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
<script>window.jQuery || document.write('<script src="_/js/libs/jquery-1.9.1.min.js"><\/script>')</script>

Testing a page. Where does this page live?


[Support Cooper](https://secure.cooper.edu/s/1289/support/interior-hybrid.aspx?sid=1289&gid=1&pgid=1599),

<center>
    <div class="photoset-grid-custom" data-layout="213">
        <img src="/~keene/images/stairs.jpg">
        <img src="/~keene/images/clock.jpg">
        <img src="/~keene/images/clock2.jpg">
        <img src="/~keene/images/lincoln.jpg">
        <img src="/~keene/images/deal.jpg">
        <img src="/~keene/images/elevator.jpg">
    </div>
</center>

<script src="/~keene/assets/js/jquery.photoset-grid.js"></script>

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

