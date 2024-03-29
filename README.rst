EasyBO
======

.. inclusion-marker-easybo-begin

**Warning: this work is still in pre-release and breaking changes wil be common!**

**EasyBO** is a Python library designed to make Bayesian optimization and Gaussian Process modeling really `easy`! 

Plenty of excellent codes already exist to perform Bayesian optimization and Gaussian Process surrogate modeling. For Gaussian Processes, these involve in no particular order, these include `scikit learn <https://scikit-learn.org/stable/modules/gaussian_process.html>`__, `GPyTorch <https://gpytorch.ai>`__, `GPCam <https://gpcam.readthedocs.io/en/latest/index.html>`__, and many others. There's even a `Wikipedia page <https://en.wikipedia.org/wiki/Comparison_of_Gaussian_process_software>`__ dedicated to documenting the different codes and their various strengths and weaknesses. In the space of Bayesian optimization there are e.g. `GPyOpt <https://sheffieldml.github.io/GPyOpt/>`__, `BoTorch <https://botorch.org>`__, and some others.

**EasyBO** does not set out to solve any new problems, it aims to make existing software and methods much more accessible to the common user. Many existing codes for Gaussian Process-based Bayesian optimization have extremely complex APIs and can be difficult for new users to pick up. **EasyBO** aims to solve this problem with documentation and tutorials `ad nauseam`, allowing new users who wish to perform e.g. autonomous experimentation to pick it up quickly.

To do this, **EasyBO** wraps two excellent libraries:

- `GPyTorch <https://gpytorch.ai>`__: for Gaussian Process modeling
- `BoTorch <https://botorch.org>`__: for the Bayesian optimization engine

These codes are well maintained and widely used. They also offer very nice features out of the box, such as compatibility with PyTorch models, GPU acceleration and the Monte Carlo backend engine of BoTorch for joint optimization.

For relatively simple cases (which will be clearly outlined in the tutorials and documentation to come), **EasyBO** can be used. However, for more complicated use cases or advanced users, we do recommend diving into these two codes and using them directly, since the downside of our simplified API is that not `all` features are directly or obviously exposed.

.. inclusion-marker-easybo-end

.. inclusion-marker-easybo-installation-begin

Installation
------------

Users
^^^^^
To simply use the software, install it as you would any Python package: `pip install EasyBO`. **COMING SOON!**

Developers
^^^^^^^^^^
If you wish to help us improve EasyBO, you should fork a copy of our repository, clone to disk, and then proceed with setting up the following:

- Create a fresh virtual environment, e.g. ``conda create -n py3.9 python=3.9``.
- Install the development requirements, ``pip install -r requirements-dev.txt``
- Setup the pre-commit hooks ``pre-commit install``
- If you want to install the package to your default paths, you can do this in "developer mode" by running ``pip install -e ".[dev]"``

.. inclusion-marker-easybo-installation-end

Funding acknowledgement
-----------------------

.. inclusion-marker-easybo-funding-begin

This material is based upon work supported by the U.S. Department of Energy, Office of Science at Brookhaven National Laboratory under Contract No. DE-SC0012704. This research is also supported by the BNL Laboratory Directed Research and Development Grant No. 22-059.

Disclaimer
^^^^^^^^^^

The Software resulted from work developed under a U.S. Government Contract No. DE-SC0012704 and are subject to the following terms: the U.S. Government is granted for itself and others acting on its behalf a paid-up, nonexclusive, irrevocable worldwide license in this computer software and data to reproduce, prepare derivative works, and perform publicly and display publicly.

THE SOFTWARE IS SUPPLIED "AS IS" WITHOUT WARRANTY OF ANY KIND. THE UNITED STATES, THE UNITED STATES DEPARTMENT OF ENERGY, AND THEIR EMPLOYEES: (1) DISCLAIM ANY WARRANTIES, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, TITLE OR NON-INFRINGEMENT, (2) DO NOT ASSUME ANY LEGAL LIABILITY OR RESPONSIBILITY FOR THE ACCURACY, COMPLETENESS, OR USEFULNESS OF THE SOFTWARE, (3) DO NOT REPRESENT THAT USE OF THE SOFTWARE WOULD NOT INFRINGE PRIVATELY OWNED RIGHTS, (4) DO NOT WARRANT THAT THE SOFTWARE WILL FUNCTION UNINTERRUPTED, THAT IT IS ERROR-FREE OR THAT ANY ERRORS WILL BE CORRECTED.

IN NO EVENT SHALL THE UNITED STATES, THE UNITED STATES DEPARTMENT OF ENERGY, OR THEIR EMPLOYEES BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, CONSEQUENTIAL, SPECIAL OR PUNITIVE DAMAGES OF ANY KIND OR NATURE RESULTING FROM EXERCISE OF THIS LICENSE AGREEMENT OR THE USE OF THE SOFTWARE.

.. inclusion-marker-easybo-funding-end
