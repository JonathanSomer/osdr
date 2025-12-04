Welcome!
===================================================================

.. image:: _static/OSDR.png
  :width: 500
  :alt: OSDR logo

.. toctree::
   :maxdepth: 1

   getting_started
   examples
   tutorials/index
   api/index


Disclaimer:
-------------

This package is released primarily for reproduction of results from the paper by Somer, Mannor, Alon in Nature 2025. We are working on several extensions of this work on a separate development repository and will not be constantly updating this one. 

In general, application of our approach requires some expertise in biology, dynamical systems, statistics and programming. From our experience, debugging a single peculiar phase-portrait could span all of these domains - requiring an understanding of how a biological/experimental phenomena could skew a statistical estimate that is then expressed in the phase-portrait. 

Remember: the package will plot a phase-portrait even if underlying assumptions aren’t satisfied. It is your responsibility as a scientist to evaluate a result's validity through the various means we described in the paper, and very likely other means we cannot yet imagine for some settings. Examples include: patient-level or spatial confounders, challenges estimating the death rate, insufficient sample size and analyzing dynamics in state-space regions with minimal data.

Please read our paper carefully, and if you are working on a particularly interesting application - feel free to reach out and we could potentially collaborate.

jonathan.somer@gmail.com


