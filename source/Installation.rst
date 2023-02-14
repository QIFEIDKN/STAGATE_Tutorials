.. StaGATE documentation master file, created by
   sphinx-quickstart on Thu Sep 16 19:43:51 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Installation (tensorflow1 framework)
============

Software dependencies
---------------------
.. code-block:: python

   scanpy
   tensorflow==1.15.0
   
The use of the mclust algorithm requires the rpy2 package and the mclust package. See https://pypi.org/project/rpy2/ and https://cran.r-project.org/web/packages/mclust/index.html for detail.


Installation
------------
Downloading STAGATE code from https://github.com/QIFEIDKN/STAGATE

.. code-block:: python

   cd STAGATE-main
   python setup.py build
   python setup.py install

.. code-block:: python

   import STAGATE
   
   
