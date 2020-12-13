# How to contribute

## Prerequisites

- Pandoc. In Mac OS you can run the following command to install:

		$ brew install pandoc

  To learn more you can read the [Pandoc documentation][Pandoc]

## Understand the build system

First you need to understand our build system. We're using pandoc to convert markdown into ebooks. Here's what you need to build the book.

        $ make # this will create epub file
        $ make clean # this will clean up the generated book
        
## Create issue first

If you think there's something we can improve on this ebook, feel free to create an issue [here](https://github.com/kulkultech/jumpstart-swe/issues).

[Pandoc]: https://pandoc.org/installing.html