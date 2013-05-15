    Thursday, December 13th, 6:53pm at FreeGeek – 1731 SE 10th Ave.

# Prime Number Generation in Perl

speaker: Dana Jacobsen

Dana will give a brief introduction to primes, primality testing, and sieves, then show examples in Perl.  Dana is the author of the [Math::Prime::Util](https://metacpan.org/module/Math::Prime::Util) module on [CPAN](http://www.cpan.org/).  Outline:

* Primes
* Applications
* Primality testing in Perl
* Sieves
* 15 sieve implementations in Perl including a new string-based sieve
* 6 CPAN modules
* Performance and memory use
* Prime Counting

Sadly a lot of the [web](http://rosettacode.org/wiki/Sieve_of_Eratosthenes#Perl) [examples](http://www.scriptol.com/programming/sieve.php) [of](http://dada.perl.it/shootout/sieve.perl.html) [Perl](http://www.stonehenge.com/merlyn/UnixReview/col26.html) [sieves](http://cpansearch.perl.org/src/ZIGDON/Math-Prime-TiedArray-0.04/lib/Math/Prime/TiedArray.pm) are quite bad, often 3-6x slower than Perl can do.  [We can do better!](https://gist.github.com/4162676)   There are also a number of CPAN modules related to primes, which will briefly be covered.
