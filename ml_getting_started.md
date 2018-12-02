# ML prep
Here is my guide for anyone looking to transition into machine learning for academia.  I will recommend courses to check out as well as things to be aware before you should try to interview at a company. I'll give a little bit of background to set the stage. I am going to try my best to introduce for keywords and ideas before diving into specifics

## What is machine learning? (optional intro)

We are constantly trying to describe phenomena to make sense of the world. To do this, we either have a theoretical basis for an equation or we have to approximate it---typically by guessing a form. In either case, we collect data points of some experiment or event. From these, we try to assign the behavior of the inputs to describe some output. You've already done this many times in your life: you have some dependent variables and independent variables and try a find a function that takes you from the input (dependent variables) to the output (independent variables). _I.e_, we have some data points and we are trying to draw a line that describes the variable.  Most people are more comfortable with continuous outputs. Meaning, the output could be some real number.  Let's run an experiment.  Let's say I want to predict how much a baby weighs from age 0-1. I go out and collect a bunch of data points (babies!) and record their age and weight. I plot weight vs age, and the data looks like it's following a linear trend (a straight line). I guess that the function that describes the behavior is weight = m * age + b ($\hat{y} = m x + b$). Note, people in machine learning like to call $x$ features and $y$ outputs or labels (this will make more sense in a bit). Now, we have a bunch of $y$ and $x$ points, and to describe the behavior I need to find $m$ and $b$. Note, this is just a linear equation! I can analytically solve the question to find what $m$ and $b$ are! However, that involves inverting a matrix, which is computationally expensive if you have a lot a points. There are ways to iteratively solve this equation. When I do this, I calculate a cost function, which describes how close my function approximation is.  I feed in some data points, calculate the cost, and update the fit parameters.  One could say that the program is learning (finding better and better fit parameters) by seeing examples, _i.e._, Machine learning!

Now, what I've described in supervised learning. I should also mention that most supervised learning problems don't look at continuous outputs, but rather discrete classes or labels.  The function will take in an input and output a class label. One fun example is feeding in an input image and it predicting if it's a cat or dog. Other types of machine learning problems are unsupervised learning and reinforcement learning.  In unsupervised, we don't have labels for the data. For unsupervised learning, we typically try are cluster things by their features. Reinforcement learning describes problems where a program can try a series of actions and is rewarded or punished for actions that get it closer to goal. (Think directing an agent through a maze with traps. Falling in a trap is bad and reaching the goal is good. A program will try sequences of events learning from the it's past successes and failures. You may also hear neural nets and deep learning.  Neural nets and deep learning are tools, not a type of problem (although they are good at solving certain classes of problems). More specifically, neural nets are a type of function approximator you can use. When calculating an output, they calculate intermediate values called activations. These activations live in things called layers.  Deep learning describes ML problems where you use deep neural networks (_i.e._, many layers) 

## General plan of attack
Well, this of course is buyer beware. Everyone is different, yada yada yada. Here is roughly what I did, and a guess on how long it took me. For all the courses and everything. I am going to assume you have some background in programming---you can write code pretty well in a certain language and are familiar with classes. If not, you may want to brush up on this, but I don't know the best resource.  Usually coding is the best way! This may seem like a lot, but you'd be surprised. I am recommending learning about deep learning. It's a powerful, and I believe any card caring DS/ML engineer (MLE) should know the methods at a high level, but more importantly, what kind of problem you can solve with these. Note, there are such good resources online. The tools are also really good. *Do not waste time reinventing the wheel*. Understand the tools your using, but don't _e.g._ write your own optimizer! The pros already did that for you.

What I did:
1) Andrew Ng's Machine Learning course (I'd say this is a must do)
2) Statistical Learning course
3) ML project (Kaggle-like)
4) Deep learning courses (Andrew Ng)
5) Some random Keras/Tensorflow tutorials
6) Insight (deep learning project)
7) fast ai
8) Pytorch tutorials

What I'd recommend:
1) Andrew Ng's Machine Learning course
2) ML project (Kaggle-like)
3) Statistical Learning course
4) Deep learning courses (Andrew Ng)
5) PyTorch/Tensorflow tutorials
6) Deep learning project
7) fastai

The best thing to do is identify your weakness and be curious! Doing ML projects is the best way to identify weaknesses.  When going through the project, did you use random forest, but really remember how it works? Now go look it up! Think you might be overfitting? Look up and understand how you can tell!  You overhear someone talking about autoencoders? Watch a youtube video on what they are! Feeling weak on coding? Try and do a more code intense project (e.g. write a Brownian dynamics simulation!).

## Courses

In my experience, MOOCs are a great way to learn ML.  You can get through them quickly if you listen to them at x2 speed. I found doing the homeworks worthwhile, and the lectures pretty enjoyable to watch. If possible, if you're interested in anything, see if Andrew Ng at Stanford has lectured on it. Here is my recommended order: I'd definitely do 1).

1) [Machine Learning](https://www.coursera.org/learn/machine-learning): Andrew Ng. This is the canonical intro course. Gives a broad overview.
2) [Statistical Learning](https://lagunita.stanford.edu/courses/HumanitiesSciences/StatLearning/Winter2016/about): Trevor Haste and Rob Tibrisani. This is more of a stats course. Not necessary for learning about deep learning (neural nets), but any card caring data scientist or ML engineer should take this. This feels like an upper division undergrad/grad course in stats.
3) [Deep learning Specialization](https://www.coursera.org/specializations/deep-learning): Andrew Ng. There are five courses here. They use Tensorflow/Keras. Even if you're more interested in doing DS (where deep learning tools aren't [currently] that frequently used), I would check these courses out. At the very least to get a sense of what we can currently do with deep learning.
4) [Fastai](https://course.fast.ai/index.html): Jeremy Howard. Deep learning course taught in pytorch. This is a top-down introductory course as opposed to bottom-up. Meaning, you start using the tools right away to start solving problem without learning how all the pieces work. Maybe I just don't like the style, but I would have not enjoyed this as intro course, but you learn some cool tricks and tips.

Note: Taking 2 is not necessary for the deep learning courses

## Python vs R
Python vs R is a pretty classic debate in data science and ML.  Historically, python was used more by computer scientists and R by statisticians. While there is back and  forth, the answer I am familiar with is: it doesn't really matter, just pick one and get good at it.  I actually disagree with this: *pick python*.   No companies just use R while many companies just use python. It's better for production code. It's more flexible. I can go on and on, but just learn python. And start linting your code!

## Tools to know

* git: this is mandatory. Start putting all your projects on GitHub and use it for everything
* pandas: data frame tool. I don't love it, but you should know it.
* sklearn: go to for standard (not deep) machine learning
* Tensorflow (and Keras)*: ML library. Developed by Google. Keras is an API that sits on top of Tensorflow. Use Keras if you can.
* Pytorch*: ML library. Don't know who started it, but actively being developed by Facebook.
* SQL: data science only. This is tricky because some companies really care. Others don't. At the very least do this [SQL blitz tutorial](https://tutorialzine.com/2016/01/learn-sql-in-20-minutes) so you have a sense of what kind of queries people make.

*People will either use Tensorflow or PyTorch for a deep learning project. You should be familiar with one (_i.e._, just go through a couple of tutorials). Both have strengths and weakness. I originally learned Tensorflow/Keras, but I think PyTorch is winning my heart. It's way more intuitive and pythonic.

## People/Companies to know of
This may sound silly, but I think it's useful to know who some of the main players are in the field. It comes frequently in conversation and let's have a better understanding of the field
* Humans
  * Geoffrey Hinton
  * Yann LeCunn
  * Andrew Ng
  * Fei-Fei Li
* Humans according to Republicans
  * OpenAI
  * FastAI
  * Google Deepmind/Brain (different companies, but I lump them together)

## Projects
The best way to learn ML is do projects! If you have some data you're interested in, do that! [Kaggle](https://www.kaggle.com/) is another place you could look---you definitely want to be aware of it.

## Tutorials
I found PyTorch, Keras, and Tensorflow have get tutorials.  If you're thinking of doing, say, a classification problem, check out a tutorial and adapt it to you problem!

## Jupyter notebooks vs scripts
Jupyter notebooks are another thing people have strong feelings for.  Definitely try them out and be familiar with them. They are things they are very useful for. However, there are many things Jupyter notebooks suck at, and no production code is going to be in a notebook.  Be familiar with running scripts and building out a repo instead of having everything buried in a notebook. I typically will do a POC in a notebook and have some examples, but most of my work is running scripts from the command line. Tools like streamlit may kill the need for the best use-case jupyter notebooks: making a nice report. I believe it's still in beta, but I think it's a good idea.

## Other resources
* Everything: Actually, I found a ton of good youtube material. Let the video rating be your guide.
* General stats: I really like [statquest](https://www.youtube.com/user/joshstarmer) for statistics one-offs. 
* Machine learning: If you can, try and find a video of Andrew Ng explaining the topic. He is a master.
* Podcasts: I actually found listen to ML themed podcasts interesting and helpful. You learn about what people are currently working on as well a background on common tools and methods.  There have been many times where I had a 'Ah-ha!' moment connecting something I was working on with something I heard in a podcast. Here are some good ones:
  * This Week in Machine Learning (TWiML)
  * Talking Machines: I only  listened to the earlier ones. I really enjoyed learning about the history of deep learning
  * Data Skeptic: I've only listened to a couple. Seems ok.
* Textbooks
  * [Intro to Statistical Learning](https://www-bcf.usc.edu/~gareth/ISL/)
