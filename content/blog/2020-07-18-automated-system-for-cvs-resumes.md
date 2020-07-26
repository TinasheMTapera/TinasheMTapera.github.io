---
title: Automated System for CVs & Résumés
author: Tinashe Tapera
date: '2020-07-18'
slug: automated-system-for-cvs-resumes
categories:
  - data science
  - automation
tags:
  - data science
  - latex
  - dplyr
  - R Markdown
  - json
  - automation
comments: no
showcomments: yes
showpagemeta: yes
---

# An Automated System for CVs & Resumes

I ***hate*** applying for things.

There's just something about the process of trying to convince someone that you are worth their time that gives me serious anxiety and distress. Part of the reason for that is because you need to make sure you have up-to-date documents like CVs and résumés, which you always imagine will only take a couple of minutes, right? *I only need to add this one poster reference, oh and also just change a line in my bio to reflect my current goals. No problem!*

And then, you open up the dreaded ***Microsoft Word***, slightly adjust the table to add a little bullet point to it and...🚨🔥💥🔥🚨 SUDDENLY THE ENTIRE DOCUMENT IS IN SHAMBLES!!! Tables crossing pages, headers halfway down the page, bullets tabbed to oblivion...

I'd do anything to avoid creating documents with WYSIWYG word processors (see: [Word Processors: Stupid and Inefficient](http://ricardo.ecn.wfu.edu/~cottrell/wp.html)), and so I typically turn to plain text that can be created with text editors, and that can be converted to fancier outputs using programs. Markdown, Latex, RMarkdown ([which I use to build this site](https://bookdown.org/yihui/blogdown/)) -- if it can be version controlled and automated, I'm all about it. And I believe as a data scientist there's no reason to not bring this attitude to the creation of application materials. So I did some digging...

# Creating a Résumé with Code

It turns out, there's a couple of options for creating a resume or CV with plain text and code. Most methods simply abstract a simple workflow:

1. Create a text file with markup for basic styling (like `markdown` or `Latex`)
2. Create an optional template for formatting and additional styling (with a language like `css`)
3. Convert (render) the basic file to a fancy file (with something like `pandoc`) to give you a PDF, HTML, or other file

There are a couple of options for exactly what system will accomplish this, but today I will focus on what worked best for me.

## Source Data

It's important that the source data can be version controlled and easily added to and edited in a text editor. For this, I decided to use 