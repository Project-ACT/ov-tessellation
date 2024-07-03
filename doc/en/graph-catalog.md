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

# Tessellation Graph Catalog

Capture discovered graph data and manage storage in a graph database or similar, facilitating queries and foreign data
interfaces, reporting in different ways as needed, etc.

## Graph Database

One of the fundamental properties of an Ontology System such as that which can be expressed RDF, is the ability to query
a database of findings for relations between nodes and other data contained within them or represented by them.

We can presume that there is a suitable database already available (this is true) to store graph data described with our
RDF findings, and that the common SPARQL query language will be available (which it will be).

We are not limited, however, to the usual database and query language options if more leading edge, or more-easily-integrated,
or even completely novel ideas arise.
