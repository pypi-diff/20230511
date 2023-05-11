# Comparing `tmp/jonky-0.0.4.tar.gz` & `tmp/jonky-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jonky-0.0.4.tar", last modified: Fri Jan  6 19:21:55 2023, max compression
+gzip compressed data, was "dist/jonky-0.0.5.tar", last modified: Thu May 11 21:24:02 2023, max compression
```

## Comparing `jonky-0.0.4.tar` & `jonky-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jari      (1000) jari      (1000)        0 2023-01-06 19:21:55.000000 jonky-0.0.4/
--rw-rw-r--   0 jari      (1000) jari      (1000)      132 2023-01-06 19:21:55.000000 jonky-0.0.4/PKG-INFO
-drwxrwxr-x   0 jari      (1000) jari      (1000)        0 2023-01-06 19:21:55.000000 jonky-0.0.4/jonky/
--rw-rw-r--   0 jari      (1000) jari      (1000)      177 2022-03-11 06:39:27.000000 jonky-0.0.4/jonky/__init__.py
--rw-rw-r--   0 jari      (1000) jari      (1000)    18170 2022-12-17 22:48:34.000000 jonky-0.0.4/jonky/drawable.py
--rw-rw-r--   0 jari      (1000) jari      (1000)     1735 2022-03-18 21:51:46.000000 jonky-0.0.4/jonky/helpers.py
--rw-rw-r--   0 jari      (1000) jari      (1000)     6028 2022-12-06 22:33:08.000000 jonky-0.0.4/jonky/jonky_main.py
--rw-rw-r--   0 jari      (1000) jari      (1000)     3011 2021-07-20 19:47:51.000000 jonky-0.0.4/jonky/widget_helpers.py
--rw-rw-r--   0 jari      (1000) jari      (1000)    14129 2022-09-26 19:24:25.000000 jonky-0.0.4/jonky/widgets.py
-drwxrwxr-x   0 jari      (1000) jari      (1000)        0 2023-01-06 19:21:55.000000 jonky-0.0.4/jonky.egg-info/
--rw-rw-r--   0 jari      (1000) jari      (1000)      132 2023-01-06 19:21:55.000000 jonky-0.0.4/jonky.egg-info/PKG-INFO
--rw-rw-r--   0 jari      (1000) jari      (1000)      266 2023-01-06 19:21:55.000000 jonky-0.0.4/jonky.egg-info/SOURCES.txt
--rw-rw-r--   0 jari      (1000) jari      (1000)        1 2023-01-06 19:21:55.000000 jonky-0.0.4/jonky.egg-info/dependency_links.txt
--rw-rw-r--   0 jari      (1000) jari      (1000)       65 2023-01-06 19:21:55.000000 jonky-0.0.4/jonky.egg-info/requires.txt
--rw-rw-r--   0 jari      (1000) jari      (1000)        6 2023-01-06 19:21:55.000000 jonky-0.0.4/jonky.egg-info/top_level.txt
--rw-rw-r--   0 jari      (1000) jari      (1000)       38 2023-01-06 19:21:55.000000 jonky-0.0.4/setup.cfg
--rw-rw-r--   0 jari      (1000) jari      (1000)      431 2023-01-06 19:21:35.000000 jonky-0.0.4/setup.py
+drwxrwxr-x   0 jari      (1000) jari      (1000)        0 2023-05-11 21:24:02.000000 jonky-0.0.5/
+-rw-rw-r--   0 jari      (1000) jari      (1000)      132 2023-05-11 21:24:02.000000 jonky-0.0.5/PKG-INFO
+drwxrwxr-x   0 jari      (1000) jari      (1000)        0 2023-05-11 21:24:02.000000 jonky-0.0.5/jonky/
+-rw-rw-r--   0 jari      (1000) jari      (1000)      177 2022-03-11 06:39:27.000000 jonky-0.0.5/jonky/__init__.py
+-rw-rw-r--   0 jari      (1000) jari      (1000)    24546 2023-04-03 15:50:56.000000 jonky-0.0.5/jonky/drawable.py
+-rw-rw-r--   0 jari      (1000) jari      (1000)     1255 2023-04-03 13:59:24.000000 jonky-0.0.5/jonky/helpers.py
+-rw-rw-r--   0 jari      (1000) jari      (1000)     7605 2023-04-03 15:52:30.000000 jonky-0.0.5/jonky/jonky_main.py
+-rw-rw-r--   0 jari      (1000) jari      (1000)     3011 2021-07-20 19:47:51.000000 jonky-0.0.5/jonky/widget_helpers.py
+-rw-rw-r--   0 jari      (1000) jari      (1000)    14374 2023-04-03 15:17:01.000000 jonky-0.0.5/jonky/widgets.py
+drwxrwxr-x   0 jari      (1000) jari      (1000)        0 2023-05-11 21:24:02.000000 jonky-0.0.5/jonky.egg-info/
+-rw-rw-r--   0 jari      (1000) jari      (1000)      132 2023-05-11 21:24:02.000000 jonky-0.0.5/jonky.egg-info/PKG-INFO
+-rw-rw-r--   0 jari      (1000) jari      (1000)      266 2023-05-11 21:24:02.000000 jonky-0.0.5/jonky.egg-info/SOURCES.txt
+-rw-rw-r--   0 jari      (1000) jari      (1000)        1 2023-05-11 21:24:02.000000 jonky-0.0.5/jonky.egg-info/dependency_links.txt
+-rw-rw-r--   0 jari      (1000) jari      (1000)       65 2023-05-11 21:24:02.000000 jonky-0.0.5/jonky.egg-info/requires.txt
+-rw-rw-r--   0 jari      (1000) jari      (1000)        6 2023-05-11 21:24:02.000000 jonky-0.0.5/jonky.egg-info/top_level.txt
+-rw-rw-r--   0 jari      (1000) jari      (1000)       38 2023-05-11 21:24:02.000000 jonky-0.0.5/setup.cfg
+-rw-rw-r--   0 jari      (1000) jari      (1000)      432 2023-05-11 21:23:30.000000 jonky-0.0.5/setup.py
```

### Comparing `jonky-0.0.4/jonky/drawable.py` & `jonky-0.0.5/jonky/drawable.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,39 +8,193 @@
 import gi
 
 gi.require_version("Pango", "1.0")
 gi.require_version("PangoCairo", "1.0")
 
 from gi.repository import Pango as pango
 from gi.repository import PangoCairo as pangocairo
+from libjari.colors import color_names, convert_color_float
 
-from libjari.colors import convert_color_float
 import math
 from dataclasses import dataclass
 import cairo
 from PIL import Image as PImage
 import PIL
 from enum import Enum
 import numpy as np
 from threading import Thread
 import time
 
 import math
 
 import PIL.Image as Image
 
+color_names.update({k.replace(" ", ""): v for k, v in color_names.items()})
+
+color_names.update(
+    {
+        "aliceblue": "#f0f8ff",
+        "antiquewhite": "#faebd7",
+        "aqua": "#00ffff",
+        "aquamarine": "#7fffd4",
+        "azure": "#f0ffff",
+        "beige": "#f5f5dc",
+        "bisque": "#ffe4c4",
+        "black": "#000000",
+        "blanchedalmond": "#ffebcd",
+        "blue": "#0000ff",
+        "blueviolet": "#8a2be2",
+        "brown": "#a52a2a",
+        "burlywood": "#deb887",
+        "cadetblue": "#5f9ea0",
+        "chartreuse": "#7fff00",
+        "chocolate": "#d2691e",
+        "coral": "#ff7f50",
+        "cornflowerblue": "#6495ed",
+        "cornsilk": "#fff8dc",
+        "crimson": "#dc143c",
+        "cyan": "#00ffff",
+        "darkblue": "#00008b",
+        "darkcyan": "#008b8b",
+        "darkgoldenrod": "#b8860b",
+        "darkgray": "#a9a9a9",
+        "darkgrey": "#a9a9a9",
+        "darkgreen": "#006400",
+        "darkkhaki": "#bdb76b",
+        "darkmagenta": "#8b008b",
+        "darkolivegreen": "#556b2f",
+        "darkorange": "#ff8c00",
+        "darkorchid": "#9932cc",
+        "darkred": "#8b0000",
+        "darksalmon": "#e9967a",
+        "darkseagreen": "#8fbc8f",
+        "darkslateblue": "#483d8b",
+        "darkslategray": "#2f4f4f",
+        "darkslategrey": "#2f4f4f",
+        "darkturquoise": "#00ced1",
+        "darkviolet": "#9400d3",
+        "deeppink": "#ff1493",
+        "deepskyblue": "#00bfff",
+        "dimgray": "#696969",
+        "dimgrey": "#696969",
+        "dodgerblue": "#1e90ff",
+        "firebrick": "#b22222",
+        "floralwhite": "#fffaf0",
+        "forestgreen": "#228b22",
+        "fuchsia": "#ff00ff",
+        "gainsboro": "#dcdcdc",
+        "ghostwhite": "#f8f8ff",
+        "gold": "#ffd700",
+        "goldenrod": "#daa520",
+        "gray": "#808080",
+        "grey": "#808080",
+        "green": "#008000",
+        "greenyellow": "#adff2f",
+        "honeydew": "#f0fff0",
+        "hotpink": "#ff69b4",
+        "indianred": "#cd5c5c",
+        "indigo": "#4b0082",
+        "ivory": "#fffff0",
+        "khaki": "#f0e68c",
+        "lavender": "#e6e6fa",
+        "lavenderblush": "#fff0f5",
+        "lawngreen": "#7cfc00",
+        "lemonchiffon": "#fffacd",
+        "lightblue": "#add8e6",
+        "lightcoral": "#f08080",
+        "lightcyan": "#e0ffff",
+        "lightgoldenrodyellow": "#fafad2",
+        "lightgray": "#d3d3d3",
+        "lightgrey": "#d3d3d3",
+        "lightgreen": "#90ee90",
+        "lightpink": "#ffb6c1",
+        "lightsalmon": "#ffa07a",
+        "lightseagreen": "#20b2aa",
+        "lightskyblue": "#87cefa",
+        "lightslategray": "#778899",
+        "lightslategrey": "#778899",
+        "lightsteelblue": "#b0c4de",
+        "lightyellow": "#ffffe0",
+        "lime": "#00ff00",
+        "limegreen": "#32cd32",
+        "linen": "#faf0e6",
+        "magenta": "#ff00ff",
+        "maroon": "#800000",
+        "mediumaquamarine": "#66cdaa",
+        "mediumblue": "#0000cd",
+        "mediumorchid": "#ba55d3",
+        "mediumpurple": "#9370db",
+        "mediumseagreen": "#3cb371",
+        "mediumslateblue": "#7b68ee",
+        "mediumspringgreen": "#00fa9a",
+        "mediumturquoise": "#48d1cc",
+        "mediumvioletred": "#c71585",
+        "midnightblue": "#191970",
+        "mintcream": "#f5fffa",
+        "mistyrose": "#ffe4e1",
+        "moccasin": "#ffe4b5",
+        "navajowhite": "#ffdead",
+        "navy": "#000080",
+        "oldlace": "#fdf5e6",
+        "olive": "#808000",
+        "olivedrab": "#6b8e23",
+        "orange": "#ffa500",
+        "orangered": "#ff4500",
+        "orchid": "#da70d6",
+        "palegoldenrod": "#eee8aa",
+        "palegreen": "#98fb98",
+        "paleturquoise": "#afeeee",
+        "palevioletred": "#db7093",
+        "papayawhip": "#ffefd5",
+        "peachpuff": "#ffdab9",
+        "peru": "#cd853f",
+        "pink": "#ffc0cb",
+        "plum": "#dda0dd",
+        "powderblue": "#b0e0e6",
+        "purple": "#800080",
+        "red": "#ff0000",
+        "rosybrown": "#bc8f8f",
+        "royalblue": "#4169e1",
+        "saddlebrown": "#8b4513",
+        "salmon": "#fa8072",
+        "sandybrown": "#f4a460",
+        "seagreen": "#2e8b57",
+        "seashell": "#fff5ee",
+        "sienna": "#a0522d",
+        "silver": "#c0c0c0",
+        "skyblue": "#87ceeb",
+        "slateblue": "#6a5acd",
+        "slategray": "#708090",
+        "slategrey": "#708090",
+        "snow": "#fffafa",
+        "springgreen": "#00ff7f",
+        "steelblue": "#4682b4",
+        "tan": "#d2b48c",
+        "teal": "#008080",
+        "thistle": "#d8bfd8",
+        "tomato": "#ff6347",
+        "turquoise": "#40e0d0",
+        "violet": "#ee82ee",
+        "wheat": "#f5deb3",
+        "white": "#ffffff",
+        "whitesmoke": "#f5f5f5",
+        "yellow": "#ffff00",
+        "yellowgreen": "#9acd32",
+    }
+)
+
 
 def _rad(deg):
     return deg * math.pi / 180
 
 
 def _ccf(color):
     if color is None:
         return color
-    return convert_color_float(color)
+    return convert_color_float(color.lower().replace(" ", ""))
 
 
 def from_pil(im, alpha=1.0, format=cairo.FORMAT_ARGB32):
     """
     :param im: Pillow Image
     :param alpha: 0..1 alpha to add to non-alpha images
     :param format: Pixel format for output surface
@@ -65,17 +219,15 @@
                 self.__setattr__(attr_name, out)
             start_time = curr_time
         else:
             time.sleep(period / 10)
 
 
 class Pose:
-    """yaw is in deg
-
-    """
+    """yaw is in deg"""
 
     def __init__(self, x=0, y=0, yaw=0):
         self.x = x
         self.y = y
         self.yaw = yaw
 
     @property
@@ -93,14 +245,18 @@
     def __add__(self, b):
         a = self
         return Pose(a.x + b.x, a.y + b.y, a.yaw + b.yaw)
 
 
 class Color:
     def __init__(self, r=0, g=0, b=0, a=1):
+        if isinstance(r, Color):
+            r, g, b = r.r, r.g, r.b
+        if isinstance(r, str):
+            r, g, b = _ccf(r)
         self.r = r
         self.g = g
         self.b = b
         self.a = a
         if any([r > 1, g > 1, b > 1, a > 1]):
             self.r = r / 255
             self.g = g / 255
@@ -188,17 +344,15 @@
     NONE = "none"
     VERTICAL = "vertical"
     HORIZONTAL = "horizontal"
     GRID = "grid"
 
 
 class Drawable:
-    """Documentation for Drawable
-
-    """
+    """Documentation for Drawable"""
 
     def __init__(
         self, pose=None, color=None, scale=1.0, fill_color=None, pose_transformer=None
     ):
         self.color = Color.new(color)
         self.fill_color = Color.new(fill_color) if fill_color else None
         if pose is None:
@@ -243,29 +397,32 @@
         self.pose_transformer = transformer
         return self
 
     def set_alpha(self, alpha):
         self.color.a = alpha
         return self
 
-    def pre_draw(self, ctx, do_xform=True):
+    def pre_draw(self, ctx, do_xform=True, dpi_converter=None):
         ctx.save()
         ctx.set_source_rgba(*(self.color.tup))
         if self.color.a != 1.0 or (self.fill_color and self.fill_color.a != 1.0):
             ctx.set_operator(cairo.OPERATOR_ATOP)
         if do_xform:
-            ctx.translate(self.pose.x, self.pose.y)
+            if not dpi_converter:
+                ctx.translate(self.pose.x, self.pose.y)
+            else:
+                ctx.translate(*dpi_converter(self.pose.x, self.pose.y))
             if self.scale:
                 ctx.scale(self.scale, self.scale)
             ctx.rotate(self.pose.yaw_rad)
 
     def post_draw(self, ctx):
         ctx.restore()
 
-    def draw(self, ctx):
+    def draw(self, ctx, dpi_converter=None):
         pass
 
 
 class Group(Drawable):
     def __init__(self, nodes=None, packing=None, pack_padding=0, *args, **kwargs):
         super(Group, self).__init__(*args, **kwargs)
         self.packing = packing
@@ -273,15 +430,15 @@
             self.packing = Packing(self.packing)
         self.pack_padding = pack_padding
         if packing is None:
             self.packing = Packing.NONE
         assert self.packing != Packing.GRID
         self.nodes = nodes if nodes is not None else []
 
-    def draw(self, ctx, do_xform=True):
+    def draw(self, ctx, do_xform=True, dpi_converter=None):
         # print(f"drawing {type(self)}")
         self.pre_draw(ctx, do_xform)
         rect = None
         xshift = 0
         yshift = 0
         for i, node in enumerate(self.nodes):
             if self.packing != Packing.NONE:
@@ -289,15 +446,15 @@
                     node.set_pose(
                         node.packing_corrections.x, yshift + node.packing_corrections.y
                     )
                 if self.packing == Packing.HORIZONTAL:
                     node.set_pose(
                         xshift + node.packing_corrections.x, node.packing_corrections.y
                     )
-            _rect = node.draw(ctx)
+            _rect = node.draw(ctx, dpi_converter=dpi_converter)
             if self.packing == Packing.NONE:
                 _rect.x += node.pose.x
                 _rect.y += node.pose.y
 
             if rect is None:
                 rect = _rect
             else:
@@ -311,79 +468,83 @@
                 ctx.set_source_rgb(0, 0, 1)
                 ctx.set_line_width(2)
                 ctx.rectangle(r.x, r.y, r.w, r.h)
                 ctx.stroke()
 
             if self.packing != Packing.NONE:
                 if self.packing == Packing.VERTICAL:
-                    yshift += _rect.h + self.pack_padding
+                    if dpi_converter:
+                        yshift += _rect.h + dpi_converter(self.pack_padding)
+                    else:
+                        yshift += _rect.h + self.pack_padding
                 if self.packing == Packing.HORIZONTAL:
-                    xshift += _rect.w + self.pack_padding
+                    if dpi_converter:
+                        xshift += _rect.w + dpi_converter(self.pack_padding)
+                    else:
+                        xshift += _rect.w + self.pack_padding
         self.post_draw(ctx)
         return rect.scale(self.scale)
 
 
 class BakedGroup(Group):
     def __init__(self, *args, **kwargs):
         super(BakedGroup, self).__init__(*args, **kwargs)
         self.surface = None
 
-    def draw(self, ctx: cairo.Context):
+    def draw(self, ctx: cairo.Context, dpi_converter=None):
         if not self.surface:
-            size = super(BakedGroup, self).draw(ctx, True)
+            size = super(BakedGroup, self).draw(ctx, True, dpi_converter=dpi_converter)
             self.surface = cairo.ImageSurface(
                 cairo.FORMAT_ARGB32, int(size.w) * 2, int(size.h) * 2
             )
             surface_ctx = cairo.Context(self.surface)
             surface_ctx.scale(2.0, 2.0)
 
             surface_ctx.set_source_rgba(1.0, 1.0, 1.0, 0.0)
             surface_ctx.set_operator(cairo.OPERATOR_SOURCE)
             surface_ctx.paint()
 
-            super(BakedGroup, self).draw(surface_ctx, False)
+            super(BakedGroup, self).draw(surface_ctx, False, dpi_converter=dpi_converter)
             self.surface.write_to_png("/tmp/test.png")
         else:
-            self.pre_draw(ctx, True)
+            self.pre_draw(ctx, True, dpi_converter=dpi_converter)
             ctx.scale(0.5, 0.5)
             ctx.rectangle(0, 0, self.surface.get_width(), self.surface.get_height())
             ctx.set_source_rgba(0, 0, 0, 0.0)
             ctx.set_source_surface(self.surface)
             ctx.clip()
             ctx.set_operator(cairo.OPERATOR_ATOP)
             ctx.paint()
             self.post_draw(ctx)
 
 
 class Text(Drawable):
-    """Documentation for Text
-
-    """
+    """Documentation for Text"""
 
     def __init__(self, font, font_size, text, on_bottom=False, *args, **kwargs):
         super(Text, self).__init__(*args, **kwargs)
         self.font = font
         self.font_size = font_size
         self.text = text
         self.on_bottom = on_bottom
 
-    def draw(self, ctx):
-        super(Text, self).draw(ctx)
+    def draw(self, ctx, dpi_converter=None):
+        super(Text, self).draw(ctx, dpi_converter=dpi_converter)
         yshift = 0
         x, y = self.pose.x, self.pose.y
         w = 0
         h = 0
         rect = None
         for line in self.text.split("\n"):
             ctx.select_font_face(self.font)
             ctx.set_font_size(self.font_size)
             (x, y, width, height, dx, dy) = ctx.text_extents(self.text)
             w = max(width, w)
 
-            self.pre_draw(ctx)
+            self.pre_draw(ctx, dpi_converter=dpi_converter)
             ctx.translate(0, yshift)
             if not self.on_bottom:
                 ctx.translate(-x, -y)
 
             ctx.show_text(line)
             if rect is None:
                 rect = Rect(-x, -y, width, height)
@@ -393,17 +554,15 @@
             yshift += self.font_size
             self.post_draw(ctx)
         h = yshift
         return rect
 
 
 class PangoText(Drawable):
-    """Documentation for Text
-
-    """
+    """Documentation for Text"""
 
     def __init__(
         self,
         text,
         font_size=50,
         font="Arial",
         alignment="left",
@@ -416,30 +575,39 @@
         self.font = font
         self.font_size = font_size
         self.text = text
         self.width = width if width else 10000
         self.alignment = alignment
         self.line_spacing = line_spacing
 
-    def draw(self, ctx):
-        super(PangoText, self).draw(ctx)
-        self.pre_draw(ctx)
+    def draw(self, ctx, dpi_converter=None):
+        super(PangoText, self).draw(ctx, dpi_converter=dpi_converter)
+        self.pre_draw(ctx, dpi_converter=dpi_converter)
 
         layout = pangocairo.create_layout(ctx)
-        layout.set_width(pango.units_from_double(self.width))
-        layout.set_line_spacing(self.line_spacing)
+        if not dpi_converter:
+            layout.set_width(pango.units_from_double(self.width))
+            layout.set_line_spacing(self.line_spacing)
+            layout.set_font_description(
+                pango.FontDescription(f"{self.font} {self.font_size}")
+            )
+        else:
+            layout.set_width(pango.units_from_double(dpi_converter(self.width)))
+            layout.set_line_spacing(dpi_converter(self.line_spacing))
+            layout.set_font_description(
+                pango.FontDescription(
+                    f"{self.font} {dpi_converter(self.font_size)}"
+                )
+            )
         alignment = pango.Alignment.LEFT
         if self.alignment == "right":
             alignment = pango.Alignment.RIGHT
         if self.alignment == "center":
             alignment = pango.Alignment.CENTER
         layout.set_alignment(alignment)
-        layout.set_font_description(
-            pango.FontDescription(f"{self.font} {self.font_size}")
-        )
         layout.set_markup(self.text)
 
         pangocairo.show_layout(ctx, layout)
 
         r = layout.get_pixel_extents()[0]
 
         self.post_draw(ctx)
@@ -465,17 +633,17 @@
         if isinstance(src, str):
             self.src = from_pil(PImage.open(src), alpha=opacity)
 
         # apparently there's no good way to figure out if an image is a PIL image ...
         if self.src is None:
             self.src = from_pil(src, alpha=opacity)
 
-    def draw(self, ctx: cairo.Context):
-        super(JImage, self).draw(ctx)
-        self.pre_draw(ctx)
+    def draw(self, ctx: cairo.Context, dpi_converter=None):
+        super(JImage, self).draw(ctx, dpi_converter=dpi_converter)
+        self.pre_draw(ctx, dpi_converter=dpi_converter)
         ctx.set_source_rgba(0, 0, 0, 0.0)
 
         # ctx.translate(-self.src.get_width() / 2, -self.src.get_height() / 2)
 
         ctx.rectangle(0, 0, self.src.get_width(), self.src.get_height())
         ctx.set_operator(cairo.OPERATOR_OVER)
         ctx.set_source_surface(self.src)
@@ -489,15 +657,15 @@
 
 class Shape(Drawable):
     def __init__(self, stroke_width=1, *args, **kwargs):
         super(Shape, self).__init__(*args, **kwargs)
         # assert fill_color is None
         self.stroke_width = stroke_width
 
-    def draw(self, ctx: cairo.Context):
+    def draw(self, ctx: cairo.Context, dpi_converter=None):
         pass
 
 
 class Arc(Shape):
     def __init__(self, radius, start_angle, end_angle, *args, **kwargs):
         super(Arc, self).__init__(*args, **kwargs)
         self.start_angle = start_angle
@@ -510,16 +678,16 @@
 
     @radius.setter
     def radius(self, val):
         self._radius = val
         self.packing_corrections.x = val
         self.packing_corrections.y = val
 
-    def draw(self, ctx: cairo.Context):
-        self.pre_draw(ctx)
+    def draw(self, ctx: cairo.Context, dpi_converter=None):
+        self.pre_draw(ctx, dpi_converter=dpi_converter)
         ctx.set_line_width(self.stroke_width)
         ctx.arc(
             0,
             0,
             self.radius,
             self.start_angle * math.pi / 180,
             self.end_angle * math.pi / 180,
@@ -546,16 +714,16 @@
 
 
 class Polygon(Shape):
     def __init__(self, point_list, *args, **kwargs):
         super(Polygon, self).__init__(*args, **kwargs)
         self.point_list = [Point2.new(p) for p in point_list]
 
-    def draw(self, ctx: cairo.Context):
-        self.pre_draw(ctx)
+    def draw(self, ctx: cairo.Context, dpi_converter=None):
+        self.pre_draw(ctx, dpi_converter=dpi_converter)
         ctx.set_line_width(self.stroke_width)
         ctx.move_to(*(self.point_list[0].tup))
         for pt in self.point_list[1:]:
             ctx.line_to(*(pt.tup))
 
         rect = Rect.from_extents(ctx.stroke_extents())
         if self.fill_color:
@@ -572,16 +740,16 @@
 class Rectangle(Shape):
     def __init__(self, width, height, corner_radius=0, *args, **kwargs):
         super(Rectangle, self).__init__(*args, **kwargs)
         self.width = width
         self.height = height
         self.corner_radius = corner_radius
 
-    def draw(self, ctx: cairo.Context):
-        self.pre_draw(ctx)
+    def draw(self, ctx: cairo.Context, dpi_converter=None):
+        self.pre_draw(ctx, dpi_converter=dpi_converter)
         w, h, r = self.width, self.height, self.corner_radius
         r = min(r, w / 2, h / 2)
         ctx.set_line_width(self.stroke_width)
         ctx.move_to(r, 0)
         ctx.line_to(w - r, 0)
         if r != 0:
             ctx.arc(w - r, r, r, _rad(-90), 0)
@@ -645,7 +813,9 @@
                     curr_r * math.cos(step * angle * math.pi / 180),
                     curr_r * math.sin(step * angle * math.pi / 180),
                 )
             )
             curr_r += exp
 
         self.point_list = pts
+
+RichText = PangoText
```

### Comparing `jonky-0.0.4/jonky/helpers.py` & `jonky-0.0.5/jonky/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,11 @@
 from .drawable import Group, Packing, Color
 from .jonky_main import JonkyImage
 
 
-class DPIConverter:
-    def __init__(self, dpi=300):
-        self.dpi = dpi
-
-    def __call__(self, inval, inval2=None, intify=False):
-        cvt = int if intify else lambda x: x
-        if inval2 is not None:
-            return [cvt(inval * self.dpi), cvt(inval2 * self.dpi)]
-        # inval is either one value or a list/tuple of inches
-        if isinstance(inval, (list, tuple)):
-            return [cvt(iv * self.dpi) for iv in inval]
-        return cvt(inval * self.dpi)
-
-
 def make_jonky_grids(items_in, columns, rows, vertical_spacing=0, horizontal_spacing=0):
     items = [i for i in items_in]
     out = []
     i = 0
     while items:
         i += 1
         print(i)
```

### Comparing `jonky-0.0.4/jonky/jonky_main.py` & `jonky-0.0.5/jonky/jonky_main.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,18 +16,33 @@
 
 def switch_channel_order(inarr):
     channels = [inarr[:, :, i] for i in range(inarr.shape[-1])]
     channels = [channels[2 - i] for i in range(inarr.shape[-1])]
     return np.stack(channels, -1)
 
 
-class Jonky(object):
-    """Base class for handling the window and other things
+class DPIConverter:
+    def __init__(self, dpi=300):
+        self.dpi = dpi
+
+    def __call__(self, inval, inval2=None, intify=False):
+        cvt = int if intify else lambda x: x
+        if inval2 is not None:
+            return [cvt(inval * self.dpi), cvt(inval2 * self.dpi)]
+        # inval is either one value or a list/tuple of inches
+        if isinstance(inval, (list, tuple)):
+            return [cvt(iv * self.dpi) for iv in inval]
+        return cvt(inval * self.dpi)
+
+    def rev(self, inval):
+        return inval / self.dpi
+
 
-    """
+class Jonky(object):
+    """Base class for handling the window and other things"""
 
     def __init__(self, period_in_sec=0.5, target_size=None):
         super(Jonky, self).__init__()
         self.start_time = time.time()
         self.period_in_sec = period_in_sec
         self.root = Gdk.get_default_root_window()
         self.last_run_time = None
@@ -81,27 +96,42 @@
                     item._pose_correction, self.curr_time - self.start_time
                 )
             item.draw(cr)
         self.root.process_all_updates()
         cr.restore()
 
 
-class JonkyImage:
-    def __init__(self, width, height, nodes=None, background_color=None, scale=1):
+class Canvas:
+    def __init__(
+        self,
+        width,
+        height,
+        nodes=None,
+        background_color="white",
+        scale=1,
+        dpi_converter=None,
+    ):
         if nodes is None:
             nodes = []
         self.start_time = time.time()
-        self.width = int(width * scale)
-        self.height = int(height * scale)
+        if dpi_converter is not None and not isinstance(dpi_converter, DPIConverter):
+            dpi_converter = DPIConverter(dpi_converter)
+        if dpi_converter is None:
+            self.width = int(width * scale)
+            self.height = int(height * scale)
+        else:
+            self.width = int(dpi_converter(width) * scale)
+            self.height = int(dpi_converter(height) * scale)
         self.buffer = cairo.ImageSurface(cairo.FORMAT_ARGB32, self.width, self.height)
         self.cairo_context = cairo.Context(self.buffer)
         self.curr_time = time.time()
         self.scale = scale
-        self.background_color = background_color
+        self.background_color = Color(background_color)
         self.nodes = nodes
+        self.dpi_converter = dpi_converter
 
     def draw(self):
         cr: cairo.Context = self.cairo_context
         cr.save()
         if self.background_color:
             cr.set_source_rgba(*(self.background_color.tup))
         else:
@@ -111,20 +141,20 @@
         cr.scale(self.scale, self.scale)
         rects = []
         for item in self.nodes:
             if item.pose_transformer:
                 item.pose_transformer(
                     item._pose_correction, self.curr_time - self.start_time
                 )
-            r = item.draw(cr)
+            r = item.draw(cr, dpi_converter=self.dpi_converter)
 
             # Debug rectangle drawing
             if DEBUG:
                 cr.save()
-                item.pre_draw(cr)
+                item.pre_draw(cr, dpi_converter=self.dpi_converter)
                 cr.set_source_rgb(1, 0, 1)
                 cr.set_line_width(1)
                 cr.rectangle(r.x, r.y, r.w, r.h)
                 cr.stroke()
                 item.post_draw(cr)
                 cr.restore()
 
@@ -147,29 +177,45 @@
             array = switch_channel_order(array)
         return array
 
     def to_opencv(self):
         return self.to_numpy(rgb=False)
 
 
-class JonkyPS:
+class CanvasPS:
     def __init__(
-        self, width, height, filename, nodes=None, background_color=None, scale=1
+        self,
+        width,
+        height,
+        filename,
+        nodes=None,
+        background_color="white",
+        scale=1,
+        dpi_converter=None,
     ):
         self.start_time = time.time()
-        self.width = int(width * scale)
-        self.height = int(height * scale)
+
+        if dpi_converter is not None and not isinstance(dpi_converter, DPIConverter):
+            dpi_converter = DPIConverter(dpi_converter)
+
+        if dpi_converter is None:
+            self.width = int(width * scale)
+            self.height = int(height * scale)
+        else:
+            self.width = int(dpi_converter(width) * scale)
+            self.height = int(dpi_converter(height) * scale)
         if ".pdf" in filename:
             self.buffer = cairo.PDFSurface(filename, self.width, self.height)
         elif ".svg" in filename:
             self.buffer = cairo.SVGSurface(filename, self.width, self.height)
         self.curr_time = time.time()
         self.scale = scale
-        self.background_color = background_color
+        self.background_color = Color(background_color)
         self.nodes = nodes or []
+        self.dpi_converter = dpi_converter
 
     def draw(self, finish=True):
         self.cairo_context = cairo.Context(self.buffer)
         cr: cairo.Context = self.cairo_context
         cr.save()
         if self.background_color:
             cr.set_source_rgba(*(self.background_color.tup))
@@ -180,15 +226,19 @@
         cr.scale(self.scale, self.scale)
         rects = []
         for item in self.nodes:
             if item.pose_transformer:
                 item.pose_transformer(
                     item._pose_correction, self.curr_time - self.start_time
                 )
-            r = item.draw(cr)
+            r = item.draw(cr, dpi_converter=self.dpi_converter)
         cr.restore()
         self.buffer.show_page()
         self.nodes = []
         if finish:
             self.buffer.finish()
 
         return self
+
+
+JonkyImage = Canvas
+JonkyPS = CanvasPS
```

### Comparing `jonky-0.0.4/jonky/widget_helpers.py` & `jonky-0.0.5/jonky/widget_helpers.py`

 * *Files identical despite different names*

### Comparing `jonky-0.0.4/jonky/widgets.py` & `jonky-0.0.5/jonky/widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,16 +82,16 @@
 
 
 class TimeDial(Group):
     def __init__(self, radius, width, *args, **kwargs):
         super(TimeDial, self).__init__(draw_ring(radius, width), *args, **kwargs)
         self.radius = radius
 
-    def draw(self, ctx, do_xform=True):
-        return super(TimeDial, self).draw(ctx, do_xform)
+    def draw(self, ctx, do_xform=True, dpi_converter=None):
+        return super(TimeDial, self).draw(ctx, do_xform, dpi_converter=dpi_converter)
 
 
 def make_scaler(max_val, intify=False):
     def scaler(frac):
         out = max_val * frac
         if intify:
             out = int(out)
@@ -117,20 +117,20 @@
                 stroke_width=1,
                 color=Color.named("white", 0.6),
                 fill_color=Color.named("white", 0.6),
             )
         )
         self.timezone = timezone
 
-    def draw(self, ctx):
+    def draw(self, ctx, dpi_converter=None):
         m = maya.when("now").datetime(to_timezone=self.timezone)
         hour_val = m.hour + m.minute / 60
         angle = 360 / 24 * (hour_val) - 9 * 15
         self.nodes[-1].set_pose(yaw=angle)
-        return super(ConcirCal, self).draw(ctx)
+        return super(ConcirCal, self).draw(ctx, dpi_converter=dpi_converter)
 
 
 class LineWithText(Group):
     def __init__(self, font, font_size, text, width, stroke_width, *args, **kwargs):
         self.nodes = []
         super(LineWithText, self).__init__(*args, **kwargs)
         self.width = width
@@ -261,15 +261,15 @@
                 (
                     maya.parse("10am", timezone=self.tz).epoch,
                     maya.parse("10pm", timezone=self.tz).epoch,
                     "RE AUTHORIZE GCALCLI " * 100,
                 )
             ]
 
-    def draw(self, ctx):
+    def draw(self, ctx, dpi_converter=None):
         _s = self._s
         final_lines = []
         timestamp = self.time_function()
         le_time = maya.MayaDT(timestamp).datetime(to_timezone=self.tz)
         offset = le_time.minute * 60
         hr = le_time.hour
 
@@ -334,15 +334,15 @@
                     stroke_width=self.stroke_width,
                     color="E8E9A1",
                     fill_color=Color.named("white", 0.4),
                 ).set_pose(self.stroke_width * 2, y=start_loc)
             )
 
         self.nodes = self.side_lines + final_lines + rects
-        return super(DayCal, self).draw(ctx)
+        return super(DayCal, self).draw(ctx, dpi_converter=dpi_converter)
 
 
 tsize = 20
 
 
 def datetime_strip_minutes_seconds(date: datetime):
     return datetime(date.year, date.month, date.day)
@@ -374,15 +374,15 @@
         self.packing = Packing.VERTICAL
         self.font = font
         self.size = size
         self.width = width
         self.pack_padding = size / 4
         self.i = 0
 
-    def draw(self, ctx):
+    def draw(self, ctx, dpi_converter=None):
         self.i += 1
         self.nodes = []
         hb = orgload(self.filename)
         seen = {}
         for child in hb.children:
             if child.heading in seen:
                 continue
@@ -415,15 +415,15 @@
                 )
             )
             self.nodes.append(
                 Group(other_group, packing=Packing.HORIZONTAL).set_scale(
                     self.size / 100
                 )
             )
-        return super(OrgHabits, self).draw(ctx)
+        return super(OrgHabits, self).draw(ctx, dpi_converter=dpi_converter)
 
 
 class Dial(Group):
     def __init__(self, radius, stroke_width, val=0, name="", *args, **kwargs):
         super(Dial, self).__init__(*args, **kwargs)
         self.radius = radius
         self.nodes.append(
@@ -470,11 +470,11 @@
             PangoText(font="", font_size=radius * 0.3, text="", color="white").set_pose(
                 radius * 0.1, radius * 0.2
             )
         )
         self.val = val
         self.name = name
 
-    def draw(self, ctx):
+    def draw(self, ctx, dpi_converter=None):
         self.nodes[-2].set_pose(yaw=90 + self.val * (360 - 90))
         self.nodes[-1].text = f"{int(self.val*100)}%\n{self.name}"
-        return super(Dial, self).draw(ctx)
+        return super(Dial, self).draw(ctx, dpi_converter=dpi_converter)
```

