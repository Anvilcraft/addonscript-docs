
.. _rel:

Relation Object
===============

A Relation object defines another addon, which is related to your addon. This can be a dependency, an incompatible addon or another addon, which is included in yours for example.

Example Relation object:
########################

.. code-block:: json

    {
        "id": "mod1",
        "file": {},
        "type": "mod",
        "meta": {},
        "options": ["required", "server", "client"]
    }

Relation object members:
########################

- id: This is a string, which defines the ID of this relation. This should be unique to a :ref:`Version object<version>`.
- script: This is a string, which contains a link to an Addonscript file for this relation. Either use this in connection with versions or file.
- versions: This is a string, which defines a :ref:`version range<vrange>` of versions, that can be used as this relation. Either use this in connection with script or file.
- file: This is a :ref:`File Object<file>`, which defines the file of this relation, that should be used. Either use this or script in connection with versions.
- type: This is the type of the relation. It can be mod, modloader or script for example.
- meta: This is a :ref:`Meta Object<meta>`, which contains meta information about this relation. This is optional and if you are using script, this is also useless, because the Addonscript already contains this information.
- options: This is an array of strings where each entry defines an option, which specifies in which context this relation should be used. Read more about this in :ref:`options<option>`.