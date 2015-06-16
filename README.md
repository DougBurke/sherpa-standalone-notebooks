
IPyton notebooks showing off how to
use the [standalone version of Sherpa](http://cxc.cfa.harvard.edu/contrib/sherpa47b/) to fit data.

 - [A simple fit](http://nbviewer.ipython.org/github/DougBurke/sherpa-standalone-notebooks/blob/master/simple%20sherpa%20fit.ipynb) which is based on
   the [NumPy/SciPy fitting example](http://python4astronomers.github.io/core/numpy_scipy.html)
   from the 
   [Practical Python for Astronomers](http://python4astronomers.github.io/index.html)
   course.

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
   
The information in these notebooks is placed in the Public Domain and
is not an official product of the Chandra X-ray Center.
