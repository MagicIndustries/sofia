# Sofia Materials

## Overview
Sofia is a knowledge management system that allows you to spatial manipulate related information around ideas, keywords or concepts, dynamically querying and working spatially with your entire knowledge base.

You give everything you know and discover to Sofia to manage, tagging articles and linking them as you browse your feeds on the web, and Sofia manages the broader network of your knowledge, helping bring research into focus as you explore relevant topics, and finding new links between items of information or areas of research.

### Relationships
Every concept is linked to source material - explainers, overviews, documents, videos, tags, key people and organizations, implementations and examples etc. Every node in the knowledge graph is linked to other nodes, with each relationship being customizable and queryable.

The map view shows the entire graph, reordered on the fly as you focus on specific areas. This view can be manipulated to emphasize nodes by number of links, trust scores, relevance to the current document and more.

### Trust
As documents and sources are cited or linked to each other, their relevant trust and reference scores affect each other, based on trust settings controlled by the user. A technology document might have a 100% trust rating for something the user has personally verified, lending weight to any document that cites or links to it.

Trust settings are completely customizable. A researcher might assign more trust to documents tagged “peer reviewed”, or even more to documents tagged “personally proven”. Citations to Wikipedia might be weighted significantly less than citations of articles marked as coming from a respected journal or textbook.

### Auto-discovery
Based on user settings, inferred links between nodes can be discovered automatically, by keywords, sources, dates, names or other information. These inferred links can be displayed in context when viewing documents, helping the user discover new links between items of information.

### Spatial Interface
Sofia’s interface can be used on the desktop but really shines in Augmented or Virtual Reality. View the full graph of your knowledge network and manipulate the nodes to get a sense of scale and relationship, or read and work on documents while surrounded by nearby related information.

Query your knowledge graph and keep multiple views suspended in the air around you. Bring relevant nodes closer and keep them visible, while auto-discovering new links between them.
Keep track of key players in a subject, both people and organizations, and easily research them on LinkedIn, in the news and other sources.

Explore your own knowledge, moving through relationships, managing your day to day learning and discovering news, new related concepts and the latest world / industry news about whatever you’re looking at. Easily craft searches on Google and research search engines based on the visible nodes in front of you.

## Browser Plugin
The browser plugin works like the Evernote Web Clipper, allowing you to save articles, videos and websites to your Sofia knowledge graphs, and manually specify relationships to existing nodes in Sofia.

## Evernote Importer
Imports knowledge nodes from Evernote, creating nodes, relationships and tags based on settings and Evernote tags and keywords.

## Structured Data Importer
Imports notes knowledge nodes from CSV / XML, creating nodes, relationships and tags based on a defined fieldset.

## Architecture
Unity Interface, talking to a Node.js API on an AWS EC2 instance.

Browser plugins will usee HTTP/REST against the same interface.
UI Layout, settings stored in client with optional server backup / transport.

Currently aimed at VR Headsets like Vive and Oculus Rift, and MR Headsets like Hololens, Meta2 and Magic Leap.

## Current State
- Data Schema, relationship structure and database setup (Neo4J) all exist.
- server / backend code and API exists
- Evernote Importer exists as a node script.
- Structured Data Importer doesn’t exist but would take a day or two to tie in to the Evernote importer.
- Interface is in design, needs some sketching and a little discussion with a unity guru / technical artists / Unity UX engineer.
- Browser plugin is approx 50% compleete
- Needs a scaling setup if offered as SaaS, less if standalone application

## To Get to MVP
**Resources**
- Full Stack Javascript Developer (a) Unity Developer (b) (Toby Tremayne)
- UI / 3D Artist (c)
- Technical Artist (d)
- Node / AWS Service Integration UI Technical Design (Toby Tremayne)
- Art & UI
- Interface Build (Toby Tremayne)
- Browser Plugins (Toby Tremayne)
- Importers (Toby Tremayne)

Plus testing / iteration / deployment
(a) 1-2 weeks
(d) 3-4 weeks (b) 1 week
(c) 2-3 weeks
(a) 1-2 weeks (b) 2-3 weeks (c) 2-3 weeks (a) 2-3 weeks
(a) 2-3 weeks
Total Duration Estimate: 2-3 months

## Example Database Graph
![alt text](/assets/graph.png "Example Graph")

## Sample Interface Mockup

**Please excuse the bad programmer art! More designs have been done as hand sketches and proper UI/UX concepts would be the first use of the grant funds**
## Example Database Graph
![alt text](/assets/sofia_screen.png "Ugly programmer representation")
