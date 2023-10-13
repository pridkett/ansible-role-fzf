ansible-role-fzf
================

Patrick Wagstrom &lt;160672+pridkett@users.noreply.github.com&gt;

October 2023

Overview
--------

I make use of fzf within my shells to handle more intelligent command line search and what not. However, some operating systems, most notably Raspbian, are based on such old versions of Debian that the packaged versions of fzf are rarely working.

There are a couple of different ways to handle this, I could go through and repackage the newest Debian version of the fzf packages for older versions of Raspbian, or I could just grab the binary distribution and install that. While I futzed with repackaging the newer versions of the Debian pacakage for a while, in the end the fastest solution was just to have this role download and install the binary directly from GitHub.

Configuration
-------------

This role takes no configuration

Issues
------

This role has only really been tested on Raspbian systems. There are probably lots of different issues out there. Like, on 64 bit Raspberry Pis running 32 bit versions of Raspbian it installs the 64 bit executable, which still works because it's completely statically linked.
