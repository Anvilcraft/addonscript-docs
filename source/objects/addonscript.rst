.. _addon:

Addonscript Object
==================

A Addonscript object is your root object, which has to be placed directly into the .json file.

Example Addonscript object:
###########################

.. code-block:: json

    {
        "asversion": 1,
        "id": "addon-id",
        "type": "modpack",
        "meta": {},
        "external": [{}],
        "apply": ["http://example.com/addon.json"],
        "versions": [{}],
        "repositories": [{}]
    }

Addonscript object members:
###########################

- asversion: This is a number, which defines the version of Addonscript you are using.
- id: This is a string, which defines the ID of the addon. If you are using your Addonscript in a repository, the ID must be unique in the repo.
- type: This is a string, which defines the type of your addon. It can be mod, modpack or script for example.
- meta: This is a :ref:`Meta Object<meta>`, which has some meta information about the addon. This is completely optional, so you don't need to define this.
- external: This is an array of :ref:`External Objects<external>`, which are defining some other external Addonscript files for this addon. This is also completely optional and only useful, if you have a very complex addon.
- apply: This is an array of strings, which are links to other Addonscript files, which should be applied to this one. For more information read :ref:`Apply rules<apply>`. This is also optional.
- versions: This is an array of :ref:`Version Objects<version>`. Each entry defines one version of this addon.
- repositories: This is an array of :ref:`Repository Objects<repo>`. Each rentry defines a repository, that can be used for relations of this addon.

.. _external:

External Object
===============

An External object contains information about an external Addonscript file.

Example External object
#######################

.. code-block:: json

    {
        "context": "*",
        "link": "http://example.com/addonscript.json"
    }

External object members:
########################

- context: This is a string, which defines the context in which the external file should be used. Read :def:`context<context>` for more information.
- link: This is a string, which contains a link to the external Addonscript file.


