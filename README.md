Yi
==

Yi is an Android app for Weiqi/Go/Baduk.  It is currently under
development and is expected to have following features:

* An AI player.
* Joseki trainer.
* Tsumego problems.
* SGF editor / viewer.

For more information about Yi, please go to
  <https://github.com/whily/yi>

Wiki pages can be found at
  <https://wiki.github.com/whily/yi>

Development
-----------

The following tools are needed to build Yi from source:

* JDK version 6/7 from <http://www.java.com> if Java is not available.
  Note that JDK is preinstalled on Mac OS X and available via package manager
  on many Linux systems.
* Android SDK r23.0.5.
* Scala (2.11.6)
* sbt (0.13.8)
* [Inkscape](http://inkscape.org) and [ImageMagick](http://www.imagemagick.org)
  to generate icons.

### Generate the icons

In project directory, run following command:

        $ ./genart

### Build the code

The library dependencies include
[scasci](https://github.com/whily/scasci), and
[scaland](https://github.com/whily/scaland).

Please follow the steps discussed in those libraries on how to use them.

To compile/run the code, run the following command to build the
   app and start it in a connected device:

        $ sbt android:run

To build a release version and start it in a connected device:

        $ sbt android:set-release android:run
