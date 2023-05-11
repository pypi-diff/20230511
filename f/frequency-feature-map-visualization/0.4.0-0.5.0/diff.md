# Comparing `tmp/frequency_feature_map_visualization-0.4.0.tar.gz` & `tmp/frequency_feature_map_visualization-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequency_feature_map_visualization-0.4.0.tar", last modified: Wed May 10 15:43:22 2023, max compression
+gzip compressed data, was "frequency_feature_map_visualization-0.5.0.tar", last modified: Thu May 11 13:33:42 2023, max compression
```

## Comparing `frequency_feature_map_visualization-0.4.0.tar` & `frequency_feature_map_visualization-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-10 15:43:22.811461 frequency_feature_map_visualization-0.4.0/
--rw-r--r--   0 fuguanghui   (501) staff       (20)      530 2023-05-10 15:43:22.811314 frequency_feature_map_visualization-0.4.0/PKG-INFO
-drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-10 15:43:22.809957 frequency_feature_map_visualization-0.4.0/frequency_feature_map_visualization/
--rw-rw-r--   0 fuguanghui   (501) staff       (20)      196 2023-05-10 15:35:39.000000 frequency_feature_map_visualization-0.4.0/frequency_feature_map_visualization/__init__.py
--rw-rw-r--   0 fuguanghui   (501) staff       (20)     8595 2023-05-10 13:44:34.000000 frequency_feature_map_visualization-0.4.0/frequency_feature_map_visualization/feature_map_visualization.py
-drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-10 15:43:22.811040 frequency_feature_map_visualization-0.4.0/frequency_feature_map_visualization.egg-info/
--rw-r--r--   0 fuguanghui   (501) staff       (20)      530 2023-05-10 15:43:22.000000 frequency_feature_map_visualization-0.4.0/frequency_feature_map_visualization.egg-info/PKG-INFO
--rw-r--r--   0 fuguanghui   (501) staff       (20)      415 2023-05-10 15:43:22.000000 frequency_feature_map_visualization-0.4.0/frequency_feature_map_visualization.egg-info/SOURCES.txt
--rw-r--r--   0 fuguanghui   (501) staff       (20)        1 2023-05-10 15:43:22.000000 frequency_feature_map_visualization-0.4.0/frequency_feature_map_visualization.egg-info/dependency_links.txt
--rw-r--r--   0 fuguanghui   (501) staff       (20)       23 2023-05-10 15:43:22.000000 frequency_feature_map_visualization-0.4.0/frequency_feature_map_visualization.egg-info/requires.txt
--rw-r--r--   0 fuguanghui   (501) staff       (20)       36 2023-05-10 15:43:22.000000 frequency_feature_map_visualization-0.4.0/frequency_feature_map_visualization.egg-info/top_level.txt
--rw-r--r--   0 fuguanghui   (501) staff       (20)       38 2023-05-10 15:43:22.811517 frequency_feature_map_visualization-0.4.0/setup.cfg
--rw-rw-r--   0 fuguanghui   (501) staff       (20)      689 2023-05-10 15:42:54.000000 frequency_feature_map_visualization-0.4.0/setup.py
+drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-11 13:33:42.201212 frequency_feature_map_visualization-0.5.0/
+-rw-r--r--   0 fuguanghui   (501) staff       (20)      530 2023-05-11 13:33:42.201086 frequency_feature_map_visualization-0.5.0/PKG-INFO
+drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-11 13:33:42.200103 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization/
+-rw-rw-r--   0 fuguanghui   (501) staff       (20)      196 2023-05-10 15:35:39.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization/__init__.py
+-rw-r--r--   0 fuguanghui   (501) staff       (20)     7548 2023-05-11 13:30:29.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization/feature_map_visualization.py
+drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-11 13:33:42.200884 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/
+-rw-r--r--   0 fuguanghui   (501) staff       (20)      530 2023-05-11 13:33:42.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/PKG-INFO
+-rw-r--r--   0 fuguanghui   (501) staff       (20)      415 2023-05-11 13:33:42.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/SOURCES.txt
+-rw-r--r--   0 fuguanghui   (501) staff       (20)        1 2023-05-11 13:33:42.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/dependency_links.txt
+-rw-r--r--   0 fuguanghui   (501) staff       (20)       23 2023-05-11 13:33:42.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/requires.txt
+-rw-r--r--   0 fuguanghui   (501) staff       (20)       36 2023-05-11 13:33:42.000000 frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/top_level.txt
+-rw-r--r--   0 fuguanghui   (501) staff       (20)       38 2023-05-11 13:33:42.201256 frequency_feature_map_visualization-0.5.0/setup.cfg
+-rw-rw-r--   0 fuguanghui   (501) staff       (20)      689 2023-05-11 13:33:28.000000 frequency_feature_map_visualization-0.5.0/setup.py
```

### Comparing `frequency_feature_map_visualization-0.4.0/PKG-INFO` & `frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: frequency_feature_map_visualization
-Version: 0.4.0
+Name: frequency-feature-map-visualization
+Version: 0.5.0
 Summary: This code is designed to visualize and save the feature maps of 3D and 2D models. The feature maps can be viewed in the image domain and frequency domain, and saved as .npy files.
 Home-page: UNKNOWN
 Author: Guanghui FU
 Author-email: aslanfu123@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `frequency_feature_map_visualization-0.4.0/frequency_feature_map_visualization/feature_map_visualization.py` & `frequency_feature_map_visualization-0.5.0/frequency_feature_map_visualization/feature_map_visualization.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,207 +1,180 @@
-import os
-import glob
-import numpy as np
-import torch
-import torch.nn as nn
-from numpy.fft import fftshift, fftn
-import matplotlib.pyplot as plt
-
-# Extract all layers of interest from the model (Conv3d, MaxPool3d, Upsample)
-def extract_all_layers(model):
-    layers = nn.ModuleList()
-    for module in model.modules():
-        if isinstance(module, (nn.Conv3d, nn.MaxPool3d, nn.Upsample)):
-            layers.append(module)
-    return layers
-
-# Normalize a numpy array
-def normalize_np(mri_np):
-    nii_np_min = mri_np.min()
-    nii_np_max = mri_np.max()
-    nii_np = (mri_np - nii_np_min) / (nii_np_max - nii_np_min)
-    return nii_np
-
-# Perform Fourier Transform on the feature map numpy array and normalize it
-def feature_map_np_fourier_transform(feature_map_np):
-    feature_map_np_fft = fftshift(fftn(feature_map_np))
-    feature_map_np_fft = np.log(np.abs(feature_map_np_fft) + 1)
-    feature_map_np_fft_normalized = normalize_np(feature_map_np_fft)
-    return feature_map_np_fft_normalized
-
-# Extract feature maps for each layer and save them to a dictionary
-def extract_feature_maps(layer_outputs):
-    feature_map_dict = {}
-    for layer_index, (layer_output, layer_name) in enumerate(layer_outputs[1:]):
-        print(f'layer index: {layer_index}, layer name: {layer_name}')
-        img_domain_maps = []
-        freq_domain_maps = []
-        for channel_idx, feature_map in enumerate(layer_output):
-            feature_map_np = feature_map.cpu().detach().numpy()
-            feature_map_np_fft = feature_map_np_fourier_transform(feature_map_np)
-            img_domain_maps.append(feature_map_np)
-            freq_domain_maps.append(feature_map_np_fft)
-        feature_map_dict[layer_index] = {
-            'name': layer_name,
-            'img_domain': np.array(img_domain_maps),
-            'freq_domain': np.array(freq_domain_maps)
-        }
-    return feature_map_dict
-
-# Visualize feature maps for 3D model
-def visualize_feature_maps_3d(model, input_tensor, device):
-    print('Visualizing feature maps')
-    input_tensor = input_tensor.to(device)
-
-    def forward_hook(module, input, output):
-        layer_name = str(module.__class__).split('.')[-1].split(''')[0]
-        layer_outputs.append((output, layer_name))
-
-    handles = []
-    for layer in model.modules():
-        if isinstance(layer, (nn.Conv3d, nn.MaxPool3d, nn.Upsample)):
-            handle = layer.register_forward_hook(forward_hook)
-            handles.append(handle)
-
-    layer_outputs = [(input_tensor, 'Input')]
-
-    with torch.no_grad():
-        _ = model(input_tensor)
-
-    for handle in handles:
-        handle.remove()
-
-    feature_map_dict = extract_feature_maps(layer_outputs)
-    return feature_map_dict
-
-# Visualize feature maps for 2D model
-def visualize_feature_maps_2d(model, input_tensor, device):
-    print('Visualizing feature maps')
-    input_tensor = input_tensor.to(device)
-
-    def forward_hook(module, input, output):
-        layer_name = str(module.__class__).split('.')[-1].split(''')[0]
-        layer_outputs.append((output, layer_name))
-
-    handles = []
-    for layer in model.modules():
-        if isinstance(layer, (nn.Conv2d, nn.MaxPool2d)):
-            handle = layer.register_forward_hook(forward_hook)
-            handles.append(handle)
-
-    layer_outputs = [(input_tensor, 'Input')]
-
-    with torch.no_grad():
-        _ = model(input_tensor)
-
-    for handle in handles:
-        handle.remove()
-
-    feature_map_dict = extract_feature_maps(layer_outputs)
-    return feature_map_dict
-# Visualize feature maps for 2D model
-def visualize_feature_maps_2d(model, input_tensor, device):
-    print('Visualizing feature maps')
-    input_tensor = input_tensor.to(device)
-
-    def forward_hook(module, input, output):
-        layer_name = str(module.__class__).split('.')[-1].split("'")[0]
-        layer_outputs.append((output, layer_name))
-
-    handles = []
-    for layer in model.modules():
-        if isinstance(layer, (nn.Conv2d, nn.MaxPool2d)):
-            handle = layer.register_forward_hook(forward_hook)
-            handles.append(handle)
-
-    layer_outputs = [(input_tensor, "Input")]
-
-    with torch.no_grad():
-        _ = model(input_tensor)
-
-    for handle in handles:
-        handle.remove()
-
-    feature_map_dict = extract_feature_maps(layer_outputs)
-    return feature_map_dict
-# Save feature maps as .npy files
-def save_feature_maps_to_npy(feature_map_dict, save_base_path):
-    print('Saving feature map to npy')
-    os.makedirs(save_base_path, exist_ok=True)
-    for layer_index, layer_info in feature_map_dict.items():
-        layer_name = layer_info['name']
-        img_domain_maps = np.squeeze(layer_info['img_domain'])
-        freq_domain_maps = np.squeeze(layer_info['freq_domain'])
-        layer_path = f'{save_base_path}/{layer_index}_{layer_name}'
-        os.makedirs(layer_path, exist_ok=True)
-        img_domain_maps_avg = np.mean(img_domain_maps, axis=0)
-        freq_domain_maps_avg = np.mean(freq_domain_maps, axis=0)
-        np.save(f'{layer_path}_avg_channel_img_domain.npy', img_domain_maps_avg)
-        np.save(f'{layer_path}_avg_channel_freq_domain.npy', freq_domain_maps_avg)
-        for channel_idx, (img_domain_map, freq_domain_map) in enumerate(zip(img_domain_maps, freq_domain_maps)):
-            img_domain_npy_path = f'{layer_path}/channel_{channel_idx}_img_domain.npy'
-            freq_domain_npy_path = f'{layer_path}/channel_{channel_idx}_freq_domain.npy'
-
-            np.save(img_domain_npy_path, np.array(img_domain_map))
-            np.save(freq_domain_npy_path, np.array(freq_domain_map))
-
-# Get the minimum and maximum values from .npy files in a directory
-def get_min_max_from_npy_files(path):
-    min_val = float('inf')
-    max_val = float('-inf')
-
-    for file_name in os.listdir(path):
-        if file_name.endswith('.npy'):
-            file_path = os.path.join(path, file_name)
-            arr = np.load(file_path)
-            min_val = min(min_val, np.min(arr))
-            max_val = max(max_val, np.max(arr))
-
-    return min_val, max_val
-
-# Adjust the range of minimum and maximum values according to a given percentage
-def adjust_range(min_val, max_val, percentage):
-    range_length = max_val - min_val
-    adjustment = range_length * ((1 - percentage) / 2)
-    lower_bound = min_val + adjustment
-    upper_bound = max_val - adjustment
-    return lower_bound, upper_bound
-
-# Plot 3D feature maps and save them as images
-def plot_feature_map_3d(base_path, clim_ranges, percen_ranges=1.0, slice_no='avg'):
-    npy_file_path_list = glob.glob(f'{base_path}/*.npy')
-    if len(clim_ranges) == 0:
-        clim_ranges = get_min_max_from_npy_files(base_path)
-        if percen_ranges!=1.0: clim_ranges = adjust_range(clim_ranges[0], clim_ranges[1], percen_ranges)
-    for npy_file_path in npy_file_path_list:
-        feature_map_name = os.path.basename(npy_file_path).replace('.npy', '')
-        feature_map_np = np.load(npy_file_path)
-        if slice_no == 'avg':
-            feature_map_np_visual = np.mean(feature_map_np, axis=2)
-        elif slice_no == 'mid':
-            slice = feature_map_np.shape[2]
-            feature_map_np_visual = feature_map_np[:, :, int(slice / 2)]
-        elif str.isdigit(slice_no):
-            feature_map_np_visual = feature_map_np[:, :, slice_no]
-        else:
-            raise ValueError(f'Wrong input: {slice_no}')
-
-        plt.imshow(feature_map_np_visual, cmap='viridis')
-        plt.colorbar()
-        plt.clim(clim_ranges)  # Set clim range based on the global min and max values for the block
-        plt.savefig(f'{base_path}/{feature_map_name}_slice_{slice_no}.png')
-        plt.close()
-
-# Plot 2D feature maps and save them as images
-def plot_feature_map_2d(base_path, clim_ranges, percen_ranges=1.0):
-    npy_file_path_list = glob.glob(f'{base_path}/*.npy')
-    if len(clim_ranges) == 0:
-        clim_ranges = get_min_max_from_npy_files(base_path)
-        if percen_ranges!=1.0: clim_ranges = adjust_range(clim_ranges[0], clim_ranges[1], percen_ranges)
-    for npy_file_path in npy_file_path_list:
-        feature_map_name = os.path.basename(npy_file_path).replace('.npy', '')
-        feature_map_np = np.load(npy_file_path)
-        plt.imshow(feature_map_np, cmap='viridis')
-        plt.colorbar()
-        plt.clim(clim_ranges)  # Set clim range based on the global min and max values for the block
-        plt.savefig(f'{base_path}/{feature_map_name}.png')
-        plt.close()
+import os
+import glob
+import numpy as np
+import torch
+import torch.nn as nn
+from numpy.fft import fftshift, fftn
+import matplotlib.pyplot as plt
+
+# Extract all layers of interest from the model (Conv3d, MaxPool3d, Upsample)
+def extract_all_layers(model):
+    layers = nn.ModuleList()
+    for module in model.modules():
+        if isinstance(module, (nn.Conv3d, nn.MaxPool3d, nn.Upsample)):
+            layers.append(module)
+    return layers
+
+# Normalize a numpy array
+def normalize_np(mri_np):
+    nii_np_min = mri_np.min()
+    nii_np_max = mri_np.max()
+    nii_np = (mri_np - nii_np_min) / (nii_np_max - nii_np_min)
+    return nii_np
+
+# Perform Fourier Transform on the feature map numpy array and normalize it
+def feature_map_np_fourier_transform(feature_map_np):
+    feature_map_np_fft = fftshift(fftn(feature_map_np))
+    feature_map_np_fft = np.log(np.abs(feature_map_np_fft) + 1)
+    feature_map_np_fft_normalized = normalize_np(feature_map_np_fft)
+    return feature_map_np_fft_normalized
+
+# Extract feature maps for each layer and save them to a dictionary
+def extract_feature_maps(layer_outputs):
+    feature_map_dict = {}
+    for layer_index, (layer_output, layer_name) in enumerate(layer_outputs[1:]):
+        print(f'layer index: {layer_index}, layer name: {layer_name}')
+        img_domain_maps = []
+        freq_domain_maps = []
+        for channel_idx, feature_map in enumerate(layer_output):
+            feature_map_np = feature_map.cpu().detach().numpy()
+            feature_map_np_fft = feature_map_np_fourier_transform(feature_map_np)
+            img_domain_maps.append(feature_map_np)
+            freq_domain_maps.append(feature_map_np_fft)
+        feature_map_dict[layer_index] = {
+            'name': layer_name,
+            'img_domain': np.array(img_domain_maps),
+            'freq_domain': np.array(freq_domain_maps)
+        }
+    return feature_map_dict
+
+# Visualize feature maps for 3D model
+def visualize_feature_maps_3d(model, input_tensor, device):
+    print('Visualizing feature maps')
+    input_tensor = input_tensor.to(device)
+
+    def forward_hook(module, input, output):
+        layer_name = str(module.__class__).split('.')[-1].split("'")[0]
+        layer_outputs.append((output, layer_name))
+
+    handles = []
+    for layer in model.modules():
+        if isinstance(layer, (nn.Conv3d, nn.MaxPool3d, nn.Upsample)):
+            handle = layer.register_forward_hook(forward_hook)
+            handles.append(handle)
+
+    layer_outputs = [(input_tensor, "Input")]
+
+    with torch.no_grad():
+        _ = model(input_tensor)
+
+    for handle in handles:
+        handle.remove()
+
+    feature_map_dict = extract_feature_maps(layer_outputs)
+    return feature_map_dict
+def visualize_feature_maps_2d(model, input_tensor, device):
+    print('Visualizing feature maps')
+    input_tensor = input_tensor.to(device)
+
+    def forward_hook(module, input, output):
+        layer_name = str(module.__class__).split('.')[-1].split("'")[0]
+        layer_outputs.append((output, layer_name))
+
+    handles = []
+    for layer in model.modules():
+        if isinstance(layer, (nn.Conv2d, nn.MaxPool2d)):
+            handle = layer.register_forward_hook(forward_hook)
+            handles.append(handle)
+
+    layer_outputs = [(input_tensor, "Input")]
+
+    with torch.no_grad():
+        _ = model(input_tensor)
+
+    for handle in handles:
+        handle.remove()
+
+    feature_map_dict = extract_feature_maps(layer_outputs)
+    return feature_map_dict
+# Save feature maps as .npy files
+def save_feature_maps_to_npy(feature_map_dict, save_base_path):
+    print('Saving feature map to npy')
+    os.makedirs(save_base_path, exist_ok=True)
+    for layer_index, layer_info in feature_map_dict.items():
+        layer_name = layer_info['name']
+        img_domain_maps = np.squeeze(layer_info['img_domain'])
+        freq_domain_maps = np.squeeze(layer_info['freq_domain'])
+        layer_path = f'{save_base_path}/{layer_index}_{layer_name}'
+        os.makedirs(layer_path, exist_ok=True)
+        img_domain_maps_avg = np.mean(img_domain_maps, axis=0)
+        freq_domain_maps_avg = np.mean(freq_domain_maps, axis=0)
+        np.save(f'{layer_path}_avg_channel_img_domain.npy', img_domain_maps_avg)
+        np.save(f'{layer_path}_avg_channel_freq_domain.npy', freq_domain_maps_avg)
+        for channel_idx, (img_domain_map, freq_domain_map) in enumerate(zip(img_domain_maps, freq_domain_maps)):
+            img_domain_npy_path = f'{layer_path}/channel_{channel_idx}_img_domain.npy'
+            freq_domain_npy_path = f'{layer_path}/channel_{channel_idx}_freq_domain.npy'
+
+            np.save(img_domain_npy_path, np.array(img_domain_map))
+            np.save(freq_domain_npy_path, np.array(freq_domain_map))
+
+# Get the minimum and maximum values from .npy files in a directory
+def get_min_max_from_npy_files(path):
+    min_val = float('inf')
+    max_val = float('-inf')
+
+    for file_name in os.listdir(path):
+        if file_name.endswith('.npy'):
+            file_path = os.path.join(path, file_name)
+            arr = np.load(file_path)
+            min_val = min(min_val, np.min(arr))
+            max_val = max(max_val, np.max(arr))
+
+    return min_val, max_val
+
+# Adjust the range of minimum and maximum values according to a given percentage
+def adjust_range(min_val, max_val, percentage):
+    range_length = max_val - min_val
+    adjustment = range_length * ((1 - percentage) / 2)
+    lower_bound = min_val + adjustment
+    upper_bound = max_val - adjustment
+    return lower_bound, upper_bound
+
+# Plot 3D feature maps and save them as images
+def plot_feature_map_3d(base_path, clim_ranges, percen_ranges=1.0, slice_no='avg'):
+    npy_file_path_list = glob.glob(f'{base_path}/*.npy')
+    if len(clim_ranges) == 0:
+        clim_ranges = get_min_max_from_npy_files(base_path)
+        if percen_ranges!=1.0: clim_ranges = adjust_range(clim_ranges[0], clim_ranges[1], percen_ranges)
+    for npy_file_path in npy_file_path_list:
+        feature_map_name = os.path.basename(npy_file_path).replace('.npy', '')
+        feature_map_np = np.load(npy_file_path)
+        if slice_no == 'avg':
+            feature_map_np_visual = np.mean(feature_map_np, axis=2)
+        elif slice_no == 'mid':
+            slice = feature_map_np.shape[2]
+            feature_map_np_visual = feature_map_np[:, :, int(slice / 2)]
+        elif str.isdigit(slice_no):
+            feature_map_np_visual = feature_map_np[:, :, slice_no]
+        else:
+            raise ValueError(f'Wrong input: {slice_no}')
+
+        plt.imshow(feature_map_np_visual, cmap='viridis')
+        plt.colorbar()
+        plt.clim(clim_ranges)  # Set clim range based on the global min and max values for the block
+        plt.savefig(f'{base_path}/{feature_map_name}_slice_{slice_no}.png')
+        plt.close()
+
+# Plot 2D feature maps and save them as images
+def plot_feature_map_2d(base_path, clim_ranges, percen_ranges=1.0):
+    npy_file_path_list = glob.glob(f'{base_path}/*.npy')
+    if len(clim_ranges) == 0:
+        clim_ranges = get_min_max_from_npy_files(base_path)
+        if percen_ranges!=1.0: clim_ranges = adjust_range(clim_ranges[0], clim_ranges[1], percen_ranges)
+    for npy_file_path in npy_file_path_list:
+        feature_map_name = os.path.basename(npy_file_path).replace('.npy', '')
+        feature_map_np = np.load(npy_file_path)
+        plt.imshow(feature_map_np, cmap='viridis')
+        plt.colorbar()
+        plt.clim(clim_ranges)  # Set clim range based on the global min and max values for the block
+        plt.savefig(f'{base_path}/{feature_map_name}.png')
+        plt.close()
```

### Comparing `frequency_feature_map_visualization-0.4.0/frequency_feature_map_visualization.egg-info/PKG-INFO` & `frequency_feature_map_visualization-0.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: frequency-feature-map-visualization
-Version: 0.4.0
+Name: frequency_feature_map_visualization
+Version: 0.5.0
 Summary: This code is designed to visualize and save the feature maps of 3D and 2D models. The feature maps can be viewed in the image domain and frequency domain, and saved as .npy files.
 Home-page: UNKNOWN
 Author: Guanghui FU
 Author-email: aslanfu123@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `frequency_feature_map_visualization-0.4.0/setup.py` & `frequency_feature_map_visualization-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="frequency_feature_map_visualization",
-    version="0.4.0",
+    version="0.5.0",
     description="This code is designed to visualize and save the feature maps of 3D and 2D models. The feature maps can be viewed in the image domain and frequency domain, and saved as .npy files.",
     author="Guanghui FU",
     author_email="aslanfu123@gmail.com",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "torch",
```

