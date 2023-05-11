# Comparing `tmp/zod-0.2.3.tar.gz` & `tmp/zod-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zod-0.2.3.tar", max compression
+gzip compressed data, was "zod-0.2.4.tar", max compression
```

## Comparing `zod-0.2.3.tar` & `zod-0.2.4.tar`

### file list

```diff
@@ -1,66 +1,68 @@
--rw-r--r--   0        0        0     1073 2023-04-24 14:28:49.228304 zod-0.2.3/LICENSE
--rw-r--r--   0        0        0     4501 2023-04-24 14:28:49.228304 zod-0.2.3/README.md
--rw-r--r--   0        0        0     1683 2023-04-24 14:28:49.232304 zod-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      982 2023-04-24 14:28:49.232304 zod-0.2.3/zod/__init__.py
--rw-r--r--   0        0        0     4083 2023-04-24 14:28:49.232304 zod-0.2.3/zod/_zod_dataset.py
--rw-r--r--   0        0        0     4945 2023-04-24 14:28:49.232304 zod-0.2.3/zod/anno/lane.py
--rw-r--r--   0        0        0     4354 2023-04-24 14:28:49.232304 zod-0.2.3/zod/anno/object.py
--rw-r--r--   0        0        0     2850 2023-04-24 14:28:49.232304 zod-0.2.3/zod/anno/parser.py
--rw-r--r--   0        0        0      349 2023-04-24 14:28:49.232304 zod-0.2.3/zod/anno/road_condition.py
--rw-r--r--   0        0        0    20456 2023-04-24 14:28:49.232304 zod-0.2.3/zod/anno/tsr/class_map.py
--rw-r--r--   0        0        0     1686 2023-04-24 14:28:49.232304 zod-0.2.3/zod/anno/tsr/traffic_sign.py
--rw-r--r--   0        0        0    14121 2023-04-24 14:28:49.232304 zod-0.2.3/zod/cli/download_zod.py
--rw-r--r--   0        0        0     7365 2023-04-24 14:28:49.232304 zod-0.2.3/zod/cli/extract_tsr_patches.py
--rw-r--r--   0        0        0     6049 2023-04-24 14:28:49.232304 zod-0.2.3/zod/cli/generate_coco_json.py
--rw-r--r--   0        0        0     1324 2023-04-24 14:28:49.232304 zod-0.2.3/zod/cli/main.py
--rw-r--r--   0        0        0      655 2023-04-24 14:28:49.232304 zod-0.2.3/zod/cli/utils.py
--rw-r--r--   0        0        0     3682 2023-04-24 14:28:49.232304 zod-0.2.3/zod/cli/visualize_lidar.py
--rw-r--r--   0        0        0     2403 2023-04-24 14:28:49.232304 zod-0.2.3/zod/constants.py
--rw-r--r--   0        0        0      184 2023-04-24 14:28:49.232304 zod-0.2.3/zod/data_classes/__init__.py
--rw-r--r--   0        0        0      400 2023-04-24 14:28:49.232304 zod-0.2.3/zod/data_classes/_serializable.py
--rw-r--r--   0        0        0    10575 2023-04-24 14:28:49.232304 zod-0.2.3/zod/data_classes/box.py
--rw-r--r--   0        0        0     3021 2023-04-24 14:28:49.232304 zod-0.2.3/zod/data_classes/calibration.py
--rw-r--r--   0        0        0     7226 2023-04-24 14:28:49.232304 zod-0.2.3/zod/data_classes/ego_motion.py
--rw-r--r--   0        0        0     5044 2023-04-24 14:28:49.232304 zod-0.2.3/zod/data_classes/frame.py
--rw-r--r--   0        0        0     1271 2023-04-24 14:28:49.232304 zod-0.2.3/zod/data_classes/geometry.py
--rw-r--r--   0        0        0     4911 2023-04-24 14:28:49.232304 zod-0.2.3/zod/data_classes/info.py
--rw-r--r--   0        0        0      894 2023-04-24 14:28:49.232304 zod-0.2.3/zod/data_classes/metadata.py
--rw-r--r--   0        0        0      317 2023-04-24 14:28:49.232304 zod-0.2.3/zod/data_classes/oxts.py
--rw-r--r--   0        0        0     5268 2023-04-24 14:28:49.232304 zod-0.2.3/zod/data_classes/sensor.py
--rw-r--r--   0        0        0     4441 2023-04-24 14:28:49.232304 zod-0.2.3/zod/data_classes/sequence.py
--rw-r--r--   0        0        0     1004 2023-04-24 14:28:49.232304 zod-0.2.3/zod/data_classes/vehicle_data.py
--rw-r--r--   0        0        0       65 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/README.md
--rw-r--r--   0        0        0      299 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/__init__.py
--rw-r--r--   0        0        0     4427 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/_experimental/eval.py
--rw-r--r--   0        0        0    12061 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/_experimental/matching.py
--rw-r--r--   0        0        0     4614 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/_experimental/utils.py
--rw-r--r--   0        0        0      548 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/_nuscenes_eval/LICENCE.txt
--rw-r--r--   0        0        0      661 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/_nuscenes_eval/changes.txt
--rw-r--r--   0        0        0     4576 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/_nuscenes_eval/common/data_classes.py
--rw-r--r--   0        0        0     4046 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/_nuscenes_eval/common/utils.py
--rw-r--r--   0        0        0    21852 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/_nuscenes_eval/detection/README.md
--rw-r--r--   0        0        0     7651 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/_nuscenes_eval/detection/algo.py
--rw-r--r--   0        0        0     1016 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/_nuscenes_eval/detection/constants.py
--rw-r--r--   0        0        0    15069 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
--rw-r--r--   0        0        0      123 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/constants.py
--rw-r--r--   0        0        0     8031 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/detection/eval_nuscenes_style.py
--rw-r--r--   0        0        0       67 2023-04-24 14:28:49.232304 zod-0.2.3/zod/eval/tsr.py
--rw-r--r--   0        0        0     1996 2023-04-24 14:28:49.232304 zod-0.2.3/zod/utils/compensation.py
--rw-r--r--   0        0        0     4443 2023-04-24 14:28:49.232304 zod-0.2.3/zod/utils/geometry.py
--rw-r--r--   0        0        0     1044 2023-04-24 14:28:49.232304 zod-0.2.3/zod/utils/polygon_transformations.py
--rw-r--r--   0        0        0      914 2023-04-24 14:28:49.232304 zod-0.2.3/zod/utils/utils.py
--rw-r--r--   0        0        0     2703 2023-04-24 14:28:49.232304 zod-0.2.3/zod/utils/visualization.py
--rw-r--r--   0        0        0     5481 2023-04-24 14:28:49.232304 zod-0.2.3/zod/visualization/bev_utils.py
--rw-r--r--   0        0        0     2941 2023-04-24 14:28:49.232304 zod-0.2.3/zod/visualization/colorlabeler.py
--rw-r--r--   0        0        0      259 2023-04-24 14:28:49.232304 zod-0.2.3/zod/visualization/ego_road_visualization.py
--rw-r--r--   0        0        0      264 2023-04-24 14:28:49.232304 zod-0.2.3/zod/visualization/lane_markings_visualization.py
--rw-r--r--   0        0        0     6028 2023-04-24 14:28:49.232304 zod-0.2.3/zod/visualization/lidar_bev.py
--rw-r--r--   0        0        0     4410 2023-04-24 14:28:49.232304 zod-0.2.3/zod/visualization/lidar_on_image.py
--rw-r--r--   0        0        0     4639 2023-04-24 14:28:49.232304 zod-0.2.3/zod/visualization/object_visualization.py
--rw-r--r--   0        0        0     1769 2023-04-24 14:28:49.232304 zod-0.2.3/zod/visualization/oxts_on_image.py
--rw-r--r--   0        0        0     3259 2023-04-24 14:28:49.232304 zod-0.2.3/zod/visualization/oxts_visualization.py
--rw-r--r--   0        0        0      762 2023-04-24 14:28:49.232304 zod-0.2.3/zod/visualization/polygon_utils.py
--rw-r--r--   0        0        0      685 2023-04-24 14:28:49.232304 zod-0.2.3/zod/zod_drives.py
--rw-r--r--   0        0        0      577 2023-04-24 14:28:49.232304 zod-0.2.3/zod/zod_frames.py
--rw-r--r--   0        0        0      576 2023-04-24 14:28:49.232304 zod-0.2.3/zod/zod_sequences.py
--rw-r--r--   0        0        0     5989 1970-01-01 00:00:00.000000 zod-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-12-12 15:34:08.451623 zod-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4809 2023-05-11 13:41:27.984739 zod-0.2.4/README.md
+-rw-r--r--   0        0        0     1783 2023-05-11 13:41:28.034721 zod-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      982 2023-04-13 11:46:50.226836 zod-0.2.4/zod/__init__.py
+-rw-r--r--   0        0        0     4083 2023-04-21 14:37:12.341966 zod-0.2.4/zod/_zod_dataset.py
+-rw-r--r--   0        0        0     4945 2023-03-14 14:11:58.653137 zod-0.2.4/zod/anno/lane.py
+-rw-r--r--   0        0        0     4354 2023-03-27 08:16:00.340536 zod-0.2.4/zod/anno/object.py
+-rw-r--r--   0        0        0     2850 2023-04-20 13:14:41.392219 zod-0.2.4/zod/anno/parser.py
+-rw-r--r--   0        0        0      349 2023-03-14 10:29:04.430175 zod-0.2.4/zod/anno/road_condition.py
+-rw-r--r--   0        0        0    20456 2023-04-12 11:17:00.636182 zod-0.2.4/zod/anno/tsr/class_map.py
+-rw-r--r--   0        0        0     1686 2023-04-12 11:17:00.636357 zod-0.2.4/zod/anno/tsr/traffic_sign.py
+-rw-r--r--   0        0        0    14121 2023-04-24 12:30:20.218578 zod-0.2.4/zod/cli/download_zod.py
+-rw-r--r--   0        0        0     7431 2023-05-11 13:41:28.035021 zod-0.2.4/zod/cli/extract_tsr_patches.py
+-rw-r--r--   0        0        0     6049 2023-03-14 09:59:25.750357 zod-0.2.4/zod/cli/generate_coco_json.py
+-rw-r--r--   0        0        0     1324 2023-05-11 13:39:43.695013 zod-0.2.4/zod/cli/main.py
+-rw-r--r--   0        0        0      655 2023-04-13 11:46:50.648380 zod-0.2.4/zod/cli/utils.py
+-rw-r--r--   0        0        0     3682 2023-03-16 14:47:39.444887 zod-0.2.4/zod/cli/visualize_lidar.py
+-rw-r--r--   0        0        0     2403 2023-04-20 13:15:16.698507 zod-0.2.4/zod/constants.py
+-rw-r--r--   0        0        0      184 2023-03-27 15:11:15.562233 zod-0.2.4/zod/data_classes/__init__.py
+-rw-r--r--   0        0        0      400 2023-01-23 08:46:58.517084 zod-0.2.4/zod/data_classes/_serializable.py
+-rw-r--r--   0        0        0    10575 2023-04-13 11:46:50.163290 zod-0.2.4/zod/data_classes/box.py
+-rw-r--r--   0        0        0     3021 2023-03-14 14:11:59.064736 zod-0.2.4/zod/data_classes/calibration.py
+-rw-r--r--   0        0        0     7226 2023-03-16 14:56:16.137698 zod-0.2.4/zod/data_classes/ego_motion.py
+-rw-r--r--   0        0        0     5044 2023-04-20 13:14:41.392777 zod-0.2.4/zod/data_classes/frame.py
+-rw-r--r--   0        0        0     1271 2023-03-14 14:11:59.065050 zod-0.2.4/zod/data_classes/geometry.py
+-rw-r--r--   0        0        0     4911 2023-04-24 10:58:56.916101 zod-0.2.4/zod/data_classes/info.py
+-rw-r--r--   0        0        0      894 2023-01-23 08:46:58.518295 zod-0.2.4/zod/data_classes/metadata.py
+-rw-r--r--   0        0        0      317 2023-03-28 15:45:20.205955 zod-0.2.4/zod/data_classes/oxts.py
+-rw-r--r--   0        0        0     5268 2023-04-20 13:14:41.393348 zod-0.2.4/zod/data_classes/sensor.py
+-rw-r--r--   0        0        0     4441 2023-04-24 08:58:20.139574 zod-0.2.4/zod/data_classes/sequence.py
+-rw-r--r--   0        0        0     1004 2023-04-20 13:14:41.393582 zod-0.2.4/zod/data_classes/vehicle_data.py
+-rw-r--r--   0        0        0       65 2023-02-08 17:58:06.326973 zod-0.2.4/zod/eval/README.md
+-rw-r--r--   0        0        0      299 2023-02-16 13:07:21.333304 zod-0.2.4/zod/eval/detection/__init__.py
+-rw-r--r--   0        0        0     4427 2023-03-14 10:01:11.503425 zod-0.2.4/zod/eval/detection/_experimental/eval.py
+-rw-r--r--   0        0        0    12061 2023-03-14 10:01:37.539418 zod-0.2.4/zod/eval/detection/_experimental/matching.py
+-rw-r--r--   0        0        0     4614 2023-03-14 10:01:46.422883 zod-0.2.4/zod/eval/detection/_experimental/utils.py
+-rw-r--r--   0        0        0      548 2023-02-08 17:15:18.717865 zod-0.2.4/zod/eval/detection/_nuscenes_eval/LICENCE.txt
+-rw-r--r--   0        0        0      661 2023-02-08 17:15:18.718293 zod-0.2.4/zod/eval/detection/_nuscenes_eval/changes.txt
+-rw-r--r--   0        0        0     4576 2023-03-13 16:23:47.678938 zod-0.2.4/zod/eval/detection/_nuscenes_eval/common/data_classes.py
+-rw-r--r--   0        0        0     4046 2023-03-13 16:23:47.678986 zod-0.2.4/zod/eval/detection/_nuscenes_eval/common/utils.py
+-rw-r--r--   0        0        0    21852 2023-02-08 17:15:18.719837 zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/README.md
+-rw-r--r--   0        0        0     7651 2023-03-13 16:23:47.679037 zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/algo.py
+-rw-r--r--   0        0        0     1016 2023-03-13 16:23:47.679090 zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/constants.py
+-rw-r--r--   0        0        0    15069 2023-03-13 16:23:47.679143 zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/data_classes.py
+-rw-r--r--   0        0        0      123 2023-02-16 12:56:34.415895 zod-0.2.4/zod/eval/detection/constants.py
+-rw-r--r--   0        0        0     8031 2023-03-14 10:34:15.457857 zod-0.2.4/zod/eval/detection/eval_nuscenes_style.py
+-rw-r--r--   0        0        0       67 2023-02-08 17:57:26.772171 zod-0.2.4/zod/eval/tsr.py
+-rw-r--r--   0        0        0     1996 2023-03-28 15:25:47.429197 zod-0.2.4/zod/utils/compensation.py
+-rw-r--r--   0        0        0     4443 2023-03-27 08:16:01.603789 zod-0.2.4/zod/utils/geometry.py
+-rw-r--r--   0        0        0     1044 2023-04-24 14:18:19.989141 zod-0.2.4/zod/utils/polygon_transformations.py
+-rw-r--r--   0        0        0      914 2023-01-19 05:12:36.969853 zod-0.2.4/zod/utils/utils.py
+-rw-r--r--   0        0        0     2703 2023-02-09 13:20:16.173558 zod-0.2.4/zod/utils/visualization.py
+-rw-r--r--   0        0        0     5481 2023-02-16 10:43:41.878456 zod-0.2.4/zod/visualization/bev_utils.py
+-rw-r--r--   0        0        0     2941 2022-12-16 13:30:48.921636 zod-0.2.4/zod/visualization/colorlabeler.py
+-rw-r--r--   0        0        0      259 2022-12-12 13:33:36.526169 zod-0.2.4/zod/visualization/ego_road_visualization.py
+-rw-r--r--   0        0        0      264 2022-12-12 13:33:36.525601 zod-0.2.4/zod/visualization/lane_markings_visualization.py
+-rw-r--r--   0        0        0     8041 2023-05-11 13:41:27.985551 zod-0.2.4/zod/visualization/lidar_3d.py
+-rw-r--r--   0        0        0     6028 2023-02-09 13:20:16.173620 zod-0.2.4/zod/visualization/lidar_bev.py
+-rw-r--r--   0        0        0     4410 2023-03-27 08:16:02.030051 zod-0.2.4/zod/visualization/lidar_on_image.py
+-rw-r--r--   0        0        0     4639 2023-04-13 11:46:50.163979 zod-0.2.4/zod/visualization/object_visualization.py
+-rw-r--r--   0        0        0     1769 2023-03-28 15:25:46.191938 zod-0.2.4/zod/visualization/oxts_on_image.py
+-rw-r--r--   0        0        0     3259 2023-03-28 15:25:44.860709 zod-0.2.4/zod/visualization/oxts_visualization.py
+-rw-r--r--   0        0        0      762 2023-02-09 13:20:16.173776 zod-0.2.4/zod/visualization/polygon_utils.py
+-rw-r--r--   0        0        0      685 2023-04-13 11:46:50.227093 zod-0.2.4/zod/zod_drives.py
+-rw-r--r--   0        0        0      577 2023-05-02 07:55:05.724595 zod-0.2.4/zod/zod_frames.py
+-rw-r--r--   0        0        0      576 2023-04-13 11:46:50.227331 zod-0.2.4/zod/zod_sequences.py
+-rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 zod-0.2.4/setup.py
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 zod-0.2.4/PKG-INFO
```

### Comparing `zod-0.2.3/LICENSE` & `zod-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/README.md` & `zod-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,23 +50,23 @@
 zod download --help
 ```
 
 ## Anonymization
 To preserve privacy, the dataset is anonymized. The anonymization is performed by [brighterAI](https://brighter.ai/), and we provide two separate modes of anonymization: deep fakes (DNAT) and blur. In our paper, we show that the performance of an object detector is not affected by the anonymization method. For more details regarding this experiment, please refer to our [coming soon]().
 
 ## Citation
-If you publish work that uses Zenseact Open Dataset, please cite: [coming soon]()
+If you publish work that uses Zenseact Open Dataset, please cite [our arxiv paper](https://arxiv.org/abs/2305.02008):
 
 ```
-@misc{zod2021,
-  author = {TODO},
-  title = {Zenseact Open Dataset},
+@article{zod2023,
+  author = {Alibeigi, Mina and Ljungbergh, William and Tonderski, Adam and Hess, Georg and Lilja, Adam and Lindstr{\"o}m, Carl and Motorniuk, Daria and Fu, Junsheng and Widahl, Jenny and Petersson, Christoffer},
+  title = {Zenseact Open Dataset: A large-scale and diverse multimodal dataset for autonomous driving},
   year = {2023},
-  publisher = {TODO},
-  journal = {TODO},
+  journal = {arXiv preprint arXiv:2305.02008},
+}
 ```
 
 ## Contact
 For questions about the dataset, please [Contact Us](mailto:opendataset@zenseact.com).
 
 ## Contributing
 We welcome contributions to the development kit. If you would like to contribute, please open a pull request.
```

### Comparing `zod-0.2.3/pyproject.toml` & `zod-0.2.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zod"
-version = "0.2.3"
+version = "0.2.4"
 description = "Zenseact Open Dataset"
 authors = ["Zenseact <opendataset@zenseact.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zod.zenseact.com"
 repository = "https://github.com/zenseact/zod"
 
@@ -25,26 +25,28 @@
 typing-extensions = { version = "*", python = "<3.8" }
 # Optional dependencies
 typer = { extras = ["all"], version = ">=0.7.0", optional = true }
 dropbox = { version = ">=11.36.0", optional = true }
 opencv-python = { version = ">=4", optional = true }
 matplotlib = { version = ">=3", optional = true }
 plotly = { version = "^5", optional = true }
+dash-bootstrap-components = { version = ">=1.1", optional = true }
 pandas = { version = "^1.3", optional = true }
 notebook = { version = ">=5", optional = true }
 imageio = { version = "^2", optional = true }
 
 [tool.poetry.extras]
 cli = ["typer", "dropbox"]
 all = [
     "typer",
     "dropbox",
     "opencv-python",
     "matplotlib",
     "plotly",
+    "dash-bootstrap-components",
     "pandas",
     "notebook",
     "imageio",
 ]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.200"
```

### Comparing `zod-0.2.3/zod/__init__.py` & `zod-0.2.4/zod/__init__.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/_zod_dataset.py` & `zod-0.2.4/zod/_zod_dataset.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/anno/lane.py` & `zod-0.2.4/zod/anno/lane.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/anno/object.py` & `zod-0.2.4/zod/anno/object.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/anno/parser.py` & `zod-0.2.4/zod/anno/parser.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/anno/tsr/class_map.py` & `zod-0.2.4/zod/anno/tsr/class_map.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/anno/tsr/traffic_sign.py` & `zod-0.2.4/zod/anno/tsr/traffic_sign.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/cli/download_zod.py` & `zod-0.2.4/zod/cli/download_zod.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/cli/extract_tsr_patches.py` & `zod-0.2.4/zod/cli/extract_tsr_patches.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 import json
 import os
 from dataclasses import dataclass
 from itertools import repeat
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set, Tuple
 
-import cv2
+try:
+    import cv2
+except ImportError:
+    pass  # TODO: rewrite to use PIL
 import typer
 from tqdm.contrib.concurrent import process_map
 
 import zod.anno.parser as parser
 import zod.constants as constants
 from zod import ZodFrames
 from zod.data_classes.frame import ZodFrame
```

### Comparing `zod-0.2.3/zod/cli/generate_coco_json.py` & `zod-0.2.4/zod/cli/generate_coco_json.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/cli/main.py` & `zod-0.2.4/zod/cli/main.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/cli/utils.py` & `zod-0.2.4/zod/cli/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/cli/visualize_lidar.py` & `zod-0.2.4/zod/cli/visualize_lidar.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/constants.py` & `zod-0.2.4/zod/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/data_classes/box.py` & `zod-0.2.4/zod/data_classes/box.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/data_classes/calibration.py` & `zod-0.2.4/zod/data_classes/calibration.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/data_classes/ego_motion.py` & `zod-0.2.4/zod/data_classes/ego_motion.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/data_classes/frame.py` & `zod-0.2.4/zod/data_classes/frame.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/data_classes/geometry.py` & `zod-0.2.4/zod/data_classes/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/data_classes/info.py` & `zod-0.2.4/zod/data_classes/info.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/data_classes/metadata.py` & `zod-0.2.4/zod/data_classes/metadata.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/data_classes/sensor.py` & `zod-0.2.4/zod/data_classes/sensor.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/data_classes/sequence.py` & `zod-0.2.4/zod/data_classes/sequence.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/data_classes/vehicle_data.py` & `zod-0.2.4/zod/data_classes/vehicle_data.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/eval/detection/_experimental/eval.py` & `zod-0.2.4/zod/eval/detection/_experimental/eval.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/eval/detection/_experimental/matching.py` & `zod-0.2.4/zod/eval/detection/_experimental/matching.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/eval/detection/_experimental/utils.py` & `zod-0.2.4/zod/eval/detection/_experimental/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/eval/detection/_nuscenes_eval/LICENCE.txt` & `zod-0.2.4/zod/eval/detection/_nuscenes_eval/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/eval/detection/_nuscenes_eval/changes.txt` & `zod-0.2.4/zod/eval/detection/_nuscenes_eval/changes.txt`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/eval/detection/_nuscenes_eval/common/data_classes.py` & `zod-0.2.4/zod/eval/detection/_nuscenes_eval/common/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/eval/detection/_nuscenes_eval/common/utils.py` & `zod-0.2.4/zod/eval/detection/_nuscenes_eval/common/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/eval/detection/_nuscenes_eval/detection/README.md` & `zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/README.md`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/eval/detection/_nuscenes_eval/detection/algo.py` & `zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/algo.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/eval/detection/_nuscenes_eval/detection/constants.py` & `zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/constants.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/eval/detection/_nuscenes_eval/detection/data_classes.py` & `zod-0.2.4/zod/eval/detection/_nuscenes_eval/detection/data_classes.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/eval/detection/eval_nuscenes_style.py` & `zod-0.2.4/zod/eval/detection/eval_nuscenes_style.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/utils/compensation.py` & `zod-0.2.4/zod/utils/compensation.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/utils/geometry.py` & `zod-0.2.4/zod/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/utils/polygon_transformations.py` & `zod-0.2.4/zod/utils/polygon_transformations.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/utils/utils.py` & `zod-0.2.4/zod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/utils/visualization.py` & `zod-0.2.4/zod/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/visualization/bev_utils.py` & `zod-0.2.4/zod/visualization/bev_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/visualization/colorlabeler.py` & `zod-0.2.4/zod/visualization/colorlabeler.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/visualization/lidar_bev.py` & `zod-0.2.4/zod/visualization/lidar_bev.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/visualization/lidar_on_image.py` & `zod-0.2.4/zod/visualization/lidar_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/visualization/object_visualization.py` & `zod-0.2.4/zod/visualization/object_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/visualization/oxts_on_image.py` & `zod-0.2.4/zod/visualization/oxts_on_image.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/visualization/oxts_visualization.py` & `zod-0.2.4/zod/visualization/oxts_visualization.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/visualization/polygon_utils.py` & `zod-0.2.4/zod/visualization/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/zod_drives.py` & `zod-0.2.4/zod/zod_drives.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/zod_frames.py` & `zod-0.2.4/zod/zod_frames.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/zod/zod_sequences.py` & `zod-0.2.4/zod/zod_sequences.py`

 * *Files identical despite different names*

### Comparing `zod-0.2.3/PKG-INFO` & `zod-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
 Name: zod
-Version: 0.2.3
+Version: 0.2.4
 Summary: Zenseact Open Dataset
 Home-page: https://zod.zenseact.com
 License: MIT
 Author: Zenseact
 Author-email: opendataset@zenseact.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: cli
+Requires-Dist: dash-bootstrap-components (>=1.1); extra == "all"
 Requires-Dist: dataclass-wizard (>=0.22.2)
-Requires-Dist: dropbox (>=11.36.0) ; extra == "cli" or extra == "all"
+Requires-Dist: dropbox (>=11.36.0); extra == "cli" or extra == "all"
 Requires-Dist: h5py (>=3.1)
-Requires-Dist: imageio (>=2,<3) ; extra == "all"
-Requires-Dist: importlib-metadata ; python_version < "3.8"
-Requires-Dist: matplotlib (>=3) ; extra == "all"
-Requires-Dist: notebook (>=5) ; extra == "all"
+Requires-Dist: imageio (>=2,<3); extra == "all"
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: matplotlib (>=3); extra == "all"
+Requires-Dist: notebook (>=5); extra == "all"
 Requires-Dist: numpy (>=1.19,<2.0)
 Requires-Dist: numpy-quaternion (>=2022.4.2)
-Requires-Dist: opencv-python (>=4) ; extra == "all"
-Requires-Dist: pandas (>=1.3,<2.0) ; extra == "all"
+Requires-Dist: opencv-python (>=4); extra == "all"
+Requires-Dist: pandas (>=1.3,<2.0); extra == "all"
 Requires-Dist: pillow (>=7)
-Requires-Dist: plotly (>=5,<6) ; extra == "all"
+Requires-Dist: plotly (>=5,<6); extra == "all"
 Requires-Dist: pyquaternion (>=0.9)
 Requires-Dist: scipy (>=1.5,<2.0)
 Requires-Dist: tqdm (>=4.60)
-Requires-Dist: typer[all] (>=0.7.0) ; extra == "cli" or extra == "all"
-Requires-Dist: typing-extensions ; python_version < "3.8"
+Requires-Dist: typer[all] (>=0.7.0); extra == "cli" or extra == "all"
+Requires-Dist: typing-extensions; python_version < "3.8"
 Project-URL: Repository, https://github.com/zenseact/zod
 Description-Content-Type: text/markdown
 
 # Zenseact Open Dataset
 
 [![Stable Version](https://img.shields.io/pypi/v/zod?label=stable)](https://pypi.org/project/zod/#history)
 [![Python Versions](https://img.shields.io/pypi/pyversions/zod)](https://pypi.org/project/zod/)
@@ -88,23 +89,23 @@
 zod download --help
 ```
 
 ## Anonymization
 To preserve privacy, the dataset is anonymized. The anonymization is performed by [brighterAI](https://brighter.ai/), and we provide two separate modes of anonymization: deep fakes (DNAT) and blur. In our paper, we show that the performance of an object detector is not affected by the anonymization method. For more details regarding this experiment, please refer to our [coming soon]().
 
 ## Citation
-If you publish work that uses Zenseact Open Dataset, please cite: [coming soon]()
+If you publish work that uses Zenseact Open Dataset, please cite [our arxiv paper](https://arxiv.org/abs/2305.02008):
 
 ```
-@misc{zod2021,
-  author = {TODO},
-  title = {Zenseact Open Dataset},
+@article{zod2023,
+  author = {Alibeigi, Mina and Ljungbergh, William and Tonderski, Adam and Hess, Georg and Lilja, Adam and Lindstr{\"o}m, Carl and Motorniuk, Daria and Fu, Junsheng and Widahl, Jenny and Petersson, Christoffer},
+  title = {Zenseact Open Dataset: A large-scale and diverse multimodal dataset for autonomous driving},
   year = {2023},
-  publisher = {TODO},
-  journal = {TODO},
+  journal = {arXiv preprint arXiv:2305.02008},
+}
 ```
 
 ## Contact
 For questions about the dataset, please [Contact Us](mailto:opendataset@zenseact.com).
 
 ## Contributing
 We welcome contributions to the development kit. If you would like to contribute, please open a pull request.
```

