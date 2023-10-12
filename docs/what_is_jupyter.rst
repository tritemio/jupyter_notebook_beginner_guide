.. _what_is_jupyther:

What is the Jupyter Notebook?
=============================

In this page briefly introduce the main components of the *Jupyter Notebook* 
environment. For a more complete overview see :ref:`references`.

.. contents::

.. _notebook_document:

Notebook document
-----------------

Notebook documents (or "notebooks", all lower case) are documents
produced by the :ref:`notebook_app`, which contain both computer code (e.g. python) 
and rich text elements (paragraph, equations, figures, links, etc...).
Notebook documents are both human-readable documents containing the analysis
description and the results (figures, tables, etc..) as well as executable documents
which can be run to perform data analysis.

**References**: Notebook documents `in the project homepage <http://ipython.org/notebook.html#notebook-documents>`__ and `in the official docs <http://jupyter-notebook.readthedocs.org/en/latest/notebook.html#notebook-documents>`__.

.. _notebook_app:

Jupyter Notebook App
--------------------

The *Jupyter Notebook App* is a server-client application that allows 
editing and running :ref:`notebook documents <notebook_document>`
via a web browser.
The *Jupyter Notebook App* can be executed on a local desktop 
requiring no internet access (as described in this document)
or can be installed on a remote server and accessed through the internet.

In addition to displaying/editing/running notebook documents, 
the *Jupyter Notebook App* has a "Dashboard" (:ref:`dashboard`),
a "control panel" showing local files and allowing to
open notebook documents or shutting down their :ref:`kernels <kernel>`.

**References**: Jupyter Notebook App 
`in the project homepage <http://ipython.org/notebook.html>`__ and
`in the official docs <http://jupyter-notebook.readthedocs.org/>`__.


.. _kernel:

kernel
------

A notebook *kernel* is a "computational engine"
that executes the code contained in a :ref:`notebook_document`.
The *ipython kernel*, referenced in this guide, executes python code. 
Kernels for many other languages exist 
(`official kernels <http://jupyter.readthedocs.org/en/latest/#kernels>`__).

When you open a :ref:`notebook_document`, the associated *kernel* is automatically launched.
When the notebook is *executed* (either cell-by-cell or with menu *Cell -> Run All*),
the *kernel* performs the computation and produces the results.
Depending on the type of computations, the *kernel* may consume significant
CPU and RAM. Note that the RAM is not released until the *kernel* is shut-down.

See also :ref:`kernel_shutdown`.

**References**: from the official docs
`Opening Notebooks <http://jupyter-notebook.readthedocs.org/en/latest/notebook.html#opening-notebooks>`__ and 
`Decoupled two-process model <http://ipython.org/ipython-doc/stable/overview.html#ipythonzmq>`__.

.. _dashboard:

Notebook Dashboard
------------------

The *Notebook Dashboard* is the component which 
is shown first when you launch :ref:`notebook_app`.
The *Notebook Dashboard* is mainly used to open :ref:`notebook documents <notebook_document>`, 
and to manage the running :ref:`kernels <kernel>` (visualize and shutdown).

The *Notebook Dashboard* has other features similar to a file manager, namely
navigating folders and renaming/deleting files.

**References**: from the official docs
`Opening Notebooks <http://jupyter-notebook.readthedocs.org/en/latest/notebook.html#opening-notebooks>`__.

.. _references:

References
----------

Official Jupyter Project Pages:

- `Project Jupyter Homepage <https://jupyter.org/>`__
- `Old IPython Notebook Homepage <http://ipython.org/notebook.html>`__

Official Documentation:

- `Jupyter Notebook Documentation <http://jupyter-notebook.readthedocs.org/>`__
- `Jupyter Project Documentation <http://jupyter.readthedocs.org/>`__

See also:

- `What is the Jupyter Notebook? <https://nbviewer.org/github/jupyter/notebook/blob/main/docs/source/examples/Notebook/What%20is%20the%20Jupyter%20Notebook.ipynb>`__

- `Notebook Basics <https://nbviewer.org/github/jupyter/notebook/blob/main/docs/source/examples/Notebook/Notebook%20Basics.ipynb>`__, an example notebook

- `Jupyter Notebook: The Definitive Guide <https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook>`__, an introductory tutorial to Jupyter


....

The *Next* button will bring you to the next section (*Installation*).
