<!--
 Copyright (C) 2024 Project-ACT
 
 This file is part of ov-tessellation.
 
 ov-tessellation is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 ov-tessellation is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with ov-tessellation.  If not, see <https://www.gnu.org/licenses/>.
-->

# Tessellation Visualization

Process catalogued graph data to build visualizations of various kinds, including but not limited to network graphs, project graphs, tiles in the tessellation with geo data for map plots, and whatever else might come in handy.

There are several forms a visualization of the Tessellation might take, a few ideas are listed here (not exhaustive).

## Traditional Output

- It may be useful to generate a csv file of organization, projects, etc for the purposes of constructing a classic spreadsheet
- Plain old text file output
- JSON output as a part of a web page generation pipeline
- Some query result (a subset, or maybe the entire catalog) in an RDF structure such as n3 or rdf/xml
- Generation of an RSS update feed (RSS v1.0 of course)

## Graph Output

- JSON output for Nodes and Edges using NetworkX for example, local display of some view of graph data
- Some fun options like KML output to render Placemarks and polygons and whatnot on a Map (Google Maps, Google Earth, WorldWind, etc etc)
  - [NASA WorldWind Project](https://worldwind.arc.nasa.gov/)
  - [Cesium Platform for 3D Geospatial](https://cesium.com/)
