# GPflow inter-domain
This package is a fork of GPflow (readme is maintained below) containing modifications to allow _inter-domain_ inducing variables. This package is released primarily in conjuction with the software for [convolutinal Gaussian processes](https://github.com/markvdw/convgp). While these features may eventually be merged into the main GPflow repo, this fork will remain in the mean time.

See below for the GPflow readme for installation instructions.

# GPflow

GPflow is a package for building Gaussian process models in python, using [TensorFlow](http://www.tensorflow.org). It was originally created and is now managed by [James Hensman](http://www.lancaster.ac.uk/staff/hensmanj/) and [Alexander G. de G. Matthews](http://mlg.eng.cam.ac.uk/?portfolio=alex-matthews). 
The full list of [contributors](http://github.com/GPflow/GPflow/graphs/contributors) (in alphabetical order) is Rasmus Bonnevie, Alexis Boukouvalas, Ivo Couckuyt, Keisuke Fujii, Zoubin Ghahramani, David J. Harris, James Hensman, Pablo Leon-Villagra, Daniel Marthaler, Alexander G. de G. Matthews, Tom Nickson, Valentine Svensson and Mark van der Wilk. GPflow is an open source project so if you feel you have some relevant skills and are interested in contributing then please do contact us.  

[![Python2.7 status](https://codeship.com/projects/26b43920-e96e-0133-3481-02cde9680eda/status?branch=master)](https://codeship.com/projects/147609)
[![Python3.5 Status](https://travis-ci.org/GPflow/GPflow.svg?branch=master)](https://travis-ci.org/GPflow/GPflow)
[![Coverage Status](http://codecov.io/github/GPflow/GPflow/coverage.svg?branch=master)](http://codecov.io/github/GPflow/GPflow?branch=master)
[![Documentation Status](https://readthedocs.org/projects/gpflow/badge/?version=latest)](http://gpflow.readthedocs.io/en/latest/?badge=latest)

# What does GPflow do?

GPflow implements modern Gaussian process inference for composable kernels and likelihoods. The [online user manual](http://gpflow.readthedocs.io/en/latest/) contains more details. The interface follows on from [GPy](http://github.com/sheffieldml/gpy), for more discussion of the comparison see [this page](http://gpflow.readthedocs.io/en/latest/intro.html#what-s-the-difference-between-gpy-and-gpflow).

# Install

## 1) Install TensorFlow. 
Please see instructions on the main TensorFlow [webpage](https://www.tensorflow.org/versions/r1.0/get_started/get_started). You will need version 1.0. We find that for most users pip installation is the fastest way to get going.

## 2) install package
GPflow includes some tensorflow extensions that are compiled when you run setup.py.  For those interested in modifying the source of GPflow, we recommend  
```
python setup.py develop
```
but installation should work well too:
```
python setup.py install
```
You can run the tests with `python setup.py test`.

Version history is documented [here.](https://github.com/GPflow/GPflow/blob/master/RELEASE.md)

## Docker image

We also provide a [Docker image](https://hub.docker.com/r/gpflow/gpflow/) which can be run using

```
docker run -it -p 8888:8888 gpflow/gpflow
```

Code to generate the image can be found [here](Dockerfile)

# Getting help
Please use gihub issues to start discussion on the use of GPflow. Tagging enquiries `discussion` helps us distinguish them from bugs. 

# Contributing
All constuctive input is gratefully received. For more information, see the [notes for contributors](contributing.md).


# Citing GPflow

To cite GPflow, please reference the [Technical report](https://arxiv.org/abs/1610.08733). Sample Bibtex is given below:

```
@ARTICLE{GPflow2016,
   author = {Matthews, Alexander G. de G. and {van der Wilk}, Mark and Nickson, Tom and 
	Fujii, Keisuke. and {Boukouvalas}, Alexis and {Le{\'o}n-Villagr{\'a}}, Pablo and 
	Ghahramani, Zoubin and Hensman, James},
    title = "{{GP}flow: A {G}aussian process library using {T}ensor{F}low}",
  journal = {arXiv preprint 1610.08733},
     year = 2016,
    month = oct
}
```
