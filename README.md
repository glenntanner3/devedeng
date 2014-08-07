# DEVEDE NG #

## WHAT IS IT? ##

Devede NG is a rewrite of the Devede DVD disc authoring program. This new
code has been writen from scratch, and uses Python 3 and Gtk3. It is also
cleaner, which will allow to add new features in the future.


## INSTALLING DEVEDE NG ##

Just type:

	sudo ./setup.py install


## USING DEVEDE NG ##

The first alpha version of Devede NG is very similar to the old devede, with the
exception that, when creating a DVD disc, there are no more "titles" and
"files". Instead, you just add files to the disc. It also lacks support for Mencoder,
and can use only FFMpeg or AVConv for video conversion.

The current visible changes are quite small in number:

* Now allows to add several files at once
* Now makes better use of multicore systems by parallelizing the conversion of several movie files
* The menu edition is interactive
* Has a new "cut" resizing method, to allow to store as widescreen movies with black bars
* Allows to create Matroska files with H.264 video and MP3 audio
* Allows to use VLC or MPlayer for preview
* Allows to choose between Brasero or K3B for burning the discs


## THINGS TO DO ##

Some of the future ideas to add to Devede NG are, without an specific order:

* allow to set properties for several files in one step
* add more backends
* add more output formats
* allow to replace the movie's audio track with one or several MP3 or OGG audio files


## History of versions ##
* version XXXXX
    * Added two-pass conversion
    * Now detects separately MKISOFS and GENISOIMAGE, allowing to have only one of them installed in the system
    * Now checks that the number of files is smaller than the limit for DVD projects
    * Now uses GLib for DBus instead of python-dbus
    * Fixed the DESKTOP file to ensure that an icon is shown in the applications menu
* version 0.1 alpha 1 (2014-08-06)
    * First public version

## CONTACTING THE AUTHOR ##

Sergio Costas Rodriguez
(Raster Software Vigo)

raster@rastersoft.com

http://www.rastersoft.com

GIT: git://github.com/rastersoft/devedeng.git