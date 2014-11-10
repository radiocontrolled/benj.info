---
layout: post
title:  "Adding keyboard accessibility to JuxtaposeJS"
date:   2014-11-05 14:33:56

---
<a href="http://juxtapose.knightlab.com/">JuxtaposeJS</a> is a tool for creating before/after image sliders. 
Supported by KnightLab and created by <a href="https://twitter.com/asduner">Alex Duner</a>, 
this project allows a user to create and embed this kind of interaction on a site. Alex wrote about his process for creating the 
project <a href="http://knightlab.northwestern.edu/2014/09/29/lessons-building-juxtaposejs/">here</a>. 

Last month I made a keyboard accessibility pull request to the project. The <a href="https://github.com/radiocontrolled/juxtapose">main thing my contribution did</a> was to apply the role of <code>slider</code> to 
the slider rails that allow the user to overlay the before/after image. I also added aria roles (<code>aria-valuenow</code>, <code>aria-valuemin</code>, <code>aria-valuemax</code>) to the slider rail
and provided :focus styling. 

If you use your keyboard to navigate through Juxtapose, you'll see the result: 

<div class="juxtapose" data-startingposition="50" data-showlabels="true" data-showcredits="true" data-animate="true">
<img src="http://juxtapose.knightlab.com/static/img/Sochi_11April2005.jpg" data-label="Apr. 2005" data-credit="">
<img src="http://juxtapose.knightlab.com/static/img/Sochi_22Nov2013.jpg" data-label="Nov. 2013" data-credit="">
</div>
<br/><br/>
<link rel="stylesheet" href="//s3.amazonaws.com/cdn.knightlab.com/libs/juxtapose/latest/css/juxtapose.css"><script type="text/javascript" src="//s3.amazonaws.com/cdn.knightlab.com/libs/juxtapose/latest/js/juxtapose.js"></script>
