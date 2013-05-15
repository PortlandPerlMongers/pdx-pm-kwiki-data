This page describes the wiki markup language used by this kwiki.  For a more general help, see KwikiHelpIndex.

---

# Level 1 Heading (H1)

    = Level 1 Heading (H1) =

---

## Level 2 Heading (H2)

    == Level 2 Heading (H2) ==

---

### Level 3 Heading (H3)

    === Level 3 Heading (H3) ===

---

#### Level 4 Heading (H4)

    ==== Level 4 Heading (H4)

---

##### Level 5 Heading (H5)

    ===== Level 5 Heading (H5)

---

###### Level 6 Heading (H6)

    ====== Level 6 Heading (H6)

---

The horizontal lines in this page are made with 4 or more dashes:
  ----
----
Paragraphs are separated by a blank line.

Like this. Another paragraph.
  Paragraphs are separated by a blank line.

    Like this. Another paragraph.

---

**Bold text**, /italic text/, and _underscore text_.
  **Bold text**, /italic text/, and _underscore text_.
/**Combination of bold and italics**/
  /**Combination of bold and italics**/
Inline code like [=/etc/passwd][] or [=CGI::Kwiki][]
  Inline code like [=/etc/passwd][] or [=CGI::Kwiki][]
----
WikiLinks are formed by two or more words in /camel-case/.
  WikiLinks are formed by two or more words in /camel-case/.
External links begin with http://[][][][][][][][]mailto:mailto:

http://www.google.com/images/logo.gif

* foo
* bar* boom
* bam


* baz

    * foo
    * bar
    ** boom
    ** bam
    * baz

---

Ordered lists begin with a '0 ' (zero):
0 foo
0 bar
00 boom
00 bam
0 baz
  0 foo
  0 bar
  00 boom
  00 bam
  0 baz
----
You can mix lists too:

* Today:

00 Eat icecream
00 Buy a pony

* Tommorrow:

00 Eat more icecream
00 Buy another pony
  * Today:
  00 Eat icecream
  00 Buy a pony
  * Tommorrow:
  00 Eat more icecream
  00 Buy another pony
----
Any text that does not begin in the first column is rendered as preformatted text.
      foo   bar
       x     y
       1     2
----
You can comment out wiki-text with '# ' at the beginning of a line. This will make the text an html comment:

1. These lines have been 
1. commented out

    # These lines have been 
    # commented out

---

Simple Tables:

|  | Dick | Jane |
| height | 72" | 65" |
| weight | 130lbs | 150lbs |


    |        | Dick   | Jane |
    | height | 72"    | 65"  |
    | weight | 130lbs | 150lbs |

---

Tables with multiline or complex data:

| <<END | <<END |


This data has vertical | bars |
END

1. This is some Perl code:

sub foo {
    print "I want a kwiki!\n"
}
END

| foo | <<MSG |


As you can see we use
the Perl heredoc syntax.
MSG
  | <<END | <<END |
  This data has vertical | bars |
  END
  # This is some Perl code:
  sub foo {
      print "I want a kwiki!\n"
  }
  END
  | foo | <<MSG |
  As you can see we use
  the Perl heredoc syntax.
  MSG
