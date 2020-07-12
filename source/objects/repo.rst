
.. _repo:

Repository Object
=================

A Repository object defines a repository, from where artifacts can be taken in an Addonscript file.

Example Repository object:
##########################

.. code-block:: JSON

    {
        "id": "coolmaven",
        "type": "maven",
        "url": "maven.example.com/coolmaven"
    }

Repository object members:
##########################

- id: This is a string, which defines the ID of the repository. This should be unique to an Addonscript file.
- type: This is a string, which defines the type of the repository. It can be maven or curseforge.
- url: This is a string, which defines the URL to the repository. You don't need this, if you are using curseforge as your type.


.. _artifact:

Artifacts
#########

Artifacts are files inside a repository. In a maven repository an artifact looks like this: package:artifact:version. In a curseforge repository it looks like this: curse:projectid:fileid.


