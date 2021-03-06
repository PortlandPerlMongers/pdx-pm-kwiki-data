CGI::Kwiki is simple yet powerful Wiki environment written in Perl as a CPAN module distribribution. It was written by [[BrianIngerson]].

**This is CGI::Kwiki Version $l**

Changes in this release:

    - RCS Support!!!
    - Changed wiki_link regexps to include '_'
    - Cleaned up html and css (AdamTrickett)
    - Support template/local/ directory
    - Add Login button to edit
    - Added Blog to navbar
    - Change localtime to gmtime
    - Added time to RecentChanges

Changes in this 0.16:

    - Support Page Privacy (Public, Protected, Private)
    - Support administrator login
    - KwikiBlog is a reality
    - Allow uppercase suffixes for urls (.GIF)
    - Display 'Site Index' for empty search (JoergBraukhoff)
    - Display 'Search' as the page_id on a search results page.
    - Bang (!) before bracket ([) negates the usual formatting effect.
    - Defeat browser caching (JoergBraukhoff)
    - Support $ENV{REMOTE_USER} for htaccess (Pardus)

Changes for version 0.15:

    - Support unicode character classes in page names
    - Search searches page names
    - Search is written in Perl now, instead of grep
    - Cookies span sessions
    - Allow ftp:// and irc:// links
    - Allow to create a new page from an old one
    - Dead wiki links use <strike>
    - Stop links from being underlined
    - Allow Wiki links like KWiki
    - Support <H4> <H5> and <H6>
    - Refactored installation and upgrade process
    - Added [#.#] format for $CGI::Kwiki::VERSION

Changes for version 0.14:

    - Works with mod_perl.
    - Preferences works.
    - Support for page metadata.
    - RecentChanges shows who last edited page.
    - Almost all non-perl content is now written to 
      appropriate files. Javascript, CSS etc. Much easier to
      maintain and extend now.
    - Support mailto links and inline code.
    - https links added. Thanks to GregSchueler.
    - ':' added to charset for page names. Suggested by 
      JamesFitzGibbon.
    - Javascript fix reported by MikeArms.
    - Security hole in CGI params fixed. Reported by 
      TimSweetman.
    - Emacs artifact bug fix by HeikkiLehvaslaiho.
    - Cleaned up unneeded <p> tags. Reported by HolgerSchurig
