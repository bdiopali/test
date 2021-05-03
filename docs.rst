Titre
=====================

Simple pygame implementation of Conway's Game of Life.

.. contents::

.. code:: 

    from jyquickhelper import add_notebook_menu
    add_notebook_menu()
    
    def topk_min(ens, k):
    "Retourne les k plus petits éléments d'un ensemble."

    heap = ens[:k]
    _heapify_max_bottom(heap)

    for el in ens[k:]:
        if el < heap[0]:
            heap[0] = el
            _heapify_max_up(heap)
    return heap

    

Screenshot
----------

.. image:: screenshots/screenshot.png


Installation
------------

Install with pip::

  pip install nanolife

Install from source::

  python setup.py install


Running
-------

Run via launch script installed with pip package::

  nanolife

Run as a Python module::

  python -m nanolife

Using inside of code
--------------------

To import the class in to your own code::

  from nanolife.LifeGame import LifeGame
  LifeGame().run()


Controls
--------

There are a couple keybinds available:

- q - Quit
- s - Start/stop (toggle pause)
- r - Randomize the grid

Links
-----------

- https://github.com/DevDungeon/NanoLifePy
- https://pypi.org/project/nanolife/

Contact
-------

NanoDano <nanodano@devdungeon.com>
