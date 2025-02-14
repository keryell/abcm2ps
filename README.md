<style>
p{margin-left:.5cm;max-width:21cm}
li{margin-left:.5cm;max-width:18cm}
li p{margin-left:0}
</style>
# abcm2ps

### Overview

abcm2ps is a C program which converts music tunes from the ABC music notation
to PostScript or SVG.

Based on [abc2ps](https://github.com/methf/abc2ps),
the Postscript generator for ABC music notation by Michael Methfessel,
abcm2ps was first developped to print barock organ scores that have independant
voices played on one or many keyboards and a pedal-board
(the 'm' of abcm2ps stands for many or multi staves/voices).
Since this time, it has evolved so it can render many more music types.

Note that this program is at end of life. Its successor is
[abc2svg](https://chiselapp.com/user/moinejf/repository/abc2svg).

### Features

The features of abcm2ps are based on the
[ABC draft 2.2 (February 2013)](http://abcnotation.com/wiki/abc:standard:v2.2).
The differences are listed in the
[abcm2ps/abc2svg documentation](http://moinejf.free.fr/abcm2ps-doc/features.html).

### Installation and usage

The installation procedure is described in the file INSTALL.
To build the program with default settings run

```
    ./configure
    make
```

Basically, the program usage is:

    abcm2ps [options] file1 [file1_options] file2 [file2_options] ...

where file1, file2, .. are the ABC input files.
This generates a Postscript file (default name: `Out.ps`).

Run `abcm2ps -h` to know the list of the command line options.

### Documentation

- The file abcm2ps.rst describes all command-line options.

  When `abcm2ps` is installed, this file may be displayed by `man abcm2ps`.

- The features and format parameters are described in
    [abcm2ps-doc](http://moinejf.free.fr/abcm2ps-doc/index.html).

### Links

Author's page: [http://moinejf.free.fr/](http://moinejf.free.fr/)

To know more about the ABC music notation, have a look at
    [abcnotation](https://abcnotation.com/).

Guido Gonzato maintains many abcm2ps binaries and more documentation at
    [abcplus](https://abcplus.sourceforge.net/).
