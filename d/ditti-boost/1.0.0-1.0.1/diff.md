# Comparing `tmp/ditti_boost-1.0.0.tar.gz` & `tmp/ditti_boost-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditti_boost-1.0.0.tar", max compression
+gzip compressed data, was "ditti_boost-1.0.1.tar", max compression
```

## Comparing `ditti_boost-1.0.0.tar` & `ditti_boost-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1194 2023-05-03 20:12:50.829677 ditti_boost-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-03 19:49:32.381121 ditti_boost-1.0.0/ditti_boost/__init__.py
--rw-r--r--   0        0        0      435 2023-05-03 17:21:58.585961 ditti_boost-1.0.0/ditti_boost/authentication.py
--rw-r--r--   0        0        0      988 2023-05-03 19:52:46.082357 ditti_boost-1.0.0/ditti_boost/cli.py
--rw-r--r--   0        0        0     1247 2023-05-03 20:02:40.619798 ditti_boost-1.0.0/ditti_boost/config.py
--rw-r--r--   0        0        0      565 2023-05-03 18:50:41.259970 ditti_boost-1.0.0/ditti_boost/menu.py
--rw-r--r--   0        0        0      289 2023-05-03 17:53:32.934877 ditti_boost-1.0.0/ditti_boost/reporting.py
--rw-r--r--   0        0        0     4921 2023-05-03 19:05:33.380638 ditti_boost-1.0.0/ditti_boost/scripts.py
--rw-r--r--   0        0        0      394 2023-05-03 20:11:16.237488 ditti_boost-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 ditti_boost-1.0.0/setup.py
--rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 ditti_boost-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1263 2023-05-11 01:49:23.252348 ditti_boost-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 19:49:32.381121 ditti_boost-1.0.1/ditti_boost/__init__.py
+-rw-r--r--   0        0        0      435 2023-05-03 17:21:58.585961 ditti_boost-1.0.1/ditti_boost/authentication.py
+-rw-r--r--   0        0        0      988 2023-05-03 19:52:46.082357 ditti_boost-1.0.1/ditti_boost/cli.py
+-rw-r--r--   0        0        0     1247 2023-05-10 23:54:22.057266 ditti_boost-1.0.1/ditti_boost/config.py
+-rw-r--r--   0        0        0      669 2023-05-11 01:02:29.776069 ditti_boost-1.0.1/ditti_boost/menu.py
+-rw-r--r--   0        0        0      289 2023-05-03 17:53:32.934877 ditti_boost-1.0.1/ditti_boost/reporting.py
+-rw-r--r--   0        0        0     8058 2023-05-11 01:43:50.840438 ditti_boost-1.0.1/ditti_boost/scripts.py
+-rw-r--r--   0        0        0      394 2023-05-11 00:24:05.905051 ditti_boost-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2021 1970-01-01 00:00:00.000000 ditti_boost-1.0.1/setup.py
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 ditti_boost-1.0.1/PKG-INFO
```

### Comparing `ditti_boost-1.0.0/README.md` & `ditti_boost-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,36 @@
+Metadata-Version: 2.1
+Name: ditti-boost
+Version: 1.0.1
+Summary: 
+Author: alex paden
+Author-email: padenalex0@gmail.com
+Requires-Python: >=3.9,<3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: farcaster (>=0.7.7,<0.8.0)
+Description-Content-Type: text/markdown
+
 # Ditti Boost
 
 Ditti Boost is a command-line tool that automates following and unfollowing users on Farcaster. It provides a simple way to grow your network, find new users, and manage your connections on the platform.
 
 ## Features
 
 - Follow users based on different criteria:
   - Copy a user's following
   - Follow new users
   - Follow collection owners
 - Unfollow users based on different criteria:
   - Unfollow all users
   - Unfollow non-follow back users
   - Unfollow collection owners
+  - Unfollow users with no casts
+  - Unfollow no casts within x days
 
 ## Installation
 
 _This project requires python3.10_
 
 To install Ditti Boost, run the following command:
 
@@ -40,7 +55,8 @@
 ## Contributing
 
 Contributions are welcome! If you'd like to help improve Ditti Boost, please feel free to open an issue, submit a pull request, or suggest new features.
 
 ## License
 
 Ditti Boost is licensed under the MIT License.
+
```

### Comparing `ditti_boost-1.0.0/ditti_boost/cli.py` & `ditti_boost-1.0.1/ditti_boost/cli.py`

 * *Files identical despite different names*

### Comparing `ditti_boost-1.0.0/ditti_boost/config.py` & `ditti_boost-1.0.1/ditti_boost/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 env_path = os.path.join(os.getcwd(), '.env')
 load_dotenv(dotenv_path=env_path)
 
 ACCESS_TOKEN = os.getenv('ACCESS_TOKEN')
 MNEMONIC_PHRASE = os.getenv('MNEMONIC_PHRASE')
 
 def save_credentials_to_env(access_token, mnemonic_phrase):
-    with open(env_path, 'a') as env_file:
+    with open(env_path, 'w') as env_file:
         if access_token:
             env_file.write(f"ACCESS_TOKEN={access_token}\n")
         if mnemonic_phrase:
             env_file.write(f"MNEMONIC_PHRASE={mnemonic_phrase}\n")
 
 def prompt_for_credentials():
     if ACCESS_TOKEN is None and MNEMONIC_PHRASE is None:
```

### Comparing `ditti_boost-1.0.0/ditti_boost/menu.py` & `ditti_boost-1.0.1/ditti_boost/menu.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,9 +12,11 @@
     choice = input("Enter your choice: ")
     return choice
 
 def display_unfollow_scripts():
     print("1. Unfollow all users")
     print("2. Unfollow non-follow back users")
     print("3. Unfollow collection owners")
+    print("4. Unfollow users with no casts")
+    print("5. Unfollow users not casting within (x) days")
     choice = input("Enter your choice: ")
     return choice
```

### Comparing `ditti_boost-1.0.0/ditti_boost/scripts.py` & `ditti_boost-1.0.1/ditti_boost/scripts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # scripts.py
 import logging
+import time
 from farcaster import Warpcast
 
 class FollowScript:
     def __init__(self, criteria, warpcast_client: Warpcast):
         self.criteria = criteria
         self.warpcast_client = warpcast_client
 
@@ -53,15 +54,15 @@
             self.follow_new_users(count)
         elif self.criteria == '3':
             collection_id = input("Enter the collection ID: ")
             self.follow_collection_owners(collection_id)
 
 
 class UnfollowScript:
-    def __init__(self, criteria, warpcast_client):
+    def __init__(self, criteria, warpcast_client: Warpcast):
         self.criteria = criteria
         self.warpcast_client = warpcast_client
 
     def unfollow_all_users(self):
         following = self.warpcast_client.get_all_following().users
         successful_unfollows = 0
 
@@ -98,16 +99,81 @@
         for owner in collection_owners:
             try:
                 self.warpcast_client.unfollow_user(owner.fid)
                 successful_unfollows += 1
             except Exception as e:
                 logging.warning("Failed to unfollow user: {}".format(owner.username))
         logging.info("You've successfully unfollowed the owners of collection: {}. Total unfollows: {}".format(collection_id, successful_unfollows))
+        
+    def unfollow_no_casters(self):
+        counter = 0
+        most_recent_fid = self.warpcast_client.get_recent_users(limit=1).users[0].fid
+        users = self.warpcast_client.get_all_following().users
+
+        for user in users:
+            if user.fid < most_recent_fid-500:
+                try:
+                    casts = self.warpcast_client.get_casts(user.fid).casts
+                    if len(casts) == 0:
+                        try:
+                            self.warpcast_client.unfollow_user(user.fid)
+                            logging.info("You've successfully unfollowed the user: {}".format(user.username))
+                            counter += 1
+                        except Exception as e:
+                            logging.warning("Failed to unfollow user: {}".format(user.username))
+                except Exception as e:
+                    logging.warning("Failed to get casts for user: {}".format(user.username))
+
+        logging.info("You've successfully unfollowed {} users who have never casted.".format(counter))
+        
+    def unfollow_no_recent_cast(self, days=60):
+        # Convert days to milliseconds
+        days_in_milliseconds = days * 24 * 60 * 60 * 1000
+
+        # Get the current timestamp in milliseconds
+        current_timestamp = int(time.time() * 1000)
+
+        # Calculate the cutoff timestamp
+        cutoff_timestamp = current_timestamp - days_in_milliseconds
+
+        most_recent_fid = self.warpcast_client.get_recent_users(limit=1).users[0].fid
+        users = self.warpcast_client.get_all_following().users
+        successful_unfollows = 0
+
+        for user in users:
+            if user.fid < most_recent_fid-500:
+                try:
+                    # Get the user's casts
+                    casts = self.warpcast_client.get_casts(user.fid).casts
+
+                    # If the user has no casts or the most recent cast is older than the cutoff, unfollow the user
+                    if not casts or max(cast.timestamp for cast in casts) < cutoff_timestamp:
+                        try:
+                            self.warpcast_client.unfollow_user(user.fid)
+                            successful_unfollows += 1
+                            logging.info("You've successfully unfollowed the user: {}".format(user.username))
+                        except Exception as e:
+                            logging.warning("Failed to unfollow user: {}".format(user.username))
+                except Exception as e:
+                    logging.warning("Failed to get casts for user: {}".format(user.username))
+
+        logging.info("You've successfully unfollowed {} users who have not cast within the last {} days.".format(successful_unfollows, days))
+
 
     def execute(self):
         if self.criteria == '1':
             self.unfollow_all_users()
         elif self.criteria == '2':
             self.unfollow_non_follow_back_users()
         elif self.criteria == '3':
             collection_id = input("Enter the collection ID: ")
             self.unfollow_collection_owners(collection_id)
+        elif self.criteria == '4':
+            self.unfollow_no_casters()
+        elif self.criteria == '5':
+            try:
+                days = input("Enter the maximum number of days the user must have cast within (default is 60): ")
+                days = int(days) if days else 60
+            except ValueError:
+                days = 60
+            self.unfollow_no_recent_cast(days)
+
```

### Comparing `ditti_boost-1.0.0/setup.py` & `ditti_boost-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['farcaster>=0.7.7,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['ditti-boost = ditti_boost.cli:main']}
 
 setup_kwargs = {
     'name': 'ditti-boost',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': '',
-    'long_description': "# Ditti Boost\n\nDitti Boost is a command-line tool that automates following and unfollowing users on Farcaster. It provides a simple way to grow your network, find new users, and manage your connections on the platform.\n\n## Features\n\n- Follow users based on different criteria:\n  - Copy a user's following\n  - Follow new users\n  - Follow collection owners\n- Unfollow users based on different criteria:\n  - Unfollow all users\n  - Unfollow non-follow back users\n  - Unfollow collection owners\n\n## Installation\n\n_This project requires python3.10_\n\nTo install Ditti Boost, run the following command:\n\n```\npip install ditti-boost\n\nditti-boost\n```\n\n## Usage\n\nTo use Ditti Boost, first navigate to the project directory and run the following command:\n\n```\npoetry env use 3.10\npoetry install\npoetry run python ditti_boost/cli.py\n```\n\nYou will be prompted to enter either an access token or a mnemonic phrase. Then, you can choose from various follow and unfollow options.\n\n## Contributing\n\nContributions are welcome! If you'd like to help improve Ditti Boost, please feel free to open an issue, submit a pull request, or suggest new features.\n\n## License\n\nDitti Boost is licensed under the MIT License.\n",
+    'long_description': "# Ditti Boost\n\nDitti Boost is a command-line tool that automates following and unfollowing users on Farcaster. It provides a simple way to grow your network, find new users, and manage your connections on the platform.\n\n## Features\n\n- Follow users based on different criteria:\n  - Copy a user's following\n  - Follow new users\n  - Follow collection owners\n- Unfollow users based on different criteria:\n  - Unfollow all users\n  - Unfollow non-follow back users\n  - Unfollow collection owners\n  - Unfollow users with no casts\n  - Unfollow no casts within x days\n\n## Installation\n\n_This project requires python3.10_\n\nTo install Ditti Boost, run the following command:\n\n```\npip install ditti-boost\n\nditti-boost\n```\n\n## Usage\n\nTo use Ditti Boost, first navigate to the project directory and run the following command:\n\n```\npoetry env use 3.10\npoetry install\npoetry run python ditti_boost/cli.py\n```\n\nYou will be prompted to enter either an access token or a mnemonic phrase. Then, you can choose from various follow and unfollow options.\n\n## Contributing\n\nContributions are welcome! If you'd like to help improve Ditti Boost, please feel free to open an issue, submit a pull request, or suggest new features.\n\n## License\n\nDitti Boost is licensed under the MIT License.\n",
     'author': 'alex paden',
     'author_email': 'padenalex0@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ditti_boost-1.0.0/PKG-INFO` & `ditti_boost-1.0.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,23 @@
-Metadata-Version: 2.1
-Name: ditti-boost
-Version: 1.0.0
-Summary: 
-Author: alex paden
-Author-email: padenalex0@gmail.com
-Requires-Python: >=3.9,<3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: farcaster (>=0.7.7,<0.8.0)
-Description-Content-Type: text/markdown
-
 # Ditti Boost
 
 Ditti Boost is a command-line tool that automates following and unfollowing users on Farcaster. It provides a simple way to grow your network, find new users, and manage your connections on the platform.
 
 ## Features
 
 - Follow users based on different criteria:
   - Copy a user's following
   - Follow new users
   - Follow collection owners
 - Unfollow users based on different criteria:
   - Unfollow all users
   - Unfollow non-follow back users
   - Unfollow collection owners
+  - Unfollow users with no casts
+  - Unfollow no casts within x days
 
 ## Installation
 
 _This project requires python3.10_
 
 To install Ditti Boost, run the following command:
 
@@ -53,8 +42,7 @@
 ## Contributing
 
 Contributions are welcome! If you'd like to help improve Ditti Boost, please feel free to open an issue, submit a pull request, or suggest new features.
 
 ## License
 
 Ditti Boost is licensed under the MIT License.
-
```

