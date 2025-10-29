# How to contribute

## Prerequisites

- Pandoc. In Mac OS you can run the following command to install:

		$ brew install pandoc

  To learn more you can read the [Pandoc documentation][Pandoc]

## Understand the build system

First you need to understand our build system. We're using pandoc to convert markdown into ebooks. Here's what you need to build the book.

        $ make # this will create epub file
        $ make clean # this will clean up the generated book

## Repository Structure

The book content is organized in the `book/` directory:

- `book/front-matter/` - Contains the foreword and preface
- `book/chapters/` - Contains all chapter files, numbered sequentially (00-11)

Each chapter is in its own markdown file, making it easier to work on individual chapters without conflicts.

## Chapter Status

Before working on a chapter, please check the README.md for the current status of each chapter:

- **📝 Draft** - Chapter has initial content/notes and is actively being worked on
- **📋 Planned** - Chapter structure exists but content needs to be written (available for contribution)
- **✅ Complete** - Chapter is fully written and reviewed

If you plan to work on a chapter, please create an issue or comment on an existing one to let others know the chapter is in progress.

## Editing Content

To edit a chapter:

1. Navigate to `book/chapters/` directory
2. Open the relevant chapter file (e.g., `01-internship.md`)
3. Make your changes
4. Run `make` to build the book and verify your changes

To edit front matter:

1. Navigate to `book/front-matter/` directory
2. Edit either `foreword.md` or `preface.md`
3. Run `make` to build the book and verify your changes

## Adding New Chapters

If you need to add a new chapter:

1. Create a new markdown file in `book/chapters/` with the appropriate number
2. Update `build.sh` to include the new chapter in the correct order
3. Update the chapter list in `README.md`

## Create issue first

If you think there's something we can improve on this ebook, feel free to create an issue [here](https://github.com/kulkultech/jumpstart-swe/issues).

[Pandoc]: https://pandoc.org/installing.html