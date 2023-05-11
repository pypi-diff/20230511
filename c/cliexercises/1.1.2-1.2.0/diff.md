# Comparing `tmp/cliexercises-1.1.2.tar.gz` & `tmp/cliexercises-1.2.0.tar.gz`

## Comparing `cliexercises-1.1.2.tar` & `cliexercises-1.2.0.tar`

### file list

```diff
@@ -1,65 +1,26 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/__init__.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/cli_exercises.css
--rw-r--r--   0        0        0     7371 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/cli_exercises.py
--rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/questions.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/user_progress.json
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/anchors.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/blocks.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/colors.txt
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/duplicates.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/file_size.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/fruits.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/greeting.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/ip.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/nums_1.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/nums_2.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/purchases.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/range.txt
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/sample.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/table.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/timings.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/varying_fields.csv
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/anchors_to_links.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/block_reverse.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/char_range.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/column_product.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/delete_regex_range.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/divide_into_two_and_paste.txt
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/empty_lines.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/except_field_x.csv
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/except_first_five_lines.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/except_x_or_y.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/extract_whole_words.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/field_duplicates.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/field_serialize.csv
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/fifth_ninth_bytes.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/filter_fields_align.csv
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/first_five_lines.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/join_lines.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/last_x_chars.txt
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/lines_till_first_match.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/match_x_and_line_before.txt
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/match_x_but_not_y.txt
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/max_display_width.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/more_than_2_vowels.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/multi_replace.txt
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/number_of_words.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/para_digits.txt
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/remove_line_number_range.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/replace_except_first_two.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/reshape.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/retain_only_alnum_space.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/sort_column_unique.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/sort_general.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/sort_human_reverse.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/sort_numbers.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/sort_version.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/sorted_count.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/starts_x_ends_y_z.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/third_block.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/third_first.csv
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cliexercises-1.1.2/src/cliexercises/sample_input/expected_output/unique_2_chars.txt
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 cliexercises-1.1.2/LICENSE
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 cliexercises-1.1.2/README.md
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 cliexercises-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 cliexercises-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/__init__.py
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/app_guide.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/cli_exercises.css
+-rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/cli_exercises.py
+-rw-r--r--   0        0        0    13766 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/questions.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/user_progress.json
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/anchors.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/blocks.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/colors.txt
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/duplicates.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/file_size.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/fruits.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/greeting.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/ip.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/nums_1.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/nums_2.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/purchases.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/range.txt
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/sample.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/table.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/timings.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cliexercises-1.2.0/src/cliexercises/sample_input/varying_fields.csv
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 cliexercises-1.2.0/LICENSE
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 cliexercises-1.2.0/README.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 cliexercises-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 cliexercises-1.2.0/PKG-INFO
```

### Comparing `cliexercises-1.1.2/LICENSE` & `cliexercises-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cliexercises-1.1.2/README.md` & `cliexercises-1.2.0/src/cliexercises/app_guide.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,70 @@
-# Linux CLI Text Processing Exercises
+### Linux CLI Text Processing Exercises
 
-This TUI application includes 40 questions to test your CLI text processing skills.
+This TUI application includes 40 questions to test your CLI text processing skills. These problems have been adapted from my [Computing from the Command Line](https://github.com/learnbyexample/cli-computing) ebook.
 
-> **Note:** This application is intended for exercises based on Linux CLI tools. You might still be able to solve the exercises on other platforms, but I'm not sure if it works.
+### Input command box
 
-# Screenshot
+You can type the command in the input box and press the **Enter** key to execute. For example, `grep 'sky' ip.txt` to display lines containing `sky` from the `ip.txt` file.
 
-![Sample question](https://raw.githubusercontent.com/learnbyexample/TUI-apps/main/CLI-Exercises/cli_exercises.png)
-
-# Guide
-
-* Press **Ctrl+p** and **Ctrl+n** to navigate the questions list.
-    * You can also click them using mouse from the footer.
-* Type the command in the box below the question. Cursor focus is meant to be always within this box.
-* Press **Enter** to execute the command.
-    * `/bin/sh` is the shell used. So, features like `echo {1..3}` (brace expansion) won't work.
-    * Output would be displayed below the command box.
-    * If the output matches the expected results, the command box will turn *green* and a reference solution will also be shown.
-    * Issues due to errors and timeout (about `2` seconds) will be displayed in *red*.
-* Contents of the input file and expected output are shown at the bottom of the screen.
-    * You might have to scroll (using mouse or the scrollbar) for longer files.
-* Press **Ctrl+s** to show the reference solution if you are unable to solve an exercise.
-* Press **Ctrl+t** to toggle between light and dark themes.
-* Press **Ctrl+q** or **Ctrl+c** to quit the app.
-* Navigating and editing in the command box:
-    * Use mouse click to position the cursor anywhere you like
-    * **←** move left by one character
-    * **→** move right by one character
-    * **Home** or **Ctrl+a** move to the start of the line
-    * **End** or **Ctrl+e** move to the end of the line
-    * **Ctrl+←** move to the start of the current/previous word
-    * **Ctrl+→** move to the start of the next word
-    * **Ctrl+w** delete till the start of the current/previous word
-    * **Ctrl+f** delete till the start of the next word
-    * **Ctrl+u** delete till the start of the line
-    * **Ctrl+k** delete till the end of the line
-    * **Backspace** or **Ctrl+h** delete character to the left of the cursor
-    * **Delete** or **Ctrl+d** delete character under the cursor
-    * **Enter** submit the code for execution
+`/bin/sh` is the shell interpreting the commands (`subprocess` module's default setting). So, features like `echo {1..3}` (brace expansion) and `grep $'\t' file.txt` (ANSI-C quoting) won't work.
 
-> **Warning:** There is no safeguard against the command you are executing. They are treated as if you typed them from a shell session. For example, `ls` will list the contents of the current directory.
+> **Warning:** There is no safeguard against the commands you have typed. They are treated as if you executed them from a shell session. For example, you can use `ls` and `tree` commands to browse the contents of the current directory.
 
-# User progress
+### Output and reference solutions
 
-Commands you have typed are automatically saved in `user_progress.json` in the same directory as the script. This happens only when you press **Enter** to execute a command — navigating to another question and closing the app won't trigger the save logic. Theme choice is also saved.
+Output (`stdout`) of the command is displayed below the input box. If the output matches the expected result, the input box will turn *green* and a reference solution box will also appear.
 
-If you close the application and open it again, the first unsolved question will be displayed (i.e. already solved questions are skipped).
+If the exit status of the command executed is non-zero, the output box will turn *red* and display text from the `stderr` stream. There is also a **two** second timeout for commands taking too long. For example, commands like `cat` and `grep` will wait forever for `stdin` data if you forget to provide an input source.
 
-If you use **Ctrl+s**, the solution *won't* be saved in `user_progress.json` — you'll have to navigate to another question and back (or close and open the app) to be considered for saving the changes.
+### Input files
 
-Once you have solved a question, only a different correct solution can override the previously saved command.
+Content of the input files and expected output for each exercise are shown in boxes with appropriate labels. You might have to scroll (using mouse or the scrollbar) for longer files.
+
+You can click the **Directory** tab at the top of the screen to browse the contents of the current working directory. Click on a particular file to view its contents.
+
+### Shortcuts
+
+You can either click the buttons using mouse or press the key combinations listed below:
+
+* **F1** view this guide
+* **F2** view exercises
+* **F3** view directory
+* **Ctrl+n** go the next question
+* **Ctrl+p** go the previous question
+* **Ctrl+s** show reference solution box
+* **Ctrl+t** toggle the theme between **light** and **dark** modes
+* **Ctrl+c** or **Ctrl+q** quit the application
+
+Shortcuts for navigating and editing in the input command box are listed below:
 
-# Video demo
+* Use mouse click to position the cursor anywhere you like
+* **←** move left by one character
+* **→** move right by one character
+* **Home** or **Ctrl+a** move to the start of the line
+* **End** or **Ctrl+e** move to the end of the line
+* **Ctrl+←** move to the start of the current/previous word
+* **Ctrl+→** move to the start of the next word
+* **Ctrl+w** delete till the start of the current/previous word
+* **Ctrl+f** delete till the start of the next word
+* **Ctrl+u** delete till the start of the line
+* **Ctrl+k** delete till the end of the line
+* **Backspace** or **Ctrl+h** delete character to the left of the cursor
+* **Delete** or **Ctrl+d** delete character under the cursor
+* **Enter** submit the command for execution
 
-You can view a video demo here: [https://youtu.be/0ggfQzXeYJg](https://youtu.be/0ggfQzXeYJg)
+### User progress
 
-# License
+Commands you have typed are automatically saved in `user_progress.json` in the same directory as the script. This happens only when you press **Enter** to execute — navigating to another question and closing the app won't trigger the save logic.
+
+Theme choice is also saved.
+
+If you close the application and open it again, the first unsolved question will be displayed (i.e. already solved questions are skipped).
+
+Using **Ctrl+s** *won't* trigger the save logic — you'll have to type and execute the command to be considered for saving the changes.
+
+Once you have solved a question, only a different correct solution can override the previously saved command.
 
-Code snippets are licensed under [MIT LICENSE](https://github.com/learnbyexample/TUI-apps/blob/main/LICENSE)
+### Computing from the Command Line
 
-Exercise questions and associated files (like `questions.json`) are licensed under [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/)
+The exercise questions in this app have been adapted from my ebook: [https://github.com/learnbyexample/cli-computing](https://github.com/learnbyexample/cli-computing)
```

### Comparing `cliexercises-1.1.2/pyproject.toml` & `cliexercises-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "cliexercises"
-version = "1.1.2"
+version = "1.2.0"
 authors = [
   { name="Sundeep Agarwal", email="learnbyexample.net@gmail.com" },
 ]
 description = "40 beginner to intermediate level questions on CLI text processing tasks"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "textual>=0.16.0",
+  "textual>=0.24.1",
 ]
 
 [project.scripts]
 cliexercises = "cliexercises.cli_exercises:main"
 
 [project.urls]
 "Source" = "https://github.com/learnbyexample/TUI-apps/tree/main/CLI-Exercises"
```

