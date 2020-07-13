
.. _file:

File Object
===========

A File object defines a specific file of a version.

Example File object
####################

.. code-block:: json

    {
        "id": "overrides",
        "installer": "internal:overrides",
        "link": "http://example.com/overrides.zip",
        "path": "TODO",
        "artifact": "TODO",
        "options": ["required", "server", "client"]
    }

File object members
####################

:id: This is a string, which defines the ID of the file. If there are multiple files with the same ID they are interpreted as the same file. In this case the installer will try the first file defined with this ID and if that fails, it will try the next one. If this File object is part of a :ref:`Relation Object<rel>`, you don't need to define an ID.
:installer: This is a string, which defines which installer should be used to install this file. Read more about this in :ref:`Installers<installers>`.
:link: This is a string, which contains a link to the file. You can either use this or path or artifact to specify the file.
:path: This is a string, which contains a relative path to a file or directory, which is this file. This can only be used, if you are distributing your Addonscript file inside a zip file. You can either use this or link or artifact.
:artifact: This is a string, which contains an artifact identifier of an artifact from a :ref:`repository<repo>`. Read more about this in :ref:`artifacts<artifact>`.
:options: This is an array of strings where each entry defines an option, which specifies in which context this file should be used. Read more about this in :ref:`options<option>`.