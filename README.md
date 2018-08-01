dis
========================================================================

Dis is a very, very simple tool for managing Internet distractions
when you're supposed to be working instead of screwing around. It
works by making entries to your /etc/hosts that will override
your machine's DNS resolution, ensuring that the (un)desired
sites won't be available when you don't want them to be.


Usage
------------------------------------------------------------------------

Dis is a command line tool. Clone or download it, install it somewhere
in your PATH, and ensure it's set executable:

 chmod +x dis

and run it like this:

`dis ok`: Allow distractions; ie. comment out disallowed domain names
so they can be resolved.

`dis off`: Disallow distractions: resolve disallowed domains to
127.0.0.1 (ie. local machine) so the site is not available.

`dis add domain`: Add new site to distractables list; ie. "dis add
twitter.com"

`dis list`: List domains on distraction list.


Caveats
------------------------------------------------------------------------

 * This is only tested on Mac OS X, but should work on Linux too.

 * It requires superuser (admin) access to modify /etc/hosts, so
   you'll need an admin password. It also assumes that your machine's
   sudo configuration will allow you to run bash, sed and perl. (On
   Mac OS X, it does by default.)

