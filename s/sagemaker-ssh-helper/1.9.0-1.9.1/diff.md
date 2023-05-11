# Comparing `tmp/sagemaker-ssh-helper-1.9.0.tar.gz` & `tmp/sagemaker-ssh-helper-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-ssh-helper-1.9.0.tar", last modified: Thu Dec 22 12:37:10 2022, max compression
+gzip compressed data, was "sagemaker-ssh-helper-1.9.1.tar", last modified: Fri Jan 20 16:15:55 2023, max compression
```

## Comparing `sagemaker-ssh-helper-1.9.0.tar` & `sagemaker-ssh-helper-1.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2022-12-22 12:37:10.468853 sagemaker-ssh-helper-1.9.0/
--rw-r--r--   0 ivankh     (504) staff       (20)      925 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/LICENSE
--rw-r--r--   0 ivankh     (504) staff       (20)     1243 2022-12-22 12:37:10.468711 sagemaker-ssh-helper-1.9.0/PKG-INFO
--rw-r--r--   0 ivankh     (504) staff       (20)    31510 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/README.md
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2022-12-22 12:37:10.467762 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/
--rw-r--r--   0 ivankh     (504) staff       (20)      684 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/__init__.py
--rw-r--r--   0 ivankh     (504) staff       (20)     4749 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/deregister_old_instances_from_ssm.py
--rw-r--r--   0 ivankh     (504) staff       (20)      435 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/env.py
--rw-r--r--   0 ivankh     (504) staff       (20)     5353 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/log.py
--rw-r--r--   0 ivankh     (504) staff       (20)     2686 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/proxy.py
--rw-r--r--   0 ivankh     (504) staff       (20)     2409 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-connect-ssh-proxy
--rw-r--r--   0 ivankh     (504) staff       (20)     2370 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-helper-functions
--rw-r--r--   0 ivankh     (504) staff       (20)     1482 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-init-ssm
--rw-r--r--   0 ivankh     (504) staff       (20)      129 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-local-install-force
--rw-r--r--   0 ivankh     (504) staff       (20)     1216 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-local-ssh-ide
--rw-r--r--   0 ivankh     (504) staff       (20)      824 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-local-ssh-inference
--rw-r--r--   0 ivankh     (504) staff       (20)      822 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-local-ssh-processing
--rw-r--r--   0 ivankh     (504) staff       (20)      818 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-local-ssh-training
--rw-r--r--   0 ivankh     (504) staff       (20)      822 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-local-ssh-transform
--rwxr-xr-x   0 ivankh     (504) staff       (20)      701 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-local-start-ssh
--rw-r--r--   0 ivankh     (504) staff       (20)      301 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-save-env
--rw-r--r--   0 ivankh     (504) staff       (20)     1137 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-setup-ssh
--rw-r--r--   0 ivankh     (504) staff       (20)     5458 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-ssh-ide
--rw-r--r--   0 ivankh     (504) staff       (20)     1372 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-start-ssh
--rw-r--r--   0 ivankh     (504) staff       (20)      679 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-wait
--rw-r--r--   0 ivankh     (504) staff       (20)    13630 2022-12-22 12:12:19.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/wrapper.py
-drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2022-12-22 12:37:10.468528 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper.egg-info/
--rw-r--r--   0 ivankh     (504) staff       (20)     1243 2022-12-22 12:37:10.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper.egg-info/PKG-INFO
--rw-r--r--   0 ivankh     (504) staff       (20)     1030 2022-12-22 12:37:10.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper.egg-info/SOURCES.txt
--rw-r--r--   0 ivankh     (504) staff       (20)        1 2022-12-22 12:37:10.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper.egg-info/dependency_links.txt
--rw-r--r--   0 ivankh     (504) staff       (20)      222 2022-12-22 12:37:10.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper.egg-info/requires.txt
--rw-r--r--   0 ivankh     (504) staff       (20)       21 2022-12-22 12:37:10.000000 sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper.egg-info/top_level.txt
--rw-r--r--   0 ivankh     (504) staff       (20)       38 2022-12-22 12:37:10.468896 sagemaker-ssh-helper-1.9.0/setup.cfg
--rw-r--r--   0 ivankh     (504) staff       (20)     2830 2022-12-22 12:21:49.000000 sagemaker-ssh-helper-1.9.0/setup.py
+drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-01-20 16:15:55.586350 sagemaker-ssh-helper-1.9.1/
+-rw-r--r--   0 ivankh     (504) staff       (20)      925 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/LICENSE
+-rw-r--r--   0 ivankh     (504) staff       (20)     1270 2023-01-20 16:15:55.586144 sagemaker-ssh-helper-1.9.1/PKG-INFO
+-rw-r--r--   0 ivankh     (504) staff       (20)    33322 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/README.md
+drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-01-20 16:15:55.584808 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/
+-rw-r--r--   0 ivankh     (504) staff       (20)      684 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/__init__.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     4749 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/deregister_old_instances_from_ssm.py
+-rw-r--r--   0 ivankh     (504) staff       (20)      435 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/env.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     5500 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/log.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     4143 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/proxy.py
+-rw-r--r--   0 ivankh     (504) staff       (20)     2409 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-connect-ssh-proxy
+-rw-r--r--   0 ivankh     (504) staff       (20)     2370 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-helper-functions
+-rw-r--r--   0 ivankh     (504) staff       (20)     1482 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-init-ssm
+-rw-r--r--   0 ivankh     (504) staff       (20)      129 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-install-force
+-rw-r--r--   0 ivankh     (504) staff       (20)     1297 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-ide
+-rw-r--r--   0 ivankh     (504) staff       (20)      881 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-inference
+-rw-r--r--   0 ivankh     (504) staff       (20)      879 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-processing
+-rw-r--r--   0 ivankh     (504) staff       (20)      875 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-training
+-rw-r--r--   0 ivankh     (504) staff       (20)      879 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-transform
+-rwxr-xr-x   0 ivankh     (504) staff       (20)      701 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-start-ssh
+-rw-r--r--   0 ivankh     (504) staff       (20)      301 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-save-env
+-rw-r--r--   0 ivankh     (504) staff       (20)     1137 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-setup-ssh
+-rw-r--r--   0 ivankh     (504) staff       (20)     5612 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-ssh-ide
+-rw-r--r--   0 ivankh     (504) staff       (20)     1372 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-start-ssh
+-rw-r--r--   0 ivankh     (504) staff       (20)      672 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-wait
+-rw-r--r--   0 ivankh     (504) staff       (20)    14088 2023-01-19 18:44:02.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/wrapper.py
+drwxr-xr-x   0 ivankh     (504) staff       (20)        0 2023-01-20 16:15:55.585869 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/
+-rw-r--r--   0 ivankh     (504) staff       (20)     1270 2023-01-20 16:15:55.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/PKG-INFO
+-rw-r--r--   0 ivankh     (504) staff       (20)     1030 2023-01-20 16:15:55.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 ivankh     (504) staff       (20)        1 2023-01-20 16:15:55.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 ivankh     (504) staff       (20)      274 2023-01-20 16:15:55.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/requires.txt
+-rw-r--r--   0 ivankh     (504) staff       (20)       21 2023-01-20 16:15:55.000000 sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/top_level.txt
+-rw-r--r--   0 ivankh     (504) staff       (20)       38 2023-01-20 16:15:55.586412 sagemaker-ssh-helper-1.9.1/setup.cfg
+-rw-r--r--   0 ivankh     (504) staff       (20)     2916 2023-01-20 16:15:34.000000 sagemaker-ssh-helper-1.9.1/setup.py
```

### Comparing `sagemaker-ssh-helper-1.9.0/LICENSE` & `sagemaker-ssh-helper-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-1.9.0/PKG-INFO` & `sagemaker-ssh-helper-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-ssh-helper
-Version: 1.9.0
+Version: 1.9.1
 Summary: A helper library to connect into Amazon SageMaker with AWS Systems Manager and SSH
 Home-page: https://github.com/aws-samples/sagemaker-ssh-helper
 Author: Amazon Web Services
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
@@ -13,12 +13,13 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: test-macos
 License-File: LICENSE
 
 SageMaker SSH Helper is a library that helps you to securely connect to Amazon SageMaker's training jobs, processing jobs, realtime inference endpoints, and SageMaker Studio notebook containers for fast interactive experimentation, remote debugging, and advanced troubleshooting.
 
 For the full description see [README.md](https://github.com/aws-samples/sagemaker-ssh-helper/blob/main/README.md).
```

### Comparing `sagemaker-ssh-helper-1.9.0/README.md` & `sagemaker-ssh-helper-1.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/sagemaker-ssh-helper.svg)](https://pypi.python.org/pypi/sagemaker-ssh-helper)
 [![License](https://img.shields.io/github/license/aws-samples/sagemaker-ssh-helper.svg)](https://github.com/aws-samples/sagemaker-ssh-helper/blob/main/LICENSE)
 
 SageMaker SSH Helper is a library that helps you to securely connect to Amazon SageMaker's training jobs, processing jobs, 
 realtime inference endpoints, and SageMaker Studio notebook containers for fast interactive experimentation, 
 remote debugging, and advanced troubleshooting.
 
-The two most common scenarios for the library are:
+The two most common scenarios for the library, also known as "SSH into SageMaker", are:
 1. Open a terminal session into a container running in SageMaker to diagnose a stuck training job, use CLI commands 
 like nvidia-smi, or iteratively fix and re-execute your training script within seconds. 
 2. Remote debug a code running in SageMaker from your local favorite IDE like 
 PyCharm Professional Edition or Visual Studio Code.
 
 Other scenarios include but not limited to connecting to a remote Jupyter Notebook in SageMaker Studio from your IDE, connect with your browser to a TensorBoard process running in the cloud, or start a VNC session to SageMaker Studio to run GUI apps.  
 
 Also see our [Frequently Asked Questions](FAQ.md), especially if you're using Windows on your local machine.
 
 ## How it works
 SageMaker SSH helper uses AWS Systems Manager (SSM) Session Manager, to register the SageMaker container in SSM, followed 
-by creating an SSM session between your client machine and the SageMaker container. You can then create an SSH connection 
+by creating an SSM session between your client machine and the SageMaker container. Then you can SSH into SageMaker by creating an SSH connection 
 on top of the SSM session, that allows opening a Linux shell, and/or configuring bidirectional SSH port forwarding to 
 enable applications like remote development/debugging/desktop, and others.
 
 ![Screenshot](images/layers.png)
 
 See detailed architecture diagrams of the complete flow of participating components 
 in [Training Diagram](Flows.md), and [IDE integration with SageMaker Studio diagram](Flows_IDE.md).
@@ -56,14 +56,16 @@
 
 ## <a name="training"></a>Connecting to SageMaker training jobs with SSM
 
 [![Download Demo (.mov)](https://user-images.githubusercontent.com/87804596/205893540-d7a08259-94b3-48f2-b96e-93798b98a06c.png)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Shell-To-Training-Jobs.mov)
 [Download Demo (.mov)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Shell-To-Training-Jobs.mov)
 
 ### Step 1: Install the library
+Before starting the whole procedure, check that both `pip` and `python` commands point to Python version 3.7 or higher with `python --version` command. 
+
 Install the latest stable version of library from the [PyPI repository](https://pypi.org/project/sagemaker-ssh-helper/):
 
 ```shell
 pip install sagemaker-ssh-helper
 ```
 
 ### Step 2: Modify your start training job code
@@ -107,15 +109,16 @@
 If you want to connect to SSH to other nodes, you can log in to either of these nodes, e.g., `algo-1`,
 and then SSH from this node to any other node of the training cluster, e.g., `algo-4`, without running SSH Helper 
 on these nodes.
 
 Alternatively, pass the additional parameter `ssh_instance_count` with the desired instance count 
 to `SSHEstimatorWrapper.create()`.
 
-*Note:* if you a/ don't use script mode, b/ use basic `Estimator` class and c/ all code is already stored in your Docker container, check the code sample in the corresponding section of the [FAQ.md](FAQ.md#what-if-i-want-to-train-and-deploy-a-model-as-a-simple-estimator-in-my-own-container-without-passing-entry_point-and-source_dir).
+*Note:* if you a/ don't use script mode, b/ use basic `Estimator` class and c/ all code is already stored in your Docker container, check the code sample in [the corresponding section of the FAQ](FAQ.md#what-if-i-want-to-train-and-deploy-a-model-as-a-simple-estimator-in-my-own-container-without-passing-entry_point-and-source_dir).
+
 
 ### Step 3: Modify your training script
 Add into your `train.py` the following lines at the top:
 
 ```python
 import sagemaker_ssh_helper
 sagemaker_ssh_helper.setup_and_start_ssh()
@@ -196,14 +199,17 @@
 6. Show Python high-level thread dump:  
 `py-bt`  
 7. It might also be useful to observe what system calls the process is making:
 `apt-get install strace`
 8. Trace the process (replace 361 with your pid):  
 `sudo strace -p 361`
 
+#### <a name="cli-commands"></a>Tip: Pipeline automation
+If you're looking for the full automation of the pipeline with SSM and SSH, and not only with `get_instance_ids()` method, take a look at the [automation question in the FAQ](FAQ.md#how-do-i-automate-my-pipeline-with-sagemaker-ssh-helper-end-to-end).
+
 ## <a name="inference"></a>Connecting to SageMaker inference endpoints with SSM
 
 Adding SageMaker SSH Helper to inference endpoint is similar to training with the following differences.
 
 1. Wrap your model into `SSHModelWrapper` before calling `deploy()` and add SSH Helper to `dependencies`:
 
 ```python
@@ -450,14 +456,16 @@
 ```shell
 sm-local-ssh-training connect <<training_job_name>>
 ```
 It will reverse-forward the remote debugger port `12345` to your local machine's Debug Server port.
 The local port `11022` will be connected to the remote SSH server port, 
 to allow you easily connect with SSH from command line.  
 
+> *Note:* Before running this command make sure that AWS CLI is configured to access the account with `aws s3 ls` and your default region is set with `aws configure` command. Your Python's `<path-to-venv>/bin/` directory should be in the `$PATH`, otherwise you will get a *"command not found"* error.
+
 *Tip:* If you want to connect processing, batch transform jor or to an inference endpoint with SSH, use
 `sm-local-ssh-processing`, `sm-local-ssh-transform` or `sm-local-ssh-inference` scripts respectively.
 
 While this script is running, you may connect with SSH to the specified local port:
 
 ```shell
 ssh -i ~/.ssh/sagemaker-ssh-gw -p 11022 root@localhost
@@ -501,19 +509,19 @@
  * [Instructions for PyCharm](https://www.jetbrains.com/help/pycharm/remote-debugging-with-product.html#remote-interpreter)
  * [Instructions for VSCode](https://code.visualstudio.com/docs/remote/ssh)
 
 Note, that after you finished the waiting loop, your training script will run only once, and you will be able 
 to execute additional code only while your script is running.
 Once the script finishes, you will need to submit another training job and repeat the procedure again.
 
-But there's a useful trick: submit a dummy script with the infinite loop, and while this loop will be running, you can 
+But there's a useful trick: submit a dummy script `train_placeholder.py` with the infinite loop, and while this loop will be running, you can 
 run your real training script again and again with the remote interpreter.
 Setting `max_run` parameter of the estimator is highly recommended in this case.
 
-A dummy script `train_placeholder.py` may look like this:
+The dummy script may look like this:
 
 ```python
 import time
 
 import sagemaker_ssh_helper
 sagemaker_ssh_helper.setup_and_start_ssh()
 
@@ -527,15 +535,15 @@
 ## <a name="studio"></a>Local IDE integration with SageMaker Studio over SSH for PyCharm / VSCode
 
 [![Download Demo (.mov)](https://user-images.githubusercontent.com/87804596/205895890-e5e87f8b-1ca6-4ce6-bac1-5cb6e6f61dde.png)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Remote-IDE.mov)
 [Download Demo (.mov)](https://aws-blogs-artifacts-public.s3.amazonaws.com/artifacts/ML-4988/SSH_Helper-Remote-IDE.mov)
 
 Follow the next steps for your local IDE integration with SageMaker Studio:
 
-1. Inside SageMaker Studio checkout (unpack) this repo and run [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb).
+1. Copy [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb) into SageMaker Studio and run it.
 
 *Tip:* Alternatively, attach to a domain the KernelGateway lifecycle config script [kernel-lc-config.sh](kernel-lc-config.sh) 
 (you may need to ask your administrator to do this).
 Once configured, from the Launcher choose the environment, puck up the lifecycle script and choose 
 'Open image terminal' (so, you don't even need to create a notebook).
 
 2. On the local machine, make sure that the latest AWS CLI **v2** is installed (v1 won't work), as described in 
@@ -556,43 +564,50 @@
 or from the image terminal as a `hostname` output, or you can find it in the list of running apps in AWS Console under Amazon SageMaker -> Control Panel -> User Details.
 It looks like this: `datascience-1-0-ml-g4dn-xlarge-1234567890abcdef0`.
 
 The local port `10022` will be connected to the remote SSH server port, to let you connect with SSH from IDE.  
 In addition, the local port `8889` will be connected to remote Jupyter notebook port, the port `5901` to the remote VNC server 
 and optionally the remote port `443` will be connected to your local PyCharm license server address.
 
+> *Note:* Before running this command make sure that AWS CLI is configured to access the account with `aws s3 ls` and your default region is set with `aws configure` command. Your Python's `<path-to-venv>/bin/` directory should be in the `$PATH`, otherwise you will get a *"command not found"* error.
+
 Feel free to use the script as a template. Clone and customize it, if you want to change the ports and hosts.
 
 6. Connect local PyCharm or VSCode with remote Python interpreter by using `root@localhost:10022` as SSH parameters.
 Also provide `~/.ssh/sagemaker-ssh-gw` as the private key.
 
 > *Note:* The SSH key is automatically generated on your local machine every time 
 > when you run `sm-local-ssh-ide` command from step 5.
 
  * [Instructions for SSH in PyCharm](https://www.jetbrains.com/help/pycharm/remote-debugging-with-product.html#remote-interpreter)
  * [Instructions for SSH in VSCode](https://code.visualstudio.com/docs/remote/ssh)
 
-You can check that connection is working by running the SSH command in command line:
+*Tip (PyCharm):* When you configure Python interpreter in PyCharm, it's recommended to configure the path mapping (*"Sync folders"* deployment option) for you project to point into `/root/project_name` instead of default `/tmp/pycharm_project_123`. This is how you will be able to see your project in SageMaker Studio and PyCharm will automatically sync your local dir to the remote dir. 
+
+*Tip (PyCharm):* Also instead of creating a new venv, point the Python interpreter to the existing location. 
+You can find this location by running a cell with `import sys; sys.executable` command in a SageMaker Studio notebook. You will get something like `/opt/conda/bin/python`.
+
+Now with PyCharm or VSCode you can run and debug the code remotely inside the kernel gateway app.
+
+You can also check from your local machine that connection is working by running the SSH command in command line:
 
 ```shell
 ssh -i ~/.ssh/sagemaker-ssh-gw -p 10022 root@localhost
 ```
 
-Now with PyCharm or VSCode you can run and debug the code remotely inside the kernel gateway app.
-
-*Tip:* If you don't want `ssh` command to complain about remote host keys, when you switch to a different node,
+If you don't want this `ssh` command to complain about remote host keys, when you switch to a different node,
 consider adding this two options to the command: `-o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null`.
 
-Moreover, you may now configure a remote Jupyter Server as 
+You may now configure a remote Jupyter Server as 
 http://127.0.0.1:8889/?token=<<your_token>>. You will find the full URL with remote token in 
 the [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb) notebook in the output after running the cell
 with `sm-ssh-ide start` command. 
 
- * [Instructions for remote notebooks in PyCharm](https://www.jetbrains.com/help/pycharm/configuring-jupyter-notebook.html#configure-server)
- * [Instructions for remote notebooks in VSCode](https://code.visualstudio.com/docs/datascience/jupyter-notebooks#_connect-to-a-remote-jupyter-server) (don't forget to switch kernel to remote after configuring the remote server).
+ * [Instructions for remote Jupyter notebooks in PyCharm](https://www.jetbrains.com/help/pycharm/configuring-jupyter-notebook.html#configure-server)
+ * [Instructions for remote Jupyter notebooks in VSCode](https://code.visualstudio.com/docs/datascience/jupyter-notebooks#_connect-to-a-remote-jupyter-server) (don't forget to switch kernel to remote after configuring the remote server).
 
 You can also start the VNC session to [vnc://localhost:5901](vnc://localhost:5901) (e.g. on macOS with Screen Sharing app)
 and run IDE or any other GUI app on the remote desktop instead of your local machine.
 
 7. If you want to switch to another [kernel](https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-run-and-manage-change-image.html) 
 or [instance](https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-run-and-manage-switch-instance-type.html), feel free to do so from SageMaker Studio UI and re-run
 [SageMaker_SSH_IDE.ipynb](SageMaker_SSH_IDE.ipynb).
```

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/__init__.py` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/deregister_old_instances_from_ssm.py` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/deregister_old_instances_from_ssm.py`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/log.py` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import boto3
 
 
 class SSHLog:
     logger = logging.getLogger('sagemaker-ssh-helper')
 
+    def __init__(self, region_name=None) -> None:
+        super().__init__()
+        self.region_name = region_name
+
     def get_ip_addresses(self, training_job_name, retry=0):
         SSHLog.logger.info(f"Querying SSH IP addresses for job {training_job_name}")
         query = "fields @timestamp, @logStream, @message" \
                 f"| filter @logStream like '{training_job_name}'" \
                 "| filter @message like /SSH Helper Log IP: [0-9]+/" \
                 "| sort @timestamp desc" \
                 "| limit 20"
@@ -93,15 +97,15 @@
             mi_ids = self.get_ssm_instance_ids_once(log_group, stream_name)
             redo_attempts -= 1
 
         SSHLog.logger.info(f"Got final SSM instance IDs: {mi_ids}")
         return mi_ids
 
     def _query_log_group(self, log_group, query):
-        boto_client = boto3.client('logs')
+        boto_client = boto3.client('logs', region_name=self.region_name)
         start_query_response = boto_client.start_query(
             logGroupName=log_group,
             startTime=int((datetime.now() - timedelta(weeks=2)).timestamp()),
             endTime=int(datetime.now().timestamp()),
             queryString=query
         )
         query_id = start_query_response['queryId']
```

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-connect-ssh-proxy` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-connect-ssh-proxy`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-helper-functions` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-helper-functions`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-init-ssm` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-init-ssm`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-local-ssh-ide` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-ide`

 * *Files 8% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 
 SM_STUDIO_KGW_NAME="$1"
 
 echo "Querying SSM instance ID for kernel gateway $SM_STUDIO_KGW_NAME"
 
 INSTANCE_ID=$(python <<EOF
 import sagemaker; from sagemaker_ssh_helper.log import SSHLog;
+import logging; logging.basicConfig(level=logging.INFO);
 print(SSHLog().get_studio_kgw_ssm_instance_ids("$SM_STUDIO_KGW_NAME", retry=30)[0])
 EOF
 )
 
 # replace with your JetBrains License Server host, or leave it as is if you don't use one
 JB_LICENSE_SERVER_HOST="jetbrains-license-server.example.com"
 
 if [ -f ~/.sm-jb-license-server ]; then
     # TODO: extract duplicating logic from sm-ssh-ide
     echo "sm-local-ssh-ide: ~/.sm-jb-license-server file with PyCharm license server host is already configured, skipping override"
     JB_LICENSE_SERVER_HOST="$(cat ~/.sm-jb-license-server)"
 else
-    echo "sm-local-ssh-ide: Configuring PyCharm License server host"
+    echo "sm-local-ssh-ide: Saving PyCharm License server host into ~/.sm-jb-license-server"
     echo "$JB_LICENSE_SERVER_HOST" > ~/.sm-jb-license-server
 fi
 
 
 sm-local-start-ssh "$INSTANCE_ID" \
     -L localhost:10022:localhost:22 \
     -L localhost:5901:localhost:5901 \
```

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-local-ssh-inference` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-inference`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 COMMAND=$1
 
 if [[ "$COMMAND" == "connect" ]]; then
   ENDPOINT_NAME=$2
 
   INSTANCE_ID=$(python <<EOF
 import sagemaker; from sagemaker_ssh_helper.log import SSHLog;
+import logging; logging.basicConfig(level=logging.INFO);
 print(SSHLog().get_endpoint_ssm_instance_ids("$ENDPOINT_NAME", retry=30)[0])
 EOF
   )
 
   sm-local-start-ssh "$INSTANCE_ID" \
       -R localhost:12345:localhost:12345 \
       -L localhost:11022:localhost:22
```

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-local-ssh-processing` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-processing`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 COMMAND=$1
 
 if [[ "$COMMAND" == "connect" ]]; then
   JOB_NAME=$2
 
   INSTANCE_ID=$(python <<EOF
 import sagemaker; from sagemaker_ssh_helper.log import SSHLog;
+import logging; logging.basicConfig(level=logging.INFO);
 print(SSHLog().get_processing_ssm_instance_ids("$JOB_NAME", retry=30)[0])
 EOF
   )
 
   sm-local-start-ssh "$INSTANCE_ID" \
       -R localhost:12345:localhost:12345 \
       -L localhost:11022:localhost:22
```

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-local-ssh-training` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-transform`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/bin/bash
 
 # Commands:
-# connect <training_job_name>
+# connect <transform_job_name>
 # stop-waiting
 # run-command <command> <args...>
 
 COMMAND=$1
 
 if [[ "$COMMAND" == "connect" ]]; then
   JOB_NAME=$2
 
   INSTANCE_ID=$(python <<EOF
 import sagemaker; from sagemaker_ssh_helper.log import SSHLog;
-print(SSHLog().get_training_ssm_instance_ids("$JOB_NAME", retry=30)[0])
+import logging; logging.basicConfig(level=logging.INFO);
+print(SSHLog().get_transformer_ssm_instance_ids("$JOB_NAME", retry=30)[0])
 EOF
   )
 
   sm-local-start-ssh "$INSTANCE_ID" \
       -R localhost:12345:localhost:12345 \
       -L localhost:11022:localhost:22
```

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-local-ssh-transform` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-ssh-training`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/bin/bash
 
 # Commands:
-# connect <transform_job_name>
+# connect <training_job_name>
 # stop-waiting
 # run-command <command> <args...>
 
 COMMAND=$1
 
 if [[ "$COMMAND" == "connect" ]]; then
   JOB_NAME=$2
 
   INSTANCE_ID=$(python <<EOF
 import sagemaker; from sagemaker_ssh_helper.log import SSHLog;
-print(SSHLog().get_transformer_ssm_instance_ids("$JOB_NAME", retry=30)[0])
+import logging; logging.basicConfig(level=logging.INFO);
+print(SSHLog().get_training_ssm_instance_ids("$JOB_NAME", retry=30)[0])
 EOF
   )
 
   sm-local-start-ssh "$INSTANCE_ID" \
       -R localhost:12345:localhost:12345 \
       -L localhost:11022:localhost:22
```

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-local-start-ssh` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-local-start-ssh`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-setup-ssh` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-setup-ssh`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-ssh-ide` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-ssh-ide`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     
     if grep -q 'Ubuntu 16' /etc/issue; then
         apt-get -qq -y install tightvncserver
     else
         apt-get -qq -y install tigervnc-standalone-server
     fi
 
-    apt-get -qq -y install ssh curl net-tools jq curl
+    apt-get -qq -y install ssh curl net-tools procps less jq curl vim rsync
     
     _install_aws_cli
     _install_ssm_agent_ubuntu
     
     echo "startxfce4" > ~/.xsession
     chmod +x ~/.xsession
 
@@ -67,50 +67,50 @@
 elif [[ "$1" == "set-jb-license-server" ]]; then
 
     JB_LICENSE_SERVER_HOST="$2"
     
     if [ -f ~/.sm-jb-license-server ]; then
         echo "sm-ssh-ide: PyCharm license server host is already configured in ~/.sm-jb-license-server, skipping override"
     else
-        echo "sm-ssh-ide: Configuring PyCharm License server host"
+        echo "sm-ssh-ide: Saving PyCharm License server host into ~/.sm-jb-license-server"
         echo "$JB_LICENSE_SERVER_HOST" > ~/.sm-jb-license-server
     fi
 
     JB_LICENSE_SERVER_HOST="$(cat ~/.sm-jb-license-server)"
 
     if grep -q "$JB_LICENSE_SERVER_HOST" /etc/hosts; then
         echo "sm-ssh-ide: Skipping the update of /etc/hosts with PyCharm license server (already there)"
     else
-        echo "sm-ssh-ide: Updating /etc/hosts with PyCharm license server"
+        echo "sm-ssh-ide: Updating /etc/hosts with PyCharm license server from ~/.sm-jb-license-server"
         echo "127.0.0.1  $JB_LICENSE_SERVER_HOST" >> /etc/hosts
     fi
 
 elif [[ "$1" == "set-vnc-password" ]]; then
 
     VNC_PASSWORD="$2"
 
     if [ -f ~/.vnc/passwd ]; then
-        echo "sm-ssh-ide: VNC password is already set, skipping override"
+        echo "sm-ssh-ide: VNC password is already set in ~/.vnc/passwd, skipping override"
     else
-        echo "sm-ssh-ide: Configuring VNC password"
+        echo "sm-ssh-ide: Encrypting and saving VNC password to ~/.vnc/passwd"
         mkdir -p ~/.vnc
         echo "$VNC_PASSWORD" | vncpasswd -f > ~/.vnc/passwd
         chmod 600 ~/.vnc/passwd
     fi
 
 elif [[ "$1" == "init-ssm" ]]; then
     echo "sm-ssh-ide: Using SageMaker Studio Python: $SM_STUDIO_PYTHON"
 
     LOCAL_USER_ID="$2"
 
     if [ -f ~/.sm-ssh-owner ]; then
-        echo "sm-ssh-ide: SSH owner user ID is already set, skipping override"
+        echo "sm-ssh-ide: SSH owner user ID is already set in ~/.sm-ssh-owner, skipping override"
         LOCAL_USER_ID="$(cat ~/.sm-ssh-owner)"
     else
-        echo "sm-ssh-ide: Configuring SSH owner user ID"
+        echo "sm-ssh-ide: Saving SSH owner user ID into ~/.sm-ssh-owner"
         echo "$LOCAL_USER_ID" > ~/.sm-ssh-owner
     fi
 
 
     SSH_SSM_ROLE=$($SM_STUDIO_PYTHON <<EOF
 import sagemaker; from sagemaker_ssh_helper.wrapper import SSHEnvironmentWrapper;
 print(SSHEnvironmentWrapper.ssm_role_from_iam_arn(sagemaker.get_execution_role()))
```

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-start-ssh` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-start-ssh`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/sm-wait` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/sm-wait`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     exit
 }
 
 trap terminate SIGTERM
 trap terminate SIGINT
 
 echo "sm-wait: Waiting for $SLEEP seconds to let you prepare you connection. "\
-  "Once you're ready, run 'pkill sm-wait' inside the container or 'sm-local-ssh-training stop-waiting' "\
+  "Once you're ready, run 'pkill sm-wait' inside the container or 'sm-local-ssh-* stop-waiting' "\
   "from your local machine."
 
 for loop in $(seq 1 1 "$SLEEP") 
 do
     sleep 1
     echo "sm-wait: Still waiting ($loop)..."
 done
```

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper/wrapper.py` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper/wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,25 +24,27 @@
     logger = logging.getLogger('sagemaker-ssh-helper')
     ssh_log = None
     augmented = False
 
     def __init__(self,
                  ssm_iam_role: str,
                  bootstrap_on_start: bool = True,
-                 connection_wait_time_seconds: int = 600):
+                 connection_wait_time_seconds: int = 600,
+                 sagemaker_session: sagemaker.Session = None):
         f"""
         :param ssm_iam_role: the SSM role without prefix, e.g. 'service-role/SageMakerRole'
             See https://docs.aws.amazon.com/systems-manager/latest/userguide/sysman-managed-instance-activation.html .
 
         :param bootstrap_on_start: Kick-off connection procedure upon sagemaker_ssh_helper.setup_and_start_ssh() .
 
         :param connection_wait_time_seconds: How long to wait before a SageMaker entry point.
             Can be 0 (don't wait).
         """
-        self.ssh_log = SSHLog()
+        self.sagemaker_session = sagemaker_session or sagemaker.Session()
+        self.ssh_log = SSHLog(region_name=self.sagemaker_session.boto_region_name)
 
         if ssm_iam_role != '':
             if ssm_iam_role.startswith("arn:aws:iam::"):
                 raise ValueError("ssm_iam_role should be only the part after role/, not ARN")
 
         self.ssm_iam_role = ssm_iam_role
         self.bootstrap_on_start = bootstrap_on_start
@@ -85,41 +87,42 @@
         f"""
         :param retry: how many retries (each retry is 10 seconds), 360 is for 1 hour
         """
         pass
 
     def start_ssm_connection_and_continue(self, ssh_listen_port: int, retry: int = 360,
                                           extra_args: str = ""):
-        p = self.start_ssm_connection(ssh_listen_port, retry, extra_args)
-        p.terminate()
+        proxy = self.start_ssm_connection(ssh_listen_port, retry, extra_args)
+        proxy.disconnect()
 
     def start_ssm_connection(self, ssh_listen_port: int, retry: int = 360,
-                             extra_args: str = ""):
+                             extra_args: str = "") -> SSMProxy:
         instance_ids = self.get_instance_ids(retry)
         if not instance_ids:
             raise ValueError("instance_ids cannot be empty")
 
         instance_id = instance_ids[0]
         if "mi-" not in instance_id:
             raise ValueError(f"instance_id doesn't start with 'mi-': {instance_id}")
 
-        ssm_proxy = SSMProxy(ssh_listen_port, extra_args)
-        p = ssm_proxy.connect_to_ssm_instance(instance_id)
+        ssm_proxy = SSMProxy(ssh_listen_port, extra_args, self.sagemaker_session.boto_region_name)
+        ssm_proxy.connect_to_ssm_instance(instance_id)
 
         if self.connection_wait_time_seconds > 0:
             ssm_proxy.terminate_waiting_loop()
 
-        return p
+        return ssm_proxy
 
 
 class SSHEstimatorWrapper(SSHEnvironmentWrapper):
     def __init__(self, estimator: sagemaker.estimator.EstimatorBase, ssm_iam_role: str = '',
                  bootstrap_on_start: bool = True, connection_wait_time_seconds: int = 600,
                  ssh_instance_count: int = 2):
-        super().__init__(ssm_iam_role, bootstrap_on_start, connection_wait_time_seconds)
+        super().__init__(ssm_iam_role, bootstrap_on_start, connection_wait_time_seconds,
+                         estimator.sagemaker_session)
 
         if estimator.instance_groups is not None:
             # TODO: add support for heterogeneous clusters
             self.logger.warning("Heterogeneous clusters are not yet supported, SSH Helper will start only on one node")
             self.ssh_instance_count = 1
         elif ssh_instance_count <= estimator.instance_count:
             self.ssh_instance_count = ssh_instance_count
@@ -164,47 +167,47 @@
 
 
 class SSHModelWrapper(SSHEnvironmentWrapper):
     def __init__(self, model: sagemaker.model.Model,
                  ssm_iam_role: str = '',
                  bootstrap_on_start: bool = True, connection_wait_time_seconds: int = 600):
         super().__init__(ssm_iam_role,
-                         bootstrap_on_start, connection_wait_time_seconds)
+                         bootstrap_on_start, connection_wait_time_seconds, model.sagemaker_session)
         if self.ssm_iam_role == '':
             self.ssm_iam_role = SSHEnvironmentWrapper.ssm_role_from_iam_arn(model.role)
         self.model = model
 
     def _augment(self):
         super()._augment()
         self.logger.info(f'Turning on SSH to endpoint for model {self.model.__class__}')
         env = self.model.env
         if env is None:
             env = {}
         self._augment_env(env)
         self.model.env = env
 
     def get_instance_ids(self, retry=360):
-        return SSHLog().get_endpoint_ssm_instance_ids(self.model.endpoint_name, retry)
+        return self.ssh_log.get_endpoint_ssm_instance_ids(self.model.endpoint_name, retry)
 
     def wait_for_endpoint(self):
-        sagemaker.Session().wait_for_endpoint(self.model.endpoint_name)
+        self.sagemaker_session.wait_for_endpoint(self.model.endpoint_name)
 
     @classmethod
     def create(cls, model: sagemaker.model.Model, connection_wait_time_seconds: int = 600):
         result = SSHModelWrapper(model, connection_wait_time_seconds=connection_wait_time_seconds)
         result._augment()
         return result
 
 
 class SSHMultiModelWrapper(SSHEnvironmentWrapper):
     def __init__(self, mdm: sagemaker.multidatamodel.MultiDataModel,
                  ssm_iam_role: str = '',
                  bootstrap_on_start: bool = True, connection_wait_time_seconds: int = 600):
         super().__init__(ssm_iam_role,
-                         bootstrap_on_start, connection_wait_time_seconds)
+                         bootstrap_on_start, connection_wait_time_seconds, mdm.sagemaker_session)
         self.mdm = mdm
         if mdm.model:
             self.model = mdm.model
             if self.ssm_iam_role == '':
                 self.ssm_iam_role = SSHEnvironmentWrapper.ssm_role_from_iam_arn(mdm.model.role)
             self.model_wrapper = SSHModelWrapper(mdm.model, self.ssm_iam_role,
                                                  bootstrap_on_start,
@@ -224,32 +227,33 @@
             env = self.mdm.env
             if env is None:
                 env = {}
             self._augment_env(env)
             self.mdm.env = env
 
     def get_instance_ids(self, retry=360):
-        return SSHLog().get_endpoint_ssm_instance_ids(self.mdm.endpoint_name, retry)
+        return self.ssh_log.get_endpoint_ssm_instance_ids(self.mdm.endpoint_name, retry)
 
     def wait_for_endpoint(self):
-        sagemaker.Session().wait_for_endpoint(self.mdm.endpoint_name)
+        self.sagemaker_session.wait_for_endpoint(self.mdm.endpoint_name)
 
     @classmethod
     def create(cls, mdm: sagemaker.multidatamodel.MultiDataModel, connection_wait_time_seconds: int = 600):
         result = SSHMultiModelWrapper(mdm, connection_wait_time_seconds=connection_wait_time_seconds)
         result._augment()
         return result
 
 
 class SSHProcessorWrapper(SSHEnvironmentWrapper):
     def __init__(self, processor: sagemaker.processing.Processor,
                  ssm_iam_role: str = '',
                  bootstrap_on_start: bool = True,
                  connection_wait_time_seconds: int = 600):
-        super().__init__(ssm_iam_role, bootstrap_on_start, connection_wait_time_seconds)
+        super().__init__(ssm_iam_role, bootstrap_on_start, connection_wait_time_seconds,
+                         processor.sagemaker_session)
         if self.ssm_iam_role == '':
             self.ssm_iam_role = SSHEnvironmentWrapper.ssm_role_from_iam_arn(processor.role)
         self.processor = processor
 
     def _augment(self):
         super()._augment()
         self.logger.info(f'Turning on SSH to processor {self.processor.__class__}')
@@ -257,15 +261,15 @@
         if env is None:
             env = {}
         self._augment_env(env)
         self.processor.env = env
 
     def get_instance_ids(self, retry=360):
         job: ProcessingJob = self.processor.latest_job
-        return SSHLog().get_processing_ssm_instance_ids(job.job_name, retry)
+        return self.ssh_log.get_processing_ssm_instance_ids(job.job_name, retry)
 
     def wait_processing_job(self):
         job: ProcessingJob = self.processor.latest_job
         job.wait()
 
     def augmented_input(self):
         f"""
@@ -290,15 +294,15 @@
         result = SSHProcessorWrapper(processor, connection_wait_time_seconds=connection_wait_time_seconds)
         result._augment()
         return result
 
 
 class SSHTransformerWrapper(SSHEnvironmentWrapper):
     def __init__(self, transformer: sagemaker.transformer.Transformer, model_wrapper: SSHModelWrapper):
-        super().__init__('', True, model_wrapper.connection_wait_time_seconds)
+        super().__init__('', True, model_wrapper.connection_wait_time_seconds, transformer.sagemaker_session)
         self.transformer = transformer
         self.model_wrapper = model_wrapper
 
     def _augment(self):
         super()._augment()
 
     def get_instance_ids(self, retry=360):
```

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper.egg-info/PKG-INFO` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-ssh-helper
-Version: 1.9.0
+Version: 1.9.1
 Summary: A helper library to connect into Amazon SageMaker with AWS Systems Manager and SSH
 Home-page: https://github.com/aws-samples/sagemaker-ssh-helper
 Author: Amazon Web Services
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT No Attribution License (MIT-0)
@@ -13,12 +13,13 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: test-macos
 License-File: LICENSE
 
 SageMaker SSH Helper is a library that helps you to securely connect to Amazon SageMaker's training jobs, processing jobs, realtime inference endpoints, and SageMaker Studio notebook containers for fast interactive experimentation, remote debugging, and advanced troubleshooting.
 
 For the full description see [README.md](https://github.com/aws-samples/sagemaker-ssh-helper/blob/main/README.md).
```

### Comparing `sagemaker-ssh-helper-1.9.0/sagemaker_ssh_helper.egg-info/SOURCES.txt` & `sagemaker-ssh-helper-1.9.1/sagemaker_ssh_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sagemaker-ssh-helper-1.9.0/setup.py` & `sagemaker-ssh-helper-1.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,23 @@
         "torch-model-archiver",
         "tox",
         "wheel",
         "build",
         "twine",
         "pydevd-pycharm~=213.6777.50",
         "scikit-learn"
+    ],
+    "test-macos": [
+        "tensorflow-macos==2.9.2",
+        "numpy==1.22.4"
     ]
 }
 setuptools.setup(
     name='sagemaker-ssh-helper',
-    version='1.9.0',
+    version='1.9.1',
     author="Amazon Web Services",
     description="A helper library to connect into Amazon SageMaker with AWS Systems Manager and SSH",
     long_description="SageMaker SSH Helper is a library that helps you to securely connect to Amazon SageMaker's "
                      "training jobs, processing jobs, realtime inference endpoints, and SageMaker Studio notebook "
                      "containers for fast interactive experimentation, remote debugging, and advanced troubleshooting."
                      "\n\n"
                      "For the full description see [README.md]"
```

