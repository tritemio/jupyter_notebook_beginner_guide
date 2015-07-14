Running the Jupyter Notebook
=============================

.. _launching_notebook:

Launching *Jupyter Notebook App*
--------------------------------

The :ref:`notebook_app` can be launched by clicking on the *IPython Notebook*
icon installed by Anaconda in the start menu (Windows) or by typing in
a terminal (*cmd* on Windows)::

   ipython notebook

This will launch a new browser window (or a new tab) showing the
:ref:`dashboard`, a sort of control panel that allows (among other things)
to select which notebook to open.

When started, the :ref:`notebook_app` can access only files within its start-up folder
(including any sub-folder). If you store the notebook documents in a subfolder
of your user folder no configuration is necessary.

Otherwise, you need to choose a folder which will contains all the notebooks
and set this as the :ref:`notebook_app` start-up folder.

See below for platform-specific instructions on how to start 
:ref:`notebook_app` in a specific folder.

Change Jupyter Notebook startup folder (Windows)
''''''''''''''''''''''''''''''''''''''''''''''''

- Copy the *IPython Notebook* launcher from the menu to the desktop.

- Right click on the new launcher and change the "Start in" field by pasting
  the full path of the folder which will contains all the notebooks.

- Double-click on the *IPython Notebook* desktop launcher (icon shows [IPy]) to start the
  :ref:`notebook_app`, which will open in a new browser window (or tab).
  Note also that a secondary terminal window (used only for error logging and  
  for shut down) will be also opened.
  If only the terminal starts, try opening this address with your browser:
  |localhost|.
  
.. |localhost| raw:: html

   <a href="http://localhost:8888/" target="_blank">http://localhost:8888/</a>


Change Jupyter Notebook startup folder (OSX)
''''''''''''''''''''''''''''''''''''''''''''''''

To launch :ref:`notebook_app`:

- Click on spotlight, type ``terminal`` to open a terminal window.

- Enter the startup folder by typing ``cd /some_folder_name``.

- Type ``ipython notebook`` to launch the :ref:`notebook_app`
  (it will appear in a new browser window or tab).


Shutting down: *Jupyter Notebook App* and *kernels*
---------------------------------------------------

In a nutshell, closing the browser (or the tab) **will not close** the
:ref:`notebook_app`. To shut it down you need to **close the associated terminal**.

More in details,
the :ref:`notebook_app` is a server that appears in your browser
at a default address (*http://localhost:8888*).
Closing the browser will not shut down the server.
You can reopen the previous address
and the :ref:`notebook_app` will be redisplayed.
In addition, each notebook has an "execution engine" (called the :ref:`kernel`)
that is started when the notebook is opened. 
The :ref:`dashboard` allows shutting-down
notebook :ref:`kernels <kernel>` or opening new notebooks.

You can run many copies of the :ref:`notebook_app` and they will show
up at a similar address (only the number after ":", which is the port, 
will increment for each new copy).

Since with a single :ref:`notebook_app` you can already open many notebooks, 
we do not recommend running multiple copies of :ref:`notebook_app`.

Running a notebook
------------------

Download the notebook you wan to execute and put it in your
notebook folder (or a sub-folder of it).

Then follow these steps:

- Launch the :ref:`notebook_app` (see :ref:`previous section <launching_notebook>`).

- In the :ref:`dashboard` navigate to find the notebook:
  clicking on its name will open it in a new browser tab.

- Click on the menu *Help -> User Interface Tour* for an overview
  of the :ref:`notebook_app` user interface.

- You can run the notebook document step-by-step (one cell a time) by pressing
  *shift + enter*.

- You can run the whole notebook in a single step by clicking on the menu
  *Cell -> Run All*.

- To restart the :ref:`kernel` (i.e. the computational engine), click on the menu
  *Kernel -> Restart*. This can be useful to start over a computation from
  scratch (e.g. variables are deleted, open files are closed, etc...).

.. note::

    **Save notebooks**: modifications to the notebooks are automatically saved every
    few minutes. To avoid modifying the original notebook, make a 
    copy of the notebook document (menu *File -> Make a copy ...*) and 
    save the modifications on the copy.

.. note::

    **Close notebooks**: Closing the browser will not shut down the :ref:`kernel`.
    The notebook document can be reopened and it will be still running.
    To "close the notebook document" and "shut-down the kernel" use the menu
    *File -> Close and Halt*. A this point the notebook and its computational
    kernel are shutted down. The
    :ref:`notebook_app` is still running and can open new notebooks.

.. warning::

    Pay attention at opening the **same** notebook document 
    on **many tabs**: edits on different tabs can overwrite each other!
    To be safe, make sure you open each notebook document in only one tab.
    If you accidentally open a notebook twice in two different tabs, just 
    close one of the tabs.

More info on using the :ref:`notebook_app` environment:

- `Jupyter Notebook documentation <http://ipython.org/notebook.html>`_

- `What is the IPython Notebook? <http://nbviewer.ipython.org/github/jupyter/strata-sv-2015-tutorial/blob/master/00%20-%20Introduction.ipynb>`__
