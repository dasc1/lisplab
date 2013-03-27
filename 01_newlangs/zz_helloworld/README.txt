
Challenge: zz_helloworld

First of all, we must install Common Lisp:

CLISP / UBUNTU LINUX
====================

CLISP is the Gnu implementation of Common Lisp.  It is available in the
repositories, so you can install it with a simple apt-get command:

  >>> sudo apt-get install clisp

You can invoke the REPL from the command line, simply type "clisp" with
no arguments, and you are in.  Type (quit) to exit the REPL when you
are finished.

====================

From the REPL, you can execute the following command to print
"Hello, World!" to the screen:

  [1]> (princ "Hello, World!")

I have also saved this command into a text file "helloworld.lisp" in
this directory.  You can run the program by typing at the command line:

  >>> clisp helloworld.lisp

