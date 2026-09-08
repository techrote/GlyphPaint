GlyphPaint — HTML/ANSI Character Painting Program
================================================

GlyphPaint is a standalone browser painting program modelled on the Windows 10-era
MS Paint workflow, but its document model is an HTML/ANSI-style character grid.
Every cell stores:

  • a text glyph
  • foreground colour
  • background colour
  • monospaced font choice
  • bold / italic / underline text attributes

No server, framework, install, or external assets are required. Double-click
GlyphPaint.html in a current desktop browser.

CORE PAINT FEATURES
-------------------
• Pencil / glyph drawing
• Brush sizes 1–5
• Brush, Calligraphy 1, Calligraphy 2, Airbrush, Oil, Crayon, Marker,
  Natural Pencil, Watercolor
• Flood fill
• Eraser
• Colour picker
• Magnifier
• Text tool with font, scale, bold, italic, underline, transparent/opaque background
• Left mouse = Color 1; right mouse = Color 2
• Standard Paint-style palette plus custom colour picker
• Foreground and background colour per glyph cell

SELECTION / IMAGE FEATURES
--------------------------
• Rectangular selection
• Free-form/lasso selection
• Move selection
• Transparent selection mode
• Cut / Copy / Paste
• Select all
• Delete selection
• Crop
• Resize by cells or percentage
• Maintain aspect ratio
• Horizontal / vertical skew
• Rotate right 90° / left 90° / 180°
• Flip horizontal / vertical
• Invert colours

SHAPES
------
• Line and curve
• Rectangle / rounded rectangle
• Ellipse
• Polygon
• Triangle / right triangle
• Diamond / pentagon / hexagon
• Arrows: left / right / up / down
• 4-, 5-, and 6-point stars
• Rectangular / rounded / oval callouts
• Heart
• Lightning bolt
• Outline modes, fill modes, and stroke sizes

VIEW
----
• Zoom 25–800%
• Gridlines
• Rulers
• Status bar
• Full screen
• Cursor coordinates and selection dimensions

FILES / INTERCHANGE
-------------------
• GlyphPaint project JSON
• Import coloured HTML containing <pre id="art">
• Directly imports the cybertree HTML format used in this conversation,
  including --fg / --bg span colours
• Import PNG/JPEG/WebP/etc. and convert it to coloured glyph cells
• Export standalone selectable-text HTML
• Export plain TXT
• Export PNG
• Export JPEG
• Export BMP
• Export GIF
• Print
• "Set as desktop background" browser-safe equivalent: exports a wallpaper PNG

SHORTCUTS
---------
Ctrl+N  New
Ctrl+S  Save project JSON
Ctrl+Z  Undo
Ctrl+Y  Redo
Ctrl+C  Copy
Ctrl+X  Cut
Ctrl+V  Paste
Ctrl+P  Print
Delete  Delete selected cells
+ / -   Zoom

NOTES
-----
The web sandbox cannot directly change Windows wallpaper, talk to scanners using
legacy Windows APIs, or attach a generated file to the native mail client. Those
OS-integrated Paint commands are represented by browser-safe file import/export
operations instead. Painting and image-editing functionality is implemented in
terms of glyph cells rather than bitmap pixels.
