Driver for (some) Brother laster printers
=========================================

Most Brother printers support a standard printer language such as PCL
or PostScript, but not all do.  If you have a monochrome Brother laser
printer (or multi-function device) and the other open source drivers
don't work, this one might help.

It is known to support these printers:

* Brother HL-L2340D
* Brother DCP-7030
* Brother DCP-7055
* Brother DCP-7065DN
* Any? Brother Monochrome Laser printer?

Installation
---------

Deb/Ubuntu:

1. apt-get install cups build-essential libcups2-dev libcupsimage2-dev automake
2. cd /usr/src && git clone https://github.com/bitbakers/brlaser.git
3. ./autogen.sh
4. make
5. make install clean
6. service cups restart
7. Add printer via CUPS interface & select any ", using brlaser v3 Modell"


Copyright
---------

Copyright © 2013 Peter De Wachter

brlaser is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 2 of the License, or
(at your option) any later version.

brlaser is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with brlaser.  If not, see <http://www.gnu.org/licenses/>.
