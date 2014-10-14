# Swiss Maps

This repository provides [TopoJSON](https://github.com/mbostock/topojson) files for Switzerland from publicly available [swisstopo](http://www.swisstopo.admin.ch/internet/swisstopo/en/home.html) geodata. 

## How to reproduce

To generate the TopoJSON files the steps descriped by [Interactive Things](https://github.com/interactivethings/swiss-maps) were followed. However, the descriped steps are difficult to reproduce on Windows and Linux machines. That is the reason why the TopoJSON files are made available in this repository. 

## Available Files

The following TopoJSON files can be found in the topo directory:

* `ch-country.json`
* `ch-cantons.json`
* `ch-districts.json`
* `ch-municipalities.json`
* `ch-country-lakes.json` (country boundaries + lakes)
* `ch-cantons-lakes.json` (canton boundaries + lakes)
* `ch-districts-lakes.json` (district boundaries + lakes)
* `ch-municipalities-lakes.json` (municipality boundaries + lakes)
* `ch-lakes.json`
* `ch.json` (all of the above combined)
* For each canton a file with its municipalities and lakes, e.g. `zh-municipalities.json` and `zh-municipalities-lakes.json`
* `ch-plz.json` (zip code boundaries)
* `ch-contours.json` (elevation countours, the `CONTOUR_INTERVAL` variable is set to 500 meters)

The file have the following characteristics:

* Projected, *cartesian* coordinates
* *Scaled* and *simplified* to a size of **960 × 500** pixels

## Examples

* [TopoJSON Cantons and Municipalities](http://bl.ocks.org/herrstucki/4327678) (stored in a single file!)
* [TopoJSON Cantons](http://bl.ocks.org/mbostock/4207744)
* [Swiss Topography](http://bl.ocks.org/herrstucki/6312708)

## Copyright and License

### Author

Jeremy Stucki, [Interactive Things](http://interactivethings.com)
Tim Hagmann (creating the topoJSON files)

### Data Source

Data source is the Swiss Federal Office of Topography, [swissBOUNDARIES3D](http://www.swisstopo.admin.ch/internet/swisstopo/en/home/products/landscape/swissBOUNDARIES3D.html) 2014.

### License

* Geodata from swisstopo is licensed under the [Licence for the free geodata of the Federal Office of Topography swisstopo](LICENSE-GEODATA)
* Everything else: [BSD](LICENSE)
