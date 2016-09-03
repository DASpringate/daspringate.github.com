---
layout: post
title: "What I am Looking for in a New Data Science Hire"
date: 2016-09-03 21:39:47 +0100
comments: true
categories: [R, Python, data science, Recruitment] 
---


This is my first post for a very long time.  At least part of this tardiness has been because I have been getting to grips with my new role as senior data scientist for [RealityMine](http://www.realitymine.com), my first data science position outside of academia. I started in November 2015 and am now in a second round of recruitment. There are any number of articles online about 'how to get your first job as a data scientist' or 'What skills a data scientist needs', but for me, many of them feel more like a wish list for the perfect data science degree course, rather than advice for getting a new job - they are too general and, frankly, are often written by people looking for work as a data scientist rather than someone trying to build up a team. In this post I hope to give a flavour of the kinds of skills and values that I specifically am looking for when I look at CVs and conduct interviews at RealityMine. Clearly different companies have different requirements and others may well disagree with me on which are the most important facets, but I wanted to give an insight into what someone on the other side of the recruitment fence values in potential new hires.

## I am looking for:

### Good conceptual knowledge of maths, statistics and machine learning

I am not necessarily looking for someone who does Gaussian elimination or eigenvalue decomposition by hand for fun, but I would need them to understand the relationships between rows and columns in matrices and be able to relate them to data and models, and to understand what a PCA is doing, what it might tell us and the impacts on further analysis.  I will always ask around these subjects in an interview, partly to assess for a minimum conceptual understanding of statistics but also to assess the ability to communicate complex ideas to people who may not be an expert in the domain. A complete algebraic understanding is far less important than knowing when to apply a logistic or a linear regression and how to interpret the output. I want people who know the difference between classification, regression, clustering, supervised, unsupervised, predictive modelling, dimension reduction etc. and be able to fairly instinctively know when to apply each, even if they are not sure exactly which model might be the best to apply within each of those groups. I am not necessarily particularly interested if you have coded your own gaussian process model from the bare metal up in C: this may well be impressive but I am looking for practical data scientists who are able to apply their knowledge under a wide range of problems, and if they don't know the answer, they at least have a pretty good idea of where to look for it. 

### Data processing and visualisation expertise

This is perhaps the only absolute essential thing I am looking for and is why 'pure' statisticians with experience only in SPSS, Stata or similar are really not likely to cut it.  I need people who are _data manipulation cyborgs_, for whom  filtering, subsetting, merging and transforming data is second nature and can do it using their preferred tool (be it `dplyr`, `Pandas`, `SQL` or whatever) with _flow_, without being hindered by those tools.  Think of the difference between a new driver, who has to think consciously about every single decision (signal, gears, brakes, accelerator, mirrors etc.) and yet is still overloaded with information and someone who has been driving for years for whom many of these tasks are handled by muscle memory and the unconscious brain. Data manipulation is not the chore to get through to get to the proper data science - it _is_ data science. The same is true for visualisation. Exploring the data always comes before understanding it and visualising data is a hugely important part of this. Personally I spent a lot of time getting familiar enough with `ggplot2` to be able to crank out quality plots on demand but if you have another favourite that you work efficiently with, go for it.  Related to this is report building, my workflow has been drastically improved by learning to generate automated reports using tools like `Rmarkdown` and `Emacs org-mode`. If new hires have already spent the time getting to grips with these tools, they can get to grips with the data that much more quickly.

### Scientific method

This is critical.  Data scientists lack the specialist and deep software development knowledge of engineers but we are constantly testing hypotheses, experimenting and proving ourselves wrong in our quest for meaning in our data. [hypothetico-deductive](https://en.wikipedia.org/wiki/Hypothetico-deductive_model) thinking is the best method humans have devised for discovery and reasoning where the information we have is incomplete, and I think this is the main reason why many say that science PhDs (rather than Statistics, maths or CS graduates) make the best data scientists. This is drilled into us for at least three years until it becomes second nature. (Conversely none of the best engineers I have met have done a PhD - make of that what you will!).

### An interest in programming

I am looking for the polyglot data scientist, they may be a wizard at using R, but I need them to understand the circumstances under which it is better to use Python or SQL or bash and be open to diving in to use newer tools like Scala/Spark, if they have not already. I need them to not be constrained to the tools they know the best. A blog, twitter feed, StackExchange presence or GitHub account is a good place to show that you have an interest in the broader issues in data science. An interest in programming and computer science more generally is another big plus - someone who has spent a little time playing with a few other languages is likely to have a better feel for how their main languages perform under certain conditions. Having a grasp of the differences between functional and object orientated programming and their relative merits for data analysis and pipelines would be a definite benefit. Knowing their way around the linux command line, git and other command line tools is pretty much a prerequisite for hitting the ground running in the first few weeks.

### Domain knowledge

I work in a fairly disruptive company in an area I had little knowledge of before I joined.  Domain knowledge is often most usefully learned on the job, at least initially. So at least there should be an interest in the industry you are looking to work in. There is little you can do to prepare yourself for the idiosyncrasies of a new data warehouse, however, an understanding that it is essentially the same models you are using whether it is in ecology, health informatics, market research or political science automatically puts you in good stead to understanding the data science needs of a  business. From then on the main requirement is curiosity and a thirst for knowledge. I'd rather have an ex-ecologist who had split the last few years between cranking out models in R and digging in the dirt for beetles  than someone who had spent 10 years in my industry but who struggled with much more than pivot table in Excel and point-and-click models in SPSS.

### Miscellaneous traits

- Need to be comfortable with meetings and explaining complex concepts to people with little or no statistical or technical knowledge
- Willingness to learn and also to impart knowledge to other departments and areas in the company.  Data science should not exist in a silo: There is much to learn from BI, engineering, architecture and infrastructure and hopefully much to teach them too!
- I don't want someone who just wants to put their headphones on and code 8 hours a day.  There will be many opportunities to get stuck into some proper hacking but I also need the ability to collaborate, tell stories with the data and explain why they are using a particular technique


## In summary

So it is conceptual knowledge, technical virtuosity, critical scientific thinking, a love of learning, a gift for communication of complex ideas and a collaborative spirit I look for in a new data scientist hire. I don't much like breaking down data scientists into groups like 'modellers', 'visualisers' 'data wranglers' etc., data science is an ever-changing environment that selects for generalists and to limit yourself to a certain facet of the discipline is to potentially limit your own opportunities.

I'd be interested to hear your opinions. And, by the way, We are hiring!

