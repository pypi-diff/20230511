# Comparing `tmp/measpy-0.0.8.tar.gz` & `tmp/measpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "measpy-0.0.8.tar", last modified: Fri Jun 10 13:39:33 2022, max compression
+gzip compressed data, was "measpy-0.0.9.tar", last modified: Thu Dec 15 14:53:48 2022, max compression
```

## Comparing `measpy-0.0.8.tar` & `measpy-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 doare     (1000) doare     (1000)        0 2022-06-10 13:39:33.399306 measpy-0.0.8/
--rw-rw-r--   0 doare     (1000) doare     (1000)     1499 2022-06-10 13:39:33.399306 measpy-0.0.8/PKG-INFO
--rw-rw-r--   0 doare     (1000) doare     (1000)     6695 2022-06-10 11:02:45.000000 measpy-0.0.8/README.md
-drwxrwxr-x   0 doare     (1000) doare     (1000)        0 2022-06-10 13:39:33.395306 measpy-0.0.8/measpy/
--rw-rw-r--   0 doare     (1000) doare     (1000)      345 2022-06-10 11:02:45.000000 measpy-0.0.8/measpy/__init__.py
--rw-rw-r--   0 doare     (1000) doare     (1000)      818 2022-06-10 11:02:45.000000 measpy-0.0.8/measpy/__main__.py
--rw-rw-r--   0 doare     (1000) doare     (1000)      715 2022-06-10 11:02:45.000000 measpy-0.0.8/measpy/_tools.py
--rw-rw-r--   0 doare     (1000) doare     (1000)     3051 2022-06-10 11:02:45.000000 measpy-0.0.8/measpy/audio.py
--rw-rw-r--   0 doare     (1000) doare     (1000)    27099 2022-06-10 12:45:27.000000 measpy-0.0.8/measpy/measurement.py
--rw-rw-r--   0 doare     (1000) doare     (1000)     5341 2022-06-10 11:02:45.000000 measpy-0.0.8/measpy/ni.py
--rw-rw-r--   0 doare     (1000) doare     (1000)    66487 2022-06-10 11:02:45.000000 measpy-0.0.8/measpy/signal.py
-drwxrwxr-x   0 doare     (1000) doare     (1000)        0 2022-06-10 13:39:33.399306 measpy-0.0.8/measpy.egg-info/
--rw-rw-r--   0 doare     (1000) doare     (1000)     1499 2022-06-10 13:39:33.000000 measpy-0.0.8/measpy.egg-info/PKG-INFO
--rw-rw-r--   0 doare     (1000) doare     (1000)      290 2022-06-10 13:39:33.000000 measpy-0.0.8/measpy.egg-info/SOURCES.txt
--rw-rw-r--   0 doare     (1000) doare     (1000)        1 2022-06-10 13:39:33.000000 measpy-0.0.8/measpy.egg-info/dependency_links.txt
--rw-rw-r--   0 doare     (1000) doare     (1000)       28 2022-06-10 13:39:33.000000 measpy-0.0.8/measpy.egg-info/requires.txt
--rw-rw-r--   0 doare     (1000) doare     (1000)        7 2022-06-10 13:39:33.000000 measpy-0.0.8/measpy.egg-info/top_level.txt
--rw-rw-r--   0 doare     (1000) doare     (1000)       38 2022-06-10 13:39:33.399306 measpy-0.0.8/setup.cfg
--rw-rw-r--   0 doare     (1000) doare     (1000)     1756 2022-06-10 13:38:16.000000 measpy-0.0.8/setup.py
+drwxrwxr-x   0 doare     (1000) doare     (1000)        0 2022-12-15 14:53:48.122190 measpy-0.0.9/
+-rw-rw-r--   0 doare     (1000) doare     (1000)     7507 2022-12-15 14:26:11.000000 measpy-0.0.9/LICENSE
+-rw-rw-r--   0 doare     (1000) doare     (1000)     1343 2022-12-15 14:53:48.122190 measpy-0.0.9/PKG-INFO
+-rw-rw-r--   0 doare     (1000) doare     (1000)     6695 2022-12-15 14:26:11.000000 measpy-0.0.9/README.md
+drwxrwxr-x   0 doare     (1000) doare     (1000)        0 2022-12-15 14:53:48.118190 measpy-0.0.9/measpy/
+-rw-rw-r--   0 doare     (1000) doare     (1000)      345 2022-12-15 14:26:12.000000 measpy-0.0.9/measpy/__init__.py
+-rw-rw-r--   0 doare     (1000) doare     (1000)      818 2022-12-15 14:26:12.000000 measpy-0.0.9/measpy/__main__.py
+-rw-rw-r--   0 doare     (1000) doare     (1000)      715 2022-12-15 14:26:12.000000 measpy-0.0.9/measpy/_tools.py
+-rw-rw-r--   0 doare     (1000) doare     (1000)     3055 2022-12-15 14:26:12.000000 measpy-0.0.9/measpy/audio.py
+-rw-rw-r--   0 doare     (1000) doare     (1000)    29236 2022-12-15 14:30:57.000000 measpy-0.0.9/measpy/measurement.py
+-rw-rw-r--   0 doare     (1000) doare     (1000)     5345 2022-12-15 14:26:12.000000 measpy-0.0.9/measpy/ni.py
+-rw-rw-r--   0 doare     (1000) doare     (1000)    68106 2022-12-15 14:26:12.000000 measpy-0.0.9/measpy/signal.py
+drwxrwxr-x   0 doare     (1000) doare     (1000)        0 2022-12-15 14:53:48.122190 measpy-0.0.9/measpy.egg-info/
+-rw-rw-r--   0 doare     (1000) doare     (1000)     1343 2022-12-15 14:53:48.000000 measpy-0.0.9/measpy.egg-info/PKG-INFO
+-rw-rw-r--   0 doare     (1000) doare     (1000)      298 2022-12-15 14:53:48.000000 measpy-0.0.9/measpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 doare     (1000) doare     (1000)        1 2022-12-15 14:53:48.000000 measpy-0.0.9/measpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 doare     (1000) doare     (1000)       28 2022-12-15 14:53:48.000000 measpy-0.0.9/measpy.egg-info/requires.txt
+-rw-rw-r--   0 doare     (1000) doare     (1000)        7 2022-12-15 14:53:48.000000 measpy-0.0.9/measpy.egg-info/top_level.txt
+-rw-rw-r--   0 doare     (1000) doare     (1000)       38 2022-12-15 14:53:48.122190 measpy-0.0.9/setup.cfg
+-rw-rw-r--   0 doare     (1000) doare     (1000)     1756 2022-12-15 14:42:34.000000 measpy-0.0.9/setup.py
```

### Comparing `measpy-0.0.8/PKG-INFO` & `measpy-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: measpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Measurements with Python
-Home-page: UNKNOWN
 Author: Olivier Doaré
 Author-email: <olivier.doare@ensta-paris.fr>
-License: UNKNOWN
-Description: 
-            measpy is a set of classes and methods to help the data acquisition and analysis of signals. It is mainly acoustics and vibrations oriented. This package is very recent, it is still incomplete and many bugs may appear.
-        
-            The base classes are:
-        
-            - ```Signal```: It is basically a class that contain a 1D numpy array, an a few other properties to describe the data as: sampling frequency, calibration and unit.
-            - ```Spectral```: A spectral data class that contains the complex amplitudes as a 1D numpy array for frequencies up to the Nyquist frequency, and some properties as sampling frequency, unit, description
-            - ```Measurement``` : A class that describe a data acquisition process, its outputs (Signal objects), its inputs (Signal objects)...
-            - ```Weighting``` : Weighting spectral functions (Not yet fully test/functionnal)
-        
-            For now, these daq devices are implemented :
-        
-            - Audio cards, via the ```sounddevice``` package,
-            - NI DAQ cards, via the ```nidaqmx``` package.
-            
 Keywords: Python,Measurements,Data acquisition,Signal processing
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
+
+    measpy is a set of classes and methods to help the data acquisition and analysis of signals. It is mainly acoustics and vibrations oriented. This package is very recent, it is still incomplete and many bugs may appear.
+
+    The base classes are:
+
+    - ```Signal```: It is basically a class that contain a 1D numpy array, an a few other properties to describe the data as: sampling frequency, calibration and unit.
+    - ```Spectral```: A spectral data class that contains the complex amplitudes as a 1D numpy array for frequencies up to the Nyquist frequency, and some properties as sampling frequency, unit, description
+    - ```Measurement``` : A class that describe a data acquisition process, its outputs (Signal objects), its inputs (Signal objects)...
+    - ```Weighting``` : Weighting spectral functions (Not yet fully test/functionnal)
+
+    For now, these daq devices are implemented :
+
+    - Audio cards, via the ```sounddevice``` package,
+    - NI DAQ cards, via the ```nidaqmx``` package.
+
```

### Comparing `measpy-0.0.8/README.md` & `measpy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `measpy-0.0.8/measpy/__main__.py` & `measpy-0.0.9/measpy/__main__.py`

 * *Files identical despite different names*

### Comparing `measpy-0.0.8/measpy/_tools.py` & `measpy-0.0.9/measpy/_tools.py`

 * *Files identical despite different names*

### Comparing `measpy-0.0.8/measpy/audio.py` & `measpy-0.0.9/measpy/audio.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         M.in_device=None
     if M.out_sig!=None:
         if M.out_device=='':
             print("Warning: no device specified, changing to None")
             M.out_device=None
 
     now = datetime.now()
-    M.date = now.strftime("%Y%m%d")
-    M.time = now.strftime("%H%M%S")
+    M.date = now.strftime("%Y-%m-%d")
+    M.time = now.strftime("%H:%M:%S")
 
     # Set the audio devices to use
     if M.out_sig!=None:
         sd.default.device=(M.in_device,M.out_device)
     else:
         sd.default.device=M.in_device
```

### Comparing `measpy-0.0.8/measpy/measurement.py` & `measpy-0.0.9/measpy/measurement.py`

 * *Files 5% similar despite different names*

```diff
@@ -298,14 +298,16 @@
         self.in_cal=convl(float,meas['in_cal'])
         self.in_dbfs=convl(float,meas['in_dbfs'])
         self.in_unit=convl(str,meas['in_unit'])
         self.in_name=convl(str,meas['in_name'])
         self.in_desc=convl(str,meas['in_desc'])
         self.extrat=convl(float,meas['extrat'])
         self.out_sig=convl1(str,meas['out_sig'])
+        if self.out_sig=='None':
+            self.out_sig=None
         try:
             self.data=meas['data']
         except:
             pass
         try:
             self.date=convl1(str,meas['date'])
             self.time=convl1(str,meas['time'])
@@ -316,14 +318,15 @@
             self.out_amp=convl1(float,meas['out_amp'])
             self.out_name=convl(str,meas['out_name'])
             self.out_desc=convl(str,meas['out_desc'])
             self.out_sig_freqs=convl(float,meas['out_sig_freqs'])
             self.out_sig_fades=convl(float,meas['out_sig_fades'])
             self.io_sync=convl1(int,meas['io_sync'])
             self.out_dbfs=convl(float,meas['out_dbfs'])
+            self.out_device=convl1(str,meas['out_device'])            
         self.in_device=convl1(str,meas['in_device'])
         self.out_device=convl1(str,meas['out_device'])
         self.device_type=convl1(str,meas['device_type'])
         self.data_keys=convl(str,meas['data_keys'])
         # print('In _from_dict')
         # print(self.data)
 
@@ -346,40 +349,73 @@
             mesu = pickle.load(handle)
         M = cls()
         M._from_dict(mesu)
         for key in M.datakeys:
             M.data[key].unit=Unit(str(M.data[key].unit))
         return M
 
+    def _data_to_array(self,includetime=False,datatype='raw'):
+        n = 0
+        if includetime:
+            out = self.data[list(self.data.keys())[0]].time[:,None]
+            n += 1
+        for key in self.data.keys():
+            if n==0:
+                if datatype=='raw':
+                    out = self.data[key].raw[:,None]
+                elif datatype=='volts':
+                    out = self.data[key].volts[:,None]
+                elif datatype=='values':
+                    out = self.data[key].values[:,None]
+                n += 1
+            else:
+                if datatype=='raw':
+                    out = np.block([out,self.data[key].raw[:,None]])
+                elif datatype=='volts':
+                    out = np.block([out,self.data[key].volts[:,None]])
+                elif datatype=='values':
+                    out = np.block([out,self.data[key].values[:,None]])
+                n += 1
+        return out
+
     def _data_to_wav(self,filename):
         """ Save all data in the measurement as a unique wav file
             It is not the recommended usage to use this method, but
             use to_csvwav or to_jsonwav to save the data, and its
             descriptions.
 
             :param filename: WAV file name
             :type filename: str
         """
-        n = 0
-        for key in self.data.keys():
-            if n==0:
-                out = self.data[key].raw[:,None]
-                n += 1
-            else:
-                out = np.block([out,self.data[key].raw[:,None]])
-                n += 1
-        wav.write(filename,int(round(self.fs)),out)
+        wav.write(filename,int(round(self.fs)),self._data_to_array())
+
+    def _data_to_txt(self,filename,includetime=True,datatype='raw'):
+        """ Save all data in the measurement as a unique txt file
+            It is not the recommended usage to use this method, but
+            use to_csvtxt or to_jsontxt to save the data, and its
+            descriptions.
+
+            :param filename: TXT file name
+            :type filename: str
+            :param datatype: Type of data ('raw', 'volts' or 'values')
+            :type datatype: str 
+        """
+        np.savetxt(filename,self._data_to_array(includetime=includetime,datatype=datatype))
+
 
     def _data_from_wav(self,filename):
         _, dat = wav.read(filename)
         n = 0
-        #print(self.data)
-        for key in self.data_keys:
-            self.data[key].raw = dat[:,n]
-            n += 1
+        if len(self.data_keys)==1:
+            for key in self.data_keys:
+                self.data[key].raw = dat
+        else:
+            for key in self.data_keys:
+                self.data[key].raw = dat[:,n]
+                n += 1        #print(self.data)
         for key in self.in_name:
             pos = self.in_name.index(key)
             self.data[key].unit = Unit(self.in_unit[pos])
             self.data[key].cal = self.in_cal[pos]
             self.data[key].dbfs = self.in_dbfs[pos]
             self.data[key].desc = self.in_desc[pos]
             self.data[key].fs = self.fs
@@ -483,14 +519,27 @@
         M._json_to_params(filebase+'.json')
         # try:
         M._data_from_wav(filebase+'.wav')
         # except:
         # print('data_from_wav failed (file not present?)')
         return M
 
+    def to_csvtxt(self,filebase,includetime=True,datatype='values'):
+        """ Saves a Measurement object to a set of files
+
+            * filebase : string from which two file names are created
+            * filebase+'.csv' : All measurement parameters
+            * filebase+'.txt' : all input and out channels + time (as readable textfile)
+        """
+        self._params_to_csv(filebase+'.csv')
+        # try:
+        self._data_to_txt(filebase+'.txt',includetime=includetime,datatype=datatype)
+        # except:
+        #     print('data_to_wav failed (no data?)')
+
     def plot(self,ytype='units',limit=None):
 
         for ii in range(self.y.shape[1]):
             if ytype=='units':
                 plt.plot(self.t,self.y[:,ii])
             if ytype=='volts':
                 plt.plot(self.t,self.y_volts[:,ii])
```

### Comparing `measpy-0.0.8/measpy/ni.py` & `measpy-0.0.9/measpy/ni.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         M.in_device=system.devices[0].name
     if M.out_sig!=None:
         if M.out_device=='':
             print("Warning: no output device specified, changing to "+system.devices[0].name)
             M.out_device=system.devices[0].name
             
     now = datetime.now()
-    M.date = now.strftime("%Y%m%d")
-    M.time = now.strftime("%H%M%S")
+    M.date = now.strftime("%Y-%m-%d")
+    M.time = now.strftime("%H:%M:%S")
 
     # Insert a synchronization peak at the begining of the output signals
     if M.out_sig==None:
         dursync=0
         effsync=False
     elif M.io_sync>0:
         if M.io_sync in M.in_map:
```

### Comparing `measpy-0.0.8/measpy/signal.py` & `measpy-0.0.9/measpy/signal.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,17 +264,20 @@
 
             - ax : an axes object to plot on
             - **kwargs : all the optionnal arguments of matplotlib.pyplot.line2D
 
             Returns:
             - ax : an axes object
         """
+
+        kwargs.setdefault("label",self.desc+' ['+str(self.unit.units)+']')
+
         if ax==None:
             _,ax = plt.subplots(1)
-        ax.plot(self.time,self.values,**kwargs,label=self.desc+' ['+str(self.unit.units)+']')
+        ax.plot(self.time,self.values,**kwargs)
         ax.set_xlabel('Time (s)')
         ax.set_position([0.1,0.25,0.85,0.7])
         ax.legend(loc=(0.05,-0.32),ncol=2)
         return ax
 
     def psd(self,**kwargs):
         """ Compute power spectral density of the signal object
@@ -299,17 +302,17 @@
             :param nperseg: Window size, defaults to 512
             :type nperseg: int, optionnal
             :return: A resampled signal
             :rtype: measpy.signal.Signal       
         """
         return self.similar(
             values=np.sqrt(smooth(self.values**2,nperseg)),
-            desc=add_step(self.desc,'RMS smoothed on '+str(nperseg)+' data points',
+            desc=add_step(self.desc,'RMS smoothed on '+str(nperseg)+' data points'),
             cal=1.0,
-            dbfs=1.0)
+            dbfs=1.0
         )
 
     def rms(self):
         """ Compute the RMS of the complete Signal
 
             :return: A quantity
             :rtype: unyt.Quantity      
@@ -346,14 +349,21 @@
 
     def dB_SPL(self):
         """ Computes 20*log10(self.values/PREF).
             PREF is the reference pressure in air (20e-6 Pa)
         """
         return self.dB(PREF)
 
+    
+    def dB_SVL(self):
+        """ Computes 20*log10(self.values/VREF).
+            VREF is the reference particle velocity (5e-8 m/s)
+        """
+        return self.dB(VREF)
+
 
     def resample(self,fs):
         """ Changes sampling rate of the signal
 
             :param fs: Desired sampling rate
             :type fs: float
             :return: A resampled signal
@@ -421,15 +431,15 @@
         return c.time[np.argmax(c.values)]
 
     def cut(self,**kwargs):
         """ Cut signal between positions.
 
             :param pos: Start and stop positions of the new signal, given as indices, defaults to (0,-1)
             :type pos: tuple of int, optionnal
-            :param dur: Start and stop positions of the new signal, given as indices
+            :param dur: Start and stop positions of the new signal, given as time values
             :type dur: tuple of float, optionnal
 
             pos and dur cannot be both specified
         """
         if ('dur' in kwargs) and ('pos' in kwargs):
             raise Exception('Error: dur and pos cannot be both specified')
         elif ('dur' in kwargs):
@@ -484,32 +494,34 @@
         return Spectral(values=Y*S,
             desc='Transfer function between input log sweep and '+self.desc,
             unit=self.unit/Unit('V'),
             fs=self.fs,
             full=False
         )
     
-    def fft(self):
+    def fft(self,norm="backward"):
         """ FFT of the signal.
             Returns a Spectral object. Unit is preserved during the process.
         """
-        return Spectral(values=np.fft.fft(self.values),
+        return Spectral(values=np.fft.fft(self.values,norm=norm),
                                 fs=self.fs,
                                 unit=self.unit,
                                 full=True,
+                                norm=norm,
                                 desc=add_step(self.desc,'FFT'))
     
-    def rfft(self):
+    def rfft(self,norm="backward"):
         """ Real FFT of the signal.
             Returns a Spectral object. Unit is preserved during the process.
         """
-        return Spectral(values=np.fft.rfft(self.values),
+        return Spectral(values=np.fft.rfft(self.values,norm=norm),
                                 fs=self.fs,
                                 unit=self.unit,
                                 full=False,
+                                norm=norm,
                                 desc=add_step(self.desc,'RFFT'))
     
     def to_csvwav_old(self,filename):
         """Saves the signal into a pair of files:
 
         * A CSV file with the signal parameters
         * A WAV file with the raw data
@@ -1060,37 +1072,40 @@
         :type desc: str, optional
         :param unit: Spectral data unit
         :type unit: str, unyt.Unit, optional
         :param values: Values of the pectral data
         :type values: numpy.array, optional
         :param full: If true, the full spectrum is given, from 0 to fs, if false, only up to fs/2
         :type full: bool, optionnal
-        
+        :param norm: Type of normalization "backward", "ortho" or "full". See numpy.fft doc.
+        :type norm: string, optionnal        
         values and dur cannot be both specified.
         If dur is given, values are initialised at 0 
     """
     def __init__(self,**kwargs):
         if ('values' in kwargs) and ('dur' in kwargs):
             raise Exception('Error: values and dur cannot be both specified.')
         values = kwargs.setdefault("values",None)
         fs = kwargs.setdefault("fs",1)
         desc = kwargs.setdefault("desc",'Spectral data')
         unit = kwargs.setdefault("unit",'1')
         full = kwargs.setdefault("full",False)
+        norm = kwargs.setdefault("norm","backward")
         if 'dur' in kwargs:
             if full:
                 self._values=np.zeros(int(round(fs*kwargs['dur'])),dtype=complex)
             else:
                 self._values=np.zeros(int(round(fs*kwargs['dur']/2)+1),dtype=complex)
         else:
             self._values=values
         self.desc = desc
         self.unit = Unit(unit)
         self.fs = fs
         self.full = full
+        self.norm = norm
 
     def similar(self,**kwargs):
         """ Returns a copy of the Spectral object
             with properties changed as specified
             by the optionnal arguments.
 
             It is possible to construct a new Spectral object
@@ -1111,15 +1126,16 @@
 
         """
         values = kwargs.setdefault("values",self.values)
         fs = kwargs.setdefault("fs",self.fs)
         desc = kwargs.setdefault("desc",self.desc)
         unit = kwargs.setdefault("unit",str(self.unit.units))
         full = kwargs.setdefault("full",self.full)
-        out = Spectral(values=values,fs=fs,desc=desc,unit=unit,full=full)
+        norm = kwargs.setdefault("norm",self.norm)
+        out = Spectral(values=values,fs=fs,desc=desc,unit=unit,full=full,norm=norm)
         if 'w' in kwargs:
             w = kwargs['w']
             spa = csaps(w.freqs, w.amp, smooth=0.9)
             spp = csaps(w.freqs, w.phase, smooth=0.9)
             out.values=spa(self.freqs)*np.exp(1j*spp(self.freqs))
         return out
 
@@ -1240,26 +1256,26 @@
 
     def irfft(self):
         """ Compute the real inverse Fourier transform
             of the spectral data set
         """
         if self.full:
             raise Exception('Error: the spectrum is full, use ifft instead')
-        return Signal(raw=np.fft.irfft(self.values),
+        return Signal(raw=np.fft.irfft(self.values,norm=self.norm),
                             desc=add_step(self.desc,'IFFT'),
                             fs=self.fs,
                             unit=self.unit)
 
     def ifft(self):
         """ Compute the inverse Fourier transform
             of the spectral data set
         """
         if not(self.full):
             raise Exception('Error: the spectrum is not full, use irfft instead')
-        return Signal(raw=np.fft.ifft(self.values),
+        return Signal(raw=np.fft.ifft(self.values,norm=self.norm),
                             desc=add_step(self.desc,'IFFT'),
                             fs=self.fs,
                             unit=self.unit)
 
     def filterout(self,freqsrange):
         """ Cancels values below and above a given frequency
             Returns a Spectral class object
@@ -1292,27 +1308,33 @@
 
     def apply_dBC(self):
         #w = Weighting.from_csv('measpy/data/dBC.csv')
         return self.apply_weighting(WDBC)
 
     def dB_SPL(self):
         return self.unit_to(Unit(PREF)).similar(
-            values=20*np.log10(self._values/PREF.v),
+            values=20*np.log10(np.abs(self._values)/PREF.v),
             desc=add_step(self.desc,'dB SPL')
         )
 
+    def dB_SVL(self):
+        return self.unit_to(Unit(VREF)).similar(
+            values=20*np.log10(np.abs(self._values)/VREF.v),
+            desc=add_step(self.desc,'dB SVL')
+        )
+
     def dBV(self):
         return self.unit_to(Unit(PREF)).similar(
-            values=20*np.log10(self._values/DBVREF.v),
+            values=20*np.log10(np.abs(self._values)/DBVREF.v),
             desc=add_step(self.desc,'dBV')
         )
     
     def dBu(self):
         return self.unit_to(Unit(PREF)).similar(
-            values=20*np.log10(self._values/DBUREF.v),
+            values=20*np.log10(np.abs(self._values)/DBUREF.v),
             desc=add_step(self.desc,'dBu')
         )
 
     def group_delay(self):
         phase = np.unwrap(np.angle(self.values))
         return self.similar(
             values=-self.dur*np.diff(phase)/2/np.pi,
@@ -1331,15 +1353,15 @@
         :type dby: bool, optional
         :param plotphase: If True, also plots the phase , defaults to True
         :type plotphase: bool, optional
         :return: An axes type object if plotphase is False, a list of two axes objects if plotphase is True
         :rtype: axes, or list of axes
         """
 
-        plotlabel = kwargs.setdefault("label",self.desc+' ['+str(self.unit.units)+']')
+        kwargs.setdefault("label",self.desc+' ['+str(self.unit.units)+']')
 
         if type(ax)==type(None):
             if plotphase:
                 _,ax = plt.subplots(2)
                 ax_0 = ax[0]
             else:
                 _,ax = plt.subplots(1)
@@ -1347,29 +1369,46 @@
         else:
             if plotphase:
                 ax_0 = ax[0]
             else:
                 ax_0 = ax
 
         if dby:
-            values_to_plot = 20*np.log10(np.abs(self.values))
-            label = '20 Log |H|'
+            if(self.unit == Unit("Pa")):
+                modulus_to_plot = self.dB_SPL().values
+                label = '20 Log |P|/P0'
+            elif(self.unit == Unit("m/s")):
+                modulus_to_plot = self.dB_SVL().values
+                label = '20 Log |V|/V0'
+            else:
+                modulus_to_plot = 20*np.log10(np.abs(self.values))
+                label = '20 Log |H|'
+
+            #Only keep finite values
+            valid_indices = np.isfinite(modulus_to_plot)
+
+            frequencies_to_plot = self.freqs[valid_indices]
+            modulus_to_plot = modulus_to_plot[valid_indices]
+            phase_to_plot = np.unwrap(np.angle(self.values))[valid_indices]
+            
         else:
-            values_to_plot = self.values
+            frequencies_to_plot = self.freqs
+            modulus_to_plot = np.abs(self.values)
+            phase_to_plot = np.unwrap(np.angle(self.values))
             label = 'H'
 
-        ax_0.plot(self.freqs,values_to_plot,label=plotlabel)
+        ax_0.plot(frequencies_to_plot,modulus_to_plot,**kwargs)
         ax_0.set_xlabel('Freq (Hz)')
         ax_0.set_ylabel(label)       
         if logx:
             ax_0.set_xscale('log')
         if plotphase:
-            ax[1].plot(self.freqs,np.unwrap(np.angle(self.values)),label=plotlabel)
+            ax[1].plot(frequencies_to_plot,phase_to_plot,**kwargs)
             ax[1].set_ylabel('Phase')
-            ax[1].set_xlabel('Freq (Hz')
+            ax[1].set_xlabel('Freq (Hz)')
             if logx:
                 ax[1].set_xscale('log')
         return ax
         
 
     def _add(self,other):
         """Add two spectra
@@ -1553,26 +1592,26 @@
             )
         else:
             raise Exception('Incompatible type when dividing something with a Signal')
 
     def __rtruediv__(self,other):
         return self.__invert__().__mul__(other)
 
-    def abs(self):
+    def _abs(self):
         """ Absolute value
             Returns a Spectral class object
         """
         return self.similar(
             values=np.abs(self.values),
             desc=add_step(self.desc,"abs")
         )
 
     def __abs__(self):
         """Absolute value """
-        return self.abs()
+        return self._abs()
 
     @classmethod
     def tfe(cls,x,y,**kwargs):
         if (type(x)!=Signal) & (type(y)!=Signal):
             raise Exception('x and y inputs have to be Signal')      
         return y.tfe_welch(x,**kwargs)
     @property
@@ -1685,14 +1724,15 @@
         return self.amp*np.exp(1j*self.phase)
 
     # END of Weighting
 
 # Constants
 
 PREF = 20e-6*Unit('Pa') # Acoustic pressure reference level
+VREF = 5e-8*Unit('m/s') # Reference particle velocity
 DBUREF = 1*Unit('V')
 DBVREF = np.sqrt(2)*Unit('V')
 
 WDBA = [
     [6.3,-85.4],
     [8,-77.8],
     [10,-70.4],
```

### Comparing `measpy-0.0.8/measpy.egg-info/PKG-INFO` & `measpy-0.0.9/measpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: measpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Measurements with Python
-Home-page: UNKNOWN
 Author: Olivier Doaré
 Author-email: <olivier.doare@ensta-paris.fr>
-License: UNKNOWN
-Description: 
-            measpy is a set of classes and methods to help the data acquisition and analysis of signals. It is mainly acoustics and vibrations oriented. This package is very recent, it is still incomplete and many bugs may appear.
-        
-            The base classes are:
-        
-            - ```Signal```: It is basically a class that contain a 1D numpy array, an a few other properties to describe the data as: sampling frequency, calibration and unit.
-            - ```Spectral```: A spectral data class that contains the complex amplitudes as a 1D numpy array for frequencies up to the Nyquist frequency, and some properties as sampling frequency, unit, description
-            - ```Measurement``` : A class that describe a data acquisition process, its outputs (Signal objects), its inputs (Signal objects)...
-            - ```Weighting``` : Weighting spectral functions (Not yet fully test/functionnal)
-        
-            For now, these daq devices are implemented :
-        
-            - Audio cards, via the ```sounddevice``` package,
-            - NI DAQ cards, via the ```nidaqmx``` package.
-            
 Keywords: Python,Measurements,Data acquisition,Signal processing
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
+
+    measpy is a set of classes and methods to help the data acquisition and analysis of signals. It is mainly acoustics and vibrations oriented. This package is very recent, it is still incomplete and many bugs may appear.
+
+    The base classes are:
+
+    - ```Signal```: It is basically a class that contain a 1D numpy array, an a few other properties to describe the data as: sampling frequency, calibration and unit.
+    - ```Spectral```: A spectral data class that contains the complex amplitudes as a 1D numpy array for frequencies up to the Nyquist frequency, and some properties as sampling frequency, unit, description
+    - ```Measurement``` : A class that describe a data acquisition process, its outputs (Signal objects), its inputs (Signal objects)...
+    - ```Weighting``` : Weighting spectral functions (Not yet fully test/functionnal)
+
+    For now, these daq devices are implemented :
+
+    - Audio cards, via the ```sounddevice``` package,
+    - NI DAQ cards, via the ```nidaqmx``` package.
+
```

### Comparing `measpy-0.0.8/setup.py` & `measpy-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 from datetime import datetime
 
 now = datetime.now()
 VERSION = 'git'+now.strftime("%Y%m%d")
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Measurements with Python'
 LONG_DESCRIPTION = """
     measpy is a set of classes and methods to help the data acquisition and analysis of signals. It is mainly acoustics and vibrations oriented. This package is very recent, it is still incomplete and many bugs may appear.
 
     The base classes are:
 
     - ```Signal```: It is basically a class that contain a 1D numpy array, an a few other properties to describe the data as: sampling frequency, calibration and unit.
```

