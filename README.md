python-liborigin2
---------------------

This code is an (almost) standalone library for reading OriginLab project files.

It is based on the code at
	http://sourceforge.net/projects/liborigin
	http://soft.proindependent.com/liborigin2

AUTHORS:  Stefan Gerlach, Ion Vasilief, Alex Kargovsky

Dependencies
---------------------------------------------------------------------------
To compile, liborigin (still) depends on
		BOOST C++ libraries  http://www.boost.org/
			boost/algorithm/string.hpp, boost/variant.hpp and its dependencies.
		tree.hh (included) http://tree.phi-sci.com/
		Note that the BOOST libraries are not needed at run time,
		neither are linked in the executable.

Compiling
---------------------------------------------------------------------------
liborigin uses CMake for the building process.
CMake is available at http://www.cmake.org/

After installing CMake and the BOOST C++ library headers on your system, issue the following commands
to build .a liborigin2 library:

    $ mkdir build
    $ cd build
    $ cmake ../
    $ make
    $ make install
    $ cd ..

To build Python module, just type

    $ python setup.py build_ext --inplace

Features
---------------------------------------------------------------------------
 * supports the import of 6.0 - 8.1 projects
---------------------------------------------------------------------------
