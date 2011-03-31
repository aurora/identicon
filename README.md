identicon.sh
============

Name
----

identicon.sh

Usage
-----

    $ ./identicon.sh -H hash [-s size-of-identicon] [-o file-name] [-t] [-h]

Description
-----------

This is a re-implementation of the PHP script "[PHP identicons](http://identicons.sf.net/)".

The original script requires PHP and the GD library, the re-implemented script is intented to be called from 
command-line and requires a bash, imagemagick and bc.

### Required parameters

    -H  hash to use for generating identicon

### Optional parameters

    -s  size of generated identicon in pixels (default: 64)
    -o  name of file to save created image to (default: stdout)
    -t  use transparent background (default: white)
    -h  display this usage information

License
-------

identicon.sh

Copyright (C) 2011 by Harald Lapp <harald@octris.org>
 
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.
 
This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.
 
You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
