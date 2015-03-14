## MOVED TO GITHUB ##

I've moved this project accross to github https://github.com/bennoleslie/pexif

At this point in time, I'm not really actively working on this code base anymore, but will happily accept and merge pull requests on github.

# pexif #

pexif is a Python library for parsing and more importantly editing EXIF data in JPEG files.

This grew out of a need to add GPS tagged data to my images, Unfortunately the other libraries out there couldn't do updates and didn't seem easily architectured to be able to add such a thing. Ain't reusable software grand!

My main reason for writing this was to provide an easy way for geo-tagging my photos, and the library now seems mature enough to do that.

The library contains some examples as well as some usable standalone PexifScripts.

## Status ##

**WARNING** This could destroy your images!! Backup your images before using.

Currently it parses files from my Canon without a problem, and is able to add a GPS tag without corrupting the rest of the image. You can also fairly easily add and modify other tags.

A reasonable test suite is provided with the app, and the library is pretty well documented with docstrings. Use help(pexif) inside the python interpreter for reference.


## Acknowledgments ##

Nick Carter provided `conker.jpg` which is used for testing FUJIFILM exif data.

Nick Burch provided `noexif.jpg` which is used for testing inputs that don't have an existing EXIF segment.

David Clark and Marcell Lengyel found a bug with big-endian files. David provided a patch to fix this problem.
