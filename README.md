# Typo3Scan

Typo3Scan is an open source penetration testing tool that I wrote to automate the process of detecting the [Typo3](https://typo3.org) CMS and it's installed [extensions](https://extensions.typo3.org/).
It also has a database with known vulnerabilities for core and extensions. 

Typo3Scan does not exploit any vulnerabilities! It´s soley purpose was to enumerate version info and installed extensions in penetration tests ever since.

## Installation

You can download the latest tarball by clicking [here](https://github.com/whoot/Typo3Scan/tarball/master) or latest zipball by clicking  [here](https://github.com/whoot/Typo3Scan/zipball/master).

Preferably, you can download Type3Scan by cloning the [Git](https://github.com/whoot/Typo3Scan) repository:

    git clone https://github.com/whoot/Typo3Scan.git

Typo3Scan works with [Python 3](http://www.python.org/download/) version **3.7** on Debian/Ubuntu and Windows platforms.

You can install all required packages with pip3:

	pip install -r requirements.txt

## Usage

To get a list of all options use:

    python typo3scan.py -h

You can use Typo3Scan with domains:

	python typo3scan.py -d DOMAIN [DOMAIN ...] [--vuln]

Or with a file with a list of domains:

	python typo3scan.py -f FILE [--vuln]

Example:

	python typo3scan.py -d http://dev001.vm-typo3.loc --vuln

<img src="./doc/core_vulns.jpg" width="450">
<img src="./doc/ext_vulns.jpg" width="450">

## Bug Reporting

Bug reports are welcome! Please report all bugs on the [issue tracker](https://github.com/whoot/Typo3Scan/issues).

I´m developing this in my spare time. If you like my work, please consider supporting my coffee consume:

[![Buy me a coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/whoot)


## Links

* Download: [.tar.gz](https://github.com/whoot/Typo3Scan/tarball/master) or [.zip](https://github.com/whoot/Typo3Scan/archive/master.zip)
* Changelog: [Here](https://github.com/whoot/Typo3Scan/blob/master/doc/CHANGELOG.md)
* Issue tracker: [Here](https://github.com/whoot/Typo3Scan/issues)

# License

Typo3Scan - Automatic Typo3 Enumeration Tool

Copyright (c) 2015-2020 Jan Rude

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see [http://www.gnu.org/licenses/](http://www.gnu.org/licenses/)
