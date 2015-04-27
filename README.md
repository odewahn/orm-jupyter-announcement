# If You're Writing in IPython Notebooks / Jupyter, O'Reilly Media Wants to Talk to You

O'Reilly Media is thrilled to announce that we're making [IPython Notebooks](http://ipython.org/notebook.html) a first class authoring environment, on par with Word or our own internal toolchain, [Atlas](atlas.oreilly.com).  As part of our move to embrace the platform, we're also experimenting with a new content format on [oreilly.com](https://beta.oreilly.com/) where readers can use this content like they're supposed to -- live an interactive.

Why the Notebooks?  Most of our best ideas over the years have come from "following the alpha geeks," and with the possible exception of Git and GitHub, the IPython Notebooks have consistently been one of the most requested features for our publishing program.  People *enjoy* writing in the Notebooks, and have created thousands of fascinating projects ranging from [courses on data science](https://github.com/jakevdp/sklearn_pycon2015/) to [detailed explanations of xkcd comics](http://nbviewer.ipython.org/url/norvig.com/ipython/xkcd1313.ipynb?create=1_1).

A huge part of the interest among our authors is that the Notebook encourages *active* learning.  They're written with the expectation that you will be *doing* something, not just reading about it.  And, knowing that the learner will be running your code and as-is changes the nature of what is created, making content that's more like a course, less like a book.

Of course, it also helps that there is  strong and welcoming community behind it.  So welcoming, in fact, that they recently rebranded the projects as Jupyter in recognition that the tool goes well beyond just Python, and now supports [over 30 additional languages](https://github.com/ipython/ipython/wiki/IPython-kernels-for-other-languages).  

So, if you're writing in Notebooks (or want to) then we want to work with you


## The writing/production process

While we're still working out the details, here's a rough outline of what the process will look like:

* You write in the notebooks
* Use [Cyrille Rossant](http://cyrille.rossant.net/)'s excellent [ipymd plugin](https://github.com/rossant/ipymd) to convert content to Markdown. (Or, just use Markdown as your native format)
* Check you're notebooks into [Atlas]() and configure the project
* Put your dependencies in a Dockerfile
* gulp-htmlbook (soon to be an Atlas worker) to publish it

We'll be adding additional details to the [Atlas documentation]() soon.

## The new oreilly.com

Built an environment where code can run live:

* We build a Docker image of the notebooks that has all the necessary dependencies and libraries preinstalled
* We use [tmpnb](https://github.com/jupyter/tmpnb) to provide temporary instances where people can run code.
* [Thebe](https://github.com/oreillymedia/thebe), a widget we're open sourcing to allow people to run Jupyter code cells in alternate frontends.  
