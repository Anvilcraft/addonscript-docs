
.. _version:

Version Object
==============

A Version object defines a specific version of an addon.

Example Version object
######################

.. code-block:: json

    {
        "version": "1.0",
        "versionid": 1,
        "mcversion": ["1.12.2"],
        "meta": {},
        "files": [{}],
        "relations": [{}]
    }

Version object members
######################

:version: This is a string, which defines the name of the version.
:versionid: This is a number, which defines the ID of the version. It is used to compare, which version is newer and which is older and to provide a unique ID for each version. If your Addonscrip file contains only one version you can set this to -1.
:mcversion: This is an array of strings where each entry defines a Minecraft version, which is compatible with this addon version.
:meta: This is an :ref:`Version Meta Object<vmeta>`, which contains meta information about this version, This is optional.
:files: This is an array of :ref:`File Objects<file>` where each entry is a file of this version.
:relations: This is an array of :ref:`Relation Objects<rel>` where each entry defines another addon, that is related to this version.
