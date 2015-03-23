Vagrantfile for building Spigot
====================

Here lies the [Vagrantfile](https://docs.vagrantup.com/v2/vagrantfile/index.html) required to build [Spigot](http://www.spigotmc.org/wiki/spigot-installation/) for a super-awesome Minecraft server experience.

Requirements
--------------
* [Vagrant](https://www.vagrantup.com/)
* [VirtualBox](https://www.virtualbox.org/)

Spigot Requirements
----------------------
* Java 1.7 or 1.8
* Git
* Download of `BuildTools.jar`

Instructions
------------
1. Clone this repository
1. run `vagrant up`
1. SSH into vagrant: `vagrant ssh`
1. Follow the directions over at [Spigot](http://www.spigotmc.org/threads/buildtools-updates-information.42865/)
1. When the build is complete, copy the `craftbukkit-*.jar` and `spigot-*.jar` (i.e. - `craftbukkit-1.8.3.jar` and `spigot-1.8.3.jar`) files from the directory where you ran the build to` /host_spigot_data` - this folder is mapped to `spigot_data` directory in this repo
1. Copy the `craftbukkit-*.jar and spigot-*.jar` files from the `spigot_data` directory on your vagrant host to your Minecraft server location
1. Follow the directions [here](http://www.spigotmc.org/wiki/spigot-installation/) to start the Spigot server