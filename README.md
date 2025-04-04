# DDMarlinPandora
[![Build Status](https://travis-ci.org/iLCSoft/DDMarlinPandora.svg?branch=master)](https://travis-ci.org/iLCSoft/DDMarlinPandora)
[![Coverity Scan Build Status](https://scan.coverity.com/projects/11933/badge.svg)](https://scan.coverity.com/projects/ilcsoft-ddmarlinpandora)

Interface between [Marlin](https://github.com/iLCSoft/Marlin) and [PandoraPFA](https://github.com/PandoraPFA)

DDMarlinPandora is distributed under the [GPLv3 License](http://www.gnu.org/licenses/gpl-3.0.en.html)

[![License](https://www.gnu.org/graphics/gplv3-127x51.png)](https://www.gnu.org/licenses/gpl-3.0.en.html)

## License and Copyright
Copyright (C), DDMarlinPandora Authors

DDMarlinPandora is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License long with this program.  If not, see <http://www.gnu.org/licenses/>.

## Options to add SDHCALContent or APRILContent

Added the compilation options to choose to include SDHCALContent or APRILContent in DDMarlinPandora.

Note, you should have sourced the init_ilcsoft.sh script

**To compile with SDHCALContent :**

1. mkdir build
2. cd build
3. cmake -C ${ILCSOFT}/ILCSoft.cmake -DPANDORA_MONITORING=ON -DUSE_SDHCALCONTENT=ON -DSDHCALContent_DIR=/absolute/path/to/SDHCALContent ..
4. make install

**To compile with APRILContent :**

mlpack should be installed. You should use the same mlpack installation as the one used to compile APRILContent


1. mkdir build
2. cd build
3. cmake -C ${ILCSOFT}/ILCSoft.cmake -DPANDORA_MONITORING=ON -DUSE_APRILCONTENT=ON -DAPRILContent_DIR=/absolute/path/to/APRILContent -Dmlpack_DIR=/absolute/path/to/mlpack/INSTALL ..
4. make install

**To compile with both SDHCALContent and APRILContent :**

Combine the two cmake options above.


