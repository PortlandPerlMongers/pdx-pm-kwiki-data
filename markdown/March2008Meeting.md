### Moose - objects and antlers

Speaker: Ben Hengst

Moose is a cute, fuzzy module (which just happens to share its name with
a big smelly creature.)

Er, it is a postmodern object system which allows you to remove much of
the hairiness from your object-oriented Perl code.  Moose borrows
features from Perl 6, CLOS (LISP), Smalltalk, Java, BETA, OCaml, Ruby
and more.

Ben will present a brief introduction to Moose, followed by an overview
of (and real-world examples from) a database-linked search/results
system built on Moose.

* Saddle the Moose (intro)

    * a perl object system
    * meta syntax for object/class declaration
    * simple example
    * not *that* weird

* Ride the Moose (code in "the real world")

    * Constructors for free
    * BUILD
    * under the hood - the meta() method
    * getters and setters
      * example
      * possible name space collisions
      * 'rw' vs 'ro'
      * timing issues ( lazy => 1 )
    * strict types
      * things die if they are wrong, just like they should (assertion)
    * roles
    * less code to test

* Love the Moose (techniques and practices)

    * composition / modularization / encapsulation
    * layout of logical file structure with roles
      * easier team workflow / merging
    * QA notes
