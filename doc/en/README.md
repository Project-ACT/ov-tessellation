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

# Tessellation Project Specification

The Tessellation project is composed of several components, each ideally developed on a platform that serves the required function and performance, and which can interoperate with other components in a language agnostic fashion.

The specification is broken down along those component lines with the following (with links to individual local specification files):

| Component                                        | Description                                                                                |
|--------------------------------------------------|--------------------------------------------------------------------------------------------|
| [Graph Local Management](graph-local.md)         | Author, manage, publish, update RDF data structures for projects and organizations         |
| [Graph Data Discovery](graph-discovery.md)       | Automated spider robot to traverse known nodes and discover new nodes and associated data  |
| [Graph Catalog Management](graph-catalog.md)     | Store, update, index, and search graph data for various uses                               |
| [Graph Visualizer](graph-visualize.md)           | Render network graphs, tessellation maps, and data charts based on catalog data            |
| [Notifier](graph-msg.md)                         | Alert RDF maintainers of data structure, format, syntax, and other errors                  |
