
.. _option:

Options
=======

An option specifies, when a file or relation should be used in a version or how a relation stands to an addon.

List of possible options
########################

:client: this file or relation is for the client.
:server: this file or relation is for the server.
:required: this file or relation is required for this version.
:optional: this file or relation is optional for this version. The user can choose, if they would like to install this.
:incompatible: this relation is incompatible with this version.
:edition\:<edition id>: this file or relation is required for a specific edition of the addon.

.. note::
    If options are left empty, it will use the defaults:

    - ``required``
    - ``client``
    - ``server``