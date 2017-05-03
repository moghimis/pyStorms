TROPICAL CYCLONE ANALYSIS
==============================

This is a development project for using the Holland parametric model to produce wind and pressure profiles of Tropical Cyclones based on available data. 

## Getting Started

Tropical Cyclone (TC) attributes are estimated by corresponding operational agencies and centers around the world. For more info see the [INPUT.ipynb](./Notebooks/INPUT.ipynb) and [BestTrack.ipynb](./Notebooks/BestTrack.ipynb).

These data include location, windradii, pressure, max wind speed among others. However, there are missing info that preclude us from The proposed workflow consists of 4 steps : 

* Step 1 : From TC bulletins or Best Track create inpData file (see [INPUT.ipynb](./Notebooks/INPUT.ipynb), [Create inpData.ipynb](./Notebooks/Create inpData.ipynb), etc.).

* Step 2 : Compute translational and Coriolis velocities in order to move to a stationary frame (see [Subtract translational and Coriolis velocity.ipynb](./Notebooks/Subtract translational and Coriolis velocity.ipynb)).

* Step 3 : Estimate the parameters of the Holland Model and save outData file (see [Estimate Holland Parameters.ipynb](./Notebooks/Estimate Holland Parameters.ipynb)).

* Step 4 : Produce the wind and pressure profiles (see [Create Output.ipynb](./Notebooks/Output.ipynb)).


### Prerequisities

The required data can be freely downloaded by the corresponding listed sources. See Notebooks for more details. 

It is assumed that Best Track data are available in the corresponding folder. The dataset used is the Allstorms.ibtracs_all.v03r09.csv and the complete 1 file per storm netcdf folder [see here](https://www.ncdc.noaa.gov/ibtracs/index.php?name=ibtracs-data).

A number of Python modules are required. A complete list is available in a file named piplist.


## Tests

No tests are available at the moment.

## Authors

* **George Breyiannis** 


## Acknowledgments

* All the people that teach me stuff.  

## License
* The project is released under the GPL v3 license. 

  This library is free software: you can redistribute it and/or modify
  it under the terms of the GNU General Public License as published by
  the Free Software Foundation, either version 3 of the License, or
  (at your option) any later version.

  This library is distributed in the hope that it will be useful,
  but WITHOUT ANY WARRANTY; without even the implied warranty of
  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  GNU General Public License for more details.

