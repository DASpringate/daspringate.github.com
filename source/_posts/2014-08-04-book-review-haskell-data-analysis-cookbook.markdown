---
layout: post
title: "Book Review: Haskell Data Analysis Cookbook"
date: 2014-08-04 13:45:29 +0100
comments: true
categories: [Haskell, Reviews, data science, Functional Programming] 
---

[Haskell Data Analysis Cookbook by Nishant Shukla](http://www.packtpub.com/haskell-data-analysis-cookbook/book)

[Full disclosure - I was given a free review copy of the book from the publisher. This review refers to the ebook version]

Data scientists are spoiled for choice with languages for statistics and data analysis these days.  There is the tried and battle-tested but sometimes plodding workhorse &#40;R), the popular general purpose language with a bunch of fairly new tools (Python), the expensive, closed-source old guard (SAS, Matlab, Stata), C++ for lightning fast calculations but slooow development time, a modern day Lisp with great Java interaction (Clojure) and a new Lisp/Python/R hybrid that is looking to steal Matlab's crown for numerical computation (Julia).  This book sees the purely functional, strongly typed language Haskell throw its hat in the data science ring.

This is a great book for data scientists wanting to leverage the power of functional programming in data analysis applications.  There are chapters on data cleaning, text scraping, hashing, tree traversal, social network analysis, basic stats and machine learning algorithms, mapReduce and visualisation.  It is also good for more general purpose beginner and intermediate level Haskell hackers, since it covers a lot of areas that can be essential in day-to-day programming such as reading and writing data from and to a variety of sources (including databases and the web), text processing, parallel programming and dealing with real time data.  Often in books on haskell (as in many books on Lisp) much space is given to show off the cool FP aspects of the language but you are left struggling with doing the practical IO tasks that are no-brainers in more traditional languages.

The book covers a wide range of subjects, but it provides only a primer for most of them to get you started.  In most cases this is enough, but there are a couple of areas I would have liked to have seen greater depth, for example in the statistics section, a more comprehensive introduction to linear modelling and regression would have been more convincing to R and Python users as to the advantages of switching to Haskell.  I would also have liked to have seen a treatment of random number generation and simulation; the purely functional nature of Haskell seems to make it difficult to generate simple random sequences because you need to set the seed for each run in order to maintain referential transparency (i.e. a function in Haskell generally needs to return the same value for the same input every time).

The examples are well written and well explained and there is a Github page with the source code from all the chapters if you don't want to type out every one from scratch.  Another nice touch is the list of list of data sources and APIs for doing your own analyses with.  I'm sure you could find them with a little Googling but it was good to have them all in one place and there were several I was not aware of.

It must be said that this is not an 'introduction to Haskell' book.  There is plenty of assumed knowledge and the syntax is hardly discussed at all.  However, I would highly recommend anyone starting off with Haskell to get this book alongside an introductory book such as the fantastic "Learn you a Haskell for Great Good" to get to grips with the mind-bending complexity of the pure FP paradigm alongside the practical real-world applications.

The quality of the book aside, after reading the book I am yet to be convinced that Haskell is a great language for data science.  The static typing and functional purity would be good for building large scale data-centric systems requiring rigorous validation but in my experience, most analytics coding involves lots of rapid prototyping, on-the-fly testing and hacking away at the REPL. It is this style of programming that Python, R and Lisp-based languages excel at - incrementally growing your codebase to deal with swiftly changing data and conditions.  Haskell seems slightly too rigid to be a comfortable fit; having to think too much about types early on slows down early development (although it could well pay off later on) and the strictness of its functional programming can feel pretty unforgiving. Also the ghci interactive environment just doesn't feel as natural as a Lisp or R REPL. Finally, Haskell seems to be missing other important features such as an equivalent to R's data.frame (which is available in Python, Clojure and Julia) and good interoperability with other systems (such as Weka, R and Hadoop). 

    
