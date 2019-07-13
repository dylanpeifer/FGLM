# The FGLM Package

The FGLM Package is a Macaulay2 package implementing the FGLM algorithm for
computing Groebner bases. FGLM is a Groebner basis conversion algorithm, which
means it takes a Groebner basis of an ideal with respect to one monomial order
and changes it into a Groebner basis of the same ideal over a different
monomial order. Conversion algorithms can be useful since sometimes when a
Groebner basis over a difficult monomial order (such as lexicographic or an
elimination order) is desired, it can be faster to compute a Groebner basis
directly over an easier order (such as graded reverse lexicographic) and then
convert rather than computing directly in the original order.

## Requirements

The package requires at least version 1.14 of [Macaulay2][1].

## Installation

The FGLM package has been distributed with Macaulay2 since version 1.14. To
load it, type

    i1 : needsPackage "FGLM"

at the Macaulay2 prompt. If you are using an older version of Macaulay2 or wish
to reinstall or update the FGLM package, first download the [archive][2] and
unpack it. Then place the file `FGLM.m2` in the `packages` directory of your
Macaulay2 install. Finally, type

    i1 : installPackage "FGLM"

at the Macaulay2 prompt to finish installation. This command may need to be
repeated if you previously had a version of FGLM installed.

## Tests

After installation, basic tests of the package can be run by typing

    i2 : check FGLM

at the Macaulay2 prompt.

## Documentation

After the package has been installed, package documentation can be accessed by
typing

    i3 : viewHelp FGLM

at the Macaulay2 prompt. Documentation for all exported functions can also be
accessed through the standard Macaulay2 help system.

## License

Copyright (C) 2019 Dylan Peifer and Mahrud Sayrafi

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

## Contact

For questions, comments, problems, and bugs, please contact the package author,
Dylan Peifer, at djp282@cornell.edu.

[1]: https://faculty.math.illinois.edu/Macaulay2/
[2]: https://github.com/dylanpeifer/FGLM/archive/v1.0.0.tar.gz
