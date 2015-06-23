.. _what_is_jupyther:

What is Jupyter Notebook
========================

**Jupyter Notebook App** (formerly **IPython Notebook**) is an application which runs inside your
browser.
For the purpose of this guide, *Jupyter Notebook App* is run locally like a normal desktop
application and does not require accessing any remote server.

"notebooks" (all lower case) are text documents
produced by the *Jupyter Notebook App* which contain both python code and rich text format elements 
(paragraph, equations, figures, links, etc...).
Notebook documents are both human-readable documents containing the analysis
description and the results (figures, tables, etc..) as well as executable documents
which can be run to perform data analysis.

External Links
--------------

Official Jupyter Project Pages:

- `Project Jupyter <https://jupyter.org/>`__
- `IPython Notebook Homepage <http://ipython.org/notebook.html>`__

Some more in-depth (but slightly outdated) introduction:

- `What is the IPython Notebook? <http://nbviewer.ipython.org/github/jupyter/strata-sv-2015-tutorial/blob/master/00%20-%20Introduction.ipynb>`__

Quick Glossary
--------------

.. _notebook_app:

*Jupyter Notebook App*
~~~~~~~~~~~~~~~~~~~~~~

The *Jupyter Notebook App* is a server application that allows 
operating on notebook documents (open, close, run, etc...).
In this guide the *Jupyter Notebook App* is run on a local desktop 
and does not require any internet access.
In addition to displaying/editing/running notebook documents, 
the *Jupyter Notebook App* has a "Dashboard" (:ref:`dashboard`),
a "control panel" showing local files and allowing to
open notebook documents or shuting down their :ref:`kernels <kernel>`.


.. _kernel:

*kernel*
~~~~~~~~

A notebook *kernel* is a "computational engine"
that executes the code contained in a notebook document.
In this guide we always refer to a specific kernel called *ipython kernel* 
that executes python code. 
Kernels for many other languages exists, the *ipython kernel* is the one
for the python language.

When opening a notebook document the associated *kernel* is automatically launched.
When the notebook is *executed* (either cell-by-cell or with menu *Cell -> Run All*)
the *kernel* performs the computation and produces the results.
Depending on the type of computations, the *kernel* may consume significant
CPU and RAM. Note that the RAM is not released until the *kernel* is shut-down.

To shut-down the kernel **is not sufficient to close the tab** where the notebook is.
You have to use the menu *File -> Close and Halt*. Alternatively, the :ref:`dashboard`
highlights notebooks with running kernels and allows to shut them dowm.


.. _dashboard:

*Notebook Dashboard*
~~~~~~~~~~~~~~~~~~~~

The *Notebook Dashboard* is the component of the *Jupyter Notebook App* that is
first shown when the :ref:`notebook_app` is launched.

Mainly, the *Notebook Dashboard* is used to open notebook documents, and to manage
the running :ref:`kernels <kernel>` (visualize and shutdown).

The *Notebook Dashboard* has other features similar to a file manager, namely
navigating folders and renaming/deleting files.

....

The *Next* button will bring you to the next section (*Installation*).
