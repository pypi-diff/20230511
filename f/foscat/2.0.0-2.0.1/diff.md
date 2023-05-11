# Comparing `tmp/foscat-2.0.0.tar.gz` & `tmp/foscat-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-g30zvbp_/foscat-2.0.0.tar", last modified: Tue Apr  4 18:11:09 2023, max compression
+gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-mi8in77j/foscat-2.0.1.tar", last modified: Wed May 10 14:16:02 2023, max compression
```

## Comparing `foscat-2.0.0.tar` & `foscat-2.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-04-04 18:11:09.000000 foscat-2.0.0/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-04-04 18:11:09.000000 foscat-2.0.0/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2022-12-13 16:07:53.000000 foscat-2.0.0/README.md
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-04-04 18:11:09.000000 foscat-2.0.0/setup.cfg
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-04-04 18:07:21.000000 foscat-2.0.0/setup.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-04-04 18:11:09.000000 foscat-2.0.0/src/
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-04-04 18:11:09.000000 foscat-2.0.0/src/foscat/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    56857 2023-04-04 16:50:09.000000 foscat-2.0.0/src/foscat/FoCUS.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.0.0/src/foscat/GetGPUinfo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1766 2023-03-31 09:38:33.000000 foscat-2.0.0/src/foscat/Rformat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    12170 2023-04-03 09:40:32.000000 foscat-2.0.0/src/foscat/Synthesis.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.0.0/src/foscat/__init__.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13465 2023-03-31 07:45:21.000000 foscat-2.0.0/src/foscat/backend.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.0.0/src/foscat/build_demo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.0.0/src/foscat/demo2d.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    18965 2023-04-04 07:56:22.000000 foscat-2.0.0/src/foscat/scat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.0.0/src/foscat/scat_cov.old.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    43464 2023-04-03 12:03:50.000000 foscat-2.0.0/src/foscat/scat_cov.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.0.0/src/foscat/scat_cov_new.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-04-04 18:11:09.000000 foscat-2.0.0/src/foscat.egg-info/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-04-04 18:11:09.000000 foscat-2.0.0/src/foscat.egg-info/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-04-04 18:11:09.000000 foscat-2.0.0/src/foscat.egg-info/SOURCES.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-04-04 18:11:09.000000 foscat-2.0.0/src/foscat.egg-info/dependency_links.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-04-04 18:11:09.000000 foscat-2.0.0/src/foscat.egg-info/requires.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-04-04 18:11:09.000000 foscat-2.0.0/src/foscat.egg-info/top_level.txt
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-10 14:16:02.000000 foscat-2.0.1/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-05-10 14:16:02.000000 foscat-2.0.1/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2022-12-13 16:07:53.000000 foscat-2.0.1/README.md
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-05-10 14:16:02.000000 foscat-2.0.1/setup.cfg
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-05-10 14:15:16.000000 foscat-2.0.1/setup.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-10 14:16:02.000000 foscat-2.0.1/src/
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57131 2023-05-02 14:56:56.000000 foscat-2.0.1/src/foscat/FoCUS.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.0.1/src/foscat/GetGPUinfo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1766 2023-03-31 09:38:33.000000 foscat-2.0.1/src/foscat/Rformat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    15268 2023-05-10 13:27:24.000000 foscat-2.0.1/src/foscat/Synthesis.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.0.1/src/foscat/__init__.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13465 2023-03-31 07:45:21.000000 foscat-2.0.1/src/foscat/backend.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.0.1/src/foscat/build_demo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.0.1/src/foscat/demo2d.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    21467 2023-05-02 15:09:32.000000 foscat-2.0.1/src/foscat/scat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.0.1/src/foscat/scat_cov.old.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    46097 2023-04-26 15:05:16.000000 foscat-2.0.1/src/foscat/scat_cov.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.0.1/src/foscat/scat_cov_new.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat.egg-info/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat.egg-info/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat.egg-info/SOURCES.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat.egg-info/dependency_links.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat.egg-info/requires.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-05-10 14:16:02.000000 foscat-2.0.1/src/foscat.egg-info/top_level.txt
```

### Comparing `foscat-2.0.0/PKG-INFO` & `foscat-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.0
+Version: 2.0.1
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

### Comparing `foscat-2.0.0/README.md` & `foscat-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `foscat-2.0.0/setup.py` & `foscat-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='foscat',
-    version='2.0.0',
+    version='2.0.1',
     description='Generate synthetic Healpix or 2D data using Cross Scattering Transform' ,
     long_description='Utilize the Cross Scattering Transform (described in https://arxiv.org/abs/2207.12527) to synthesize Healpix or 2D data that is suitable for component separation purposes, such as denoising. \n A demo package for this process can be found at https://github.com/jmdelouis/FOSCAT_DEMO. \n\n List of developers : J.-M. Delouis, T. Foulqieur, L. Mousset, E. Allys ' ,
     license='MIT',
     author='Jean-Marc DELOUIS',
     author_email='jean.marc.delouis@ifremer.fr',
     maintainer='Theo Foulquier',
     maintainer_email='theo.foulquier@ifremer.fr',
```

### Comparing `foscat-2.0.0/src/foscat/FoCUS.py` & `foscat-2.0.1/src/foscat/FoCUS.py`

 * *Files 2% similar despite different names*

```diff
@@ -1083,15 +1083,15 @@
         shape=x.shape.as_list()
         
         l_x=self.backend.bk_expand_dims(x,axis)
             
         if self.use_R_format:
             nside=mask.nside
             if self.remove_border[nside] is None:
-                self.remove_border[nside]=np.ones([1,12,nside+2*self.R_off,nside+2*self.R_off])
+                self.remove_border[nside]=np.ones([1,shape[axis-1],nside+2*self.R_off,nside+2*self.R_off])
                 self.remove_border[nside][0,:,0:self.R_off,:]=0.0
                 self.remove_border[nside][0,:,-self.R_off:,:]=0.0
                 self.remove_border[nside][0,:,:,0:self.R_off]=0.0
                 self.remove_border[nside][0,:,:,-self.R_off:]=0.0
                 
             l_mask=mask.get()*self.remove_border[nside]
         else:
@@ -1102,16 +1102,22 @@
             
         if self.use_R_format:
             for i in range(axis+3,len(x.shape)):
                 l_mask=self.backend.bk_expand_dims(l_mask,-1)
 
             if l_x.get().dtype==self.all_cbk_type:
                 l_mask=self.backend.bk_complex(l_mask,0*l_mask)
-                
-            return self.backend.bk_reduce_sum(self.backend.bk_reduce_sum(self.backend.bk_reduce_sum(l_mask*l_x.get(),axis=axis+1),axis=axis+1),axis=axis+1)/(12*nside*nside)
+
+            shape1=list(l_mask.shape)
+            shape2=list(l_x.get().shape)
+
+            oshape1=shape1[0:axis+1]+[shape1[axis+3]*shape1[axis+1]*shape1[axis+2]]+shape1[axis+4:]
+            oshape2=shape2[0:axis+1]+[shape2[axis+3]*shape2[axis+1]*shape2[axis+2]]+shape2[axis+4:]
+            
+            return self.backend.bk_reduce_sum(self.backend.bk_reshape(l_mask,oshape1)*self.backend.bk_reshape(l_x.get(),oshape2),axis=axis+1)/(12*nside*nside)
         else:
             for i in range(axis+1,len(x.shape)):
                 l_mask=self.backend.bk_expand_dims(l_mask,-1)
 
             if l_x.dtype==self.all_cbk_type:
                 l_mask=self.backend.bk_complex(l_mask,0.0)
             return self.backend.bk_reduce_mean(l_mask*l_x,axis=axis+1)
```

### Comparing `foscat-2.0.0/src/foscat/GetGPUinfo.py` & `foscat-2.0.1/src/foscat/GetGPUinfo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.0/src/foscat/Rformat.py` & `foscat-2.0.1/src/foscat/Rformat.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.0/src/foscat/backend.py` & `foscat-2.0.1/src/foscat/backend.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.0/src/foscat/build_demo.py` & `foscat-2.0.1/src/foscat/build_demo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.0/src/foscat/scat.py` & `foscat-2.0.1/src/foscat/scat.py`

 * *Files 22% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         
     def __add__(self,other):
         assert isinstance(other, float) or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.doadd(self.P00,other.P00), \
-                        (self.S0+ other.S0), \
+                        self.doadd(self.S0, other.S0), \
                         self.doadd(self.S1, other.S1), \
                         self.doadd(self.S2, other.S2),backend=self.backend)
         else:
             return scat((self.P00+ other), \
                         (self.S0+ other), \
                         (self.S1+ other), \
                         (self.S2+ other),backend=self.backend)
@@ -87,15 +87,15 @@
 
     def __truediv__(self,other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.dodiv(self.P00, other.P00), \
-                        (self.S0/ other.S0), \
+                        self.dodiv(self.S0, other.S0), \
                         self.dodiv(self.S1, other.S1), \
                         self.dodiv(self.S2, other.S2),backend=self.backend)
         else:
             return scat((self.P00/ other), \
                         (self.S0/ other), \
                         (self.S1/ other), \
                         (self.S2/ other),backend=self.backend)
@@ -103,119 +103,136 @@
 
     def __rtruediv__(self,other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.dodiv(other.P00, self.P00), \
-                        (other.S0 / self.S0), \
+                        self.dodiv(other.S0 , self.S0), \
                         self.dodiv(other.S1 , self.S1), \
                         self.dodiv(other.S2 , self.S2),backend=self.backend)
         else:
             return scat((other/ self.P00), \
                         (other / self.S0), \
                         (other / self.S1), \
                         (other / self.S2),backend=self.backend)
         
     def __sub__(self,other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.domin(self.P00, other.P00), \
-                        (self.S0- other.S0), \
+                        self.domin(self.S0, other.S0), \
                         self.domin(self.S1, other.S1), \
                         self.domin(self.S2, other.S2),backend=self.backend)
         else:
             return scat((self.P00- other), \
                         (self.S0- other), \
                         (self.S1- other), \
                         (self.S2- other),backend=self.backend)
         
     def __rsub__(self,other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.domin(other.P00,self.P00), \
-                        (other.S0- self.S0), \
+                        self.domin(other.S0, self.S0), \
                         self.domin(other.S1, self.S1), \
                         self.domin(other.S2, self.S2),backend=self.backend)
         else:
             return scat((other-self.P00), \
                         (other-self.S0), \
                         (other-self.S1), \
                         (other-self.S2),backend=self.backend)
         
     def __mul__(self,other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.domult(self.P00, other.P00), \
-                        (self.S0* other.S0), \
+                        self.domult(self.S0, other.S0), \
                         self.domult(self.S1, other.S1), \
                         self.domult(self.S2, other.S2),backend=self.backend)
         else:
             return scat((self.P00* other), \
                         (self.S0* other), \
                         (self.S1* other), \
                         (self.S2* other),backend=self.backend)
 
     def __rmul__(self,other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.domult(self.P00, other.P00), \
-                        (self.S0* other.S0), \
+                        self.domult(self.S0, other.S0), \
                         self.domult(self.S1, other.S1), \
                         self.domult(self.S2, other.S2),backend=self.backend)
         else:
             return scat((self.P00* other), \
                         (self.S0* other), \
                         (self.S1* other), \
                         (self.S2* other),backend=self.backend)
 
+    def l1_abs(self,x):
+        y=self.get_np(x)
+        if y.dtype=='complex64' or y.dtype=='complex128':
+            tmp=y.real*y.real+y.imag*y.imag
+            tmp=np.sign(tmp)*np.sqrt(np.fabs(tmp))
+            y=tmp
+        
+        return(y)
+    
     def plot(self,name=None,hold=True,color='blue',lw=1,legend=True):
 
         import matplotlib.pyplot as plt
         
         if name is None:
             name=''
 
         if hold:
             plt.figure(figsize=(8,8))
         
         plt.subplot(2,2,1)
         if legend:
-            plt.plot(self.get_np(abs(self.S0)).flatten(),color=color,label=r'%s $S_0$'%(name),lw=lw)
+            plt.plot(abs(self.l1_abs(self.S0).flatten()),':',color=color,lw=lw)
+            plt.plot(self.l1_abs(self.S0).flatten(),color=color,label=r'%s $S_0$'%(name),lw=lw)
         else:
-            plt.plot(self.get_np(abs(self.S0)).flatten(),color=color,lw=lw)
+            plt.plot(abs(self.l1_abs(self.S0).flatten()),':',color=color,lw=lw)
+            plt.plot(self.l1_abs(self.S0).flatten(),color=color,lw=lw)
         plt.yscale('log')
         plt.legend()
         plt.subplot(2,2,2)
         if legend:
-            plt.plot(self.get_np(abs(self.S1)).flatten(),color=color,label=r'%s $S_1$'%(name),lw=lw)
+            plt.plot(abs(self.l1_abs(self.S1).flatten()),':',color=color,lw=lw)
+            plt.plot(self.l1_abs(self.S1).flatten(),color=color,label=r'%s $S_1$'%(name),lw=lw)
         else:
-            plt.plot(self.get_np(abs(self.S1)).flatten(),color=color,lw=lw)
+            plt.plot(abs(self.l1_abs(self.S1).flatten()),':',color=color,lw=lw)
+            plt.plot(self.l1_abs(self.S1).flatten(),color=color,lw=lw)
         plt.yscale('log')
         plt.legend()
         plt.subplot(2,2,3)
         if legend:
-            plt.plot(self.get_np(abs(self.P00)).flatten(),color=color,label=r'%s $P_{00}$'%(name),lw=lw)
+            plt.plot(abs(self.l1_abs(self.P00).flatten()),':',color=color,lw=lw)
+            plt.plot(self.l1_abs(self.P00).flatten(),color=color,label=r'%s $P_{00}$'%(name),lw=lw)
         else:
-            plt.plot(self.get_np(abs(self.P00)).flatten(),color=color,lw=lw)
+            plt.plot(abs(self.l1_abs(self.P00).flatten()),':',color=color,lw=lw)
+            plt.plot(self.l1_abs(self.P00).flatten(),color=color,lw=lw)
         plt.yscale('log')
         plt.legend()
         plt.subplot(2,2,4)
         if legend:
-            plt.plot(self.get_np(abs(self.S2)).flatten(),color=color,label=r'%s $S_2$'%(name),lw=lw)
+            plt.plot(abs(self.l1_abs(self.S2).flatten()),':',color=color,lw=lw)
+            plt.plot(self.l1_abs(self.S2).flatten(),color=color,label=r'%s $S_2$'%(name),lw=lw)
         else:
-            plt.plot(self.get_np(abs(self.S2)).flatten(),color=color,lw=lw)
+            plt.plot(abs(self.l1_abs(self.S2).flatten()),':',color=color,lw=lw)
+            plt.plot(self.l1_abs(self.S2).flatten(),color=color,lw=lw)
         plt.yscale('log')
         plt.legend()
         
     def save(self,filename):
         np.save('%s_s0.npy'%(filename), self.get_S0().numpy())
         np.save('%s_s1.npy'%(filename), self.get_S1().numpy())
         np.save('%s_s2.npy'%(filename), self.get_S2().numpy())
@@ -321,19 +338,25 @@
             l_image1=I1
             if cross:
                 l_image2=I2
 
         s0=None
         s0 = self.masked_mean(l_image1,vmask,axis=axis)+s0_off
         
-        if cross:
+        if cross and Auto==False:
             if len(image1.shape)==1 or (len(image1.shape)==3 and isinstance(image1,Rformat.Rformat)):
-                s0 = self.backend.bk_concat([s0,self.masked_mean(l_image2,vmask,axis=axis)],1)+s0_off
+                if s0.dtype!='complex64' and s0.dtype!='complex128':
+                    s0 = self.backend.bk_complex(s0,self.masked_mean(l_image2,vmask,axis=axis)+s0_off)
+                else:
+                    s0 = self.backend.bk_concat([s0,self.masked_mean(l_image2,vmask,axis=axis)],axis=0)
             else:
-                s0 = self.backend.bk_concat([s0,self.masked_mean(l_image2,vmask,axis=axis)],0)+s0_off
+                if s0.dtype!='complex64' and s0.dtype!='complex128':
+                    s0 = self.backend.bk_complex(s0,self.masked_mean(l_image2,vmask,axis=axis)+s0_off)
+                else:
+                    s0 = self.backend.bk_concat([s0,self.masked_mean(l_image2,vmask,axis=axis)],axis=0)
 
         s1=None
         s2=None
         p00=None
         l2_image=None
         l2_image_imag=None
 
@@ -345,14 +368,15 @@
             if cross:
                 c_image2=self.convol(l_image2,axis=axis)
             else:
                 c_image2=c_image1
 
             # Compute (a+ib)*(a+ib)* the last c_image column is the real and imaginary part
             conj=c_image1*self.backend.bk_conjugate(c_image2)
+            
             if Auto:
                 conj=self.backend.bk_real(conj)
 
             # Compute l_p00 [....,....,Nmask,1,Norient]  
             l_p00 = self.backend.bk_expand_dims(self.masked_mean(conj,vmask,axis=axis),-2)
 
             conj=self.backend.bk_L1(conj)
@@ -364,15 +388,15 @@
             if s1 is None:
                 s1=l_s1
                 p00=l_p00
             else:
                 s1=self.backend.bk_concat([s1,l_s1],axis=-2)
                 p00=self.backend.bk_concat([p00,l_p00],axis=-2)
 
-            # Concat l2_image [....,Npix_j1,....,j1,Norient]
+                # Concat l2_image [....,Npix_j1,....,j1,Norient]
             if l2_image is None:
                 l2_image=self.backend.bk_expand_dims(self.update_R_border(conj,axis=axis),axis=-2)
             else:
                 l2_image=self.backend.bk_concat([self.backend.bk_expand_dims(self.update_R_border(conj,axis=axis),axis=-2),l2_image],axis=-2)
 
             # Convol l2_image [....,Npix_j1,....,j1,Norient,Norient]
             c2_image=self.convol(self.backend.bk_relu(l2_image),axis=axis)
@@ -407,15 +431,15 @@
 
                 # Rescale l_image [....,Npix_j1//4,....]  
                 l_image1 = self.smooth(l_image1,axis=axis)
                 l_image1 = self.ud_grade_2(l_image1,axis=axis)
                 if cross:
                     l_image2 = self.smooth(l_image2,axis=axis)
                     l_image2 = self.ud_grade_2(l_image2,axis=axis)
-
+                    
         if len(image1.shape)==1 or (len(image1.shape)==3 and isinstance(image1,Rformat.Rformat)):
             return(scat(p00[0],s0[0],s1[0],s2[0],cross,backend=self.backend))
 
         return(scat(p00,s0,s1,s2,cross,backend=self.backend))
 
     def square(self,x):
         # the abs make the complex value usable for reduce_sum or mean
@@ -429,41 +453,65 @@
         return scat(self.backend.bk_sqrt(self.backend.bk_abs(x.P00)),
                     self.backend.bk_sqrt(self.backend.bk_abs(x.S0)),
                     self.backend.bk_sqrt(self.backend.bk_abs(x.S1)),
                     self.backend.bk_sqrt(self.backend.bk_abs(x.S2)),backend=self.backend)
 
     def reduce_mean(self,x,axis=None):
         if axis is None:
-            return  (self.backend.bk_abs(self.backend.bk_reduce_mean(x.P00))+
-                     self.backend.bk_abs(self.backend.bk_reduce_mean(x.S0))+
-                     self.backend.bk_abs(self.backend.bk_reduce_mean(x.S1))+
-                     self.backend.bk_abs(self.backend.bk_reduce_mean(x.S2)))/4.0
-        else:
-            return (self.backend.bk_reduce_mean(x.P00,axis=axis)+
-                    self.backend.bk_reduce_mean(x.S0,axis=axis)+
-                    self.backend.bk_reduce_mean(x.S1,axis=axis)+
-                    self.backend.bk_reduce_mean(x.S2,axis=axis))/4.0
+            tmp=self.backend.bk_abs(self.backend.bk_reduce_sum(x.P00))+ \
+                 self.backend.bk_abs(self.backend.bk_reduce_sum(x.S0))+ \
+                 self.backend.bk_abs(self.backend.bk_reduce_sum(x.S1))+ \
+                 self.backend.bk_abs(self.backend.bk_reduce_sum(x.S2))
+            
+            ntmp=np.array(list(x.P00.shape)).prod()+ \
+                  np.array(list(x.S0.shape)).prod()+ \
+                  np.array(list(x.S1.shape)).prod()+ \
+                  np.array(list(x.S2.shape)).prod()
+            
+            return  tmp/ntmp
+        else:
+            tmp=self.backend.bk_abs(self.backend.bk_reduce_sum(x.P00,axis=axis))+ \
+                 self.backend.bk_abs(self.backend.bk_reduce_sum(x.S0,axis=axis))+ \
+                 self.backend.bk_abs(self.backend.bk_reduce_sum(x.S1,axis=axis))+ \
+                 self.backend.bk_abs(self.backend.bk_reduce_sum(x.S2,axis=axis))
+            
+            ntmp=np.array(list(x.P00.shape)).prod()+ \
+                  np.array(list(x.S0.shape)).prod()+ \
+                  np.array(list(x.S1.shape)).prod()+ \
+                  np.array(list(x.S2.shape)).prod()
+            
+            return  tmp/ntmp
 
     def reduce_sum(self,x,axis=None):
         if axis is None:
             return  self.backend.bk_reduce_sum(self.backend.bk_abs(x.P00))+ \
                 self.backend.bk_reduce_sum(self.backend.bk_abs(x.S0))+ \
                 self.backend.bk_reduce_sum(self.backend.bk_abs(x.S1))+ \
                 self.backend.bk_reduce_sum(self.backend.bk_abs(x.S2))
         else:
             return scat(self.backend.bk_reduce_sum(x.P00,axis=axis),
                         self.backend.bk_reduce_sum(x.S0,axis=axis),
                         self.backend.bk_reduce_sum(x.S1,axis=axis),
                         self.backend.bk_reduce_sum(x.S2,axis=axis),backend=self.backend)
-            
+        
+    def ldiff(self,sig,x):
+        return scat(x.domult(sig.P00,x.P00)*x.domult(sig.P00,x.P00),
+                    x.domult(sig.S0,x.S0)*x.domult(sig.S0,x.S0),
+                    x.domult(sig.S1,x.S1)*x.domult(sig.S1,x.S1),
+                    x.domult(sig.S2,x.S2)*x.domult(sig.S2,x.S2),backend=self.backend)
 
     def log(self,x):
         return scat(self.backend.bk_log(x.P00),
                     self.backend.bk_log(x.S0),
                     self.backend.bk_log(x.S1),
                     self.backend.bk_log(x.S2),backend=self.backend)
+    def abs(self,x):
+        return scat(self.backend.bk_abs(x.P00),
+                    self.backend.bk_abs(x.S0),
+                    self.backend.bk_abs(x.S1),
+                    self.backend.bk_abs(x.S2),backend=self.backend)
     def inv(self,x):
         return scat(1/(x.P00),1/(x.S0),1/(x.S1),1/(x.S2),backend=self.backend)
 
     def one(self):
         return scat(1.0,1.0,1.0,1.0,backend=self.backend)
```

### Comparing `foscat-2.0.0/src/foscat/scat_cov.old.py` & `foscat-2.0.1/src/foscat/scat_cov.old.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.0/src/foscat/scat_cov.py` & `foscat-2.0.1/src/foscat/scat_cov.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 
 def read(filename):
     thescat = scat_cov(1, 1, 1)
     return thescat.read(filename)
 
 
+testwarn=0
+
 class scat_cov:
     def __init__(self, p00, c01, c11, s1=None, c10=None,backend=None):
         self.P00     = p00
         self.C01     = c01
         self.C11     = c11
         self.S1      = s1
         self.C10     = c10
@@ -69,28 +71,37 @@
         if self.C10 is None:
             c10 = None
         else:
             if isinstance(other, scat_cov):
                 if other.C10 is None:
                     c10=None
                 else:
-                    c10 = self.C10 + other.C10
+                    c10 = self.doadd(self.C10 , other.C10)
             else:
                 c10 = self.C10 + other
+                
+        if self.C11 is None:
+            c11 = None
+        else:
+            if isinstance(other, scat_cov):
+                if other.C11 is None:
+                    c11 = None
+                else:
+                    c11 = self.doadd(self.C11, other.C11 )
+            else:
+                c11 = self.C11+other 
 
         if isinstance(other, scat_cov):
             return scat_cov(self.doadd(self.P00,other.P00),
                             (self.C01 + other.C01),
-                            (self.C11 + other.C11),
-                            s1=s1, c10=c10,backend=self.backend)
+                            c11,s1=s1, c10=c10,backend=self.backend)
         else:
             return scat_cov((self.P00 + other),
                             (self.C01 + other),
-                            (self.C11 + other),
-                            s1=s1, c10=c10,backend=self.backend)
+                            c11,s1=s1, c10=c10,backend=self.backend)
 
     def __radd__(self, other):
         return self.__add__(other)
     
     def __truediv__(self, other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
                isinstance(other, bool) or isinstance(other, scat_cov)
@@ -109,28 +120,37 @@
         if self.C10 is None:
             c10 = None
         else:
             if isinstance(other, scat_cov):
                 if other.C10 is None:
                     c10 = None
                 else:
-                    c10 = self.C10 / other.C10
+                    c10 = self.dodiv(self.C10 , other.C10)
             else:
                 c10 = self.C10 / other
+                
+        if self.C11 is None:
+            c11 = None
+        else:
+            if isinstance(other, scat_cov):
+                if other.C11 is None:
+                    c11 = None
+                else:
+                    c11 = self.dodiv(self.C11, other.C11 )
+            else:
+                c11 = self.C11/other 
 
         if isinstance(other, scat_cov):
             return scat_cov(self.dodiv(self.P00,other.P00),
                             (self.C01 / other.C01),
-                            (self.C11 / other.C11),
-                            s1=s1, c10=c10,backend=self.backend)
+                            c11,s1=s1, c10=c10,backend=self.backend)
         else:
             return scat_cov((self.P00 / other),
                             (self.C01 / other),
-                            (self.C11 / other),
-                            s1=s1, c10=c10,backend=self.backend)
+                            c11,s1=s1, c10=c10,backend=self.backend)
 
     def __rtruediv__(self, other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
                isinstance(other, bool) or isinstance(other, scat_cov)
 
         if self.S1 is None:
             s1 = None
@@ -140,30 +160,41 @@
             else:
                 s1 = other.S1 / other
 
         if self.C10 is None:
             c10 = None
         else:
             if isinstance(other, scat_cov):
-                c10 = other.C10 / self.C10
+                c10 = self.dodiv(other.C10 , self.C10)
             else:
                 c10 = other/self.C10
+                
+        if self.C11 is None:
+            c11 = None
+        else:
+            if isinstance(other, scat_cov):
+                if other.C11 is None:
+                    c11 = None
+                else:
+                    c11 = self.dodiv( other.C11,self.C11 )
+            else:
+                c11 = other/self.C11
 
         if isinstance(other, scat_cov):
             return scat_cov(self.dodiv(other.P00,self.P00),
                             (other.C01 / self.C01),
-                            (other.C11 / self.C11),
-                            s1=s1, c10=c10,backend=self.backend)
+                            c11,s1=s1, c10=c10,backend=self.backend)
         else:
             return scat_cov((other/self.P00 ),
                             (other/self.C01 ),
                             (other/self.C11 ),
                             s1=s1, c10=c10,backend=self.backend)
 
     def __rsub__(self, other):
+
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
                isinstance(other, bool) or isinstance(other, scat_cov)
 
         if self.S1 is None:
             s1 = None
         else:
             if isinstance(other, scat_cov):
@@ -177,29 +208,38 @@
         if self.C10 is None:
             c10 = None
         else:
             if isinstance(other, scat_cov):
                 if other.C10 is None:
                     c10 = None
                 else:
-                    c10 = other.C10 - self.C10 
+                    c10 = self.domin(other.C10 , self.C10 )
             else:
                 c10 = other - self.C10
+                
+        if self.C11 is None:
+            c11 = None
+        else:
+            if isinstance(other, scat_cov):
+                if other.C11 is None:
+                    c11 = None
+                else:
+                    c11 = self.domin( other.C11,self.C11 )
+            else:
+                c11 = other - self.C11
 
         if isinstance(other, scat_cov):
             return scat_cov(self.domin(other.P00,self.P00),
                             (other.C01 - self.C01),
-                            (other.C11 - self.C11),
-                            s1=s1, c10=c10,
+                            c11,s1=s1, c10=c10,
                             backend=self.backend)
         else:
             return scat_cov((other-self.P00),
                             (other-self.C01),
-                            (other-self.C11),
-                            s1=s1, c10=c10,
+                            c11,s1=s1, c10=c10,
                             backend=self.backend)
         
     def __sub__(self, other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
                isinstance(other, bool) or isinstance(other, scat_cov)
 
         if self.S1 is None:
@@ -216,29 +256,40 @@
         if self.C10 is None:
             c10 = None
         else:
             if isinstance(other, scat_cov):
                 if other.C10 is None:
                     c10 = None
                 else:
-                    c10 = self.C10 - other.C10
+                    c10 = self.domin(self.C10 , other.C10)
             else:
                 c10 = self.C10 - other
+                
+        if self.C11 is None:
+            c11 = None
+        else:
+            if isinstance(other, scat_cov):
+                if other.C11 is None:
+                    c11 = None
+                else:
+                    c11 = self.domin(self.C11 , other.C11)
+            else:
+                c11 = self.C11 - other
 
         if isinstance(other, scat_cov):
             return scat_cov(self.domin(self.P00,other.P00),
                             (self.C01 - other.C01),
-                            (self.C11 - other.C11),
+                            c11,
                             s1=s1, c10=c10,backend=self.backend)
         else:
             return scat_cov((self.P00 - other),
                             (self.C01 - other),
-                            (self.C11 - other),
+                            c11,
                             s1=s1, c10=c10,backend=self.backend)
-
+        
     def domult(self,x,y):
         if x.dtype==y.dtype:
             return x*y
         if x.dtype=='complex64' or x.dtype=='complex128':
             
             return self.backend.bk_complex(self.backend.bk_real(x)*y,self.backend.bk_imag(x)*y)
         else:
@@ -290,27 +341,38 @@
         if self.C10 is None:
             c10 = None
         else:
             if isinstance(other, scat_cov):
                 if other.C10 is None:
                     c10 = None
                 else:
-                    c10 = self.C10 * other.C10
+                    c10 = self.domult(self.C10 , other.C10)
             else:
                 c10 = self.C10 * other
 
+        if self.C11 is None:
+            c11 = None
+        else:
+            if isinstance(other, scat_cov):
+                if other.C11 is None:
+                    c11 = None
+                else:
+                    c11 = self.domult(self.C11 , other.C11)
+            else:
+                c11 = self.C11 * other
+
         if isinstance(other, scat_cov):
             return scat_cov(self.domult(self.P00,other.P00),
-                            (self.C01 * other.C01),
-                            (self.C11 * other.C11),
+                            self.domult(self.C01,other.C01),
+                            c11,
                             s1=s1, c10=c10,backend=self.backend)
         else:
             return scat_cov((self.P00 * other),
                             (self.C01 * other),
-                            (self.C11 * other),
+                            c11,
                             s1=s1, c10=c10,backend=self.backend)
 
     
     def __rmul__(self, other):
         return self.__mul__(other)
 
     def plot(self, name=None, hold=True, color='blue', lw=1, legend=True):
@@ -357,18 +419,19 @@
             plt.plot(abs(self.get_np(self.C11)).flatten(), color=color, label=r'%s $C_{11}$' % (name), lw=lw)
         else:
             plt.plot(abs(self.get_np(self.C11)).flatten(), color=color, lw=lw)
         plt.yscale('log')
         plt.legend()
 
     def get_np(self, x):
-        if isinstance(x, np.ndarray):
-            return x
-        else:
-            return x.numpy()
+        if x is not None:
+            if isinstance(x, np.ndarray):
+                return x
+            else:
+                return x.numpy()
         
     def save(self, filename):
         if self.S1 is not None:  # Auto
             np.save('%s_s1.npy' % filename, self.get_np(self.get_S1()))
         if self.C10 is not None:  # Cross
             np.save('%s_c10.npy' % filename, self.get_np(self.get_C10()))
         np.save('%s_c01.npy' % filename, self.get_np(self.get_C01()))
@@ -920,15 +983,15 @@
                 nside_j3 = nside_j3 // 2
 
         ### Store P1_dic and P2_dic in self
         if (norm == 'auto') and (self.P1_dic is None):
             self.P1_dic = P1_dic
             if cross:
                 self.P2_dic = P2_dic
-
+            
         if not cross:
             return scat_cov(P00, C01, C11, s1=S1,backend=self.backend)
         else:
             return scat_cov(P00, C01, C11, c10=C10,backend=self.backend)
 
     def clean_norm(self):
         self.P1_dic = None
@@ -1010,22 +1073,22 @@
                                 s1=self.backend.bk_sqrt(self.backend.bk_abs(x.S1)),backend=self.backend)
         else:
             return self.backend.bk_abs(self.backend.bk_sqrt(x))
 
     def reduce_mean(self, x):
         if isinstance(x, scat_cov):
             if x.S1 is None:
-                result = (self.backend.bk_reduce_mean(x.P00) + \
-                         self.backend.bk_reduce_mean(x.C01) + \
-                         self.backend.bk_reduce_mean(x.C11))/3
-            else:
-                result = (self.backend.bk_reduce_mean(x.P00) + \
-                         self.backend.bk_reduce_mean(x.S1) + \
-                         self.backend.bk_reduce_mean(x.C01) + \
-                         self.backend.bk_reduce_mean(x.C11))/4
+                result = (self.backend.bk_reduce_mean(self.backend.bk_abs(x.P00)) + \
+                         self.backend.bk_reduce_mean(self.backend.bk_abs(x.C01)) + \
+                          self.backend.bk_reduce_mean(self.backend.bk_abs(x.C11)))/3
+            else:
+                result = (self.backend.bk_reduce_mean(self.backend.bk_abs(x.P00)) + \
+                         self.backend.bk_reduce_mean(self.backend.bk_abs(x.S1)) + \
+                         self.backend.bk_reduce_mean(self.backend.bk_abs(x.C01)) + \
+                         self.backend.bk_reduce_mean(self.backend.bk_abs(x.C11)))/4
         else:
             return self.backend.bk_reduce_mean(x)
         return result
 
     def reduce_sum(self, x):
         
         if isinstance(x, scat_cov):
@@ -1038,14 +1101,30 @@
                          self.backend.bk_reduce_sum(x.S1) + \
                          self.backend.bk_reduce_sum(x.C01) + \
                          self.backend.bk_reduce_sum(x.C11)
         else:
             return self.backend.bk_reduce_sum(x)
         return result
 
+        
+    def ldiff(self,sig,x):
+
+                
+        if x.S1 is None:
+            return scat_cov(x.domult(sig.P00,x.P00)*x.domult(sig.P00,x.P00),
+                            x.domult(sig.C01,x.C01)*x.domult(sig.C01,x.C01),
+                            x.domult(sig.C11,x.C11)*x.domult(sig.C11,x.C11),
+                            backend=self.backend)
+        else:
+            return scat_cov(x.domult(sig.P00,x.P00)*x.domult(sig.P00,x.P00),
+                            x.domult(sig.S1,x.S1)*x.domult(sig.S1,x.S1),
+                            x.domult(sig.C01,x.C01)*x.domult(sig.C01,x.C01),
+                            x.domult(sig.C11,x.C11)*x.domult(sig.C11,x.C11),
+                            backend=self.backend)
+    
     def log(self, x):
         if isinstance(x, scat_cov):
 
             if x.S1 is None:
                 result = self.backend.bk_log(x.P00) + \
                          self.backend.bk_log(x.C01) + \
                          self.backend.bk_log(x.C11)
```

### Comparing `foscat-2.0.0/src/foscat/scat_cov_new.py` & `foscat-2.0.1/src/foscat/scat_cov_new.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.0/src/foscat.egg-info/PKG-INFO` & `foscat-2.0.1/src/foscat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.0
+Version: 2.0.1
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

