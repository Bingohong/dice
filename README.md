DICe
====

### Pushing DIC technology to new levels, together

DICe is an open source digital image correlation (DIC) tool intended for use as a module in an external application or as a standalone analysis code. Its primary capability is computing full-field displacements and strains from sequences of digital images. These images are typically of a material sample undergoing a characterization experiment, but DICe is also useful for other applications (for example, trajectory tracking). DICe is machine portable (Windows, Linux and Mac) and can be effectively deployed on a high performance computing platform (DICe uses MPI parallelism as well as threaded on-core parallelism). Capabilities from DICe can be invoked through a customized library interface, via source code integration of DICe classes or through a standalone executable.

![screen shot 2017-05-16 at 8 38 14 am](https://cloud.githubusercontent.com/assets/15202746/26112065/167c12b0-3a14-11e7-8361-a4978dc54bf0.png)

Features
--------

DICe is different than other available DIC codes in the following ways:

First, subsets can be of arbitrary shape. This enables tracking of oblong objects that otherwise would not be trackable with a square subset.

DICe also incudes a robust simplex optimization method that does not use image gradients (this method is useful for data sets that are impossible to analyze with the traditional Lucas-Kanade-type algorithms, for example,  objects without speckles, images with low contrast, and small subset sizes < 10 pixels).

Lastly, DICe also includes a well-posed global DIC formulation that addresses instabilities associated with the saddle-point problem in DIC (This capability will be released later this year).

For more information visit: https://dice.sandia.gov

Documentation
-------------
[http://dicengine.github.io/dice](http://dicengine.github.io/dice)

Tutorials
---------
[http://dicengine.github.io/dice/pages.html](http://dicengine.github.io/dice/pages.html)

Releases (and Installers)
-------------------------
Windows 7 and Mac OSX Yosemite  package installers for DICe can be found [here](https://github.com/dicengine/dice/releases)

Contributing to DICe
--------------------

Fork the DICe repo, develop new algorithms and send us a pull request. We suggest the following guidelines be followed to keep a high degree of software quality:

* Ensure that all existing tests pass with your changes applied
* Create tests for new features
* Document code with Doxygen formatted comments
* Have your changes reviewed by an objective party
* Use descriptive commit messages

Reporting Bugs or Requesting New Features
-----------------------------------------

Use the [issues link](https://github.com/dicengine/dice/issues) above to report bugs and request new features.

### Citing DICe:

DZ Turner, Digital Image Correlation Engine (DICe) Reference Manual, Sandia Report, SAND2015-10606 O, 2015
