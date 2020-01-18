*********************
Python Sample Project
*********************

This is a blueprint for a basic python project using the *Pipenv* development
workflow tool. It is intended for projects and apps that you (or your company)
run directly. *Pipenvs* deterministic locking system in the form of
*pipfile.lock* helps with this [#f1]_ .

Project dependencies
####################

With the *Pipenv* installation the following development dependencies are
defined:

* pytest: The defacto standard for testing in Python
* pytest-cov: Additional test coverage reports
* mypy: Optional static type checker for Python
* flake8: Tool for style guide enforcement
* pep8-naming: Checks code against PEP 8 naming conventions
* flake8-import-order: Check import order style
* flake8-quotes: Check quotes -- this project uses "
* black: Code formatter

The runtime dependencies are:

* exitstatus: Provides expressive, portable definitions for the standard POSIX exit codes 


Installation
############

Checkout the repository. To install the development dependencies, run:
::

    pipenv install --dev

To install the dependencies for running the sample program, run:
::

    pipenv install

To run the unit tests of the project, run:
::

    pipenv run test

Credits
#######

The sample code for the factorial implementation is attributed to `johnthagen <https://github.com/johnthagen>`_.

Footnote
########

.. [#f1] If you want to provide you code to others to install it, then you
    should define dependencies as ranges of compatible versions, instead of
    locked versions. Currently the tools for distribution like *Setuptools*,
    *Flit* or *Poetry* do not integrate well with *Pipenv*.
