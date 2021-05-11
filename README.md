# Graphmatic

JavaScript backed Visual Scripting solution

## Introduction

Graphmatic aims to be a full-featured Visual Scripting solution enabling development of software solutions using a graph based visual scripting interface.
This should easily allow low-tech users (and of course high-technicall ability users as well) to create dynamic solutions, whether that be full fledged
runnable programs, third-party integrations for other systems, data-science and transformation algorithms, or any other project that can be described using
a logical flow (aka "program flow").

For now, this is achieved with a browser based JavaScript environment. But can be extended using the schema-based files to save and transfer Graphs for execution or compilation in other systems/languages.

## The Plan, For How It Works

There will be multiple pieces of software, that when combined will provide the full service of: editing/creating Graphs, saving/loading Graphs to file, validating Graphs for early error checking and helpful "linting", pre-compiling Graphs to a (proprietary) byte-code, interpretation and execution of the byte-code for in-browser or standalone virtual machines, compilation of Graphs to source code languages (JavaScript, C++, Python, etc.), compilation of Graphs to executable code, and many other possibilities.

Each piece is categorized for it's part of the solution, and will be explained in the following sub-chapters.

### Human Readable File Format

The primary data format for retaining and exchanging Graphs is XML. XML Schema Definitions (XSD) files are provided to help validate and for third-party tool development. XML was chosen because Graphs by nature require a tree-like structure (hence, "graph"), and with a DOM style document format, this fits nicely. Not
all the information contained within the XML file is considered actionable, these files also contain presentation information for Graph editors, or compiler hints.

In all, the XML file format can be considered a project file format. Within a Graph, external files may be referenced to help break up large projects or for third-party library and dependencies.

Refer to the `/schema` folder, and the [Schema Readme](schema/README.md) within that folder for more information on this schema format.

### Machine Readable Byte-Code Format

TODO: Write this sub-chapter

### Development Environment - Graph Editor

TODO: Write this sub-chapter

### Byte-Code Pre-Compiler

TODO: Write this sub-chapter

### In-Browser Virtual Machine

TODO: Write this sub-chapter

### Standalone Virtual Machine

TODO: Write this sub-chapter

### Transpiler/Transliterator - Graph Converter

TODO: Write this sub-chapter

### Executable Compiler

TODO: Write this sub-chapter

## License

Graphmatic is currently under the `GNU General Public License 3.0` license. This license is subject to change in later versions. The license used for the source code is maintained in the `LICENSE` file found at the root folder of the repository, so regardless of this message refer to that when cloning branches or commits.
