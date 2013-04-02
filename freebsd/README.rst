This is a draft script for FreeBSD.

Please, install ``Xvfb``::

    cd /usr/ports/x11-servers/xorg-vfbserver
    make install clean

And, for example, you can install FireFox and run it later::

    cd /usr/ports/www/firefox
    make install clean

Install script::

    fetch -o /usr/local/bin/xvfb-run https://raw.github.com/adw0rd/xvfb-run/master/freebsd/xvfb-run
    chmod +x /usr/local/bin/xvfb-run

Examples of launch programs::

    xvfb-run firefox
    xvfb-run python manage.py harvest -S --apps=tests --verbosity=4
