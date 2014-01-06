dis
===

Dis is a very very simple tool for managing Internet distractions
when you're supposed to be working instead of screwing around. It
works by making entries to your /etc/hosts that will override
your machine's DNS resolution, ensuring that the (un)desired
sites won't be available when you don't want them to be.

Caveats
-------

 * This is only tested on Mac OS X, but should work on Linux too.

 * It requires superuser (admin) access to modify /etc/hosts, so
   you'll need an admin password. It also assumes that your machine's
   sudo configuration will allow you to run bash, sed and perl. (On
   Mac OS X, it does by default.)

Usage
-----

 dis ok: allow distractions
 dis off: disallow distractions
 dis add domain (eg. twitter.com): add new site to distractables
 dis list: list domains on distraction list"
