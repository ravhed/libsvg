# libsvg - a library for SVG files
======

libsvg library with a Visual Studio 2017 project. Dependencies are available as well in this repository if somebody wants to compile it as a dynamic library.
All dependencies except uriparser was downloaded from http://www.gisinternals.com. See http://uriparser.sourceforge.net/ for uriparser.
Source code was retrieved from https://sourceforge.net/projects/svg2swf/ - this version has several fixes to the libsvg library. 

Description
-----------
libsvg provides a parser for SVG content in files or buffers.

Dependencies
------------
libsvg depends on libxml2, and should be easy to build on any
reasonable system.

Usage
-----
libsvg does not do any rendering, but instead provides a
function-based interface that can be used by various rendering
engines. See the declaration of svg_render_engine_t in svg.h.

It is anticipated that the primary uses of libsvg would be in small
libraries that connect the libsvg parser to a rendering engine. Those
libraries, in turn, would provide the capability to applications to
directly render SVG content from files or buffers.

Known uses
----------
At this time, the only known library using libsvg is libsvg-cairo which
uses the cairo graphics library. A port of librsvg, (using libart), to
use libsvg is expected.

History
-------
libsvg was developed by Carl Worth <cworth@isi.edu>
libsvg was based on code from librsvg by Raph Levien <raph@acm.org>
