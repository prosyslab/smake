# smake
A program analysis preparation tool for C programs made with GNU Make

`smake` observes the build process driven by `make`, and derives the 
standalone, preprocessed form of the source code that makes up each
C program linked during the process. `smake` creates a directory
`sparrow/`, where you can perform program analyses.

You can instantly start your program analysis in three steps:
 1. Initialize `sparrow`
 2. Use `smake` instead of `make` to build your programs.

### Usage:

`smake --init [<options>]`

This command initializes `sparrow/` to handle the regular use of `smake`.

`smake --clean`

It completely removes `smake`.

`smake <parameters for make>`

It runs `make [<with parameters>]` and bookkeeps `sparrow/`.

`smake ./configure`

It runs `./configure` under the same environment `smake` runs.

`smake --help`

It shows this message.
