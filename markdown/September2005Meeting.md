## September Meeting

#### Wednesday, September 14th, 2005 6:30pm at Free Geek, 1741 SE 10th Ave

chromatic, Seven Sins of OO Perl

Perl's OO model is flexible and minimal so that capable programmers can
change it to make their problems. Unfortunately, sometimes it's a little
too flexible and minimal. This talk shows why seven too-common practices
are dangerous (or at least wrong) and what to do instead.

In lieu of the slides, here are the seven sins:

0 Don't call methods as functions (especially methods in UNIVERSAL)
0 Don't use AUTOLOAD() to generate methods unless you know the four things you need to do to make it work reliably
0 Don't use indirect object method calls, even for constructors
0 Access instance data directly only from accessor methods
0 Don't forbid inheritance from your classes
0 Use Test::Class to make everyone's life easier
0 Don't use inheritance when aggregation, delegation, roles, or mixins would do

---

Afterwards, as always, beer at the [[LuckyLab]]!
