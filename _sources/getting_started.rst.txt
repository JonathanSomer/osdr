Getting Started
===============

Requirements
----------------

Make sure you have Python 3.10 or higher installed.

.. code-block:: bash
    
    python --version

[Optional] setup and activate a new virtualenv:


Mac / Linux:

.. code-block:: bash

    python -m venv .venv
    source .venv/bin/activate

Windows:

.. code-block:: batch

    python -m venv .venv
    .venv\Scripts\activate


Installation
--------------------------------------


.. rubric:: Option 1: Install the package from Github (recommended)

.. code-block:: bash

    pip install git+https://github.com/JonathanSomer/osdr.git

.. rubric:: Option 2: Install the package locally for development

The following commands will clone the repo and install the ``tdm`` package locally:

.. code-block:: bash
    
    git clone git@github.com:JonathanSomer/osdr.git
    pip install -e ./osdr

.. note::

    The ``-e`` flag is used to install the package in editable mode, which allows you to make changes to the code and have them reflected in the installed package without needing to reinstall.

.. tip::

    You can clone the repo into any directory, just make sure to modify the path ``./osdr`` provided to the ``pip install`` command.


Testing the installation
--------------------------------------

After installation the following command should display the value ``1e-06``:

.. code-block:: bash

    python -c "from tdm.utils import microns; print(microns(1))"


Next steps
----------------

Proceed to the :ref:`examples` section to run some examples.




