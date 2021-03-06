Somewhere on the web, there should be a compendium of useful (or near-useful) Perl Regular Expressions (also called patterns, regexes, and REs). Does it already exist? Until we can link to a more authoritative list from this page, let's put them here.

---

## Regexp::Common

The `Regexp::Common` module provides some commonly-needed patterns. See http://search.cpan.org/~abigail/Regexp-Common-2.113/

---

## The Patterns

Reader beware: Although we do our best to keep these accurate, the [[KwikiFormattingRules]] (and careless editing) may mangle some of these patterns. Use them at your own risk! (And help everybody out: Correct the bugs when you find them.)

These are somewhat modified from the perlfaq, section 4:

| <<NONDIGITS | has nondigits |

_\D_
NONDIGITS

| <<WHOLE | a whole number |

_^\d+$_
WHOLE

| <<INT | an integer |

_^-?\d+$_
INT

| <<SIGNED | an integer which may or may not have a leading + sign |

_^$l?\d+$_
SIGNED

| <<REAL | real number |

_^-?\d+\.?\d*$_
REAL

| <<DECIMAL | decimal (real) number |

/^-?(?:\d+(?:\.\d*)?|
\.\d+)$/x
DECIMAL

| <<FLOAT | C-style float |

/^($l?) (?=\d|\.\d)\d*(\.\d*)?

    ([Ee]([+-]?\d+))?$/x

FLOAT

| <<RBFLOAT | Root beer float |

_\broot\s+beer\b_ &&

    /\bice\s+cream\b/ &&
    /\bstraw\b/

RBFLOAT

---

US/Canada-style phone number with required area code and no "1" prefix:

    /
       \(?     # optional parentheses
         \d{3} # area code required
       \)?     # optional parentheses
       [-\s.]? # separator is either a dash, a space, or a period.
         \d{3} # 3-digit prefix
       [-.]    # another separator
         \d{4} # 4-digit line number
    /x

That pattern was shamelessly stolen from http://www.onlamp.com/pub/a/onlamp/2003/08/21/regexp.html

---

Everything you could possibly need to know about Regexp and newlines
http://ali.as/devel/newlines.html

---

Use this to check for text that **looks** like an email address:

    my $valid_email=1 if $email=~m|^[\w.\-]+\@[\w.\-]+\.\w{2,3}$|;

But beware! Some valid addresses don't match that pattern, through no fault of their owners. Send e-mail to Fred & Barney if you don't believe it:

    Fred and Barney <"fred&barney"@redcat.com>

---

Add more, please!
