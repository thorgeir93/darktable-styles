Darktable Custom Styles
=======================
Copy files from `./styles/*` table to `~/.config/darktable/styles/`.

After installing Darktable.
You could run following command:

.. code-block::

    $ rsync -v ./styles/* ~/.config/darktable/styles/

To sync local changes run:


.. code-block::

    $ rsync -v /home/thorgeir/.config/darktable/styles/* styles


Shortcuts
---------
Darktable keeps shortcuts configs in a file called `shortcutsrc`.
Our shortcut config file is located undir this repo root path.

Update current darktable configs with our shortcuts configs:

.. code-block::

    $ rsync -vc --backup --suffix=.backup ./shortcutsrc ~/.config/darktable/shortcutsrc

Update newest changes darktable

.. code-block::

    $ rsync -v ~/.config/darktable/shortcutsrc ./shortcutsrc 




TODO
----

* link the /home/thorgeir/.config/darktable/styles folder to the styles folder in here.
