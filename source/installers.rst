
.. _installers:

Installers
==========

Installers define, how a file should be installed. Currently only the internal installers are available, but in the future there may be support for custom python installers.

.. note::
    Arguments are supplied to installers seperated by a ``:``.
    Example: ``internal.dir:resourcepacks``

Internal Installers
###################

.. csv-table::
    :header-rows: 1

    "Name", "Arguments", "Description"
    "internal.dir", "``<relative dir path>``", "Moves the file to the relative path inside the Minecraft directory."
    "internal.override",, "Extracts a zip or moves all subdirs of the file or directory into the Minecraft directory."
    "internal.unzip", "``<relative dir path>``", "Unzips a zip file to the relative path inside the Minecraft directory."
    "internal.jar",, "Adds the contents of the jar or zip file to the minecraft.jar or the minecraft_server.jar."
    "internal.modloader", "``<modloader id>-<modloader version>``", "Installs a modloader. Fabric and Forge are supported."

