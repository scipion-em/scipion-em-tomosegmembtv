=====================================================
Scipion plugin for TomoSegMemTV and MembraneAnnotator
=====================================================

.. image:: https://img.shields.io/pypi/v/scipion-em-tomosegmemtv.svg
        :target: https://pypi.python.org/pypi/scipion-em-tomosegmemtv
        :alt: PyPI release

.. image:: https://img.shields.io/pypi/l/scipion-em-tomosegmemtv.svg
        :target: https://pypi.python.org/pypi/scipion-em-tomosegmemtv
        :alt: License

.. image:: https://img.shields.io/pypi/pyversions/scipion-em-tomosegmemtv.svg
        :target: https://pypi.python.org/pypi/scipion-em-tomosegmemtv
        :alt: Supported Python versions

.. image:: https://img.shields.io/pypi/dm/scipion-em-tomosegmemtv
        :target: https://pypi.python.org/pypi/scipion-em-tomosegmemtv
        :alt: Downloads

Scipion plugin for segmentation and annotation of membranes in tomograms (with TomoSegmenTV_ and memb-annotator_,
respectively)

============
Installation
============
The plugin can be installed in user (stable) or developer (latest, may be unstable) mode:

**1. User (stable) version:**:

.. code-block::

    scipion3 installp -p scipion-em-tomosegmemtv

**2. Developer (latest, may be unstable) version:**:

* Clone the source code repository:

.. code-block::

    git clone https://github.com/scipion-em/scipion-em-tomosegmemtv.git

* Install:

.. code-block::

    scipion3 installp -p local/path/to/scipion-em-tomosegmemtv --devel

=========
Protocols
=========
The integrated protocols are:

1. tomosegmemtv - annotate segmented membranes: Manual annotation tool for segmented membranes.

2. tomosegmemtv - resize segmented or annotated volume: Resize segmented volumes or annotated (TomoMasks).

3. tomosegmemtv - tomogram segmentation: segment membranes in tomograms.

=====
Tests
=====

The installation can be checked out running some tests (Important: test_resize_tomomask requires the plugin
scipion-em-imod_ to be installed).

.. code-block::

    scipion3 tests tomosegmemtv.tests.test_tomosegmemtv

.. code-block::

    scipion3 tests tomosegmemtv.tests.test_resize_tomomask

========
Tutorial
========
A tutorial about how to use tomosegmemtv and the membrane annotator within Scipion can be found here_.

==========
References
==========

* `Robust membrane detection based on tensor voting for electron tomography. <https://doi.org/10.1016/j.jsb.2014.02.015>`_

    A. Martinez-Sanchez, I. Garcia, S. Asano, V. Lucic, J.J. Fernandez.
    Journal of Structural Biology  186:49-61, 2014.

===================
Contact information
===================

If you experiment any problem, please contact us here: scipion-users@lists.sourceforge.net, scipion@cnb.csic.es or open
an issue_.

We'll be pleased to help.

*Scipion Team*


.. _TomoSegmenTV: https://sites.google.com/site/3demimageprocessing/tomosegmemtv
.. _memb-annotator: https://github.com/anmartinezs/memb-anotator
.. _scipion-em-imod: https://github.com/scipion-em/scipion-em-imod
.. _here: https://scipion-em.github.io/docs/release-3.0.0/docs/user/denoising_mbSegmentation_pysegDirPicking/tomosegmemTV-pySeg-workflow.html#tomosegmemtv-pyseg-workflow
.. _issue: https://github.com/scipion-em/scipion-em-tomosegmemtv/issues

