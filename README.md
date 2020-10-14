# Mkinfo for Micro

THIS PROGRAM IS NO LONGER NECESSARY, PLEASE DO NOT USE. Newer versions of micro will automatically read terminfo entries from your system, so that micro can understand them at runtime.

This program will read you terminal info and store it so that [micro](https://github.com/zyedidia/micro) can run in obscure terminals that it doesn't understand by default.

This program is adapted from the `mkinfo.go` file in [tcell](https://github.com/gdamore/tcell) written by gdamore.

# Usage

If you encounter the `terminal entry not found` error in micro, then you should try running this program.

```
$ ./mkinfo
```

Note: this program will create a file called `.tcelldb` in your home directory.

If you would like to put the file in a different location you may pass an additional output filename argument (`./mkinfo -o filename`). Then set the `$TCELLDB` environment flag to that
file so that micro will know where to look for the database.

Then try running micro again.

# Installation

Just [download a binary](https://github.com/zyedidia/mkinfo/releases) from the releases page. You can also compile from source if you'd like.

Make sure you have curses installed (this should be installed by default in most places).
