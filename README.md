# If You're Writing in IPython Notebooks / Jupyter, O'Reilly Media Wants to Talk to You

O'Reilly Media is thrilled to announce that we're making [IPython Notebooks](http://ipython.org/notebook.html) a first class authoring environment for our publishing program, on par with Word or our [Atlas](atlas.oreilly.com) platform.  As part of our move to embrace the platform, we're also experimenting on [beta.oreilly.com](https://beta.oreilly.com/) for ways for readers to experience this content like they're supposed to -- live and interactive:

* [Simple Line Plots with Matplotlib](https://beta.oreilly.com/learning/simple-line-plots-with-matplotlib)
* [Three-dimensional Plotting in Matplotlib](https://beta.oreilly.com/learning/three-dimensional-plotting-in-matplotlib)
* [Supervised Learning In-Depth: Support Vector Machines](https://beta.oreilly.com/learning/scikit-learn/page/4/03.1-Classification-SVMs)

Why the Notebooks, and why now?  Most of our best ideas over the years have come from "following the alpha geeks," and with the possible exception of Git and GitHub, the IPython Notebooks have consistently been one of the most requested features for our publishing program.  People *enjoy* writing in the Notebooks, and have created thousands of fascinating projects ranging from [courses on data science](https://github.com/jakevdp/sklearn_pycon2015/) to [detailed explanations of xkcd comics](http://nbviewer.ipython.org/url/norvig.com/ipython/xkcd1313.ipynb?create=1_1).  Knowing that the learner will be actively engaged with the content, not just passively reading, changes the nature of what's possible.  

Of course, it also helps that there is  strong and welcoming community behind it.  So welcoming, in fact, that they recently rebranded the projects as Jupyter in recognition that the tool goes well beyond just Python, and now supports [over 30 additional languages](https://github.com/ipython/ipython/wiki/IPython-kernels-for-other-languages).  

So, if you're writing in Notebooks (or want to) then we want to work with you.  Let us know what you're interested in doing on our [work with us](http://www.oreilly.com/work-with-us.html) page.  

## What to expect while working with us

While we're still working out the details, here's a rough outline of what the process will look like:

* You write in the notebooks, like always.
* You (or we) use [Cyrille Rossant](http://cyrille.rossant.net/)'s excellent [ipymd plugin](https://github.com/rossant/ipymd) to convert the content to Markdown. (Or, you can even just use Markdown as your native format.)
* You check the Markdown version of the notebooks into [Atlas](atlas.oreilly.com) to collaborate with your editor, reviewers, and the O'Reilly production department.
* In addition, you can run our toolchain locally to reduce the "edit -> push -> build -> review" cycle.

Our goal is to build a workflow that will feel familiar to anyone who has used a static site generator like [Jekyll](http://jekyllrb.com/) or [Pelican](http://blog.getpelican.com/).

## The new oreilly.com

In addition to this new toolchain to support the Notebooks as an authoring environment, we're also working on a new way to publish live, beautifully designed notebooks on oreilly.com.  Here's the key idea:

* We help you create a [Docker](https://www.docker.com/) image of your notebook that has all the necessary dependencies and libraries preinstalled.
* On the backend, we use [tmpnb](https://github.com/jupyter/tmpnb) to provide temporary Notebook server that runs a kernel.
* On the frontend, we use our new [Thebe](https://github.com/oreillymedia/thebe) widget, which provides a slimmed down notebook frontend that handles code cells.  (Think of Thebe as a way to plug out the "Code" cell box from the Notebook and drop it into a static site.)  

We'll be making lot's of improvements in this workflow, so stay tuned.  



