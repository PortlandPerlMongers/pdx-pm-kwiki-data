Kwiki allows the administrator of the website to set a privacy level on each page. There are 3 privacy levels:

* Public - Anyone can read or edit the page.
* Protected - Anyone can read, but only the administrator can edit.
* Private - Only the administrator can read or edit.

By default, all pages are public.

---

### Installation

You need to turn on the privacy feature. It is not installed by default. To do so simply type this command:

    kwiki-install --privacy

inside your Kwiki installation directory.

---

### Server Configuration

You'll also need to modify your web server configuration to make the program `admin.cgi` protected by an authentication scheme. Here's an example of how you might do it with Apache:

    Alias /kwiki/ /home/ingy/kwiki/
    <Directory /home/ingy/kwiki/>
        Order allow,deny
        Allow from all
        AllowOverride None
        Options ExecCGI
        AddHandler cgi-script .cgi
        <Files admin.cgi>
            Require user admin
            AuthType Basic
            AuthName Restricted
            AuthUserFile /home/ingy/kwiki/passwd
        </Files>
    </Directory>

You'll also need to set the administrative password. With Apache you can simply do this:

    htpasswd -bc passwd admin foo

which will set the `admin` password to `foo`.

---

### Administration

To login as the site administrator, go to [admin.cgi](http:admin.cgi) instead of [index.cgi](http:index.cgi). If everything is set up correctly, you should be prompted for a password.

Enter `admin` for the username and `foo` (or whatever password you selected) for the password.

After you've logged in, you should be able to set the privacy level on pages when you edit them.
