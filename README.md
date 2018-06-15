# scripts

A collection of semi-useful bash scripts I've written. All were written and
tested on GNU bash version 4.4.19.

**prelude**: Sets a bunch of shell options that I've found to be universally useful
in scripts, as well as ones I've never used, but whose man page description
makes them seem like good ideas.

**extract-args**: A very useful script that parses arguments to shell functions.
It's like 'getopt' or 'getopts', except with many more features (and many more
bugs...). I've found that, even after learning to use getopt(s), I'd need to set
up some loop of some kind to extract the parameters to options and whatnot; all
that getopt or getopts would do is state if the arguments were well-formed.
extract-args creates two global arrays: an associative array for options and
their parameters, as well as a linear array for command parameters. The end
result is that the boilerplate crap that goes with making a bash script is
greatly reduced--down to few lines--for parsing all of a script's arguments.

**git-create**: Creates a remote git repository. Currently only works for
  GitHub.

TODO: document structure change; prelude now in BASH_ENV, not explicitly called
