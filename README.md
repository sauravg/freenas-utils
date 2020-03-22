# freenas-utils

This repository contains some scripts for automating certain tasks with FreeNAS.

* repl: enable/disable all replication tasks


#### repl

Use this script to avoid having to sign on to FreeNAS web UI and toggle each replication task manually. It has been tested/used on Linux & macOS, with FreeNAS 11.1 and FreeNAS 11.2

> Usage: repl --enable-all|--disable-all [--verbose]

This requires root password for your FreeNAS server. You can put them in your ~/.netrc, which would look something like

> machine 192.168.1.10 login root password secretpassword

Dependencies:
* [httpie](https://httpie.org)
* [jq](https://stedolan.github.io/jq/)

How you install these depends on your platform. On macOS, you can use [homebrew](https://brew.sh/). On debian-based Linux'es, apt-get should be able to find & install them.


