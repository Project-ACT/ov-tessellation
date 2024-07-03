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

# Automated Tessellation Graph Node Discovery and Interrogation

Tools and methods to locate new and update existing Project-ACT nodes, whether Project (eg DOAP files) or
Organization (eg FOAF files), and iterate over a known graph to do so, updating the known graph in the process.

## Spiders, Bots, and Crawlers

These are well-known machinations moving around through the modern internet.

In the old days of RDF and other published data at particular locations, the internet was mostly open, or as we
might say of the time, the Wild Wild West, urls for these files were plainly accessible, for the most part. In the
modern era, hosts, platforms, and other schemes may make accessing some data a slight challenge, but not one that is
unsurmountable.

Luckily, we may confine our crawling to public, published items (there should be no hidden or secure files in these
transactions), the challenge here will be navigating platforms such as GitHub, for example, to look for specific
locations such as an organization root and the FOAF file which should be there, organization projects, project
roots and a DOAP file which may be found there, and so on.

On the other hand, we cannot require that these target items are located in a GitHub project nor organization (or
a similarly-structured user account), since the files we are looking for may be placed on a personal blog, project
website, organization or group website, or anywhere else. We can make use of the HTML link scheme used for
automated discovery of RSS feeds and similar, with a
