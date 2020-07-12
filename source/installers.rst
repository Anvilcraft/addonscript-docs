
.. _installers:

Installers
==========

Installers define, how a file should be installed. Currently only the internal installers are available, but in the future there may be support for custom python installers.

Internal Installers:
####################

- internal.dir:<relative dir path> moves the file to the relative path inside the Minecraft directory.
- internal.override extracts a zip or moves all subdirs of the file or directory into the Minecraft directory.
- internal.unzip:<relative dir path> unzips a zip file to the relative path inside the Minecraft directory.
- internal.jar adds the contents of the jar or zip file to the minecraft.jar or the minecraft_server.jar.
- internal.modloader:<modloader id>-<modloader version> installs a modloader. Fabric and Forge are supported.

