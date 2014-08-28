# identicon.sh

## Usage

    $ ./identicon.sh [arguments]

## Description

An Identicon is a visual representation of a hash value. Please have a look at "[wikipedia](http://en.wikipedia.org/wiki/Identicon)"
for a detailed explanation of identicons and have a look at the "[wiki](https://github.com/aurora/identicon/wiki/Examples)" for some
generated "[example identicons](https://github.com/aurora/identicon/wiki/Examples)". 

This is a re-implementation of the PHP script "[PHP identicons](http://identicons.sf.net/)".

The original script requires PHP and the GD library, the re-implemented script is intented to be called from 
command-line and requires a bash, imagemagick (only if output is not SVG) and bc.

### Arguments

    -H  hash to use for generating identicon
    -s  size of generated identicon in pixels (default: 64)
    -w  apply swirl effect, expects a degree value (eg.: 180, -60, etc.) (default: 0)
    -o  name of file to save created image to (default: stdout)
    -t  use transparent background (default: white)
    -h  display this usage information

It's allowed to specify an output format by prefixing the the file (argument: -o) with the name
of the format for example:

    $ ./identicon.sh -o svg:-

The default output format is 'png'. Imagemagick is not required when specifying 'svg' as output
format.

## Examples

<img src="http://dl.dropbox.com/u/5014780/github/identicons/example1.png" />&nbsp;&nbsp;<img src="http://dl.dropbox.com/u/5014780/github/identicons/example2.png" />&nbsp;&nbsp;<img src="http://dl.dropbox.com/u/5014780/github/identicons/example3.png" />&nbsp;&nbsp;<img src="http://dl.dropbox.com/u/5014780/github/identicons/example4.png" />

## License

identicon.sh

Copyright (C) 2011-2014 by Harald Lapp <<harald@octris.org>>
 
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.
 
This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.
 
You should have received a copy of the GNU General Public License
along with this program.  If not, see <<http://www.gnu.org/licenses/>>.

## Thanks

Thanks to all contributors! 

*   Liviu Cristian Mirea-Ghiban, http://github.com/liviumirea
    
    1.  The sprites were being drawn with an additional 1px per width and height 
        and had bleeding edges in the final image.

    2.  The rotations didn't completely match the ones in the original PHP 
        Identicon script.

*   Luis Martin Gil, https://github.com/luismartingil

    *   Optional hash / hash generation

