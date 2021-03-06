Apache's mod_perl makes Perl applications run much faster and scale well to heavy usage. Using Kwiki with mod_perl is a piece of cake.

First you need is an Apache server built with mod_perl support. See http://perl.apache.org for more information.

Then install a Kwiki site following the normal [[KwikiInstallation]] procedures.

Finally add something like this to your Apache configuration:

    Alias /kwiki/ /home/ingy/kwiki/
    <Directory /home/ingy/kwiki/>
        Order allow,deny
        Allow from all
        AllowOverride None
        Options None
        SetHandler perl-script
        PerlHandler CGI::Kwiki
    </Directory>
    <Directory /home/ingy/kwiki/css/>
        Order allow,deny
        Allow from all
        AllowOverride None
        Options None
        SetHandler none
    </Directory>
    <Directory /home/ingy/kwiki/javascript/>
        Order allow,deny
        Allow from all
        AllowOverride None
        Options None
        SetHandler none
    </Directory>

That's it! You'll get an instant **performance boost**.

You can switch from the standard CGI installation to mod_perl anytime you want.
