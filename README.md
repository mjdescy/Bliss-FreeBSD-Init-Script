# Bliss-FreeBSD-Init-Script

A rc.d script to run Bliss as a daemon under FreeBSD (as in a FreeNAS jail)

## Purpose

[Bliss][1] is ideal for running on home servers, but it is not evident (as of the 2015-03-16 release) how to install and run it properly on FreeBSD, as you would in a FreeNAS jail. This repository contains instructions and an init (rc.d) script to run Bliss properly on FreeBSD or in a FreeNAS jail.

[blisshq]: http://www.blisshq.com

## What is Bliss?

[Bliss][blisshq] is an album artwork finder and tagger for music files (MP3, AAC, FLAC, ALAC, etc.). It's unique features include:

1. Running as a web service, rather than as a local application
2. Automatically assessing your music collection for compliance with the rules that you configure

## The init script

The init script in question is found in the `bliss` file within this repository. The `bliss` script must be made executable and should be stored in `/usr/local/etc/rc.d`. It assumes that you installed the Bliss application to `/usr/local/bin/bliss`. See the wiki for full installation instructions. 

## Instructions

See the [wiki][wikihome] for full installation instructions for Bliss on FreeBSD/FreeNAS jails. 

[wikihome]: https://github.com/mjdescy/Bliss-FreeBSD-Init-Script/wiki

## Version info

The current version of the script is based on the Bash startup script for  Release 20150316 of Bliss, and was tested in a FreeNAS 9.2 jail.