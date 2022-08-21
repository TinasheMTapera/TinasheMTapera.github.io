---
title: 'EncourageMe: A Shiny App for Encouragement'
author: Tinashe M. Tapera
date: '2018-09-22'
slug: encourageme-a-shiny-app-for-encouragements
categories:
  - R
  - data science
  - psychology
  - RShiny
  - web programming
tags: []
# comments: no
showcomments: yes
showpagemeta: yes
---

During my time at Drexel, I volunteered on the University's <a href=https://drexel.edu/counselingandhealth/counseling-center/peer-counseling/>Peer Counseling Helpline</a>. Being a peer counselor teaches you a multitude of important conversational and relational skills in what's called <i>active listening</i>, and one of the most effective ones is <i>encouragement</i>. As you can guess, an encouragement in active listening involves conveying to the caller that their efforts, whatever they may be, are not in vain. Used appropriately, it can be a powerful tool for helping callers process their problems.

Ironically, I only learned exactly how effective they could be when someone was kind enough to use them with me. Earlier this year, a close friend^[This "friend" is now my wife. Go figure!] went through the trouble of handwriting a bunch of encouragements for me when I was struggling to keep up with thesis work, research, classes, depression/anxiety, job search, and everything else that was happening in life at the time. After pulling myself out of that difficult period, I decided to return the favour by building an RShiny app that she (or anybody else) could use if they ever needed some encouragement. 

The app is hosted by R Studio at <a href=https://tinashemtapera.shinyapps.io/encouragemeshiny/>shinyapps.io</a>, but I've embedded it below:


<script type="text/javascript" src="iframeResizer.min.js"></script>
<style>
  iframe {
    min-width: 100%;
  }
</style>
<iframe id="myIframe" src="https://tinashemtapera.shinyapps.io/encouragemeshiny" scrolling="yes" frameborder="no" height=500px></iframe>
<script>
  iFrameResize({
    heightCalculationMethod: 'taggedElement'
  });
</script>

### Tech Specs

The app itself is very simple: on launch, it reads in a file of quotes I hand picked, and simply samples one every time you hit the action button. 

Web programming with RShiny gets more and more intersting every time you do it. I highly recommend it to anybody who has experience with R and wants to grow. RShiny allows you to write all of your basic application/dashboard functionality in R, and then when you want to spice it up, you can get your hands dirty (slowly) with HTML and CSS pretty seamlessly. In this app, I made aesthetic modifications (like the fonts and footer), but with web programming your only limitations are your imagination, and determination to make it work! You can examine the code on <a href=https://github.com/TinasheMTapera/EncourageMeShiny>Github</a>.