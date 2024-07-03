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

# Tessellation Messaging and Notifications

In conjunction with a discovery and interrogation process, enable communication with identified maintainers of published RDF files and graph structures, particularly to notify these parties of parse errors, structure errors, or any other issues specific to a particular published graph data file.

## Scenarios

- Crawl Confirmations (this may also be general update items in a news feed)
  - New FOAF found, welcome org to the graph!
  - New DOAP found, notify org of newly-found project
  - New “friend” edge, notify both in case of a one-sided add?
- Crawl Errors
  - Missing FOAF that was previously found (this is more a warning or notice)
  - Missing DOAP that was previously found (also more a warning or notice)
  - Any parse error
  - Consider, any logical error that parses correctly but does not work (pointing to non-existent repos, etc)
- Issue Crawl Notices
  - Newly-opened issues
  - Alerts for issues marked Help Wanted or similar
  - Recently-closed issues
- General announcements
  - Tool updates
  - Organizational news
  - TBD

## Channels

The way notifications are shared may vary per subscriber or interest, maybe including these

- A public feed of any or all of the above scenarios
- A mailing list of any or all of the above scenarios
- A non-private but personalized update feed of relevant, classified issues and projects added/updated/closed
- TBD

Very generally speaking, feed generation (eg RSS 1.0) may fall to the [visualization](graph-visualization.md) component based on msg content from this component (ie send a msg to visualize as a feed some notification), where the boundary is between these two components may require some discussion.
