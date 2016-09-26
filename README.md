
IPyton notebooks showing off how to
use the [standalone version of Sherpa](http://cxc.cfa.harvard.edu/contrib/sherpa/)
to fit data.

You can now try them out *directly in your browser*
via the magic of the MyBinder project (unfortunately the offer does
not extend to the XSPEC example as there's no easy build of the XSPEC
user models that the binder project can use,
I appear to have forgotten to set up the SciPy requirement so this
will cause some problems in some notebooks,
and it is not likely to
be as fast as when run on your own machine):
[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/DougBurke/sherpa-standalone-notebooks)

 - [A really simple "fit"](http://nbviewer.ipython.org/github/DougBurke/sherpa-standalone-notebooks/blob/master/really%20simple%20fit.ipynb),
   which also doubles as my go-to-guide when cooking my kids porridge
   for breakfast.

   January 18 2016   
 
 - [A simple fit](http://nbviewer.ipython.org/github/DougBurke/sherpa-standalone-notebooks/blob/master/simple%20sherpa%20fit.ipynb) which is based on
   the [NumPy/SciPy fitting example](http://python4astronomers.github.io/core/numpy_scipy.html)
   from the 
   [Practical Python for Astronomers](http://python4astronomers.github.io/index.html)
   course.

   Last updated: September 26 2016 to use the Sherpa 4.8.2 release
   
 - [Writing your own user model](http://nbviewer.ipython.org/github/DougBurke/sherpa-standalone-notebooks/blob/master/user%20model.ipynb),
   which fits the cumulative distribution function of a data set
   with the Gamma CDF. The same code can be run from the CIAO version
   of Sherpa (I added this as we are currently lacking in documentation
   for how to use the `add_user_model` routine).

   May 26 2015.

 - [An integrated user model](http://nbviewer.ipython.org/github/DougBurke/sherpa-standalone-notebooks/blob/master/an%20integrated%20user%20model.ipynb),
   which fits the Gamma probability distribution function to the data
   set used in the 'Writing your own user model' example. This is
   an example of handling "integrated" data sets, and also shows off
   how to write a `guess` routine for your model, and some plot
   manipulations (in particular, re-creating a region-projection plot
   and adding extra annotations to it).

   June 4 2015.

 - [How can I plot data and models when using the lower-level routines](http://nbviewer.ipython.org/github/DougBurke/sherpa-standalone-notebooks/blob/master/plotting%20using%20the%20lower-level%20routines.ipynb),
   which came up (in my mind) in the "Writing your own user model"
   example, where I started off using the lower-level API, but quickly
   switched to the higher-level (data management) API in part because
   I did not know how to create the plots. Well, I do know, and so
   can *you*.

   June 5 2015.

 - [Extending existing models (and an example of using XSPEC models)](http://nbviewer.ipython.org/github/DougBurke/sherpa-standalone-notebooks/blob/master/extending%20existing%20models%20%28and%20XSPEC%29.ipynb),
   which shows how to write a user model that extends the behavior of
   an existing model (in this case, subtracting a model from itself with
   different parameter values). It also shows how to build the XSPEC module,
   and so use the
   [XSPEC models](https://heasarc.gsfc.nasa.gov/xanadu/xspec/manual/Models.html)
   from standalone Sherpa.

   June 16 2015.

 - [Simulating 2D data with a dash of error analysis](http://nbviewer.ipython.org/github/DougBurke/sherpa-standalone-notebooks/blob/master/simulating%20a%202D%20image%20and%20a%20bit%20of%20error%20analysis.ipynb),
   which uses the object API to simulate a 2D model (i.e. an image),
   fit it, and calculate errors on the parameters. This can be thought of
   as an extension of the previous notebooks that show how to replicate
   the functionality of the high-level UI layer using the object API
   (it also marks the start of me using the term "object API" for what I
   previously referred to as the "low-level API").

   June 19 2015

 - [Simulating and fitting a 2D image (this time with a Bayesian approach)](http://nbviewer.ipython.org/github/DougBurke/sherpa-standalone-notebooks/blob/master/simulating%20and%20fitting%20a%202D%20image%20%28this%20time%20with%20a%20Bayesian%20approach%29.ipynb),
   which is based on the previous notebook, this time showing how
   you can use the Monte Carlo Markov Chain (MCMC) analysis module
   in Sherpa (that is, the
   [Bayesian Low-Count X-ray Spectral (pyBLoCXS)](http://hea-www.harvard.edu/astrostat/pyblocxs/)
   module). This notebook is mainly intended to show *how* to do this,
   rather than explain why (or the differences between the various
   frequentist and Bayesian methods for coming up with an error estimate).

   June 22 2015

The information in these notebooks is placed in the Public Domain and
is not an official product of the Chandra X-ray Center.
