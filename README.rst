Ncurses
=======

This Go package is a wrapper for the ncurses library.  It provides
access to the ncurses terminal handling library functions.
To use the Go package, you need to have the ncurses library installed.
This must include the header files and the shared library.

Why Fork
--------

This fork fixes the `issue <https://github.com/seehuhn/go-ncurses/issues/3>`` in the original
repository. The problematic line there was indeed commented out. For some reason the author didn't
push an updated version tag after he committed that change. This way ``go get`` currently still
downloads unpatched ``keys.go``, which won't compile.

Installation
------------

This package can be installed using the ``go get`` command::

    go get github.com/pshatov/go-ncurses

Usage
-----

Documentation is available via the package's online help, either on
pkg.go.dev_ or on the command line::

    godoc seehuhn.de/go/ncurses

.. _pkg.go.dev: https://pkg.go.dev/seehuhn.de/go/ncurses
