
Challenge: zz_compileToBytecode

First of all, we must install Common Lisp:

CLISP / UBUNTU LINUX
====================

CLISP is the Gnu implementation of Common Lisp.  It is available in the
repositories, so you can install it with a simple apt-get command:

  >>> sudo apt-get install clisp

====================

In this directory, I have included the source file "helloworld.lisp".  To
compile it, run from the same directory the following command:

  >>> clisp -c helloworld.lisp

This will generate two new files, "helloworld.fas" and "helloworld.lib".

The ".fas" file is the compiled version of the program, and you can
run it with the clisp program directly.  It will obviously run much
faster, as it will skip the compilation step.  Apparently, these .fas
files are also portable across systems, as long as you execute them
with CLISP.  To run the program:

  >>> clisp helloworld.fas

The ".lib" file contains lisp source library information, in other words,
it is a header file.  You DO NOT need it to run a compiled file, but
if your compiled file is a library to be used by other files (via the
REQUIRE command), you need to keep this header file around.  See the
challenges related to libraries for more details.

