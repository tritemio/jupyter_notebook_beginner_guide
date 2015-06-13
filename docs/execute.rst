Running the Jupyter Notebook
=============================

Launching Jupyter Notebook
--------------------------

The Jupyter Notebook App can be launched by clicking on the IPython Notebook
icon installed by Anaconda in the start menu (Windows) or by typing in
a terminal (*cmd* on Windows)::

   ipython notebook

This will launch a new browser window (or a new tab) showing the
Notebook Dashboard, a sort of control panel that allows (among other things)
to select which notebook to open.

When started, Jupyter Notebook can access only files within its start-up folder
(including any sub-folder). If you store the notebooks in a subfolder
of your user folder no configuration is necessary.

Otherwise, you need to choose a folder which will contains all the notebooks
and set this as the Jupyter Notebook start-up folder.

See below for platform-specific instructions on how to start Jupyter Notebook
in a specific folder.

Change Jupyter Notebook startup folder (Windows)
''''''''''''''''''''''''''''''''''''''''''''''''

- Copy the IPython Notebook launcher from the menu to the desktop.

- Right click on the new launcher and change the "Start in" field by pasting
  the folder previously chosen.

- Double-click on the IPython Notebook launcher to start the
  Notebook application. Note that this will open two new windows:
  a terminal (used only for error logging and for shut down) and a new
  browser window showing the Jupyter Notebook application.


Change Jupyter Notebook startup folder (OSX)
''''''''''''''''''''''''''''''''''''''''''''''''

To launch Jupyter Notebook:

- Click on spotlight, type `terminal` to open a terminal window.

- Enter the startup folder by typing ``cd /some_folder_name``

- Type ``ipython notebook``. This will open a new window in your
  default browser showing the content of your home folder.


Shutting down Jupyter Notebook
------------------------------

In a nutshell, closing the browser (or the tab) will not close the
Jupyter Notebook application. To completely shut down Jupyter Notebook
you need to close the associated terminal.

More in details,
the Jupyter Notebook application (the server) appears in your browser
at a default address (*http://localhost:8888*).
Closing the browser will not close the Jupyter Notebook application.
You can reopen the previous address (just start typing *localhost* in the
browser addressbar) and the Jupyter Notebook application will be redisplayed.
In addition, each notebook has an "execution engine" (called the kernel)
that is started when the notebook is opened. The Dashboard allows to shut-down
the notebook kernels or open new notebooks.

You can run many copies of the Jupyter Notebook application and they will show
up at a similar address except that the number (which is the port number)
will increment for each new copy.

For simplicity we do not recommend running multiple copies of Jupyter Notebook.
Note that with a single Jupyter Notebook Application you can as many notebooks
as you like.

Running a notebook
------------------

Download the notebook you wan to execute and put it in your
notebook folder (or a sub-folder of it).

Then follow these steps:

- Launch the Jupyter Notebook (see previous section).

- In the new Jupyter Notebook Dashboard navigate to find the notebook:
  clicking on its name will open it in a new browser tab.

- Click on the menu *Help -> User Interface Tour* for an overview
  of the Notebook environment.

- You can run the notebooks step-by-step (one cell a time) by hitting
  *shift + enter*.

- You can run the whole notebook in a single step by clicking on the menu
  *Cell -> Run All*.

- To restart the notebook computations (the component performing the
  computation is called the kernel), click on the menu
  *Kernel -> Restart*.

.. note::

    Modifications to the notebooks are automatically saved every
    few minutes. It is suggested that you make a copy of the
    original tutorial (menu *File -> Make a copy ...*) and make
    modifications on the copy.

.. note::

    Closing the browser will not shut down the notebook computational kernel.
    The notebook can be reopened and it will be still running.
    To close a notebook and shut-down the kernel use the menu
    *File -> Close and Halt*. A this point the notebook is closed,
    Jupyter Notebook is still running and can open new notebooks.

.. warning::

    Please pay attention that if you open the **same** notebook on many
    tabs and do edits, the edits on different tabs can overwrite each other.
    To be safe, make sure you open each notebook in only one tab.
    If by mistake you open a notebook twice in two tabs, please close one tab.

More info on using the Notebook environment:

- `Jupyter Notebook documentation <http://ipython.org/notebook.html>`_

- `What is the IPython Notebook? <http://nbviewer.ipython.org/github/jupyter/strata-sv-2015-tutorial/blob/master/00%20-%20Introduction.ipynb>`__
