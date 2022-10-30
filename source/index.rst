.. StaGATE documentation master file, created by
   sphinx-quickstart on Thu Sep 16 19:43:51 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

STAGATE – deciphering spatial domains from spatially resolved transcriptomics
=============================================================================

.. toctree::
   :maxdepth: 1

   Installation
   Installation_pyG
   T1_DLPFC
   T2_MouseBrain
   T3_Slide-seqV2
   T4_Stereo
   T5_3D
   T6_Denoising
   T7_pyG
   T8_Batch
   T9_STARmap
   AT1
   AT2

.. image:: ../Images/StaGATE_Fig1.png
   :width: 600

News
========
2022.03.05 STAGATE based on pyG (PyTorch Geometric) framework is availble at STAGATE_pyG (https://github.com/QIFEIDKN/STAGATE_pyG).

Benefit from the optimization of the pyG package for training graph neural networks, it is more than 10x faster than STAGATE based on the tensorflow1 framework, and can use a batch training strategy to deal with large-scale data (See Tutorials 7 and 8 for details).

The cell type-aware module has not been supported by STAGATE_pyG yet.

Introduction
========
STAGATE is designed for spatial clustering and denoising expressions of spatial resolved transcriptomics (ST) data. 

STAGATE learns low-dimensional latent embeddings with both spatial information and gene expressions via a graph attention auto-encoder. 
The method adopts an attention mechanism in the middle layer of the encoder and decoder, which adaptively learns the edge weights of spatial neighbor networks, and further uses them to update the spot representation by collectively aggregating information from its neighbors.
The latent embeddings and the reconstructed expression profiles can be used to downstream tasks such as spatial domain identification, visualization, spatial trajectory inference, data denoising and 3D expression domain extraction.

Citation
========
Dong, Kangning, and Shihua Zhang. "Deciphering spatial domains from spatially resolved transcriptomics with an adaptive graph attention auto-encoder." Nature Communications 13.1 (2022): 1-12.
