climpred: verification of weather and climate forecasts
=======================================================

..
    Table version of badges inspired by pySTEPS.

.. list-table::
    :stub-columns: 1
    :widths: 10 90

    * - docs
      - |docs| |joss| |DOI|
    * - tests
      - |ci| |requires| |codecov|
    * - package
      - |conda| |pypi|
    * - license
      - |license|
    * - community
      - |gitter| |contributors| |downloads|
    * - tutorials
      - |gallery| |workshop| |cloud|

.. |docs| image:: https://img.shields.io/readthedocs/climpred/stable.svg?style=flat
    :target: https://climpred.readthedocs.io/en/stable/?badge=stable
    :alt: Documentation Status

.. |joss| image:: https://joss.theoj.org/papers/246d440e3fcb19025a3b0e56e1af54ef/status.svg
    :target: https://joss.theoj.org/papers/246d440e3fcb19025a3b0e56e1af54ef

.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4556086.svg
   :target: https://doi.org/10.5281/zenodo.4556086

.. |ci|  image:: https://github.com/pangeo-data/climpred/workflows/climpred%20testing/badge.svg
    :target: https://github.com/pangeo-data/climpred/actions/workflows/climpred_testing.yml

.. |requires| image:: https://requires.io/github/pangeo-data/climpred/requirements.svg?branch=main
     :target: https://requires.io/github/pangeo-data/climpred/requirements/?branch=main
     :alt: Requirements Status

.. |codecov| image:: https://codecov.io/gh/pangeo-data/climpred/branch/main/graph/badge.svg
      :target: https://codecov.io/gh/pangeo-data/climpred

.. |conda| image:: https://img.shields.io/conda/vn/conda-forge/climpred.svg
    :target: https://anaconda.org/conda-forge/climpred
    :alt: Conda Version

.. |pypi| image:: https://img.shields.io/pypi/v/climpred.svg
   :target: https://pypi.python.org/pypi/climpred/

.. |license| image:: https://img.shields.io/github/license/pangeo-data/climpred.svg
    :alt: license
    :target: ../../LICENSE.txt

.. |gitter| image:: https://badges.gitter.im/Join%20Chat.svg
    :target: https://gitter.im/climpred

.. |contributors| image:: https://img.shields.io/github/contributors/pangeo-data/climpred
    :alt: GitHub contributors
    :target: https://github.com/pangeo-data/climpred/graphs/contributors

.. |downloads| image:: https://img.shields.io/conda/dn/conda-forge/climpred
    :alt: Conda downloads
    :target: https://anaconda.org/conda-forge/climpred

.. |gallery| image:: https://img.shields.io/badge/climpred-examples-ed7b0e.svg
    :alt: climpred gallery
    :target: https://mybinder.org/v2/gh/pangeo-data/climpred/main?urlpath=lab%2Ftree%2Fdocs%2Fsource%2Fquick-start.ipynb


.. |workshop| image:: https://img.shields.io/badge/climpred-workshop-f5a252
    :alt: climpred workshop
    :target: https://mybinder.org/v2/gh/bradyrx/climpred_workshop/master

.. |cloud| image:: https://img.shields.io/badge/climpred-cloud_demo-f9c99a
    :alt: climpred cloud demo
    :target: https://github.com/aaronspring/climpred-cloud-demo


.. note::
    We are actively looking for new contributors for climpred! Riley moved to McKinsey's
    Climate Analytics team. Aaron is finishing his PhD, but will stay in academia.
    We especially hope for python enthusiasts from seasonal, subseasonal or weather
    prediction community. In our past coding journey, collaborative coding, feedbacking
    issues and pull requests advanced our code and thinking about forecast verification
    more than we could have ever expected.
    `Aaron <https://github.com/aaronspring/>`_ can provide guidance on
    implementing new features into climpred. Feel free to implement
    your own new feature or take a look at the
    `good first issue <https://github.com/pangeo-data/climpred/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22>`_
    tag in the issues. Please reach out to us via `gitter <https://gitter.im/climpred>`_.


Version 2.1.3 Release
=====================

*March 23th, 2021*

After our `JOSS <https://joss.theoj.org/papers/246d440e3fcb19025a3b0e56e1af54ef>`_
paper is published, the climatology reference forecast was introduced and persistence
forecasts are extended for all metrics (before probabilistic persistence skill was not
calculated) (:pr:`566`).
Furthermore, any errors in ``PredictionEnsemble.map(func)`` or
``PredictionEnsemble.call()`` does not call silently anymore, but raises warnings
instead (:pr:`552`).


Installation
============

You can install the latest release of ``climpred`` using ``pip`` or ``conda``:

.. code-block:: bash

    pip install climpred

.. code-block:: bash

    conda install -c conda-forge climpred

You can also install the bleeding edge (pre-release versions) by cloning this
repository and running ``pip install . --upgrade`` in the main directory or

.. code-block:: bash

    pip install git+https://github.com/pangeo-data/climpred.git



**Getting Started**


* :doc:`why-climpred`
* :doc:`scope`
* :doc:`quick-start`
* :doc:`examples`

.. toctree::
    :maxdepth: 1
    :hidden:
    :caption: Getting Started

    why-climpred
    scope
    quick-start.ipynb
    examples

**User Guide**

* :doc:`setting-up-data`
* :doc:`prediction-ensemble-object`
* :doc:`alignment`
* :doc:`metrics`
* :doc:`comparisons`
* :doc:`significance`
* :doc:`bias_removal`
* :doc:`smoothing`
* :doc:`terminology`
* :doc:`reference_forecast`

.. toctree::
    :maxdepth: 2
    :hidden:
    :caption: User Guide

    setting-up-data
    prediction-ensemble-object.ipynb
    alignment.ipynb
    metrics
    comparisons
    significance
    bias_removal.ipynb
    smoothing
    terminology
    reference_forecast

**Help & Reference**

* :doc:`api`
* :doc:`changelog`
* :doc:`code_of_conduct`
* :doc:`contributing`
* :doc:`contributors`
* :doc:`helpful-links`
* :doc:`publications`
* :doc:`related-packages`
* :doc:`release_procedure`

.. toctree::
    :maxdepth: 1
    :hidden:
    :caption: Help & Reference

    api
    changelog
    code_of_conduct
    contributing
    contributors
    helpful-links
    publications
    related-packages
    release_procedure
