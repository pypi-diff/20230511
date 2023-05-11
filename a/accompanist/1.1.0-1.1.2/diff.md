# Comparing `tmp/accompanist-1.1.0-py3-none-any.whl.zip` & `tmp/accompanist-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 42155 bytes, number of entries: 19
--rw-r--r--  2.0 unx     1423 b- defN 23-May-05 12:22 accompanist/cmd_init.py
--rw-r--r--  2.0 unx     5229 b- defN 23-May-05 08:48 accompanist/cmd_listen.py
--rw-r--r--  2.0 unx     2968 b- defN 23-May-05 06:29 accompanist/cmd_play.py
--rw-r--r--  2.0 unx      732 b- defN 23-May-04 15:46 accompanist/main.py
--rw-r--r--  2.0 unx       22 b- defN 23-May-03 12:20 accompanist/version.py
--rw-r--r--  2.0 unx     3945 b- defN 23-May-02 14:21 accompanist/report/draw_histgram.py
--rw-r--r--  2.0 unx     3593 b- defN 23-May-03 12:19 accompanist/report/draw_pie_chart.py
--rw-r--r--  2.0 unx     3375 b- defN 23-May-05 08:48 accompanist/report/draw_table.py
--rw-r--r--  2.0 unx     2907 b- defN 23-May-05 12:37 accompanist/report/utility_module.py
--rw-r--r--  2.0 unx     1419 b- defN 23-May-05 12:21 accompanist/report/write_comment.py
--rw-r--r--  2.0 unx     1317 b- defN 23-May-03 16:29 accompanist/report/write_front_cover.py
+Zip file size: 43779 bytes, number of entries: 20
+-rw-r--r--  2.0 unx     1488 b- defN 23-May-10 08:47 accompanist/cmd_init.py
+-rw-r--r--  2.0 unx     5985 b- defN 23-May-10 08:47 accompanist/cmd_listen.py
+-rw-r--r--  2.0 unx     3305 b- defN 23-May-10 11:53 accompanist/cmd_play.py
+-rw-r--r--  2.0 unx      733 b- defN 23-May-10 08:48 accompanist/main.py
+-rw-r--r--  2.0 unx      292 b- defN 23-May-10 08:47 accompanist/utility.py
+-rw-r--r--  2.0 unx       18 b- defN 23-May-11 14:46 accompanist/version.py
+-rw-r--r--  2.0 unx     3946 b- defN 23-May-10 08:49 accompanist/report/draw_histgram.py
+-rw-r--r--  2.0 unx     3593 b- defN 23-May-10 08:49 accompanist/report/draw_pie_chart.py
+-rw-r--r--  2.0 unx     3416 b- defN 23-May-11 11:10 accompanist/report/draw_table.py
+-rw-r--r--  2.0 unx     1548 b- defN 23-May-10 08:49 accompanist/report/write_comment.py
+-rw-r--r--  2.0 unx     1368 b- defN 23-May-11 14:50 accompanist/report/write_front_cover.py
+-rw-r--r--  2.0 unx     3057 b- defN 23-May-10 08:49 accompanist/report/write_header_footer.py
 -rw-r--r--  2.0 unx    19193 b- defN 23-Mar-26 08:39 accompanist/resource/logo_trans.png
 -rw-r--r--  2.0 unx     6761 b- defN 23-Mar-26 08:25 accompanist/resource/logo_trans_small.png
--rw-r--r--  2.0 unx     1063 b- defN 23-May-05 13:16 accompanist-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3477 b- defN 23-May-05 13:16 accompanist-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 13:16 accompanist-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-May-05 13:16 accompanist-1.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       31 b- defN 23-May-05 13:16 accompanist-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1645 b- defN 23-May-05 13:16 accompanist-1.1.0.dist-info/RECORD
-19 files, 59245 bytes uncompressed, 39441 bytes compressed:  33.4%
+-rw-r--r--  2.0 unx     1063 b- defN 23-May-11 14:58 accompanist-1.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5744 b- defN 23-May-11 14:58 accompanist-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 14:58 accompanist-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-May-11 14:58 accompanist-1.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       31 b- defN 23-May-11 14:58 accompanist-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1728 b- defN 23-May-11 14:58 accompanist-1.1.2.dist-info/RECORD
+20 files, 63414 bytes uncompressed, 40935 bytes compressed:  35.4%
```

## zipnote {}

```diff
@@ -6,53 +6,56 @@
 
 Filename: accompanist/cmd_play.py
 Comment: 
 
 Filename: accompanist/main.py
 Comment: 
 
+Filename: accompanist/utility.py
+Comment: 
+
 Filename: accompanist/version.py
 Comment: 
 
 Filename: accompanist/report/draw_histgram.py
 Comment: 
 
 Filename: accompanist/report/draw_pie_chart.py
 Comment: 
 
 Filename: accompanist/report/draw_table.py
 Comment: 
 
-Filename: accompanist/report/utility_module.py
-Comment: 
-
 Filename: accompanist/report/write_comment.py
 Comment: 
 
 Filename: accompanist/report/write_front_cover.py
 Comment: 
 
+Filename: accompanist/report/write_header_footer.py
+Comment: 
+
 Filename: accompanist/resource/logo_trans.png
 Comment: 
 
 Filename: accompanist/resource/logo_trans_small.png
 Comment: 
 
-Filename: accompanist-1.1.0.dist-info/LICENSE
+Filename: accompanist-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: accompanist-1.1.0.dist-info/METADATA
+Filename: accompanist-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: accompanist-1.1.0.dist-info/WHEEL
+Filename: accompanist-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: accompanist-1.1.0.dist-info/entry_points.txt
+Filename: accompanist-1.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: accompanist-1.1.0.dist-info/top_level.txt
+Filename: accompanist-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: accompanist-1.1.0.dist-info/RECORD
+Filename: accompanist-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## accompanist/cmd_init.py

```diff
@@ -1,31 +1,36 @@
-import click
 import json
 
+import click
+
+import accompanist.utility as ut
+
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
 @click.command(name="init", context_settings=CONTEXT_SETTINGS,
                help="Configure CWL log group setting.")
 @click.option("-l", "--log-group", required=True, default="aws-waf-logs-xxxxxxx", type=str,
               prompt="Please input a log group name",
               help="Set a CloudWatch Logs Log group name.")
 @click.option("-p", "--path", required=True, default="/.env", type=str,
               prompt="Please input a analysis target URI path",
               help="Set a URI path for counts that is blocked/counted.")
 @click.option("-c", "--comment", required=True,
-              default="This is a sample comment.(English and Japanese are available)", type=str,
-              prompt="Please input a comment for the report (It's editable optionally after)",
+              default="This is a sample comment.", type=str,
+              prompt="Please input a comment on the report",
               help="Set a comment for report.")
 def init(log_group, path, comment):
 
     configure_items = {
         "log_group": log_group,
         "target_uri": [path],
         "comment": [comment]
     }
 
     with open("config.json", mode="w", encoding="utf-8") as f:
         json.dump(configure_items, f, indent=2)
 
-    print("\n[Info] The configuration file \"config.json\" is generated!")
-    print("[Info] The other path names and comment can also be added optionally by editing that file. They were omitted in this automatically initialized process.\n")
+    info_config = "\n[Info] A configuration file \"config.json\" is generated!"
+    info_omitted = "[Info] The other path names and comment can also be added optionally by editing that file. They were omitted in this automatically initialized process.\n"
+    ut.colorize_print(info_config, "cyan")
+    ut.colorize_print(info_omitted, "cyan")
```

## accompanist/cmd_listen.py

```diff
@@ -1,16 +1,20 @@
-import sys
-import time
-import json
 import csv
 import datetime
+import json
+import os
+import sys
+import time
 
-import click
 import boto3
+import click
+
+import accompanist.utility as ut
 
+CONFIG_FILE = "config.json"
 SHEET_MUSIC_FILE = "sheet_music.json"
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
 @click.command(name="listen", context_settings=CONTEXT_SETTINGS,
                help="Get a WAF log file in CSV format.")
 @click.option("-a", "--action", required=True, default="BLOCK",
@@ -21,66 +25,78 @@
               prompt="Please input the number of analysis target days",
               help="Set a number of the past days until today for analysis target period.")
 @click.option("-s", "--start_time", required=False, type=int,
               help="Set a UNIX time of the oldest time for analysis target period (instead of \"--days\").")
 @click.option("-e", "--end_time", required=False, type=int,
               help="Set a UNIX time of the latest time for analysis target period (instead of \"--days\").")
 @click.option("-r", "--raw-log", required=False, is_flag=True,
-              help="Output raw log file and the excerpted log file for debug.")
+              help="Output raw log file and the excerpted log file for debugging.")
 def listen(days, start_time, end_time, action, raw_log):
 
-    with open("config.json", mode="r") as f:
-        config_dict = json.load(f)
+    if os.path.isfile(CONFIG_FILE):
+        with open(CONFIG_FILE, mode="r") as f:
+            config_dict = json.load(f)
+    else:
+        error_file = "[Error] " + CONFIG_FILE + " is not found in the ccurrent directory."
+        info_before = "[Info] You may have to run \"accompanist init\" at first."
+        ut.colorize_print(error_file, "red")
+        ut.colorize_print(info_before, "cyan")
+        sys.exit()
 
     log_group = config_dict["log_group"]
     client = boto3.client("logs")
 
     if action == "BLOCK":
         query = 'fields @timestamp, @message | filter @message like "BLOCK" | sort @timestamp desc'
     elif action == "COUNT":
         query = 'fields @timestamp, @message | filter @message like /"action":"COUNT"/ | sort @timestamp desc'
     else:
-        print("Error: action is empty or invalid")
+        error_action = "[Error] action is empty or invalid"
+        ut.colorize_text(error_action, "red")
         sys.exit()
 
     if days is not None and (start_time is None or end_time is None):
         end_time = int(time.time())
         start_time = end_time - days * 24 * 3600
     else:
         days_warning = "[Warning] The inputted number of days is ignored as the start & end times had been set."
-        print("\033[33m" + days_warning + "\033[0m")
+        ut.colorize_text(days_warning, "yellow")
 
     start_query_response = client.start_query(
         logGroupName=log_group,
         startTime=start_time,
         endTime=end_time,
         queryString=query,
         limit=10000
     )
 
     response = None
-    print("[Info] The CloudWatch Logs Insights query started.")
+    info_start = "[Info] A CloudWatch Logs Insights query started."
+    ut.colorize_print(info_start, "cyan")
 
     while response is None or response["status"] == "Running":
         time.sleep(3)
         print(" ... ... ... ")
         response = client.get_query_results(queryId=start_query_response["queryId"])
-    print("[Info] The query has been completed!")
+    info_complete = "[Info] The query has been completed!"
+    ut.colorize_print(info_complete, "cyan")
 
     if raw_log:
         with open("raw-log.json", mode="w", encoding="utf-8") as f:
             json.dump(response, f, indent=4)
         log_json = []
         for i in range(len(response["results"])):
             log_json.append(response["results"][i][1]["value"])
 
         with open("waf-log.json", mode="w", encoding="utf-8") as f:
-            f.write("[" + str(', '.join(log_json)) + "]")
+            log_str = "[" + str(', '.join(log_json)) + "]"
+            json.dump(json.loads(log_str), f, indent=2)
+
         debug_message = "[Debug] A raw log file and the excerpted log file were outputted."
-        print("\033[36m" + debug_message + "\033[0m")
+        ut.colorize_print(debug_message, "purple")
 
     with open("waf-log.csv", mode="w", encoding="utf-8") as f:
         writer = csv.writer(f, quoting=csv.QUOTE_NONE, lineterminator="\n", delimiter="\t")
 
         if action == "BLOCK":
             for i in range(len(response["results"])):
                 message = json.loads(response["results"][i][1]["value"])
@@ -97,17 +113,19 @@
                     row = str(message["timestamp"]) + "," + \
                         message["nonTerminatingMatchingRules"][j]["ruleId"] + "," + \
                         message["httpRequest"]["uri"] + "," + \
                         message["httpRequest"]["clientIp"] + "," + \
                         message["httpRequest"]["country"]
                     writer.writerow([row])
         else:
-            print("Error: action is invalid")
+            error_action = "Error: action is invalid"
+            ut.colorize_print(error_action, "red")
             sys.exit()
-    print("[Info] The WAF log file in CSV format for analysis was outputted.")
+    info_csv = "[Info] A WAF log file in CSV format was outputted."
+    ut.colorize_print(info_csv, "cyan")
 
     # Calc dates
     s_time = datetime.datetime.fromtimestamp(start_time)
     e_time = datetime.datetime.fromtimestamp(end_time)
     days = (e_time - s_time).days
 
     # Dump data for creating report
@@ -117,8 +135,9 @@
         "end_time": end_time,
         "days": days,
         "log_group": log_group,
         "action": action,
     }
     with open(SHEET_MUSIC_FILE, mode="w", encoding="utf-8") as f:
         json.dump(sheet_music, f, indent=2)
-    print("[Info] The \"sheet_music.json\" file was created for analysis.")
+    info_sheet = "[Info] A " + SHEET_MUSIC_FILE + " file was created for analysis."
+    ut.colorize_print(info_sheet, "cyan")
```

## accompanist/cmd_play.py

```diff
@@ -1,45 +1,54 @@
-import click
-import subprocess
+import os
 import random
+import subprocess
+import sys
 
-import pandas as pd
+import click
 import matplotlib.pyplot as plt
+import pandas as pd
 from matplotlib.backends.backend_pdf import PdfPages as pp
 
-import accompanist.report.write_front_cover as wf
 import accompanist.report.draw_histgram as dh
 import accompanist.report.draw_pie_chart as dp
 import accompanist.report.draw_table as dt
 import accompanist.report.write_comment as wc
-import accompanist.report.utility_module as um
+import accompanist.report.write_front_cover as wf
+import accompanist.report.write_header_footer as wh
+import accompanist.utility as ut
 
-INPUT_CSV_FILE = "./waf-log.csv"
-OUTPUT_PDF_FILE = "./report.pdf"
+INPUT_CSV_FILE = "waf-log.csv"
+OUTPUT_PDF_FILE = "report.pdf"
 A4_SIZE = (11.69, 8.27)
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
 @click.command(name="play", context_settings=CONTEXT_SETTINGS,
-               help="Analysis WAF logs and generate a report.")
+               help="Analyze WAF logs and generate a report.")
 @click.option("-c", "--colorful", required=False, is_flag=True,
               help="Set a random color of report theme (instead of color).")
 @click.option("-d", "--color", required=False, type=str,
               help="Customize a color of report theme with color code,  (e.g.) #cccccc.")
 @click.option("-m", "--mask-ip", required=False, is_flag=True,
               help="Mask IP addresses on pie chart.")
 @click.option("-u", "--utc-offset", required=False, type=int, default=9,
               help="Set a number of UTC offest. The defaut offset is UTC+9 (Asia/Tokyo).")
 @click.option("-y", "--y-limit", required=False, default="50",
               type=click.Choice(["50", "100", "500", "1000"]),
               help="Adjust a Y-axis max limitation for histograms due to many requests.")
 def play(color, colorful, mask_ip, utc_offset, y_limit):
 
     # Pre-Process
-    waf_log = pd.read_csv(INPUT_CSV_FILE, header=None)
+    if os.path.isfile(INPUT_CSV_FILE):
+        waf_log = pd.read_csv(INPUT_CSV_FILE, header=None)
+    else:
+        error_log = "[Error] A WAF log file, " + INPUT_CSV_FILE + " is not found in the current directory."
+        ut.colorize_print(error_log, "red")
+        sys.exit()
+
     waf_log.columns = ["time", "rule", "uri", "ip", "country"]
 
     plt.rcParams["font.family"] = "Arial"
 
     fig_1 = plt.figure(figsize=A4_SIZE)
     fig_2 = plt.figure(figsize=A4_SIZE)
     fig_3 = plt.figure(figsize=A4_SIZE)
@@ -52,29 +61,30 @@
     color_list = ["#154f74", "#1397ab", "#9a540f",
                   "#ffa50d", "#74bd97", "#2fcdfa", "#f595ff", "#9a5bc0", "#000000"]
 
     if color is None:
         if colorful:
             index = random.randint(0, len(color_list) - 1)
             color = color_list[index]
-            print("[Info] A theme color of the report was chosen randomly:", color)
+            info_color = "[Info] A theme color of the report was chosen randomly: " + color
+            ut.colorize_print(info_color, "cyan")
         else:
             color = "#154f74"  # Default color
 
     # Add front cover
     wf.write_front_cover(fig_1, color)
 
     # Calculation & Draw
     dh.draw_histgram(waf_log, fig_2, utc_offset, y_limit)
     dp.draw_pie_chart(waf_log, fig_3, fig_4, mask_ip)
     dt.draw_table(waf_log, fig_5)
     wc.write_comment(fig_6)
 
     # Post-Process
-    um.write_header_and_footer(waf_log["time"], figs[1:], utc_offset, color)
+    wh.write_header_and_footer(waf_log["time"], figs[1:], utc_offset, color)
 
     pdf = pp(OUTPUT_PDF_FILE)
 
     for i in figs:
         pdf.savefig(i)
 
     pdf.close()
```

## accompanist/main.py

```diff
@@ -1,8 +1,9 @@
 import click
+
 from accompanist.cmd_init import init as init_cmd
 from accompanist.cmd_listen import listen as listen_cmd
 from accompanist.cmd_play import play as play_cmd
 
 
 @click.group(help="\
         \"Accompanist\" is your accompanist on AWS WAF log analyses.               \
```

## accompanist/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.0"
+VERSION = "1.1.2"
```

## accompanist/report/draw_histgram.py

```diff
@@ -1,8 +1,9 @@
 import datetime
+
 import numpy as np
 
 
 class DrawHistgramClass:
     def __init__(self):
         self._hours = 3
         self._bins = 0
```

## accompanist/report/draw_pie_chart.py

 * *Ordering differences only*

```diff
@@ -1,9 +1,9 @@
-import pandas as pd
 import matplotlib.lines as lines
+import pandas as pd
 
 
 class CalcTop5Class:
     def __init__(self):
         self._data = []
         self._top5 = []
         self._dropped = []
```

## accompanist/report/draw_table.py

```diff
@@ -1,17 +1,20 @@
 import json
+
+import accompanist.utility as ut
 import numpy as np
 
 CONFIG_FILE = "config.json"
 
+
 def draw_table(waf_log, fig):
     """
     Draw a table
     """
-    TABLE_TITLE = "Number of Requests per Path Name"
+    TABLE_TITLE = "Requests Matched Specific Paths"
     uri_data = calc_count_of_uris(waf_log)
 
     fig.subplots_adjust(top=0.64, left=0.04, right=0.82, hspace=0)
     ax = fig.add_subplot(1, 1, 1)
     ax.axis("off")
     ax.set_title(TABLE_TITLE, loc="left", y=1.17, x=0.07, fontsize="20",
                  fontweight="bold", color="black")
@@ -87,16 +90,16 @@
         count = 0
         index = index + 1
         if index <= 12:
             if uri in waf_log["uri"].values:
                 count = waf_log.groupby("uri").get_group(uri)["uri"].count()
             counted_uris.append([index, uri, count])
         else:
-            warning = "[Warning] Some paths can't be shown because the number of paths may be exceeded."
-            print("\033[33m" + warning + "\033[0m")
+            warning_path = "[Warning] Some paths can't be shown because the number of paths may be exceeded."
+            ut.colorize_print(warning_path, "yellow")
             exit
 
     if len(uris) < 12:
         index = len(uris)
         for i in range(12 - len(uris)):
             index = index + 1
             counted_uris.append([index, "", ""])
```

## accompanist/report/write_comment.py

```diff
@@ -1,8 +1,10 @@
 import json
+
+import accompanist.utility as ut
 import matplotlib.patches as patches
 
 CONFIG_FILE = "config.json"
 JP_FONT = "YuGothic"
 
 
 def write_comment(fig):
@@ -21,18 +23,19 @@
                           linewidth=0, fill=True)
     ax.add_patch(r)
 
     comment_item = []
     for i in range(len(config_dict["comment"])):
         if i < 6:
             comment_item.append(config_dict["comment"][i])
-            y_pos = 0.9 - 0.16 * i
+            y_pos = 0.9 - 0.18 * i
             ax.text(0.02, y_pos, "-", color="black", fontsize=18,
                     va="top", ha="left", wrap=True)
-            ax.text(0.04, y_pos, comment_item[i], color="black", fontsize=18,
-                    va="top", ha="left", fontfamily=JP_FONT, wrap=True)
+            txt = ax.text(0.04, y_pos, comment_item[i], color="black", fontsize=18,
+                          va="top", ha="left", fontfamily=JP_FONT, wrap=True, linespacing=1.8)
+            txt._get_wrap_line_width = lambda: 710.0
         else:
-            warning = "[Warning] Some commnets can't be shown because the number of comments may be exceeded."
-            print("\033[33m" + warning + "\033[0m")
+            warning_comment = "[Warning] Some commnets can't be shown because the number of comments may be exceeded."
+            ut.colorize_print(warning_comment, "yellow")
 
     note = "[Note] You can add comments optionally in the above area with editing \"sheet_music.json\"."
     ax.text(0.1, -0.06, note, color="black", fontsize=12)
```

## accompanist/report/write_front_cover.py

```diff
@@ -1,21 +1,24 @@
+import datetime
+# import re
 import site
+
 import matplotlib.lines as lines
 from PIL import Image
-import datetime
-import re
+
+import accompanist.version as ve
 
 LOGO_FILE = "logo_trans.png"
+VERSION_FILE = "".join(site.getsitepackages()) + "/accompanist/version.py"
 
 # ToDo: Refactor
-VERSIONFILE = "".join(site.getsitepackages()) + "/accompanist/version.py"
-verstrline = open(VERSIONFILE, "rt").read()
-VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
-mo = re.search(VSRE, verstrline, re.M)
-verstr = mo.group(1)
+# verstrline = open(VERSION_FILE, "rt").read()
+# VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
+# mo = re.search(VSRE, verstrline, re.M)
+# verstr = mo.group(1)
 
 
 def write_front_cover(fig, color):
     """
     Write cover of report
     """
     fig.add_artist(lines.Line2D([0, 1], [0.24, 0.24], color=color, linewidth=306, zorder=0))
@@ -30,8 +33,8 @@
     fig.text(0.1, 0.66, title_2, color="#000000", fontsize=50, fontweight="bold")
     fig.text(0.7, 0.52, creation_date, color="#757575", fontsize=18, fontweight="bold")
     fig.text(0.262, 0.3, description, color="#ffffff", fontsize=18)
 
     logo_location = "".join(site.getsitepackages()) + "/accompanist/resource/" + LOGO_FILE
     fig.figimage(Image.open(logo_location), xo=360, yo=100)
 
-    fig.text(0.44, 0.05, "Version: " + verstr, color="#ffffff", fontsize=16, fontweight="bold")
+    fig.text(0.44, 0.05, "Version: " + ve.VERSION, color="#ffffff", fontsize=16, fontweight="bold")
```

## Comparing `accompanist/report/utility_module.py` & `accompanist/report/write_header_footer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import datetime
 import json
-import site
 import os
+import site
+
+import accompanist.utility as ut
 import matplotlib.lines as lines
 from PIL import Image
 
 LOGO_FILE = "logo_trans_small.png"
 SHEET_MUSIC_FILE = "sheet_music.json"
 
 
@@ -45,26 +47,28 @@
         fig.text(0.92, 0.02, page_number, color="#949494", fontsize=20, fontweight="bold")
 
         # Logo
         logo_path = "".join(site.getsitepackages()) + "/accompanist/resource/" + LOGO_FILE
         if os.path.isfile(logo_path):
             fig.figimage(Image.open(logo_path), xo=500, yo=10)
         else:
-            print("Logo file is not found.")
+            warning_logo = "[Warning] Logo file is not found."
+            ut.colorize_print(warning_logo, "yellow")
 
 
 def calc_term(time, utc_offset):
     """
     Show term
     """
     with open(SHEET_MUSIC_FILE, mode="r") as f:
         settings_dict = json.load(f)
 
     offset = 3600 * utc_offset
-    print("[Info] The current UTC offset is \"" + str(utc_offset) + "\". You can change the offset with an option, --utc-offset N.")
+    info_utc = "[Info] The current UTC offset is \"" + str(utc_offset) + "\". You can change the offset with an option, --utc-offset N."
+    ut.colorize_print(info_utc, "cyan")
 
     oldest_time = datetime.datetime.fromtimestamp(time[len(time) - 1] / 1000.0 + offset, tz=datetime.timezone.utc).strftime("%m/%d %H:%M")
     latest_time = datetime.datetime.fromtimestamp(time[0] / 1000.0 + offset, tz=datetime.timezone.utc).strftime("%m/%d %H:%M")
 
     days = str(settings_dict["days"])
 
     if int(days) > 1:
```

## Comparing `accompanist-1.1.0.dist-info/LICENSE` & `accompanist-1.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `accompanist-1.1.0.dist-info/RECORD` & `accompanist-1.1.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-accompanist/cmd_init.py,sha256=OLo47_jHWs60veUjy2UwLOU4LnXzWE7OrPg792F06jw,1423
-accompanist/cmd_listen.py,sha256=bLEMLzyFMQYxZI06JvJVyyWBMP4KDMxC-9xLixPYrQg,5229
-accompanist/cmd_play.py,sha256=UUmb5vK0q4GwWBEya-8XfBzcAzWLtGaGr61P9cnWXdg,2968
-accompanist/main.py,sha256=xlbFfTD9O7s_6IOoOFjrXQs0EaT1M4pAFxSmCdmr_SA,732
-accompanist/version.py,sha256=LGVQyDsWifdACo7qztwb8RWWHds1E7uQ-ZqD8SAjyw4,22
-accompanist/report/draw_histgram.py,sha256=Pfx-Aeof53v3FsYF0kEeilmNAGi8NIppnX_SwPMHw-o,3945
-accompanist/report/draw_pie_chart.py,sha256=nbboVXR2--dCc65QyvfaHLgmb3Hk_fK17SM5ScC0Noc,3593
-accompanist/report/draw_table.py,sha256=Q8alH0uWr7E4dfobgyKQGZy0RdSOlHshAChyVE1Qa74,3375
-accompanist/report/utility_module.py,sha256=7bWcRuJNK7iNNvEmsm0LXeEqSB4SkVTXto33_o-oiKU,2907
-accompanist/report/write_comment.py,sha256=igcU0ZSAHwYGaq3itCtfIDXLAKNi-8fGiYxjWagh00Q,1419
-accompanist/report/write_front_cover.py,sha256=XbUTRbiBhn5qI4cM14rYAgvKPMJqtYhVQS_42GYMQNY,1317
+accompanist/cmd_init.py,sha256=vcZ6KtdGJt8iDKbh85EuwwCh5eYJFKLeXqbSWxoaP2A,1488
+accompanist/cmd_listen.py,sha256=45LR7uhJv3s7iRmBz3HmYPnzIujk9SJuzD-fS7P-qWg,5985
+accompanist/cmd_play.py,sha256=vXh6fV7GVTcG2mbUHRpDdyuOM3esNtSR79DWGi5yolo,3305
+accompanist/main.py,sha256=Lm_KbVNrglhxzPDnof0cSmm0Z1ainQj-c-vAhmknVyw,733
+accompanist/utility.py,sha256=zwBY1ZlI0atmvAKPF7pfj6K4qrZALdsRdH77hmNwI7E,292
+accompanist/version.py,sha256=tr2dMUFshB0V7YlDRbNgwbPa_pUX5HAgJ388cVKIj1Y,18
+accompanist/report/draw_histgram.py,sha256=6B6-t3rWsMEhckj8s4WNd9VWX2tXapNxfYFo-iT-UXU,3946
+accompanist/report/draw_pie_chart.py,sha256=ENcYXO_E-W6rnsB1dUGjVYqLHU1zmzb8V77rQV3gry4,3593
+accompanist/report/draw_table.py,sha256=gaVd1scT4d6x-PnzUwhzW_EYHAAS-TPZiHPUWjhe8bM,3416
+accompanist/report/write_comment.py,sha256=BZ0YWFu60UJSjLTsBALvhxDKUiCJzcBocSg6z3UdXv0,1548
+accompanist/report/write_front_cover.py,sha256=F8zoUVvJTzwzhh6WP888ib4M_V2rf0mw3sO3FtuqPNg,1368
+accompanist/report/write_header_footer.py,sha256=6njo0lestW_akei3fazHsPTXCvchPTPXBl0NnAia7o8,3057
 accompanist/resource/logo_trans.png,sha256=IbkfTLMa9qzSifN32YocbOdpDRecelHA7k8cLrBVK_4,19193
 accompanist/resource/logo_trans_small.png,sha256=SS9AlZGL3Ce-6BbD4EW5rbn7zuDcje7HkEXW_lHE2zs,6761
-accompanist-1.1.0.dist-info/LICENSE,sha256=EHImwl3uAjnXzz33MkVgnfcyDByFp0t6O-H4QaGLs4M,1063
-accompanist-1.1.0.dist-info/METADATA,sha256=9y2PTU9AvaZvtuf5Be_yz6OBfrbcFGMEZYNjgrFDX0U,3477
-accompanist-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-accompanist-1.1.0.dist-info/entry_points.txt,sha256=gLZwXDl7kf85kYQ1HNQZSxCe81vLub8Eb8wWqrThDeM,53
-accompanist-1.1.0.dist-info/top_level.txt,sha256=vUeFtOUVsBOaqJK8b1z7iVPvaRhz3jGN4Uw79o1o9Ck,31
-accompanist-1.1.0.dist-info/RECORD,,
+accompanist-1.1.2.dist-info/LICENSE,sha256=EHImwl3uAjnXzz33MkVgnfcyDByFp0t6O-H4QaGLs4M,1063
+accompanist-1.1.2.dist-info/METADATA,sha256=CkMV8gjI8U-2I-N3OISuxOyX1WVGuVPiQ_ygJKovEpI,5744
+accompanist-1.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+accompanist-1.1.2.dist-info/entry_points.txt,sha256=gLZwXDl7kf85kYQ1HNQZSxCe81vLub8Eb8wWqrThDeM,53
+accompanist-1.1.2.dist-info/top_level.txt,sha256=vUeFtOUVsBOaqJK8b1z7iVPvaRhz3jGN4Uw79o1o9Ck,31
+accompanist-1.1.2.dist-info/RECORD,,
```

