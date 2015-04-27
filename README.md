# If You're Writing in IPython Notebooks / Jupyter, O'Reilly Media Wants to Talk to You

* Jupyter / IPython Notebooks as a first class authoring environment, on par with Word or Atlas.
* A new oreilly.com where people can use this content like they're supposed to


## Why the Notebooks 

* Following the Alpha Geeks. Many of our best ideas over the years have come from "following the alpha geeks," and from this perspective, the Notebooks are a clear winner.  People *want* to write in the Notebooks, and we want to support them.
* Part of the reason it's such an exciting tool is that it encourages active learning.  Notebooks are written with the expectation that you will be *doing* something, not just reading about it.  Knowing that the learner will be running your code and as-is changes the nature of what is created, making content that's more like a course, less like a book.
* Language kernels. Thanks to it's well-documented [kernel spec](http://ipython.org/ipython-doc/dev/development/kernels.html), Jupyter supports well over 30 [language kernels for other languages](https://github.com/ipython/ipython/wiki/IPython-kernels-for-other-languages) than Python.  
* If you're writing in notebooks (or want to) then we want to work with you


## The writing/production process

* You write in the notebooks
* Use [ipymd](https://github.com/rossant/ipymd) to convert content to Markdown (or, just use Markdown as your native format)
* Check you're notebooks into [Atlas]() and configure the project
* Put your dependencies in a Dockerfile
* gulp-htmlbook (soon to be an Atlas worker) to publish it

## The new oreilly.com

Built an environment where code can run live:

* We build a Docker image of the notebooks that has all the necessary dependencies and libraries preinstalled
* We use [tmpnb](https://github.com/jupyter/tmpnb) to provide temporary instances where people can run code.
* [Thebe](https://github.com/oreillymedia/thebe), a widget we're open sourcing to allow people to run Jupyter code cells in alternate frontends.  
