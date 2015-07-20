**gridutils** provides C library functions and command line utilities for working with curvilinear grids. **gridutils** has been developed and used mainly for grids generated by [gridgen](http://code.google.com/p/gridgen-c), but can be used to handle arbitrary 2D quadrilateral simply connected multi-corner grids.

Contains the following utilities:

  * **getbound** - extracts the bounding polygon

  * **getnodes** - validates and converts grids between double density, center and corner formats

  * **gridbathy** - interpolates scattered data onto the grid

  * **insertgrid** - inserts nodes from one grid into another at a specified location in index space

  * **setbathy** - given a three-column data file (X Y Z), sets values in specified index range to a specified value

  * **subgrid** - extracts nodes for a subgrid specified by index range

  * **xy2ij** - converts point coordinates between physical and index spaces

To build the interpolation utility **gridbathy** one needs to install [nn](http://code.google.com/p/nn-c), a Natural Neighbours interpolation library and [csa](http://code.google.com/p/csa-c), a cubic spline approximation library. Apart from that **gridutils** does not depend on other codes.

Checkout **gridutils** by running "`svn checkout https://gridutils-c.googlecode.com/svn/gridutils`"

[README](http://code.google.com/p/gridutils-c/source/browse/gridutils/README)