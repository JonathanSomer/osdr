.. _Preprocess:

===============
Preprocessing
===============


Overview
============

The goal of preprocessing is to prepare a single-cell dataframe that can be provided as input to the :class:`~tdm.analysis.Analysis` class. 

A processed single-cell dataframe will hold the following columns:

- ``x (float)`` and ``y (float)``: spatial coordinates of the cell in the tissue. Standard units are expected (e.g 1 micron = 1e-6)
- ``division (bool)``: a binary label that marks a cell as "curently dividing".
- ``cell_type (str)``: the cell type (e.g "Fibroblast")
- ``img_num (int, optional)``: identifier of the tissue sample.
- ``subject_id (int | str, optional)``: identifier of the subject (patient).


Preparing the single-cell dataframe
===================================

.. autosummary::
   :toctree: generated/
   :nosignatures:

   ~tdm.preprocess.single_cell_df.check_single_cell_df


Defining cell-division events
==============================

The :mod:`tdm.preprocess.ki67` and :mod:`tdm.plot.preprocess.ki67` modules provide tools for defining cell-division events based on raw Ki67 measurements.
See :ref:`Tutorial 1<Tutorials>` for a detailed walk-through.


.. rubric:: Find the background noise level

.. autosummary::
   :toctree: generated/
   :nosignatures:

   ~tdm.plot.preprocess.ki67.plot_marker_distributions
   ~tdm.preprocess.ki67.transform_ki67


.. rubric:: Define binary cell-division labels

.. autosummary::
   :toctree: generated/
   :nosignatures:

   ~tdm.preprocess.ki67.is_dividing


.. rubric:: Quality control

.. autosummary::
   :toctree: generated/
   :nosignatures:

   ~tdm.plot.preprocess.ki67.plot_fraction_of_dividing_cells
   ~tdm.plot.preprocess.ki67.plot_divisions_per_image



   



