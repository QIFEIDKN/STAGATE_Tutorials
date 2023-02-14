.. StaGATE documentation master file, created by
   sphinx-quickstart on Thu Sep 16 19:43:51 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Installation (pyG framework)
============

Software dependencies
---------------------
.. code-block:: python

   scanpy
   pytorch
   pyG
   
The use of the mclust algorithm requires the rpy2 package and the mclust package. See https://pypi.org/project/rpy2/ and https://cran.r-project.org/web/packages/mclust/index.html for detail.

The cell type-aware module has not been supported by STAGATE_pyG yet.

Installation
------------
Downloading STAGATE_pyG code from https://github.com/QIFEIDKN/STAGATE_pyG

.. code-block:: python

   cd STAGATE_pyG-main
   python setup.py build
   python setup.py install

.. code-block:: python

   import STAGATE_pyG
   
   
