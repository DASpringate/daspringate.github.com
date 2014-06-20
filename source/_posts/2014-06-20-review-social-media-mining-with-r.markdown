---
layout: post
title: "Book review: Social Media Mining with R"
date: 2014-06-20 21:40:37 +0100
comments: true
categories: [rstats, Reviews, data science]
---

[Social Media Mining with R by Nathan Danneman and Richard Heimann](http://www.packtpub.com/social-media-mining-with-r/book)

[Full disclosure - I was given a free review copy of the book from the publisher. This review refers to the ebook version]

I worry when a book proposes that it will appeal to everyone.  The trouble is that it could well end up appealing to no-one. The introduction to this new book on social media mining in R says that it will be suitable for skilled programmers with little social science background, people who lack any sort of programming background, people wanting an introduction to social data mining and advanced social science researchers. That doesn't leave many people out!

It turns out that this book doesn't really cover much social media mining.  It does cover basic sentiment analysis and text-mining with some references to twitter data but other social media platforms are barely mentioned and there is no discussion of any of the other social media APIs (e.g. Facebook, Linkedin and Github).  The authors also miss an opportunity to discuss other analysis techniques such as social network analysis and network graphs, which twitter (and other social media) data would be ideal for.

In the first third of the book, much mention is made of big data and how researchers are going to have to prepare for it, but the actual content for dealing with big data (or at least data that would struggle to fit in the RAM of an average laptop) amounts to little more than "check that you have enough memory to read in your data and read the manual for the `read.table` function". R has a reputation for not coping well with large datasets but there are some packages that really assist with this (like `fread`, `data.table`, `sqldf` and `dplyr`) that could easily have been discussed, along with any number of tips for speeding up I/O using base R functions.

The introductory and background material and theory is interesting and provides a good high level introduction to sentiment analysis, though it still feels somewhat rushed (for example, why completely leave out semi-supervised approaches?  It would have been nice to have at least a page or two describing what they are and why they might be useful) and there is little detail on the assumptions of the different models. The introduction would make a good springboard for deeper research however, and the further reading and bibliography sections are very good.

I like there to be code on nearly every page of a programming book but this one is very light on R code examples. There is a chapter on setting up R and installing packages (This is not going to be anyone's first R book so this chapter feels like a waste, particularly in a book that only clocks in at 120 pages), another covering getting tweets via the `twitteR` package (but not the streaming API for collecting tweets over a prolonged period of time or any way of storing tweets in a database) and then nothing until two thirds of the way through where there are three short case studies of different methods of sentiment analysis.  It also seems strange to separate out the theory in the earlier chapters and the practical applications later on. 

The case studies are mostly decent, covering lexicon-based, naive Bayes and the authors' own unsupervised _Item Response Theory_ sentiment analysis methods.  It seems strange to me in a book on social media mining that the first example doesn't even use social media data, but US government reports which even the authors admit bears little resemblance to twitter data. Some of the code is poorly explained (or not explained at all), idiosyncratic (there may be reasons for using `scan` to read in a text file, but what are they?) and makes use of out of date packages (Hadley Wickham shipped `reshape2` back in 2012, why still use `reshape`?).  The authors miss several opportunities to flesh out the book: One minute they say how important data cleaning is and how useful regular expressions are and then they just point you in the direction of a website teaching regular expressions.  The same is true for the plotting package ggplot2 (Is Wilkinson's _The Grammar of Graphics_ really an appropriate introductory text for this package?) and the `rWeka` machine learning package.  A lot of the information is good (in particular the description of the `tm` text-mining package functions) but it all feels a little lightweight, like a collection of blog posts.  The case study analyses were interesting, though choosing such obviously polarised subjects as abortion and Obamacare resulted in much neater, cleaner results than would have been found had subjects been used where opinions are less black-and-white.

Sentiment analysis seems to be everywhere at the moment.  It reminds me of word clouds a few years ago:  Everyone starting out in data science was using them but they soon became a little embarrassing as they became more ubiquitous and were even famously described as the "[mullets of the internet](http://www.zeldman.com/daily/0405d.shtml)". Make of it what you will that word clouds are used several times as an analysis method in this book. 

Users who have maybe done a Coursera data science course or two and want to try their hand at some simple analyses to boost their portfolio will probably find this book useful but more serious users are likely to be left disappointed.  

