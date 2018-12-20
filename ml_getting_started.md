# ML prep
Here is my guide for anyone looking to transition into machine learning for academia.  I will recommend courses to check out as well as things to be aware before you should try to interview at a company. I'll give a little bit of background to set the stage. I am going to try my best to introduce for keywords and ideas before diving into specifics. Note, this mainly applies to PhDs in the hard sciences. I mention that because I am assuming the reader has a basic understanding of linear algebra, probability, and calculus.

## General plan of attack
Well, this of course is buyer beware. Everyone is different, yada yada yada. Here is roughly what Mike and Tom did. Our paths diverged, but so it should be nice to see different thoughts. I am going to assume you have some background in programming---you can write code pretty well in a certain language and are familiar with classes. If not, you may want to brush up on this, but I don't know what the best resource is.  Usually coding is the best way!

This may seem like a lot, but you'd be surprised how fun it is! I am recommending learning about deep learning. It's a powerful tool, [and](and) I believe any card caring data scientist (DS)/machine learning engineer (MLE) should know the methods at a high level, but more importantly, what kind of problem you can solve with these. Note, there are such good resources online. The tools are also really good. *Do not waste time reinventing the wheel*. Understand the tools your using, but don't _e.g._ write your own optimizer! The pros already did that for you.

What Mike did:
1) Andrew Ng's Machine Learning course (I'd say this is a must do)
2) Statistical Learning course
3) ML project (Kaggle-like)
4) Deep learning courses (Andrew Ng)
5) Some random Keras/Tensorflow tutorials
6) Insight (deep learning project)
7) fast ai
8) Pytorch tutorials

What Mike would recommend:
1) Andrew Ng's Machine Learning course
2) ML project (Kaggle-like)
3) Statistical Learning course
4) Deep learning courses (Andrew Ng)
5) PyTorch/Tensorflow tutorials
6) Deep learning project
7) fastai

The best thing to do is to identify your weakness and be curious! Doing ML projects is the best way to identify weaknesses.  When going through the project, did you use random forest, but not really remember how it works? Now go look it up! Think you might be overfitting? Look up and understand how you can tell!  You overhear someone talking about autoencoders? Watch a youtube video on what they are! Feeling weak on coding? Try and do a more code intense project (e.g. write a Brownian dynamics simulation!).

## Courses

In Mike's experience, MOOCs are a great way to learn ML.  You can get through them quickly if you listen to them at x2 speed. I found doing the homeworks worthwhile, and the lectures pretty enjoyable to watch. If possible, if you're interested in anything, see if Andrew Ng at Stanford has lectured on it. Here is my recommended order: I'd definitely do 1).

1) [Machine Learning](https://www.coursera.org/learn/machine-learning): Andrew Ng. This is the canonical intro course. Gives a broad overview. I'd say it's a must take.
2) [Statistical Learning](https://lagunita.stanford.edu/courses/HumanitiesSciences/StatLearning/Winter2016/about): Trevor Haste and Rob Tibrisani. This is more of a stats course. Not necessary for learning about deep learning (neural nets), but any card caring data scientist or MLE should take this. This feels like an upper division undergrad/grad course in stats.
3) [Deep learning Specialization](https://www.coursera.org/specializations/deep-learning): Andrew Ng. There are five courses here. They use Tensorflow/Keras. Even if you're more interested in doing DS (where deep learning tools aren't [currently] that frequently used), I would check these courses out. At the very least to get a sense of what we can currently do with deep learning.
4) [Fastai](https://course.fast.ai/index.html): Jeremy Howard. Deep learning course taught in pytorch. This is a top-down introductory course as opposed to bottom-up. Meaning, you start using the tools right away to start solving problem without learning how all the pieces work. Maybe I just don't like the style, but I would have not enjoyed this as intro course, but you learn some cool tricks and tips.

Note: Taking 2 is not necessary for the deep learning courses

## Python vs R
Python vs R is a pretty classic debate in data science and ML.  Historically, python was used more by computer scientists and R by statisticians. While there is back and  forth, the answer I am familiar with is: it doesn't really matter, just pick one and get good at it.  I actually disagree with this: *pick python*.   No companies just use R while many companies just use python. It's better for production code. It's more flexible. I can go on and on, but just learn python. And start linting your code!

## Tools to know

* git: this is mandatory. Start putting all your projects on GitHub and use it for everything
* Docker: At the very least, be familiar with this. It's not hard to learn and is a great tool
* pandas: data frame tool. I don't love it, but you should know it.
* sklearn: go to for standard (not deep) machine learning
* Tensorflow (and Keras)*: ML library. Developed by Google. Keras is an API that sits on top of Tensorflow. Use Keras if you can.
* PyTorch*: ML library. Don't know who started it, but actively being developed by Facebook.
* SQL: data science only. This is tricky because some companies really care. Others don't. At the very least do this [SQL blitz tutorial](https://tutorialzine.com/2016/01/learn-sql-in-20-minutes) so you have a sense of what kind of queries people make.

*People will either use Tensorflow or PyTorch for a deep learning project. You should be familiar with one (_i.e._, just go through a couple of tutorials). Both have strengths and weakness. I originally learned Tensorflow/Keras, but I think PyTorch is winning my heart. It's way more intuitive and pythonic.

## People/Companies to know of
This may sound silly, but I think it's useful to know who some of the main players are in the field. It comes up frequently in conversation and let's you have a better understanding of the field
* Humans
  * Geoffrey Hinton
  * Yann LeCunn
  * Andrew Ng
  * Fei-Fei Li
  * Karl Friston
  * Andrej Karpathy
* Humans according to Republicans
  * OpenAI
  * FastAI
  * Google Deepmind/Brain (different companies, but I lump them together)

## Projects
The best way to learn ML is do projects! If you have some data you're interested in, do that! [Kaggle](https://www.kaggle.com/) is another place you could look---you definitely want to be aware of it.

## Tutorials
I found PyTorch, Keras, and Tensorflow have great tutorials.  If you're thinking of doing, say, a classification problem, check out a tutorial and adapt it to you problem!

## Jupyter notebooks vs scripts
Jupyter notebooks are another thing people have strong feelings for.  Definitely try them out and be familiar with them. They are things they are very useful for. However, there are many things Jupyter notebooks suck at, and no production code is going to be in a notebook.  Be familiar with running scripts and building out a repo instead of having everything buried in a notebook. I typically will do a POC in a notebook and have some examples as a reference, but most of my work is running scripts from the command line. Tools like [streamlit](http://streamlit.io/) may kill the need for the best use-case Jupyter notebooks: making a nice report. I believe it's still in beta, but I think it's a good idea.

## Other resources
* YouTube: Actually, I found a ton of good youtube material. Let the video rating be your guide.
  * [statquest](https://www.youtube.com/user/joshstarmer): general statistics one-offs. 
  * [Computerphile](https://www.youtube.com/channel/UC9-y-6csu5WGm29I7JiwpnA): General high-level software concepts. They are also British, which is fun.
  * [HackerRack](https://www.youtube.com/channel/UCOf7UPMHBjAavgD0Qw5q5ww): This is essentially cracking the coding interview's YouTube channel. Check this out for data structures and algorithms
  * [ArxivInsight](https://www.youtube.com/channel/UCNIkB2IeJ-6AmZv7bQ1oBYg): This guy is good at giving high-level explanations of various deep and reinforcement learning.
  * Machine learning: If you can, try and find a video of Andrew Ng explaining the topic. He is a master. His coursera lectures are scattered on YouTube.
* Podcasts: I actually found listening to ML themed podcasts interesting and helpful. You learn about what people are currently working on as well a background on common tools and methods.  There have been many times where I had a 'Ah-ha!' moment connecting something I was working on with something I heard in a podcast. Here are some good ones:
  * This Week in Machine Learning (TWiML)
  * Talking Machines: I only  listened to the earlier ones. I really enjoyed learning about the history of deep learning
  * Data Skeptic: I've only listened to a couple. Seems ok.
* Textbooks
  * [Intro to Statistical Learning](https://www-bcf.usc.edu/~gareth/ISL/)
