.. _meta:

Meta Object
===========

A Meta object contains meta information about an addon. Meta objects are different from other objects, because here you can add custom members, if you need one, that is not predefined.

Example Meta object
###################

.. code-block:: json

    {
        "name": "Addon name",
        "icon": "http://example.com/icon.png",
        "contributors": [{}],
        "website": "http://example.com",
        "description": ["http://exampler.com/description.html", "This is the first line of the description", "This is the second line"]
    }

Meta object members
####################

:name: The name of the addon as a string.
:icon: This is a string, which contains a link to the icon of the addon.
:contributors: This is an array of :ref:`Contributor Objects<contrib>`. Each entry defines one contributor of the addon.
:webiste: This is a string, which contains a link to the website of the addon.
:description: The is an array of strings. Each entry is one line of the description or a link to an external description.

.. _vmeta:

Version Meta Object
===================

Like the :ref:`Meta object<meta>`, a Version Meta object can also contain custom members. It contains meta information about a specific version of an addon.

Example Version Meta object
###########################

.. code-block:: json

    {
        "timestamp": 1594684800,
        "changelog": ["-Added cool stuff", "-Added more cool stuff"]
    }

Version Meta object members
############################

:timestamp: This is a number, which is the UNIX timestamp, when this version was released/created.
:changelog: This is an array of strings, where each member is one line of the changelog or a link to an external changelog.

.. _contrib:

Contributor Object
==================

A Contributor objects contains information about a specific contributor of an addon.

Example Contributor object
##########################

.. code-block:: json

    {
        "name": "Cool Dude",
        "roles": ["owner", "author"]
    }

Contributor object members
###########################

:name: This is a string with the name of the contributor
:roles: This is an array of strings where each entry is a role of the contributor in the addon.
