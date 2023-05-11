# Comparing `tmp/FicImageScript-1.0.0.tar.gz` & `tmp/FicImageScript-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FicImageScript-1.0.0.tar", last modified: Mon May  8 22:54:10 2023, max compression
+gzip compressed data, was "FicImageScript-1.0.1.tar", last modified: Thu May 11 13:34:29 2023, max compression
```

## Comparing `FicImageScript-1.0.0.tar` & `FicImageScript-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 22:54:10.617731 FicImageScript-1.0.0/
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 22:54:10.617731 FicImageScript-1.0.0/FicImage/
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        0 2023-05-06 04:09:38.000000 FicImageScript-1.0.0/FicImage/__init__.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     5514 2023-05-08 22:25:50.000000 FicImageScript-1.0.0/FicImage/image.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     3927 2023-05-08 22:33:20.000000 FicImageScript-1.0.0/FicImage/main.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     2271 2023-05-08 22:25:50.000000 FicImageScript-1.0.0/FicImage/utils.py
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-08 22:54:10.617731 FicImageScript-1.0.0/FicImageScript.egg-info/
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     7313 2023-05-08 22:54:10.000000 FicImageScript-1.0.0/FicImageScript.egg-info/PKG-INFO
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      345 2023-05-08 22:54:10.000000 FicImageScript-1.0.0/FicImageScript.egg-info/SOURCES.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        1 2023-05-08 22:54:10.000000 FicImageScript-1.0.0/FicImageScript.egg-info/dependency_links.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)       48 2023-05-08 22:54:10.000000 FicImageScript-1.0.0/FicImageScript.egg-info/entry_points.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      182 2023-05-08 22:54:10.000000 FicImageScript-1.0.0/FicImageScript.egg-info/requires.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        9 2023-05-08 22:54:10.000000 FicImageScript-1.0.0/FicImageScript.egg-info/top_level.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     1075 2023-04-28 12:48:04.000000 FicImageScript-1.0.0/LICENSE
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     7313 2023-05-08 22:54:10.617731 FicImageScript-1.0.0/PKG-INFO
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     5264 2023-05-07 15:48:12.000000 FicImageScript-1.0.0/README.md
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      927 2023-05-08 22:53:38.000000 FicImageScript-1.0.0/pyproject.toml
--rw-rw-r--   0 nonso     (1000) nonso     (1001)       38 2023-05-08 22:54:10.617731 FicImageScript-1.0.0/setup.cfg
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     1249 2023-05-08 22:53:38.000000 FicImageScript-1.0.0/setup.py
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-11 13:34:29.651168 FicImageScript-1.0.1/
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-11 13:34:29.647168 FicImageScript-1.0.1/FicImage/
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        0 2023-05-06 04:09:38.000000 FicImageScript-1.0.1/FicImage/__init__.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     5514 2023-05-08 22:25:50.000000 FicImageScript-1.0.1/FicImage/image.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     4629 2023-05-11 13:28:32.000000 FicImageScript-1.0.1/FicImage/main.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     2271 2023-05-08 22:25:50.000000 FicImageScript-1.0.1/FicImage/utils.py
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-11 13:34:29.651168 FicImageScript-1.0.1/FicImageScript.egg-info/
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     7747 2023-05-11 13:34:29.000000 FicImageScript-1.0.1/FicImageScript.egg-info/PKG-INFO
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      345 2023-05-11 13:34:29.000000 FicImageScript-1.0.1/FicImageScript.egg-info/SOURCES.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        1 2023-05-11 13:34:29.000000 FicImageScript-1.0.1/FicImageScript.egg-info/dependency_links.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)       48 2023-05-11 13:34:29.000000 FicImageScript-1.0.1/FicImageScript.egg-info/entry_points.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      182 2023-05-11 13:34:29.000000 FicImageScript-1.0.1/FicImageScript.egg-info/requires.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        9 2023-05-11 13:34:29.000000 FicImageScript-1.0.1/FicImageScript.egg-info/top_level.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     1075 2023-04-28 12:48:04.000000 FicImageScript-1.0.1/LICENSE
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     7747 2023-05-11 13:34:29.651168 FicImageScript-1.0.1/PKG-INFO
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     5698 2023-05-08 23:07:54.000000 FicImageScript-1.0.1/README.md
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      927 2023-05-11 11:38:32.000000 FicImageScript-1.0.1/pyproject.toml
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)       38 2023-05-11 13:34:29.651168 FicImageScript-1.0.1/setup.cfg
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     1249 2023-05-11 11:38:33.000000 FicImageScript-1.0.1/setup.py
```

### Comparing `FicImageScript-1.0.0/FicImage/image.py` & `FicImageScript-1.0.1/FicImage/image.py`

 * *Files identical despite different names*

### Comparing `FicImageScript-1.0.0/FicImage/main.py` & `FicImageScript-1.0.1/FicImage/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,74 +12,76 @@
 	:return: None
 	"""
 	parser = argparse.ArgumentParser(description="Update a FicHub epub file with images.")
 	parser.add_argument("path_to_epub", help="The path to the FicHub epub file.")
 	parser.add_argument("-c", "--config_file_path", help="The path to the ficimage.json file.")
 	parser.add_argument("-d", "--debug", help="Enable debug mode.", action="store_true")
 	args = parser.parse_args()
-	
+
 	path_to_epub = args.path_to_epub
 	config_file_path = args.config_file_path
 	debug = args.debug
-	
+
 	try:
 		book = epub.read_epub(path_to_epub)
 		print(f'Opened {path_to_epub}')
-		
+
 		(config_file_exists, config_file_location) = config_check(config_file_path)
 		if config_file_exists:
 			ficimage_config = load_config_json(config_file_location)
 		else:
 			ficimage_config = default_ficimage_settings()
 		compress_images_config: bool = ficimage_config.get("compress_images", True)
 		default_image_format_config: str = ficimage_config.get("default_image_format", "JPEG")
 		if str(default_image_format_config).lower() not in ("jpg", "jpeg", "png"):
 			default_image_format_config = "JPEG"
 		max_image_size_config: int = ficimage_config.get("max_image_size", 1_000_000)
-		
+
 		file_name = path_to_epub.split('/')[-1].split('.')[0]
-		
+		images_downloaded = {}
+
 		for item in book.get_items_of_type(ebooklib.ITEM_DOCUMENT):
 			try:
 				soup = BeautifulSoup(item.content, "lxml-xml")
 				p_tags = soup.find_all('p')
 				images = [i for i in p_tags if '[img:' in i.text]
 				print(f'Found {len(images)} images in {item.file_name}')
+				item_file_name = item.file_name.split('.')[0]
+				images_downloaded[item.file_name] = [0, len(images)]
 				# Clean up the images link
 				# Right now they look like this: <p>[img: <a
 				# href="https://i.imgur.com/ABCDEF.jpg" rel="noopener noreferrer">data:image/gif;base64,R0lGODlhA</a>]</p>
 				# But we want to get the link in the href attribute:
 				try:
 					for image in images:
 						if image is None:
 							print("NoneType, Skipping")
 						else:
-							item_file_name = item.file_name.split('.')[0]
 							image_link = image.a['href']
 							print(f"[{item_file_name}] Image {images.index(image) + 1} "
 							      f"(out of {len(images)}). Source: {image_link}")
-							
 							try:
 								(
 									image_content,
 									image_extension,
 									image_media_type
 								) = get_image_from_url(
 									url=image_link,
 									image_format=default_image_format_config,
 									compress_images=compress_images_config,
 									max_image_size=max_image_size_config,
 									debug=debug
 								)
+								images_downloaded[item.file_name][0] += 1
 								image_path = f"images/" \
 								             f"{item_file_name}_image_{images.index(image)}.{image_extension.lower()}"
 								new_image = f"<img alt='Image {images.index(image)} from {item.file_name}' " \
 								            f"style='text-align: center; margin: 2em auto; display: block;'" \
 								            f" src='{image_path}' />"
-								
+
 								img = epub.EpubItem(
 									uid=f"{item_file_name}_{images.index(image)}",
 									file_name=image_path,
 									media_type=image_media_type,
 									content=image_content,
 								)
 								book.add_item(img)
@@ -87,18 +89,33 @@
 							except Exception as e:
 								print(f"Error with image {images.index(image) + 1}: {e}, skipping ...")
 					item.content = (str(soup).encode('utf-8'))
 				except Exception as e:
 					print(f'Error while parsing images: {e}')
 			except TypeError:
 				print("NoneType error, skipping ...")
-		
+
 		try:
 			epub.write_epub(f"[FicImage]{file_name}.epub", book)
+			total_number_of_images_downloaded = 0
+			number_of_all_images_found = 0
+			for _, chapter_image_list in images_downloaded.items():
+				total_number_of_images_downloaded += chapter_image_list[0]
+				number_of_all_images_found += chapter_image_list[1]
+
 			print(f'Wrote [FicImage]{file_name}.epub')
+			print(f"Image overview of {file_name}")
+			print("=" * 54)
+			for k, v in images_downloaded.items():
+				print(f"{k}{' ' * (18 - len(k))}\t{v[0]} out of {v[1]} images downloaded")
+			print("=" * 54)
+			print(f"Total images downloaded: {total_number_of_images_downloaded}"
+			      f" out of {number_of_all_images_found}")
+			print("=" * 54)
+
 		except Exception as e:
 			print(f'Error while writing epub: {e}')
 	except FileNotFoundError:
 		print(f'File {path_to_epub} not found.')
 		return
```

### Comparing `FicImageScript-1.0.0/FicImage/utils.py` & `FicImageScript-1.0.1/FicImage/utils.py`

 * *Files identical despite different names*

### Comparing `FicImageScript-1.0.0/FicImageScript.egg-info/PKG-INFO` & `FicImageScript-1.0.1/FicImageScript.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FicImageScript
-Version: 1.0.0
+Version: 1.0.1
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
 Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Emmanuel C. Jemeni
@@ -35,28 +35,45 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# FicImage
+# FicImage/FicImageScript
 
 ## Introduction
 FicImage is an application designed to enhance the reading experience of FicHub epubs. With FicImage, users can easily add missing images to their FicHub epubs, bringing the stories to life with vibrant visuals. This user-friendly tool allows readers to fully immerse themselves in their favorite fan fiction stories and enjoy them in a whole new way.
 
 ## How to Use
 
-### Installation
-1. Download FicImage by cloning this repo.
-2. Install the dependencies using `pip install -r requirements.txt`.
-3. Run the program using `python3 ficimage.py path/to/epub path/to/ficimage/json` where `path/to/epub` is the
-path to the **FicHub epub** you want to add images to and `path/to/ficimage/json` is the path to a file called
-**ficimage.json** . ficimage.json lets you configure FicImage. See more [below](#configuration).
-4. Enjoy your new and improved epub!
+### Installation with PIP
+1. Install FicImage using `pip install FicImageScript`.
+2.  After installation, run the program using `ficimage path/to/epub -c path/to/ficimage/json` 
+where `path/to/epub` is the path to the **FicHub epub** you want to add 
+images to and `path/to/ficimage/json` is the path to a file called **ficimage.json** . 
+ficimage.json lets you configure FicImage. See more [below](#configuration).
+
+
+```shell
+(virt) nonso@HPEnvy:~/Documents/Code$ ficimage -h
+usage: ficimage [-h] [-c CONFIG_FILE_PATH] [-d] path_to_epub
+
+Update a FicHub epub file with images.
+
+positional arguments:
+  path_to_epub          The path to the FicHub epub file.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
+                        The path to the ficimage.json file.
+  -d, --debug           Enable debug mode.
+
+```
 
 ### Image Support
 
 [FicHub](https://fichub.net/) creates EPUB 3.3 files, which means that FicImage only save images 
 in the following file format:
 - JPEG
 - PNG
@@ -142,17 +159,17 @@
 > If you set `max_image_size` to 1 000 000, FicImage will probably be able to
 > compress the image to 1 000 000 bytes (1 MB).
 
 > Warning: FicImage will not compress GIFs or WEBPs, that might damage the animation.
 
 
 ## TODO
+- [x] Improve logs
 - [ ] Conversion to other FicHub supported formats from ePub.
 - [ ] More testing 
-- [ ] Improve logs
 
 
 ## Contributing
 Fork the repo and get started!
 
 
 ## Links
```

### Comparing `FicImageScript-1.0.0/LICENSE` & `FicImageScript-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FicImageScript-1.0.0/PKG-INFO` & `FicImageScript-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FicImageScript
-Version: 1.0.0
+Version: 1.0.1
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
 Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Emmanuel C. Jemeni
@@ -35,28 +35,45 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# FicImage
+# FicImage/FicImageScript
 
 ## Introduction
 FicImage is an application designed to enhance the reading experience of FicHub epubs. With FicImage, users can easily add missing images to their FicHub epubs, bringing the stories to life with vibrant visuals. This user-friendly tool allows readers to fully immerse themselves in their favorite fan fiction stories and enjoy them in a whole new way.
 
 ## How to Use
 
-### Installation
-1. Download FicImage by cloning this repo.
-2. Install the dependencies using `pip install -r requirements.txt`.
-3. Run the program using `python3 ficimage.py path/to/epub path/to/ficimage/json` where `path/to/epub` is the
-path to the **FicHub epub** you want to add images to and `path/to/ficimage/json` is the path to a file called
-**ficimage.json** . ficimage.json lets you configure FicImage. See more [below](#configuration).
-4. Enjoy your new and improved epub!
+### Installation with PIP
+1. Install FicImage using `pip install FicImageScript`.
+2.  After installation, run the program using `ficimage path/to/epub -c path/to/ficimage/json` 
+where `path/to/epub` is the path to the **FicHub epub** you want to add 
+images to and `path/to/ficimage/json` is the path to a file called **ficimage.json** . 
+ficimage.json lets you configure FicImage. See more [below](#configuration).
+
+
+```shell
+(virt) nonso@HPEnvy:~/Documents/Code$ ficimage -h
+usage: ficimage [-h] [-c CONFIG_FILE_PATH] [-d] path_to_epub
+
+Update a FicHub epub file with images.
+
+positional arguments:
+  path_to_epub          The path to the FicHub epub file.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
+                        The path to the ficimage.json file.
+  -d, --debug           Enable debug mode.
+
+```
 
 ### Image Support
 
 [FicHub](https://fichub.net/) creates EPUB 3.3 files, which means that FicImage only save images 
 in the following file format:
 - JPEG
 - PNG
@@ -142,17 +159,17 @@
 > If you set `max_image_size` to 1 000 000, FicImage will probably be able to
 > compress the image to 1 000 000 bytes (1 MB).
 
 > Warning: FicImage will not compress GIFs or WEBPs, that might damage the animation.
 
 
 ## TODO
+- [x] Improve logs
 - [ ] Conversion to other FicHub supported formats from ePub.
 - [ ] More testing 
-- [ ] Improve logs
 
 
 ## Contributing
 Fork the repo and get started!
 
 
 ## Links
```

### Comparing `FicImageScript-1.0.0/README.md` & `FicImageScript-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,38 @@
-# FicImage
+# FicImage/FicImageScript
 
 ## Introduction
 FicImage is an application designed to enhance the reading experience of FicHub epubs. With FicImage, users can easily add missing images to their FicHub epubs, bringing the stories to life with vibrant visuals. This user-friendly tool allows readers to fully immerse themselves in their favorite fan fiction stories and enjoy them in a whole new way.
 
 ## How to Use
 
-### Installation
-1. Download FicImage by cloning this repo.
-2. Install the dependencies using `pip install -r requirements.txt`.
-3. Run the program using `python3 ficimage.py path/to/epub path/to/ficimage/json` where `path/to/epub` is the
-path to the **FicHub epub** you want to add images to and `path/to/ficimage/json` is the path to a file called
-**ficimage.json** . ficimage.json lets you configure FicImage. See more [below](#configuration).
-4. Enjoy your new and improved epub!
+### Installation with PIP
+1. Install FicImage using `pip install FicImageScript`.
+2.  After installation, run the program using `ficimage path/to/epub -c path/to/ficimage/json` 
+where `path/to/epub` is the path to the **FicHub epub** you want to add 
+images to and `path/to/ficimage/json` is the path to a file called **ficimage.json** . 
+ficimage.json lets you configure FicImage. See more [below](#configuration).
+
+
+```shell
+(virt) nonso@HPEnvy:~/Documents/Code$ ficimage -h
+usage: ficimage [-h] [-c CONFIG_FILE_PATH] [-d] path_to_epub
+
+Update a FicHub epub file with images.
+
+positional arguments:
+  path_to_epub          The path to the FicHub epub file.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
+                        The path to the ficimage.json file.
+  -d, --debug           Enable debug mode.
+
+```
 
 ### Image Support
 
 [FicHub](https://fichub.net/) creates EPUB 3.3 files, which means that FicImage only save images 
 in the following file format:
 - JPEG
 - PNG
@@ -101,17 +118,17 @@
 > If you set `max_image_size` to 1 000 000, FicImage will probably be able to
 > compress the image to 1 000 000 bytes (1 MB).
 
 > Warning: FicImage will not compress GIFs or WEBPs, that might damage the animation.
 
 
 ## TODO
+- [x] Improve logs
 - [ ] Conversion to other FicHub supported formats from ePub.
 - [ ] More testing 
-- [ ] Improve logs
 
 
 ## Contributing
 Fork the repo and get started!
 
 
 ## Links
```

### Comparing `FicImageScript-1.0.0/pyproject.toml` & `FicImageScript-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "FicImageScript"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Emmanuel C. Jemeni", email="jemenichinonso11@gmail.com" }
 ]
 description = "FicImage is an application designed to enhance the reading experience of FicHub epubs."
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
```

### Comparing `FicImageScript-1.0.0/setup.py` & `FicImageScript-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="FicImageScript",
-	version="1.0.0",
+	version="1.0.1",
 	author="Emmanuel C. Jemeni",
 	author_email="jemenichinonso11@gmail.com",
 	description="FicImage is an application designed to enhance the reading experience of FicHub epubs.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/Jemeni11/FicImage",
 	project_urls={
```

