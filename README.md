ftgl-align-hack
===============

Hacked up ftlg (OpenGL font library) to make it support more and better types of alignment.

This code basically gives access to some of the internals of FTGL font. 
Then FormatText.h/.cpp is a static class that aligns text
- left, center, right  on the x-axis
- top, center, bottom on the y-axis
- wrapping text after a certain length
Examples of the alignment are available here: http://www.godpatterns.com/2013/01/kerning-wrapping-and-text-alignment.html

I needed this functionality. My format code doesn't support non-ascii :(, this is because I'm iterating character by character when calculating line length.
