# Comparing `tmp/lecture-automator-0.2.1.tar.gz` & `tmp/lecture_automator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lecture-automator-0.2.1.tar", max compression
+gzip compressed data, was "lecture_automator-1.0.0.tar", max compression
```

## Comparing `lecture-automator-0.2.1.tar` & `lecture_automator-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0     2209 2023-05-01 10:48:41.606355 lecture-automator-0.2.1/README.md
--rw-r--r--   0        0        0     1224 2023-05-01 10:48:09.375810 lecture-automator-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 16:38:42.823945 lecture-automator-0.2.1/src/lecture_automator/__init__.py
--rw-r--r--   0        0        0     1284 2023-05-01 10:48:09.376089 lecture-automator-0.2.1/src/lecture_automator/cli.py
--rw-r--r--   0        0        0     1393 2023-04-23 14:22:41.591129 lecture-automator-0.2.1/src/lecture_automator/command_handler.py
--rw-r--r--   0        0        0        0 2023-05-01 10:48:09.376126 lecture-automator-0.2.1/src/lecture_automator/gen_speech/__init__.py
--rw-r--r--   0        0        0     7098 2023-05-01 10:48:09.376513 lecture-automator-0.2.1/src/lecture_automator/gen_speech/gen_speech.py
--rw-r--r--   0        0        0     1953 2023-05-01 10:48:09.376811 lecture-automator-0.2.1/src/lecture_automator/gen_speech/utils.py
--rw-r--r--   0        0        0     1995 2023-04-13 20:31:53.497461 lecture-automator-0.2.1/src/lecture_automator/gen_video.py
--rw-r--r--   0        0        0     1089 2023-04-23 14:22:41.591679 lecture-automator-0.2.1/src/lecture_automator/marp_api.py
--rw-r--r--   0        0        0     4492 2023-04-23 14:22:41.591888 lecture-automator-0.2.1/src/lecture_automator/parser.py
--rw-r--r--   0        0        0      192 2023-04-11 15:39:34.023953 lecture-automator-0.2.1/src/lecture_automator/settings.py
--rw-r--r--   0        0        0     3241 2023-05-01 10:49:39.205483 lecture-automator-0.2.1/setup.py
--rw-r--r--   0        0        0     2846 2023-05-01 10:49:39.205726 lecture-automator-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2733 2023-05-11 20:11:42.478981 lecture_automator-1.0.0/README.md
+-rw-r--r--   0        0        0     2208 2023-05-11 20:10:35.111655 lecture_automator-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-09 16:38:42.823945 lecture_automator-1.0.0/src/lecture_automator/__init__.py
+-rw-r--r--   0        0        0     1142 2023-05-11 20:10:35.112014 lecture_automator-1.0.0/src/lecture_automator/cli.py
+-rw-r--r--   0        0        0      792 2023-05-11 20:10:35.112300 lecture_automator-1.0.0/src/lecture_automator/compiler.py
+-rw-r--r--   0        0        0        0 2023-05-01 10:48:09.376126 lecture_automator-1.0.0/src/lecture_automator/gen_speech/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-11 20:10:35.112561 lecture_automator-1.0.0/src/lecture_automator/gen_speech/exceptions.py
+-rw-r--r--   0        0        0     3082 2023-05-11 20:10:35.113119 lecture_automator-1.0.0/src/lecture_automator/gen_speech/gen_speech.py
+-rw-r--r--   0        0        0     1970 2023-05-11 20:10:35.113510 lecture_automator-1.0.0/src/lecture_automator/gen_speech/utils.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:10:35.113563 lecture_automator-1.0.0/src/lecture_automator/gen_video/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-11 20:10:35.113973 lecture_automator-1.0.0/src/lecture_automator/gen_video/exceptions.py
+-rw-r--r--   0        0        0     1179 2023-05-11 20:10:35.114255 lecture_automator-1.0.0/src/lecture_automator/gen_video/gen_video.py
+-rw-r--r--   0        0        0      469 2023-05-11 20:10:35.114460 lecture_automator-1.0.0/src/lecture_automator/gen_video/utils.py
+-rw-r--r--   0        0        0     1090 2023-05-11 20:10:35.114753 lecture_automator-1.0.0/src/lecture_automator/marp_api.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:10:35.114804 lecture_automator-1.0.0/src/lecture_automator/parser/__init__.py
+-rw-r--r--   0        0        0     1394 2023-05-11 20:10:35.119965 lecture_automator-1.0.0/src/lecture_automator/parser/command_handler.py
+-rw-r--r--   0        0        0       84 2023-05-11 20:10:35.115338 lecture_automator-1.0.0/src/lecture_automator/parser/exceptions.py
+-rw-r--r--   0        0        0     4364 2023-05-11 20:10:35.119793 lecture_automator-1.0.0/src/lecture_automator/parser/parser.py
+-rw-r--r--   0        0        0      369 2023-05-11 20:10:35.115995 lecture_automator-1.0.0/src/lecture_automator/settings.py
+-rw-r--r--   0        0        0      749 2023-05-11 20:10:35.116220 lecture_automator-1.0.0/src/lecture_automator/web.py
+-rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 lecture_automator-1.0.0/PKG-INFO
```

### Comparing `lecture-automator-0.2.1/README.md` & `lecture_automator-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 С помощью pip (также необходимо установить ffmpeg и [Marp](https://github.com/marp-team/marp-cli)):
 ```
 pip install lecture-automator
 ```
 
 ## Использование
 
-Для использования необходимо создать Markdown-файл с описаниями слайдов (см. [Marp](https://marp.app/#get-started)) и [управляющими конструкциями](#управляющие-конструкции):
+### Через CLI
+
+Для использование необходимо создать Markdown-файл с описаниями слайдов (см. [Marp](https://marp.app/#get-started)) и [управляющими конструкциями](#управляющие-конструкции):
 ````md
 # Python
 
 ```
 print('Привет, мир')
 ```
 
@@ -33,19 +35,30 @@
 
 /speech{А здесь представлена другая программа, которая умножается число два на число четыре.}
 
 ````
 
 Затем для генерации необходимо использовать следующую CLI команду в терминале:
 ```bash
-lecture-automator Example.md Example.mp4
+lecture-automator convert Example.md Example.mp4
 ```
 
 Пример сгенерированного видео:
 
 [Example.webm](https://user-images.githubusercontent.com/33065236/231875817-1d3aae09-2a63-4bb1-8380-8b7f024bbe45.webm)
 
+### Через Web
+
+Lecture Automator может развернуть небольшой сервер с веб-интерфейсом, в котором можно
+описывать слайды и тут же генерировать видео с возможность его просмотра прямо в данном
+веб-интерфейсе.
+
+Для его запуска необходимо выполнить следующую команду:
+```bash
+lecture-automator web
+```
+
 
 ### Управляющие конструкции 
 
 На данный момент реализованы следующие управляющие конструкции:
 - `/speech{...}` - текст для озвучивания слайда (каждый слайд должен содержать данную конструкцию).
```

### Comparing `lecture-automator-0.2.1/src/lecture_automator/cli.py` & `lecture_automator-1.0.0/src/lecture_automator/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,55 @@
-import os
-import glob
-import tempfile
-
 import click
 
-from lecture_automator.parser import parse_md
-from lecture_automator.marp_api import generate_marp_slides
-from lecture_automator.gen_speech.gen_speech import texts_to_speeches
-from lecture_automator.gen_video import generate_video
+from lecture_automator.compiler import compile_text_md
+from lecture_automator.web import run_web
+
+
+@click.group()
+def cli():
+    pass
 
 
-@click.command()
+@cli.command()
 @click.argument(
-    'input_md', 
+    'input_md',
     type=click.STRING,
 )
 @click.argument(
-    'out_path', 
+    'out_path',
     type=click.STRING,
 )
 @click.option(
-    '--scale', 
-    type=click.FLOAT, 
-    default=1.5, 
+    '--vformat',
+    type=click.Choice(['mp4', 'webm']),
+    default='mp4',
+    help=(
+        'Формат генерируемого видео.'
+    )
+)
+@click.option(
+    '--scale',
+    type=click.FLOAT,
+    default=1.5,
     help=(
         'Коэффициент масштабирования генерируемого видео, '
         'по умолчанию равен 1.5, что соответствует разрешению 1920x1080,'
         'значение 1 соответствует разрешению 1280x720.'
     )
 )
-def convert_md_to_mp4(input_md, out_path, scale):
-    md_data = parse_md(input_md)
+def convert(input_md, out_path, scale, vformat):
+    with open(input_md) as file:
+        md_text = file.read()
+
+    compile_text_md(
+        md_text, out_path=out_path,
+        vformat=vformat, scale=scale
+    )
+
 
-    with tempfile.TemporaryDirectory() as tmpdirname:
-        generate_marp_slides(tmpdirname, md_data['md_text'], scale=scale)
-        slide_images = glob.glob(os.path.join(tmpdirname, 'Slide.*'))
-        audio_paths = texts_to_speeches(md_data['speech'], tmpdirname)
-        generate_video(slide_images, audio_paths, out_path)
+@cli.command()
+def web():
+    run_web()
 
 
 if __name__ == '__main__':
-    convert_md_to_mp4()
+    cli()
```

### Comparing `lecture-automator-0.2.1/src/lecture_automator/command_handler.py` & `lecture_automator-1.0.0/src/lecture_automator/parser/command_handler.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from abc import ABC, abstractmethod
 import re
+from abc import ABC, abstractmethod
 
 
 class CommandHandler(ABC):
     def __init__(self, handler = None) -> None:
         self._next: CommandHandler = handler
 
     @abstractmethod
@@ -29,8 +29,8 @@
             metadata.update(
                 {
                     'speech': arg
                 }
             )
             return ''
         else:
-            return super().handle(slide, name_command, arg, start_pos, end_pos)
+            return super().handle(slide, name_command, arg, start_pos, end_pos)
```

### Comparing `lecture-automator-0.2.1/src/lecture_automator/gen_speech/utils.py` & `lecture_automator-1.0.0/src/lecture_automator/gen_speech/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import re
-from typing import List
 import wave
+from typing import List
 
 
 def divide_text(text: str, max_length: int = 1000) -> List[str]:
-    """Разделение текста по точкам таким образом, чтобы каждая часть текста не превышала указанный максимум.
+    """Разделение текста по точкам таким образом, чтобы каждая часть текста не превышала
+    указанный максимум.
     Args:
         text (str): текст для разделения.
-        max_length (int, optional): максимальная длина одной части текста. Defaults to 1000.
+        max_length (int, optional): максимальная длина одной части текста. Defaults to
+            1000.
     Raises:
         Exception: _description_
     Returns:
         List[str]: список частей текста.
     """
 
     split_texts = re.split(r'\.', text)
@@ -47,8 +49,8 @@
             data.append([w.getparams(), w.readframes(w.getnframes())])
 
     with wave.open(output_wav, 'wb') as output:
         output.setparams(data[0][0])
         for i in range(len(data)):
             output.writeframes(data[i][1])
 
-    return output_wav
+    return output_wav
```

### Comparing `lecture-automator-0.2.1/src/lecture_automator/marp_api.py` & `lecture_automator-1.0.0/src/lecture_automator/marp_api.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import os
 import subprocess
 import tempfile
-import os
 
 
 def generate_marp_slides(outdir: str, md_text: str, type_images: str = 'png', scale: float = 2.0) -> None:
     """Генерация слайдов презентации Marp в виде набора изображений.
 
     Args:
         outdir (str): директория для сохранения изображений.
@@ -23,8 +23,8 @@
         )
 
 
 if __name__ == '__main__':
     with open('examples/Example.md') as file:
         text = file.read()
 
-    generate_marp_slides('examples', text, scale=1.5)
+    generate_marp_slides('examples', text, scale=1.5)
```

### Comparing `lecture-automator-0.2.1/src/lecture_automator/parser.py` & `lecture_automator-1.0.0/src/lecture_automator/parser/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,84 +1,86 @@
 import re
-from typing import List, Dict, Tuple
+from typing import List, Tuple
 
-from lecture_automator.command_handler import CommandHandler
+from lecture_automator.parser.command_handler import CommandHandler
+from lecture_automator.parser.exceptions import SpeechNotFound
 
 
 def join_slides(slides: List[str], metaslide=None):
     md_text = '---\n'.join(slides)
     if metaslide:
         metaslide = '---\n{}---\n'.format(metaslide)
         md_text = '{}{}'.format(metaslide, md_text)
-        
+
     return md_text
 
 
 def parse_commands(slide: str) -> List[Tuple[str, str, int, int]]:
     """Парсинг управляющих конструкций для каждого слайда в презентации Markdown.
 
     Args:
         slide (str): текст слайда Markdown.
 
     Returns:
-        List[Tuple[str, str, int, int]]: список кортежей 
-            (название команды, ее аргумент, 
+        List[Tuple[str, str, int, int]]: список кортежей
+            (название команды, ее аргумент,
             начальная позиция в файле, конечная позиция в файле).
     """
 
     commands = []
     p = re.compile(r'/([a-z]+) *\{([^\{\}]+)\}')
 
     for match in p.finditer(slide):
         name_command = match.group(1)
         arg = match.group(2)
         start_pos = match.start()
         end_pos = match.end()
 
         if len(re.findall(r'(?m)\`{3}', slide[:start_pos])) % 2 != 0:
             continue
-        
+
         commands.append(
             (name_command, arg, start_pos, end_pos)
         )
 
     return commands
 
 
 def process_commands(slides: List[str]) -> Tuple[list, dict]:
     """Обработка управляющих конструкций.
 
     Args:
         slides (List[str]): список текстов слайдов Markdown.
 
     Returns:
-        Tuple[str, dict]: кортеж (список обработанных текстов Markdown для каждого слайда, словарь метаданных для каждого слайда).
+        Tuple[str, dict]: кортеж (список обработанных текстов Markdown для каждого
+            слайда, словарь метаданных для каждого слайда).
     """
-    
+
     metadata = dict()
     processed_slides = []
     for idx, slide in enumerate(slides, start=1):
         metadata[idx] = dict()
         parsed_commands = parse_commands(slide)
 
         for name_command, arg, start_pos, end_pos in parsed_commands:
             command_replacer = CommandHandler.process(
                 slide, name_command,
                 arg, start_pos,
                 end_pos, metadata[idx]
             )
 
             slide = "{}{}{}".format(
-                slide[:start_pos], 
-                command_replacer, 
+                slide[:start_pos],
+                command_replacer,
                 slide[end_pos:]
             )
 
         if 'speech' not in metadata[idx]:
-            raise Exception('Каждый слайд должен иметь описание речи.')
+            raise SpeechNotFound('Каждый слайд должен иметь описание речи.')
 
         processed_slides.append(slide)
 
     return processed_slides, metadata
 
 
 def parse_slides(text: str) -> tuple:
@@ -108,37 +110,29 @@
         if idx == len(slides) - 1:
             break
 
         idx += 1
 
     return metaslide, slides
 
-def parse_md(path: str) -> dict:
-    """Парсинг Markdown презентации формата Marp с дополнительными управляющими командами (/speech и т.д.)
+def parse_md(md_text: str) -> dict:
+    """Парсинг Markdown презентации формата Marp с дополнительными управляющими
+    командами (/speech и т.д.)
 
     Args:
         path (str): путь к файлу Markdown.
 
     Returns:
-        dict: словарь, содержащий текст Markdown для Marp (с удаленными управляющими командами) и метаданные.
+        dict: словарь, содержащий текст Markdown для Marp
+            (с удаленными управляющими командами) и метаданные.
     """
 
-    with open(path) as file:
-        md_text = file.read()
-
     metaslide, slides = parse_slides(md_text)
     processed_slides, metadata = process_commands(slides)
     processed_marp_text = join_slides(processed_slides, metaslide=metaslide)
 
     speech_metadata = [metadata[slide]['speech'] for slide in metadata]
 
     return {
         'md_text': processed_marp_text,
         'speech': speech_metadata
     }
-
-    
-if __name__ == '__main__':
-    res = parse_md("examples/Example.md")
-    print(res)
-    # print(res['md_text'])
-    # print(res['speech'])
```

### Comparing `lecture-automator-0.2.1/PKG-INFO` & `lecture_automator-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: lecture-automator
-Version: 0.2.1
+Version: 1.0.0
 Summary: 
 Home-page: https://github.com/CapBlood/lecture-automator.git
 Author: CapBlood
 Author-email: stalker.anonim@mail.ru
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<=3.9
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: test
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: streamlit (>=1.22.0,<2.0.0)
+Requires-Dist: sympy (>=1.11.1,<2.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Lecture Automator
 
 Lecture Automator позволяет автоматически генерировать презентации с озвучкой для каждого из слайдов. Всё, что вам нужно сделать - написать текстовый файл Markdown со специальной разметкой, а остальное за вас сделает Lecture Automator.
 
@@ -26,15 +27,17 @@
 С помощью pip (также необходимо установить ffmpeg и [Marp](https://github.com/marp-team/marp-cli)):
 ```
 pip install lecture-automator
 ```
 
 ## Использование
 
-Для использования необходимо создать Markdown-файл с описаниями слайдов (см. [Marp](https://marp.app/#get-started)) и [управляющими конструкциями](#управляющие-конструкции):
+### Через CLI
+
+Для использование необходимо создать Markdown-файл с описаниями слайдов (см. [Marp](https://marp.app/#get-started)) и [управляющими конструкциями](#управляющие-конструкции):
 ````md
 # Python
 
 ```
 print('Привет, мир')
 ```
 
@@ -52,20 +55,31 @@
 
 /speech{А здесь представлена другая программа, которая умножается число два на число четыре.}
 
 ````
 
 Затем для генерации необходимо использовать следующую CLI команду в терминале:
 ```bash
-lecture-automator Example.md Example.mp4
+lecture-automator convert Example.md Example.mp4
 ```
 
 Пример сгенерированного видео:
 
 [Example.webm](https://user-images.githubusercontent.com/33065236/231875817-1d3aae09-2a63-4bb1-8380-8b7f024bbe45.webm)
 
+### Через Web
+
+Lecture Automator может развернуть небольшой сервер с веб-интерфейсом, в котором можно
+описывать слайды и тут же генерировать видео с возможность его просмотра прямо в данном
+веб-интерфейсе.
+
+Для его запуска необходимо выполнить следующую команду:
+```bash
+lecture-automator web
+```
+
 
 ### Управляющие конструкции 
 
 На данный момент реализованы следующие управляющие конструкции:
 - `/speech{...}` - текст для озвучивания слайда (каждый слайд должен содержать данную конструкцию).
```

