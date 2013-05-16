# Hands on Perl 6

    Wed. October 8th, 6:53pm at FreeGeek -- 1731 SE 10th Ave.

Come join us for a hands-on session of learning to use Perl 6 and running rakudo.

Jerry Gay of [Rakudo Consulting Group](http://www.rakudoconsulting.com/) will be visiting from Seattle.  Jerry is a key contributor to parrot/rakudo and will be very helpful in understanding what rakudo can do right now and diagnosing any troubles that come up.

We will begin with a quick overview by Jerry and take a few minutes to answer any pressing questions.  Then we break into pairs or small groups and **write code**!

Lots of people will be available to answer questions, and there may be some reading involved.  Whether you want to explore the new OO system and other language features or just want to get a feel for how common tasks would be done in Perl 6 is up to you.

# Preparation

If you can bring a computer, please try to have a running Perl 6 _before_ the meeting so we can avoid getting bogged down in setup issues or derailed by network failure.  Feel free to ask for help on the [[MailingList]] or in [the irc channel](irc://irc.perl.org/#pdx.pm).

If you have a fairly well-equipped development system with Perl 5 and a C compiler, you should have no problems compiling from the svn:

    svn co https://svn.perl.org/parrot/trunk parrot
    cd parrot
    perl Configure.pl
    make perl6

[Binaries](http://www.parrotcode.org/source.html
Downloadable) are also available for many systems (including windows and darwin.)  It would be best to compile the latest code from svn, but the important thing is to **run** Perl 6.

If you cannot bring a computer, please contact [[EricWilhelm]] (ewilhelm at cpan dot org) -- more computers may be available (and we'll be in the uh... room full of computers.)

If you can bring an extra computer, please also contact [[EricWilhelm]].

# Links

[Official Test Suite](http://svn.pugscode.org/pugs/t/spec/
The) is the best place to find real Perl 6 code, much of which is runnable in rakudo.  These tests contain 'fudge' annotations for unsupported constructs and are guaranteed to be current.

[Perl 6 for Perl 5 users](http://perlgeek.de/blog-en/perl-5-to-6/
Moritz's) is a great overview and rather recent.

[Introduction with Examples](http://www.szabgab.com/talks/perl6/
Gabor's) seems to assume a more general audience.

[can I do with Perl 6 Today?](http://www.perlfoundation.org/perl6/index.cgi?what_can_i_do_with_perl_6_today
What) - Examples like Tower of Hanoi, etc.
You can add your code to this after the meeting!

[Syntax File](http://svn.pugscode.org/pugs/util/perl6.vim
Vim) is optional -- just download to your ~_.vim/syntax_ directory.  Perl 5 syntax highlighters will work, but note that Perl 6 pod stops at qr/^=end/ instead of qr/^=cut/.

[post on Rakudo Multi-Method Dispatch](http://use.perl.org/~JonathanWorthington/journal/37430
Jonathan's) has some advanced OO examples.
