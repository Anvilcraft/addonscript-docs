
.. _vrange:

Version Range
=============

A version range defines a collection of versions.

Examples
########
:[1;3]: All versions from versionid 1 to versionid 3 are included.
:]6]: All versions, that are older than versionid 6 including versionid 6 are included.
:[6[: All versions, that are newer than versionid 6 including versionid 6 are included.
:\*: All versions are included.


.. _context:

Context
=======

A context defines, when an external Addonscript file should be used.

Examples
########

:1\:lite: It will be used, when the versionid is 1 and the edition is lite.
:1: It will be used, when the versionid is 1.
:lite: It will be used, if the edition is lite.
:\*: It will always be used.

.. _apply:

Apply
=====

Currently not available.

