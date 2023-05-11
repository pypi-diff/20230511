# Comparing `tmp/pagexml_tools-0.3.3.tar.gz` & `tmp/pagexml_tools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pagexml_tools-0.3.3.tar", max compression
+gzip compressed data, was "pagexml_tools-0.3.4.tar", max compression
```

## Comparing `pagexml_tools-0.3.3.tar` & `pagexml_tools-0.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1090 2023-02-16 14:56:00.647522 pagexml_tools-0.3.3/LICENSE
--rw-r--r--   0        0        0     3617 2023-03-14 15:54:03.335111 pagexml_tools-0.3.3/README.md
--rw-r--r--   0        0        0       22 2023-04-12 10:15:14.149186 pagexml_tools-0.3.3/pagexml/__init__.py
--rw-r--r--   0        0        0        0 2022-07-06 13:20:40.880517 pagexml_tools-0.3.3/pagexml/analysis/__init__.py
--rw-r--r--   0        0        0    23754 2023-03-14 15:54:03.352243 pagexml_tools-0.3.3/pagexml/analysis/layout_stats.py
--rw-r--r--   0        0        0     5201 2023-03-14 15:54:03.352545 pagexml_tools-0.3.3/pagexml/analysis/stats.py
--rw-r--r--   0        0        0    49127 2023-03-14 15:54:03.353422 pagexml_tools-0.3.3/pagexml/analysis/text_stats.py
--rw-r--r--   0        0        0    15944 2023-03-14 16:06:33.454463 pagexml_tools-0.3.3/pagexml/column_parser.py
--rw-r--r--   0        0        0        0 2022-07-06 13:20:40.881048 pagexml_tools-0.3.3/pagexml/helper/__init__.py
--rw-r--r--   0        0        0    12061 2023-03-14 16:35:08.831818 pagexml_tools-0.3.3/pagexml/helper/file_helper.py
--rw-r--r--   0        0        0    22113 2023-03-14 16:08:28.033909 pagexml_tools-0.3.3/pagexml/helper/pagexml_helper.py
--rw-r--r--   0        0        0    17353 2023-03-14 16:09:34.238525 pagexml_tools-0.3.3/pagexml/helper/text_helper.py
--rwxr-xr-x   0        0        0        0 2022-04-25 11:16:08.181810 pagexml_tools-0.3.3/pagexml/model/__init__.py
--rw-r--r--   0        0        0    38072 2023-03-14 15:54:03.355625 pagexml_tools-0.3.3/pagexml/model/physical_document_model.py
--rw-r--r--   0        0        0    20899 2023-04-12 10:15:00.526775 pagexml_tools-0.3.3/pagexml/parser.py
--rw-r--r--   0        0        0        0 2022-07-06 13:20:40.882557 pagexml_tools-0.3.3/pagexml/plotting/__init__.py
--rw-r--r--   0        0        0     1235 2023-03-01 09:40:10.838606 pagexml_tools-0.3.3/pagexml/plotting/plot_dist.py
--rw-r--r--   0        0        0      963 2023-03-01 13:10:44.524749 pagexml_tools-0.3.3/pagexml/transform/segmentation.py
--rw-r--r--   0        0        0     1312 2023-04-12 10:15:14.122787 pagexml_tools-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     4923 1970-01-01 00:00:00.000000 pagexml_tools-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-02-16 14:56:00.647522 pagexml_tools-0.3.4/LICENSE
+-rw-r--r--   0        0        0     3617 2023-03-14 15:54:03.335111 pagexml_tools-0.3.4/README.md
+-rw-r--r--   0        0        0       22 2023-05-11 11:05:23.354405 pagexml_tools-0.3.4/pagexml/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-06 13:20:40.880517 pagexml_tools-0.3.4/pagexml/analysis/__init__.py
+-rw-r--r--   0        0        0    27578 2023-05-11 08:26:46.070362 pagexml_tools-0.3.4/pagexml/analysis/layout_stats.py
+-rw-r--r--   0        0        0     5201 2023-03-14 15:54:03.352545 pagexml_tools-0.3.4/pagexml/analysis/stats.py
+-rw-r--r--   0        0        0    49127 2023-03-14 15:54:03.353422 pagexml_tools-0.3.4/pagexml/analysis/text_stats.py
+-rw-r--r--   0        0        0    15944 2023-03-14 16:06:33.454463 pagexml_tools-0.3.4/pagexml/column_parser.py
+-rw-r--r--   0        0        0        0 2022-07-06 13:20:40.881048 pagexml_tools-0.3.4/pagexml/helper/__init__.py
+-rw-r--r--   0        0        0    12074 2023-05-11 08:26:46.071073 pagexml_tools-0.3.4/pagexml/helper/file_helper.py
+-rw-r--r--   0        0        0    22113 2023-03-14 16:08:28.033909 pagexml_tools-0.3.4/pagexml/helper/pagexml_helper.py
+-rw-r--r--   0        0        0    17662 2023-05-11 08:26:46.071879 pagexml_tools-0.3.4/pagexml/helper/text_helper.py
+-rwxr-xr-x   0        0        0        0 2022-04-25 11:16:08.181810 pagexml_tools-0.3.4/pagexml/model/__init__.py
+-rw-r--r--   0        0        0    39967 2023-05-11 10:53:09.323084 pagexml_tools-0.3.4/pagexml/model/physical_document_model.py
+-rw-r--r--   0        0        0    22174 2023-05-11 08:26:46.072606 pagexml_tools-0.3.4/pagexml/parser.py
+-rw-r--r--   0        0        0        0 2022-07-06 13:20:40.882557 pagexml_tools-0.3.4/pagexml/plotting/__init__.py
+-rw-r--r--   0        0        0     1235 2023-03-01 09:40:10.838606 pagexml_tools-0.3.4/pagexml/plotting/plot_dist.py
+-rw-r--r--   0        0        0      963 2023-03-01 13:10:44.524749 pagexml_tools-0.3.4/pagexml/transform/segmentation.py
+-rw-r--r--   0        0        0     1312 2023-05-11 11:05:23.329835 pagexml_tools-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4923 1970-01-01 00:00:00.000000 pagexml_tools-0.3.4/PKG-INFO
```

### Comparing `pagexml_tools-0.3.3/LICENSE` & `pagexml_tools-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.3/README.md` & `pagexml_tools-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.3/pagexml/analysis/layout_stats.py` & `pagexml_tools-0.3.4/pagexml/analysis/layout_stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -175,14 +175,108 @@
         right_x = max(xcoords)
         if left_x != right_x:
             return int(total_avg / (right_x - left_x))
         else:
             return int(total_avg)
 
 
+def sort_coords_above_below_baseline(line: pdm.PageXMLTextLine, debug: int = 0) -> Tuple[List[Tuple[int, int]],
+                                                                                         List[Tuple[int, int]]]:
+    """Split the list of bounding polygon coordinates of a line in sets of points above and below
+    the baseline. When a line has no baseline or no bounding polygon, empty lists are
+    returned
+
+    :param line: a PageXML text line
+    :type line: PageXMLTextLine
+    :param debug: the detail level of debug information (0 = none, higher is more)
+    :type debug: int
+    :return: two lists of bounding polygon points
+    :rtype: tuple
+    """
+    ci_c = 0
+    below_baseline = []
+    above_baseline = []
+    if line.baseline is None:
+        return above_baseline, below_baseline
+    interpolated_baseline_points = [i for i in interpolate_baseline_points(line.baseline.points, step=50).items()]
+    if debug > 2:
+        print('interpolated_baseline_points:', interpolated_baseline_points)
+    sorted_coord_points = sorted(line.coords.points, key=lambda p: p[0])
+    if debug > 0:
+        print('sorted_coord_points:', sorted_coord_points)
+        print('len(sorted_coord_points):', len(sorted_coord_points))
+    if debug > 1:
+        print('ci_c:', ci_c)
+    num_baseline_points = len(line.baseline.points)
+    num_coord_points = len(sorted_coord_points)
+    for ci_b, curr_b in enumerate(interpolated_baseline_points):
+        curr_bx, curr_by = curr_b
+        next_b = interpolated_baseline_points[ci_b + 1] if ci_b + 1 < num_baseline_points else None
+        if debug > 0:
+            print(f'sort_above_below - curr_b: {curr_b}')
+            print('\tci_c:', ci_c, '\tnum_coord_points:', num_coord_points)
+        if ci_c == num_coord_points:
+            break
+        for curr_c in sorted_coord_points[ci_c:]:
+            curr_cx, curr_cy = curr_c
+            if next_b and abs(next_b[0] - curr_cx) < abs(curr_b[0] - curr_cx):
+                break
+            if debug > 0:
+                print(f'sort_above_below - curr_c ({ci_c}): {curr_c}')
+            ci_c += 1
+            if curr_cy > curr_by:
+                if debug > 0:
+                    print(f'sort_above_below - below')
+                below_baseline.append(curr_c)
+            elif curr_cy < curr_by:
+                if debug > 0:
+                    print(f'sort_above_below - above')
+                above_baseline.append(curr_c)
+            else:
+                if debug > 0:
+                    print(f'sort_above_below - neither')
+                pass
+
+    return above_baseline, below_baseline
+
+
+def get_text_heights(line: pdm.PageXMLTextLine, step: int = 50) -> np.array:
+    above_baseline, below_baseline = sort_coords_above_below_baseline(line)
+    int_base = interpolate_baseline_points(line.baseline.points, step=step)
+    int_above = interpolate_baseline_points(above_baseline, step=step)
+
+    height = {}
+    for x in int_base:
+        if x in int_above:
+            height[x] = int_base[x] - int_above[x]
+
+    return np.array(list(height.values()))
+
+
+def get_height_stats(line_heights: np.array) -> Dict[str, int]:
+    return {
+        'max': line_heights.max(),
+        'min': line_heights.min(),
+        'mean': int(round(line_heights.mean())),
+        'median': int(np.median(line_heights))
+    }
+
+
+def get_line_distances(lines: List[pdm.PageXMLTextLine]) -> List[np.ndarray]:
+    all_distances = []
+    for li, curr_line in enumerate(lines):
+        next_line = None
+        if li + 1 < len(lines):
+            next_line = lines[li + 1]
+        if next_line:
+            distances = compute_baseline_distances(curr_line, next_line)
+            all_distances.append(distances)
+        return all_distances
+
+
 def get_textregion_line_distances(text_region: pdm.PageXMLTextRegion) -> List[np.ndarray]:
     """Returns a list of line distance numpy arrays. For each line, its distance
     to the next at 50 pixel intervals is computed and stored in a numpy ndarray.
 
     :param text_region: a TextRegion object that contains TextLines
     :type text_region: PageXMLTextRegion
     :return: a list of numpy ndarrays of line distances
```

### Comparing `pagexml_tools-0.3.3/pagexml/analysis/stats.py` & `pagexml_tools-0.3.4/pagexml/analysis/stats.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.3/pagexml/analysis/text_stats.py` & `pagexml_tools-0.3.4/pagexml/analysis/text_stats.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.3/pagexml/column_parser.py` & `pagexml_tools-0.3.4/pagexml/column_parser.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.3/pagexml/helper/file_helper.py` & `pagexml_tools-0.3.4/pagexml/helper/file_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import glob
 import os
 import tarfile
 import zipfile
 from tarfile import TarFile
 from typing import Dict, Generator, IO, List, Literal, Tuple, Union
 from zipfile import ZipFile
```

### Comparing `pagexml_tools-0.3.3/pagexml/helper/pagexml_helper.py` & `pagexml_tools-0.3.4/pagexml/helper/pagexml_helper.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.3/pagexml/helper/text_helper.py` & `pagexml_tools-0.3.4/pagexml/helper/text_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     for line_file in pagexml_line_files:
         with gzip.open(line_file, 'rt') as fh:
             for line in fh:
                 yield line
 
 
 def get_bbox(doc: pdm.PageXMLDoc):
-    if doc.coords.points is None:
+    if doc is None or doc.coords is None or doc.coords.points is None:
         return None
     return f"{doc.coords.x},{doc.coords.y},{doc.coords.w},{doc.coords.h}"
 
 
 def get_line_format_json(page_doc: pdm.PageXMLTextRegion,
                          use_outer_textregions: bool = False,
                          add_bounding_box: bool = False) -> Generator[Dict[str, any], None, None]:
@@ -174,36 +174,43 @@
     x, y, w, h = [int(part) for part in box_string.split(',')]
     points = [(x, y), (x+w, y), (x+w, y+h), (x, y+h)]
     return pdm.Coords(points)
 
 
 def read_pagexml_docs_from_line_file(line_files: Union[str, List[str]], has_headers: bool = True,
                                      headers: List[str] = None,
-                                     add_bounding_box: bool = False) -> Generator[pdm.PageXMLTextRegion, None, None]:
+                                     add_bounding_box: bool = True) -> Generator[pdm.PageXMLTextRegion, None, None]:
     """Read lines from one or more PageXML line format files and return them
     as PageXMLTextLine objects, grouped by their PageXML document."""
     line_iterator = LineReader(pagexml_line_files=line_files, line_file_headers=headers,
                                has_headers=has_headers, add_bounding_box=add_bounding_box)
     curr_doc = None
     curr_tr = None
     for li, line_dict in enumerate(line_iterator):
+        # print(line_dict.keys())
+        # print(line_dict)
         doc_coords, tr_coords, line_coords = None, None, None
         if add_bounding_box is True:
             doc_coords = transform_box_to_coords(line_dict['doc_box'])
             tr_coords = transform_box_to_coords(line_dict['textregion_box'])
-            line_coords = transform_box_to_coords(line_dict['line_box'])
+            # print('\t', tr_coords, line_dict['textregion_box'])
+            if line_dict['line_box'] is None:
+                line_coords = None
+            else:
+                line_coords = transform_box_to_coords(line_dict['line_box'])
         if curr_doc is None or curr_doc.id != line_dict['doc_id']:
             if curr_doc is not None:
                 yield curr_doc
             curr_doc = pdm.PageXMLScan(doc_id=line_dict['doc_id'], coords=doc_coords)
             curr_tr = None
         if curr_tr is None or curr_tr.id != line_dict['textregion_id']:
             curr_tr = pdm.PageXMLTextRegion(doc_id=line_dict['textregion_id'], coords=tr_coords)
             curr_doc.add_child(curr_tr)
             # print(f'creating tr with id {curr_tr.id} and appending to doc with id {curr_doc.id}')
+            # print(curr_tr.coords)
         line = pdm.PageXMLTextLine(doc_id=line_dict['line_id'],
                                    text=line_dict['text'], coords=line_coords)
         curr_tr.add_child(line)
         # print('curr_doc:', curr_doc.id, '\tline doc_id:', line_dict['doc_id'])
         # print('curr_tr:', curr_tr.id, '\tline textregion_id:', line_dict['textregion_id'])
     if curr_doc is not None:
         yield curr_doc
```

### Comparing `pagexml_tools-0.3.3/pagexml/model/physical_document_model.py` & `pagexml_tools-0.3.4/pagexml/model/physical_document_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,15 +301,20 @@
     return coords_list_to_hull_coords([document.coords for document in document_list])
 
 
 def coords_list_to_hull_coords(coords_list):
     # print(coords_list)
     points = np.array([point for coords in coords_list for point in coords.points])
     # print(points)
-    edges = points_to_hull_edges(points)
+    try:
+        edges = points_to_hull_edges(points)
+    except IndexError:
+        print([coords for coords in coords_list])
+        print('points:', points)
+        raise
     # print(edges)
     hull_points = edges_to_hull_points(edges)
     return Coords(hull_points)
 
 
 def points_to_hull_edges(points):
     hull = ConvexHull(points)
@@ -339,17 +344,22 @@
 
     def __init__(self, doc_id: Union[None, str] = None, doc_type: Union[None, str, List[str]] = None,
                  metadata: Dict[str, any] = None, reading_order: Dict[int, str] = None):
         self.id = doc_id
         self.type = doc_type
         self.main_type = 'doc'
         self.metadata = metadata if metadata else {}
+        # if self.id and 'id' not in self.metadata:
+        #     self.metadata['id'] = self.id
+        # if self.metadata and 'type' not in self.metadata:
+        #     self.metadata['type'] = self.type
         self.reading_order: Dict[int, str] = reading_order if reading_order else {}
         self.reading_order_number = {}
         self.parent: Union[StructureDoc, None] = None
+        self.logical_parent: Union[StructureDoc, None] = None
 
     def set_parent(self, parent: StructureDoc):
         """Set parent document and add metadata of parent to this document's metadata"""
         self.parent = parent
         self.add_parent_id_to_metadata()
 
     def add_type(self, doc_type: Union[str, List[str]]) -> None:
@@ -390,14 +400,19 @@
 
     def add_parent_id_to_metadata(self):
         if self.parent:
             self.metadata['parent_type'] = self.parent.main_type
             self.metadata['parent_id'] = self.parent.id
             if hasattr(self.parent, 'main_type'):
                 self.metadata[f'{self.parent.main_type}_id'] = self.parent.id
+        if self.logical_parent:
+            self.metadata['logical_parent_type'] = self.logical_parent.main_type
+            self.metadata['logical_parent_id'] = self.logical_parent.id
+            if hasattr(self.logical_parent, 'main_type'):
+                self.metadata[f'{self.logical_parent.main_type}_id'] = self.logical_parent.id
 
     @property
     def json(self) -> Dict[str, any]:
         json_data = {
             'id': self.id,
             'type': self.type,
             'metadata': self.metadata
@@ -405,16 +420,19 @@
         if self.reading_order:
             json_data['reading_order'] = self.reading_order
         return json_data
 
 
 class PhysicalStructureDoc(StructureDoc):
 
-    def __init__(self, doc_id: str = None, doc_type: Union[str, List[str]] = None,
-                 metadata: Dict[str, any] = None, coords: Coords = None, reading_order: Dict[int, str] = None):
+    def __init__(self, doc_id: str = None,
+                 doc_type: Union[str, List[str]] = None,
+                 metadata: Dict[str, any] = None,
+                 coords: Coords = None,
+                 reading_order: Dict[int, str] = None):
         super().__init__(doc_id=doc_id, doc_type=doc_type, metadata=metadata, reading_order=reading_order)
         self.coords: Union[None, Coords] = coords
         self.main_type = 'physical_structure_doc'
 
     @property
     def json(self) -> Dict[str, any]:
         doc_json = super().json
@@ -439,14 +457,20 @@
         self.logical_parent: Union[StructureDoc, None] = None
 
     def set_logical_parent(self, parent: StructureDoc):
         """Set parent document and add metadata of parent to this document's metadata"""
         self.logical_parent = parent
         self.add_logical_parent_id_to_metadata()
 
+    def set_as_logical_parent(self, children: Union[StructureDoc, List[StructureDoc]]):
+        if isinstance(children, StructureDoc):
+            children = [children]
+        for child in children:
+            child.parent = self
+
     def add_logical_parent_id_to_metadata(self):
         if self.logical_parent:
             self.metadata['logical_parent_type'] = self.logical_parent.main_type
             self.metadata['logical_parent_id'] = self.logical_parent.id
             if hasattr(self.logical_parent, 'main_type'):
                 self.metadata[f'{self.logical_parent.main_type}_id'] = self.logical_parent.id
 
@@ -509,15 +533,15 @@
         self.words: List[PageXMLWord] = words if words else []
         self.metadata['type'] = 'line'
         self.set_as_parent(self.words)
         if doc_type:
             self.add_type(doc_type)
 
     def __repr__(self):
-        content_string = f"id={self.id}, type={self.type}, text={self.text} conf={self.conf}"
+        content_string = f"id={self.id}, type={self.type}, text=\"{self.text}\" conf={self.conf}"
         return f"{self.__class__.__name__}({content_string})"
 
     def __lt__(self, other: PageXMLTextLine):
         """For sorting text lines. Assumptions: reading from left to right,
         top to bottom. If two lines are horizontally overlapping, sort from
         top to bottom, even if the upper lines is more horizontally indented."""
         if other == self:
@@ -603,14 +627,16 @@
         self.text_regions: List[PageXMLTextRegion] = text_regions if text_regions is not None else []
         self.lines: List[PageXMLTextLine] = lines if lines is not None else []
         self.orientation: Union[None, float] = orientation
         self.reading_order_number = {}
         self.text = text
         if self.lines is not None:
             self.set_as_parent(self.lines)
+        if self.lines is not None:
+            self.set_as_parent(self.lines)
         if self.text_regions is not None:
             self.set_as_parent(self.text_regions)
         if self.reading_order:
             self.set_text_regions_in_reader_order()
         if doc_type:
             self.add_type(doc_type)
 
@@ -674,14 +700,22 @@
             if tr_id not in self.reading_order_number:
                 # there is a text_region that was not in the original PageXML output:
                 # ignore reading order
                 self.reading_order = None
                 return None
         self.text_regions = self.get_text_regions_in_reading_order()
 
+    def get_all_text_regions(self):
+        text_regions: Set[PageXMLTextRegion] = set()
+        for text_region in self.text_regions:
+            text_regions.add(text_region)
+            if text_region.text_regions:
+                text_regions += text_region.get_all_text_regions()
+        return text_regions
+
     def get_inner_text_regions(self) -> List[PageXMLTextRegion]:
         text_regions: List[PageXMLTextRegion] = []
         for text_region in self.text_regions:
             if text_region.text_regions:
                 text_regions += text_region.get_inner_text_regions()
             elif text_region.lines:
                 text_regions.append(text_region)
@@ -855,26 +889,37 @@
         self.main_type = 'scan'
         self.pages: List[PageXMLPage] = pages if pages else []
         self.columns: List[PageXMLColumn] = columns if columns else []
         self.set_as_parent(self.pages)
         self.set_as_parent(self.columns)
         if doc_type:
             self.add_type(doc_type)
+        self.set_scan_id_as_metadata()
 
     def add_child(self, child: PageXMLDoc):
         child.set_parent(self)
         if isinstance(child, PageXMLPage):
             self.pages.append(child)
         elif isinstance(child, PageXMLColumn):
             self.columns.append(child)
         elif isinstance(child, PageXMLTextRegion):
             self.text_regions.append(child)
         elif isinstance(child, PageXMLTextLine):
             self.lines.append(child)
 
+    def set_scan_id_as_metadata(self):
+        self.metadata['scan_id'] = self.id
+        for tr in self.get_all_text_regions():
+            tr.metadata['scan_id'] = self.id
+        for line in self.get_lines():
+            line.metadata['scan_id'] = self.id
+        for word in self.get_words():
+            if isinstance(word, PageXMLWord):
+                word.metadata['scan_id'] = self.id
+
     @property
     def json(self) -> Dict[str, any]:
         doc_json = super().json
         # if self.lines:
         #     doc_json['lines'] = [line.json for line in self.lines]
         # if self.text_regions:
         #     doc_json['text_regions'] = [text_region.json for text_region in self.text_regions]
```

### Comparing `pagexml_tools-0.3.3/pagexml/parser.py` & `pagexml_tools-0.3.4/pagexml/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import glob
 import json
 import re
+from xml.parsers import expat
 from datetime import datetime
 from typing import Generator, List, Dict, Union
 
 import xmltodict
 from dateutil.parser import parse as date_parse
+from tqdm import tqdm
 
 import pagexml.model.physical_document_model as pdm
 from pagexml.helper.file_helper import read_page_archive_file
 from pagexml.model.physical_document_model import Baseline, Coords, parse_derived_coords
 
 
 def parse_coords(coords: dict) -> Union[Coords, None]:
@@ -255,21 +257,22 @@
         for tr in parse_textregion_list(scan_json['TextRegion']):
             if tr is not None:
                 text_regions.append(tr)
     if 'ReadingOrder' in scan_json and scan_json['ReadingOrder']:
         reading_order = parse_page_reading_order(scan_json)
     else:
         reading_order = {}
-    return pdm.PageXMLScan(
+    scan_doc = pdm.PageXMLScan(
         doc_id=doc_id,
         metadata=metadata,
         coords=coords,
         text_regions=text_regions,
         reading_order=reading_order,
     )
+    return scan_doc
 
 
 def read_pagexml_file(pagexml_file: str, encoding: str = 'utf-8') -> str:
     """Return the content of a PageXML file as text string."""
     with open(pagexml_file, 'rt', encoding=encoding) as fh:
         return fh.read()
 
@@ -325,14 +328,38 @@
     if isinstance(pagexml_dirs, str):
         pagexml_dirs = [pagexml_dirs]
     for pagexml_dir in pagexml_dirs:
         pagexml_files += glob.glob(pagexml_dir + "**/*.xml", recursive=True)
     return pagexml_files
 
 
+def parse_pagexml_files_from_directory(pagexml_directories: List[str],
+                                       show_progress: bool = False) -> Generator[pdm.PageXMLScan, None, None]:
+    """Parse PageXML files from one or more directories.
+
+    :param pagexml_directories: the name of one or more directories containing uncompressed PageXML files
+    :type pagexml_directories: List[str]
+    :param show_progress: flag to determine whether a TQDM progress bar is shown
+    :type show_progress: bool
+    :return: a generator that yields a tuple of archived file name and content
+    :rtype: Generator[Tuple[str, str], None, None]
+    """
+    if isinstance(pagexml_directories, str):
+        pagexml_directories = [pagexml_directories]
+    for pagexml_directory in pagexml_directories:
+        dir_files = glob.glob(pagexml_directory, recursive=True)
+        pagexml_files = [fname for fname in dir_files if fname.endswith('.xml')]
+        if show_progress is True:
+            for pagexml_file in tqdm(pagexml_files, desc=f'Parsing files from directory {pagexml_directory}'):
+                yield parse_pagexml_file(pagexml_file)
+        else:
+            for pagexml_file in pagexml_files:
+                yield parse_pagexml_file(pagexml_file)
+
+
 def parse_pagexml_files_from_archive(archive_file: str, ignore_errors: bool = False,
                                      encoding: str = 'utf-8') -> Generator[pdm.PageXMLScan, None, None]:
     """Parse a list of PageXML files from an archive (e.g. zip, tar) and return each
     PageXML file as a PageXMLScan object.
 
     :param archive_file: filepath of a archive (zip, tar) containing PageXML files
     :type archive_file: str
@@ -343,17 +370,20 @@
     :return: a PageXMLScan object
     :rtype: PageXMLScan
     """
     for pagefile_info, pagefile_data in read_page_archive_file(archive_file):
         try:
             yield parse_pagexml_file(pagefile_info['archived_filename'], pagexml_data=pagefile_data,
                                      encoding=encoding)
-        except (KeyError, AttributeError, IndexError, ValueError, TypeError) as err:
+        except (KeyError, AttributeError, IndexError,
+                ValueError, TypeError, FileNotFoundError,
+                expat.ExpatError) as err:
             if ignore_errors is True:
                 print(f"Skipping file with parser error: {pagefile_info['archived_filename']}")
+                print(err)
                 continue
             else:
                 raise
 
 
 def json_to_pagexml_word(json_doc: dict) -> pdm.PageXMLWord:
     word = pdm.PageXMLWord(doc_id=json_doc['id'], doc_type=json_doc['type'], metadata=json_doc['metadata'],
@@ -397,42 +427,42 @@
     column = pdm.PageXMLColumn(doc_id=json_doc['id'], doc_type=json_doc['type'], metadata=json_doc['metadata'],
                                coords=pdm.Coords(json_doc['coords']), text_regions=text_regions, lines=lines,
                                reading_order=reading_order)
     pdm.set_parentage(column)
     return column
 
 
-def json_to_pagexml_page(json_doc: dict) -> pdm.PageXMLPage:
-    extra = [json_to_pagexml_text_region(text_region) for text_region in json_doc['extra']] \
-        if 'extra' in json_doc else []
+def json_to_column_container(json_doc: dict) -> tuple:
     columns = [json_to_pagexml_column(column) for column in json_doc['columns']] if 'columns' in json_doc else []
     text_regions = [json_to_pagexml_text_region(text_region) for text_region in json_doc['text_regions']] \
         if 'text_regions' in json_doc else []
     lines = [json_to_pagexml_line(line) for line in json_doc['lines']] if 'lines' in json_doc else []
     reading_order = json_doc['reading_order'] if 'reading_order' in json_doc else {}
 
     coords = pdm.Coords(json_doc['coords']) if 'coords' in json_doc else None
+    return columns, text_regions, lines, reading_order, coords
+
+
+def json_to_pagexml_page(json_doc: dict) -> pdm.PageXMLPage:
+    extra = [json_to_pagexml_text_region(text_region) for text_region in json_doc['extra']] \
+        if 'extra' in json_doc else []
+    columns, text_regions, lines, reading_order, coords = json_to_column_container(json_doc)
     page = pdm.PageXMLPage(doc_id=json_doc['id'], doc_type=json_doc['type'], metadata=json_doc['metadata'],
                            coords=coords, extra=extra, columns=columns,
                            text_regions=text_regions, lines=lines,
                            reading_order=reading_order)
     pdm.set_parentage(page)
     return page
 
 
 def json_to_pagexml_scan(json_doc: dict) -> pdm.PageXMLScan:
     pages = [json_to_pagexml_page(page) for page in json_doc['pages']] if 'pages' in json_doc else []
-    columns = [json_to_pagexml_column(column) for column in json_doc['columns']] if 'columns' in json_doc else []
-    text_regions = [json_to_pagexml_text_region(text_region) for text_region in json_doc['text_regions']] \
-        if 'text_regions' in json_doc else []
-    lines = [json_to_pagexml_line(line) for line in json_doc['lines']] if 'lines' in json_doc else []
-    reading_order = json_doc['reading_order'] if 'reading_order' in json_doc else {}
-
+    columns, text_regions, lines, reading_order, coords = json_to_column_container(json_doc)
     scan = pdm.PageXMLScan(doc_id=json_doc['id'], doc_type=json_doc['type'], metadata=json_doc['metadata'],
-                           coords=pdm.Coords(json_doc['coords']), pages=pages, columns=columns,
+                           coords=coords, pages=pages, columns=columns,
                            text_regions=text_regions, lines=lines, reading_order=reading_order)
     pdm.set_parentage(scan)
     return scan
 
 
 def json_to_pagexml_doc(json_doc: dict) -> pdm.PageXMLDoc:
     if 'pagexml_doc' not in json_doc['type']:
```

### Comparing `pagexml_tools-0.3.3/pagexml/plotting/plot_dist.py` & `pagexml_tools-0.3.4/pagexml/plotting/plot_dist.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.3/pagexml/transform/segmentation.py` & `pagexml_tools-0.3.4/pagexml/transform/segmentation.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.3/pyproject.toml` & `pagexml_tools-0.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pagexml-tools"
-version = "0.3.3"
+version = "0.3.4"
 description = "Utility functions for reading PageXML files"
 authors = ["Marijn Koolen <marijn.koolen@huygens.knaw.nl>", "Bram Buitendijk <bram.buitendijk@di.huc.knaw.nl>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/knaw-huc/pagexml"
 repository = "https://github.com/knaw-huc/pagexml"
 classifiers = [
@@ -15,24 +15,24 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 packages = [{ include = "pagexml" }]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
-numpy = "^1.22.3"
+fuzzy-search = "^1.5.0"
 matplotlib = "^3.7.0"
+numpy = "^1.22.3"
 pandas = "^1.5.3"
 py7zr = "^0.20.2"
 python-dateutil = "^2.8.2"
 scipy = "^1.7.0"
 seaborn = "^0.12.2"
 tqdm = "^4.64.1"
-xmltodict = "^0.12.0"
-fuzzy-search = "^1.5.0"
+xmltodict = "^0.13.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.test.dependencies]
 icecream = "^2.1.2"
 loguru = "^0.6.0"
```

### Comparing `pagexml_tools-0.3.3/PKG-INFO` & `pagexml_tools-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pagexml-tools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Utility functions for reading PageXML files
 Home-page: https://github.com/knaw-huc/pagexml
 License: MIT
 Author: Marijn Koolen
 Author-email: marijn.koolen@huygens.knaw.nl
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,15 @@
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: py7zr (>=0.20.2,<0.21.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: scipy (>=1.7.0,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: xmltodict (>=0.12.0,<0.13.0)
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Bug Tracker, https://github.com/knaw-huc/pagexml/issues
 Project-URL: Repository, https://github.com/knaw-huc/pagexml
 Description-Content-Type: text/markdown
 
 # pagexml-tools
 
 [![GitHub Actions](https://github.com/knaw-huc/pagexml/workflows/tests/badge.svg)](https://github.com/knaw-huc/pagexml/actions)
```

