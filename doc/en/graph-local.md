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

# Local Tessellation Graph Management

Given a local organization or project, facilitate the creation and maintenance of RDF source files (eg Notation3 graph description, typically indicated with a .n3 filename extension) for the organization or its projects, and serialization of graph data to the most common RDF/XML (or application/rdf+xml) output for publication and interrogation.

## Intended Audience

This is a tool, or collection of tools or methods or processes, which enable

- an organization maintainer or manager to create, publish, and maintain a top-level FOAF
- a project maintainer or manager to crate, publish, and maintain a top-level DOAP
- an individual contributor to create, publish, and maintain a personal FOAF

Note that in the individual contributor case, it may be that the individual maintains a FOAF for use in the context of the Project-ACT universe, but also maintains one or more additional FOAF graphs for personal, professional, or other uses. There should not be a presumption that this notion is exclusively Project-ACT.

## Implementation Hiding

The core features of FOAF and DOAP on which the initial Project-ACT effort shall depend, are minimal and rather easy. Perhaps.

The user of this tool should not be overly concerned about FOAF, DOAP, Notation3 syntax, nor RDF/XML publication format, and so on. Success should depend on filling in some form fields or responding to some prompts, not on editing source files and manually transforming them for publication.

At the same time, the core workings should not be obscured; source Notation3 files, for example, should be visible and editable, and the connection between these source files and a resulting RDF/XML files in xml format should be apparent. If the user would rather use a different source format, or manually edit the XML output, these should be allowed, though perhaps not encouraged.

## Workflow Use

It makes sense to enable a GitHub Action or similar, a command line tool which may run as part of any automation, or that command line tool running in some interactive fashion to perform the needed workflow steps to publish the DOAP and FOAF files (at a minimum).

A more interactive tool with gui or tui form fields and rich help text and so on is also a sensible possibility.
