# Ocean

This is a fork of Numix, a modern flat theme of [Numix Project](https://numixproject.org/), adapted to use the [Base 16 Ocean](http://chriskempson.github.io/base16/#ocean) colour scheme.

## Installation

The [Sass](http://sass-lang.com/) compiler is required to build the theme. To install Sass, first install Ruby with RubyGems and then install `sass` with `gem install sass`.

You'll also need `glib-compile-schemas` and `gdk-pixbuf-pixdata` in your path to generate the gresource binary. On Debian, those can be installed by the following command:

```sh
sudo apt-get install libglib2.0-dev libgdk-pixbuf2.0-dev libxml2-utils
```

After installing all the dependencies, switch to the cloned directory and, run the following:

```sh
make
sudo make install
```

## For developers

If you want to hack on the theme, make sure you have the `inotifywait` command available, which is used for watching and automatically building the files.

To start watching for changes, run the following,

```sh
make watch
```

If you change any assets, you'll need to regenerate the `gtk.gresource.xml` and `gtk.gresource` files. You can use [grrr](https://github.com/satya164/grrr) to do it easily.

## Requirements

 * GTK+ 3.16 or above
 * Murrine theme engine
