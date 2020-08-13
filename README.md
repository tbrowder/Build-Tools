[![Build Status](https://travis-ci.org/tbrowder/Build-Tools.svg?branch=master)](https://travis-ci.org/tbrowder/Build-Tools)

# Build::Tools

This module provides some routines to ease the Build step
for module authors using the build hook for installation.

## Synopsis:

Use this module in your Build.pm6 file:

```
use Build::Tools; # which also uses File::Copy

# ...create some directories and files...
copy $file, $dir1;
copy $dir1, $dir1;

# manipulate the resources directory
copy-resource $foo, $dir1;
copy-resources $dir2 :createonly;
```

See the internal documentation in the terminal window
by entering:

```
$ p6doc Build::Tools
```

CREDITS
=======

Thanks for help from IRC `#perl6` friends:

+ `ugexe` (for insights on zef and the installation process)

AUTHOR
======

Tom Browder, `<tom.browder@gmail.com>`

## COPYRIGHT

Copyright (c) 2019 Tom Browder, all rights reserved.

## LICENSE

Artistic 2.0.  See that license [here](./LICENSE).
