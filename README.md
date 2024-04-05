# gs-plugin-ultramarine-pkgdb-collections

A GNOME Software plugin for the ultramarine pkgdb collections, allowing for system upgrades between major UM versions.
This is a soft fork of the in-tree module used for [Fedora](https://gitlab.gnome.org/GNOME/gnome-software/-/blob/main/plugins/fedora-pkgdb-collections). We basically just renamed the symbols from "fedora" to "ultramarine" and updated the URL to use our own "pkgdb collections" API.

Major thanks to https://github.com/Cogitri/gnome-software-plugin-apk, which I referenced in order to make this module work out-of-tree.

The plan is to have this module as a stop gap for upgrading from 39 -> 40, and work with upstream to develop an better solution for subsequent upgrades. Ideally something that all Fedora derivatives could use.
