Running the Jupyter Notebook
=============================

.. _launching_notebook:

Launching *Jupyter Notebook App*
--------------------------------

The :ref:`notebook_app` can be launched by clicking on the *Jupyter Notebook*
icon installed by Anaconda in the start menu (Windows) or by typing in
a terminal (*cmd* on Windows)::

   jupyter notebook

This will launch a new browser window (or a new tab) showing the
:ref:`dashboard`, a sort of control panel that allows (among other things)
to select which notebook to open.

When started, the :ref:`notebook_app` can access only files within its start-up folder
(including any sub-folder). If you store the notebook documents in a subfolder
of your user folder no configuration is necessary.
Otherwise, you need to choose a folder which will contain all the notebooks
and set this as the :ref:`notebook_app` start-up folder.

See below for platform-specific instructions on how to start 
:ref:`notebook_app` in a specific folder.

Change Jupyter Notebook startup folder (Windows)
''''''''''''''''''''''''''''''''''''''''''''''''

- Copy the *Jupyter Notebook* launcher from the menu to the desktop.

- Right click on the new launcher and change the "Start in" field by pasting
  the full path of the folder which will contain all the notebooks.

- Double-click on the *Jupyter Notebook* desktop launcher (icon shows [IPy]) to start the
  :ref:`notebook_app`, which will open in a new browser window (or tab).
  Note also that a secondary terminal window (used only for error logging and  
  for shut down) will be also opened.
  If only the terminal starts, try opening this address with your browser:
  |localhost|.
  
.. |localhost| raw:: html

   <a href="http://localhost:8888/" target="_blank">http://localhost:8888/</a>


Change Jupyter Notebook startup folder (OS X)
''''''''''''''''''''''''''''''''''''''''''''''''

To launch :ref:`notebook_app`:

- Click on spotlight, type ``terminal`` to open a terminal window.

- Enter the startup folder by typing ``cd /some_folder_name``.

- Type ``jupyter notebook`` to launch the :ref:`notebook_app`
  (it will appear in a new browser window or tab).


Shut down the *Jupyter Notebook App*
------------------------------------

In a nutshell, closing the browser (or the tab) **will not close** the
:ref:`notebook_app`. To completely shut it down you need to 
**close the associated terminal**.

In more detail,
the :ref:`notebook_app` is a server that appears in your browser
at a default address (*http://localhost:8888*).
Closing the browser will not shut down the server.
You can reopen the previous address
and the :ref:`notebook_app` will be redisplayed.

You can run many copies of the :ref:`notebook_app` and they will show
up at a similar address (only the number after ":", which is the port, 
will increment for each new copy).
Since with a single :ref:`notebook_app` you can already open many notebooks, 
we do not recommend running multiple copies of :ref:`notebook_app`.


.. _kernel_shutdown:

Close a notebook: *kernel* shut down
------------------------------------

When a notebook is opened, its "computational engine" (called the :ref:`kernel`)
is automatically started. 
Closing the notebook browser tab, will not shut down the :ref:`kernel`, 
instead the kernel will keep running until is explicitly shut down. 

To shut down a kernel, go to the associated notebook
and click on menu *File* -> *Close and Halt*. Alternatively, the :ref:`dashboard` 
has a tab named *Running* that shows all the running notebooks (i.e. kernels)
and allows shutting them down (by clicking on a *Shutdown* button).

Executing a notebook
--------------------

Download the notebook you want to execute and put it in your
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
  
More information on editing a notebook:

- `Notebook Basics <http://nbviewer.jupyter.org/github/jupyter/notebook/blob/master/docs/source/examples/Notebook/Notebook%20Basics.ipynb>`_
  (or `alternate link <https://github.com/jupyter/notebook/blob/master/docs/source/examples/Notebook/Notebook%20Basics.ipynb>`_)

.. note::

    **Save notebooks**: modifications to the notebooks are automatically saved every
    few minutes. To avoid modifying the original notebook, make a 
    copy of the notebook document (menu *File -> Make a copy ...*) and 
    save the modifications on the copy.


.. warning::

    Pay attention to not open the **same** notebook document 
    on **many tabs**: edits on different tabs can overwrite each other!
    To be safe, make sure you open each notebook document in only one tab.
    If you accidentally open a notebook twice in two different tabs, just 
    close one of the tabs.

More info on the :ref:`notebook_app` environment see :ref:`references`.
