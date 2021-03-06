# Remove dated files

This script removes dated files.

Contents:

* [Introduction](#introduction)
* [Which files?](#which-files)
* [Related](#related)
* [Compatibility notes](#compatibility-notes)
* [Tracking](#tracking)


## Introduction

Syntax:

    $ rm-dated-files [dir]

Example to do the current directory:

    $ rm-dated-files

Example to do a specific directory:

    $ rm-dated-files /foo/goo


## Which files?

This deletes files with names that end in a separator then ISO date:

  * Example: foo-2017-12-31, foo_2017_12_31, etc.

The file name separator can be a period, dash, or underscore.


## Related

These scripts are for related purposes:

  * [rm-compressed-files](https://github.com/SixArm/rm-compressed-files)

  * [rm-dated-files](https://github.com/SixArm/rm-dated-files)

  * [rm-numbered-files](https://github.com/SixArm/rm-numbered-files)

  * [rm-rotated-files](https://github.com/SixArm/rm-rotated-files)


## Compatibility notes

We prefer to be more compatible rather than system-specific.

  * To delete files, we prefer `-exec rm` vs. `-delete`.
    The former is more compatible, the latter is faster.

  * To regex match, we prefer patterns to be basic vs. extended.
    The former is more compatible, the latter is more modern.

  * We prefer POSIX code vs. shell-specific code.


## Tracking

  * Command: rm-dated-files
  * Website: http://sixarm.com/rm-dated-files
  * Cloning: https://github.com/sixarm/rm-dated-files
  * Version: 4.0.0
  * Created: 2013-12-09
  * Updated: 2019-01-01
  * License: GPL
  * Contact: Joel Parker Henderson (joel@joelparkerhenderson.com)
  * Tracker: bac247f0bfa7328306f2db7e5910a610
