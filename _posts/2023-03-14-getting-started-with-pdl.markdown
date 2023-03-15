---
layout: post
title:  "Getting Started With Practical Deep Learning for Coders"
date:   2023-03-14 19:31:47 -07:00
categories: fastai
---
[Practical Deep Learning for Coders](https://course.fast.ai/) is a
terrific free course offered by fast.ai, but it doesn't 
exactly hold your hand. I'm an experienced C++ and Python 
coder, but I found myself puzzling over a few things at the start. 
Hopefully this helps you get going quickly! 

## Watch Lesson 0

I didn't see it linked from the course site, but I found it on YouTube,
and it contains all kinds of useful background:

<iframe width="560" height="315" src="https://www.youtube.com/embed/gGxe2mN3kAg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

[Practical Deep Learning for Coders Lesson 0](https://youtu.be/gGxe2mN3kAg)

## Notebooks

The course lectures make heavy use of Python *notebooks*, which are a cross between an IDE
and a lab notebook. They allow you to interactively iterate with your code,
and annotate it with text and graphics.

[Kaggle](http://kaggle.com), [Google Colab](https://colab.research.google.com/), 
and [Paperspace Gradient](https://www.paperspace.com/gradient) are hosted 
services that offer notebooks running on managed hardware hardware,
and are definitely the fastest and easiest way to get going with the course.
All three provide a free tier (some with GPUs), which may be all you need for the course, 
and the option to pay for enhanced
services like increased runtime quotas and more powerful GPUs. Each has a slightly different UI, 
CPU/GPU hardware, and pricing. 

![Paperspace + Fast.AI](/assets/gettingstarted/paperspace.png)
*Paperspace + Fast.AI runtime, with all the textbook chapters*

The recommendation as of this writing 
is to use [Paperspace Gradient](https://www.paperspace.com/gradient), 
which has a fast.ai 'runtime' that's preloaded with 
the course textbook's chapters in notebook form, as well as convenient persistent 
storage for data files and the like.

# Do I have to use a notebook?

No! If you prefer, you can develop and run fastai code in the IDE of your
choice, or use the command-line interpreter. In fact, in the second lesson you're
going to be creating a standalone Python program from your notebook for deployment, 
so some familiarity with "standard" Python tooling will be handy.

If you don't own a supported GPU, hosted notebooks are
an easy way to get access to one, but for ultimate flexibility,
[configure an AWS instance](https://course20.fast.ai/start_aws)  
and run the tooling of your choice. 

One downside of using notebooks that's worth noting is that code cells can be 
executed in any order, so you might have issues with repeatability.

# Jupyter

The gold standard of notebooks is *Jupyter Notebooks*, an application which you can 
[install on your own computer](https://jupyter.org/install). You'll need a working 
Python environment,
and you'll have to manage dependencies and navigate the complexities of Python 
environment and package management
(pip? conda? mamba?). You interact with Juptyer via a browser, just like the
hosted services described above, but generally the server is localhost 
(port 8888 by default, i.e. http://localhost:8888). As mentioned above,
you can [use an AWS instance](https://course20.fast.ai/start_aws) to run
Jupyter if you don't have a supported GPU.


So why would you want to Jupyter? There are a few possibile reasons that I can think of:

* You have your own high-powered GPU that you want to take advantage of.
* You want to install Jupyter extensions such as nbdev for coding in a notebook, 
or fastpages for blogging. Jeremy discusses several extensions during the
lectures, but these don't apply to the hosted services AFAIK.
* You need more control over the environment, i.e. you use proprietary Python code
or data that can't be uploaded to hosted services.
* Other reasons I haven't thought of? Please comment below.

## Finish it!

Hopefully that helps you get started with this great free course. Be sure to share your 
own experiences to help others along the way.
