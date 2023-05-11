# Comparing `tmp/mlgame-9.5.3.2a0.tar.gz` & `tmp/mlgame-9.5.4.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlgame-9.5.3.2a0.tar", last modified: Tue Aug  2 09:35:19 2022, max compression
+gzip compressed data, was "mlgame-9.5.4.1b0.tar", last modified: Fri Aug 19 06:37:37 2022, max compression
```

## Comparing `mlgame-9.5.3.2a0.tar` & `mlgame-9.5.4.1b0.tar`

### file list

```diff
@@ -1,160 +1,64 @@
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.759249 mlgame-9.5.3.2a0/
--rw-r--r--   0 kylin      (501) staff       (20)      101 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/MANIFEST.in
--rw-r--r--   0 kylin      (501) staff       (20)     4022 2022-08-02 09:35:19.759079 mlgame-9.5.3.2a0/PKG-INFO
--rw-r--r--   0 kylin      (501) staff       (20)     3535 2022-08-02 02:43:41.000000 mlgame-9.5.3.2a0/README.md
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.722298 mlgame-9.5.3.2a0/games/
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.731670 mlgame-9.5.3.2a0/games/Maze_Car/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2022-05-26 03:17:06.000000 mlgame-9.5.3.2a0/games/Maze_Car/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)      141 2022-08-02 03:14:01.000000 mlgame-9.5.3.2a0/games/Maze_Car/config.py
--rw-r--r--   0 kylin      (501) staff       (20)      895 2022-08-02 03:14:01.000000 mlgame-9.5.3.2a0/games/Maze_Car/main.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.732279 mlgame-9.5.3.2a0/games/Maze_Car/ml/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2022-05-26 03:17:06.000000 mlgame-9.5.3.2a0/games/Maze_Car/ml/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     1474 2022-08-02 03:14:01.000000 mlgame-9.5.3.2a0/games/Maze_Car/ml/ml_play_manual.py
--rw-r--r--   0 kylin      (501) staff       (20)     1094 2022-08-02 03:14:01.000000 mlgame-9.5.3.2a0/games/Maze_Car/ml/ml_play_template.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.736201 mlgame-9.5.3.2a0/games/Maze_Car/src/
--rw-r--r--   0 kylin      (501) staff       (20)     2227 2022-05-26 03:17:06.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/I_Commander.py
--rw-r--r--   0 kylin      (501) staff       (20)    18361 2022-08-02 03:14:01.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/MazeCar.py
--rw-r--r--   0 kylin      (501) staff       (20)        0 2022-05-26 03:17:06.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     4414 2022-08-02 03:14:01.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/car.py
--rw-r--r--   0 kylin      (501) staff       (20)      127 2022-05-26 03:17:06.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/coin.py
--rw-r--r--   0 kylin      (501) staff       (20)     2654 2022-05-26 03:17:06.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/env.py
--rw-r--r--   0 kylin      (501) staff       (20)    15813 2022-05-26 03:17:06.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/gameMode.py
--rw-r--r--   0 kylin      (501) staff       (20)     6641 2022-07-20 03:02:36.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/gameView.py
--rw-r--r--   0 kylin      (501) staff       (20)    11684 2022-05-26 03:17:06.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/game_object_data.py
--rw-r--r--   0 kylin      (501) staff       (20)     2064 2022-05-26 03:17:06.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/math_function.py
--rw-r--r--   0 kylin      (501) staff       (20)     6401 2022-08-02 03:14:01.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/mazeMode.py
--rw-r--r--   0 kylin      (501) staff       (20)     2814 2022-05-26 03:17:06.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/maze_wall.py
--rw-r--r--   0 kylin      (501) staff       (20)     6785 2022-08-02 03:14:01.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/moveMazeMode.py
--rw-r--r--   0 kylin      (501) staff       (20)     3453 2022-08-02 03:14:01.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/points.py
--rw-r--r--   0 kylin      (501) staff       (20)     5509 2022-08-02 03:14:01.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/practiceMode.py
--rw-r--r--   0 kylin      (501) staff       (20)     4344 2022-05-26 03:17:06.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/sensor.py
--rw-r--r--   0 kylin      (501) staff       (20)      610 2022-05-26 03:17:06.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/sound_controller.py
--rw-r--r--   0 kylin      (501) staff       (20)     1503 2022-05-26 03:17:06.000000 mlgame-9.5.3.2a0/games/Maze_Car/src/tilemap.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.736763 mlgame-9.5.3.2a0/games/RacingCar/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2022-05-26 03:14:48.000000 mlgame-9.5.3.2a0/games/RacingCar/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)      149 2022-07-13 06:52:03.000000 mlgame-9.5.3.2a0/games/RacingCar/config.py
--rw-r--r--   0 kylin      (501) staff       (20)      930 2022-07-13 06:52:03.000000 mlgame-9.5.3.2a0/games/RacingCar/main.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.737470 mlgame-9.5.3.2a0/games/RacingCar/ml/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2022-05-26 03:14:48.000000 mlgame-9.5.3.2a0/games/RacingCar/ml/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)      910 2022-05-26 03:14:48.000000 mlgame-9.5.3.2a0/games/RacingCar/ml/ml_play_manual.py
--rw-r--r--   0 kylin      (501) staff       (20)      644 2022-08-02 02:30:35.000000 mlgame-9.5.3.2a0/games/RacingCar/ml/ml_play_template.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.739609 mlgame-9.5.3.2a0/games/RacingCar/src/
--rw-r--r--   0 kylin      (501) staff       (20)     1671 2022-05-26 03:14:48.000000 mlgame-9.5.3.2a0/games/RacingCar/src/I_Commander.py
--rw-r--r--   0 kylin      (501) staff       (20)    12913 2022-07-13 06:52:03.000000 mlgame-9.5.3.2a0/games/RacingCar/src/RacingCar.py
--rw-r--r--   0 kylin      (501) staff       (20)        0 2022-05-26 03:14:48.000000 mlgame-9.5.3.2a0/games/RacingCar/src/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     4901 2022-07-13 06:52:03.000000 mlgame-9.5.3.2a0/games/RacingCar/src/car.py
--rw-r--r--   0 kylin      (501) staff       (20)      525 2022-05-26 03:14:48.000000 mlgame-9.5.3.2a0/games/RacingCar/src/coin.py
--rw-r--r--   0 kylin      (501) staff       (20)     6183 2022-07-13 06:52:03.000000 mlgame-9.5.3.2a0/games/RacingCar/src/coinPlayMode.py
--rw-r--r--   0 kylin      (501) staff       (20)     2803 2022-05-26 03:14:48.000000 mlgame-9.5.3.2a0/games/RacingCar/src/env.py
--rw-r--r--   0 kylin      (501) staff       (20)     4108 2022-07-13 06:52:03.000000 mlgame-9.5.3.2a0/games/RacingCar/src/gameMode.py
--rw-r--r--   0 kylin      (501) staff       (20)     1477 2022-05-26 03:14:48.000000 mlgame-9.5.3.2a0/games/RacingCar/src/highway.py
--rw-r--r--   0 kylin      (501) staff       (20)     5082 2022-07-13 06:52:03.000000 mlgame-9.5.3.2a0/games/RacingCar/src/playingMode.py
--rw-r--r--   0 kylin      (501) staff       (20)     6761 2022-07-13 06:52:03.000000 mlgame-9.5.3.2a0/games/RacingCar/src/reliveMode.py
--rw-r--r--   0 kylin      (501) staff       (20)     1258 2022-05-26 03:14:48.000000 mlgame-9.5.3.2a0/games/RacingCar/src/sound_controller.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.740447 mlgame-9.5.3.2a0/games/arkanoid/
--rw-r--r--   0 kylin      (501) staff       (20)        1 2022-06-15 05:07:55.000000 mlgame-9.5.3.2a0/games/arkanoid/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)      141 2022-06-15 07:27:27.000000 mlgame-9.5.3.2a0/games/arkanoid/config.py
--rw-r--r--   0 kylin      (501) staff       (20)      715 2022-06-15 07:27:27.000000 mlgame-9.5.3.2a0/games/arkanoid/main.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.741273 mlgame-9.5.3.2a0/games/arkanoid/ml/
--rw-r--r--   0 kylin      (501) staff       (20)        1 2022-06-15 05:07:55.000000 mlgame-9.5.3.2a0/games/arkanoid/ml/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     1228 2022-05-26 03:14:03.000000 mlgame-9.5.3.2a0/games/arkanoid/ml/ml_play_manual.py
--rw-r--r--   0 kylin      (501) staff       (20)      772 2022-06-15 05:07:55.000000 mlgame-9.5.3.2a0/games/arkanoid/ml/ml_play_template.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.742014 mlgame-9.5.3.2a0/games/arkanoid/src/
--rw-r--r--   0 kylin      (501) staff       (20)        1 2022-06-15 05:07:55.000000 mlgame-9.5.3.2a0/games/arkanoid/src/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     8739 2022-06-15 07:27:27.000000 mlgame-9.5.3.2a0/games/arkanoid/src/game.py
--rw-r--r--   0 kylin      (501) staff       (20)    10274 2022-06-15 07:27:27.000000 mlgame-9.5.3.2a0/games/arkanoid/src/game_object.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.742720 mlgame-9.5.3.2a0/games/easy_game/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2022-06-15 08:10:54.000000 mlgame-9.5.3.2a0/games/easy_game/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)      192 2022-06-15 08:10:54.000000 mlgame-9.5.3.2a0/games/easy_game/config.py
--rw-r--r--   0 kylin      (501) staff       (20)      780 2022-06-15 08:10:54.000000 mlgame-9.5.3.2a0/games/easy_game/main.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.743444 mlgame-9.5.3.2a0/games/easy_game/src/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2022-06-15 08:10:54.000000 mlgame-9.5.3.2a0/games/easy_game/src/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     6028 2022-06-15 08:10:54.000000 mlgame-9.5.3.2a0/games/easy_game/src/game.py
--rw-r--r--   0 kylin      (501) staff       (20)     1816 2022-06-15 08:10:54.000000 mlgame-9.5.3.2a0/games/easy_game/src/game_object.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.744068 mlgame-9.5.3.2a0/games/fake_game_unvalid_import/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2021-09-08 07:23:18.000000 mlgame-9.5.3.2a0/games/fake_game_unvalid_import/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)      540 2022-04-28 02:02:48.000000 mlgame-9.5.3.2a0/games/fake_game_unvalid_import/config.py
--rw-r--r--   0 kylin      (501) staff       (20)      783 2022-04-20 03:07:01.000000 mlgame-9.5.3.2a0/games/fake_game_unvalid_import/main.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.744741 mlgame-9.5.3.2a0/games/fake_game_unvalid_import/ml/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2021-09-08 07:23:18.000000 mlgame-9.5.3.2a0/games/fake_game_unvalid_import/ml/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     1008 2022-04-22 07:08:38.000000 mlgame-9.5.3.2a0/games/fake_game_unvalid_import/ml/ml_play_manual.py
--rw-r--r--   0 kylin      (501) staff       (20)      570 2022-04-22 06:41:56.000000 mlgame-9.5.3.2a0/games/fake_game_unvalid_import/ml/ml_play_template.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.745324 mlgame-9.5.3.2a0/games/fake_game_unvalid_import/src/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2021-09-08 07:23:18.000000 mlgame-9.5.3.2a0/games/fake_game_unvalid_import/src/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     6215 2022-05-12 01:35:33.000000 mlgame-9.5.3.2a0/games/fake_game_unvalid_import/src/game.py
--rw-r--r--   0 kylin      (501) staff       (20)     1816 2021-11-26 07:52:40.000000 mlgame-9.5.3.2a0/games/fake_game_unvalid_import/src/game_object.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.745886 mlgame-9.5.3.2a0/games/fake_game_with_error/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2021-09-08 07:23:18.000000 mlgame-9.5.3.2a0/games/fake_game_with_error/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)      540 2022-04-28 02:02:48.000000 mlgame-9.5.3.2a0/games/fake_game_with_error/config.py
--rw-r--r--   0 kylin      (501) staff       (20)      783 2022-04-20 03:07:01.000000 mlgame-9.5.3.2a0/games/fake_game_with_error/main.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.746457 mlgame-9.5.3.2a0/games/fake_game_with_error/ml/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2021-09-08 07:23:18.000000 mlgame-9.5.3.2a0/games/fake_game_with_error/ml/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     1008 2022-04-22 07:08:38.000000 mlgame-9.5.3.2a0/games/fake_game_with_error/ml/ml_play_manual.py
--rw-r--r--   0 kylin      (501) staff       (20)      570 2022-04-22 06:41:56.000000 mlgame-9.5.3.2a0/games/fake_game_with_error/ml/ml_play_template.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.747039 mlgame-9.5.3.2a0/games/fake_game_with_error/src/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2021-09-08 07:23:18.000000 mlgame-9.5.3.2a0/games/fake_game_with_error/src/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     6285 2022-05-12 01:35:33.000000 mlgame-9.5.3.2a0/games/fake_game_with_error/src/game.py
--rw-r--r--   0 kylin      (501) staff       (20)     1816 2021-11-26 07:52:40.000000 mlgame-9.5.3.2a0/games/fake_game_with_error/src/game_object.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.747310 mlgame-9.5.3.2a0/games/pingpong/
--rw-r--r--   0 kylin      (501) staff       (20)      141 2022-06-15 07:27:32.000000 mlgame-9.5.3.2a0/games/pingpong/config.py
--rw-r--r--   0 kylin      (501) staff       (20)      848 2022-06-15 07:27:32.000000 mlgame-9.5.3.2a0/games/pingpong/main.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.731109 mlgame-9.5.3.2a0/mlgame/
--rw-r--r--   0 kylin      (501) staff       (20)     1069 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/LICIENCE.txt
--rw-r--r--   0 kylin      (501) staff       (20)        2 2021-08-12 09:10:29.000000 mlgame-9.5.3.2a0/mlgame/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     2985 2022-08-02 02:43:41.000000 mlgame-9.5.3.2a0/mlgame/__main__.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.748839 mlgame-9.5.3.2a0/mlgame/argument/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/argument/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     3384 2022-07-20 06:35:55.000000 mlgame-9.5.3.2a0/mlgame/argument/cmd_argument.py
--rw-r--r--   0 kylin      (501) staff       (20)     7071 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/argument/game_argument.py
--rw-r--r--   0 kylin      (501) staff       (20)     1023 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/argument/model.py
--rw-r--r--   0 kylin      (501) staff       (20)      971 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/argument/tool.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.750551 mlgame-9.5.3.2a0/mlgame/core/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/core/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)    11822 2022-07-20 03:17:01.000000 mlgame-9.5.3.2a0/mlgame/core/communication.py
--rw-r--r--   0 kylin      (501) staff       (20)       53 2022-08-02 09:31:05.000000 mlgame-9.5.3.2a0/mlgame/core/env.py
--rw-r--r--   0 kylin      (501) staff       (20)      300 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/core/errno.py
--rw-r--r--   0 kylin      (501) staff       (20)     2437 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/core/exceptions.py
--rw-r--r--   0 kylin      (501) staff       (20)    19178 2022-08-02 09:33:01.000000 mlgame-9.5.3.2a0/mlgame/core/executor.py
--rw-r--r--   0 kylin      (501) staff       (20)     2709 2022-08-02 09:33:01.000000 mlgame-9.5.3.2a0/mlgame/core/process.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.751621 mlgame-9.5.3.2a0/mlgame/crosslang/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2021-08-12 09:10:29.000000 mlgame-9.5.3.2a0/mlgame/crosslang/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     2945 2021-08-12 09:10:29.000000 mlgame-9.5.3.2a0/mlgame/crosslang/client.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.751767 mlgame-9.5.3.2a0/mlgame/crosslang/compile/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2021-08-12 09:10:29.000000 mlgame-9.5.3.2a0/mlgame/crosslang/compile/__init__.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.751960 mlgame-9.5.3.2a0/mlgame/crosslang/compile/cpp/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2021-08-12 09:10:29.000000 mlgame-9.5.3.2a0/mlgame/crosslang/compile/cpp/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     2261 2021-08-12 09:10:29.000000 mlgame-9.5.3.2a0/mlgame/crosslang/compile/cpp/main.py
--rw-r--r--   0 kylin      (501) staff       (20)      649 2021-08-12 09:10:29.000000 mlgame-9.5.3.2a0/mlgame/crosslang/exceptions.py
--rw-r--r--   0 kylin      (501) staff       (20)      100 2021-08-12 09:10:29.000000 mlgame-9.5.3.2a0/mlgame/crosslang/ext_lang_map.py
--rw-r--r--   0 kylin      (501) staff       (20)      892 2021-08-12 09:10:29.000000 mlgame-9.5.3.2a0/mlgame/crosslang/main.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.752801 mlgame-9.5.3.2a0/mlgame/game/
--rw-r--r--   0 kylin      (501) staff       (20)        1 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/game/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     2603 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/game/generic.py
--rw-r--r--   0 kylin      (501) staff       (20)     3430 2022-08-02 02:43:41.000000 mlgame-9.5.3.2a0/mlgame/game/paia_game.py
--rw-r--r--   0 kylin      (501) staff       (20)     9792 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/game/physics.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.753670 mlgame-9.5.3.2a0/mlgame/tests/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2021-09-08 07:23:18.000000 mlgame-9.5.3.2a0/mlgame/tests/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)      955 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/tests/test_decorator.py
--rw-r--r--   0 kylin      (501) staff       (20)     1246 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/tests/test_game_argument.py
--rw-r--r--   0 kylin      (501) staff       (20)      220 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/tests/test_logger.py
--rw-r--r--   0 kylin      (501) staff       (20)     1360 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/tests/test_tools.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.757096 mlgame-9.5.3.2a0/mlgame/utils/
--rw-r--r--   0 kylin      (501) staff       (20)        1 2021-08-12 09:10:29.000000 mlgame-9.5.3.2a0/mlgame/utils/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)      652 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/utils/enum.py
--rw-r--r--   0 kylin      (501) staff       (20)      325 2022-08-02 09:30:16.000000 mlgame-9.5.3.2a0/mlgame/utils/logger.py
--rw-r--r--   0 kylin      (501) staff       (20)     3551 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/utils/recorder.py
--rw-r--r--   0 kylin      (501) staff       (20)       26 2022-08-02 09:34:20.000000 mlgame-9.5.3.2a0/mlgame/version.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.758758 mlgame-9.5.3.2a0/mlgame/view/
--rw-r--r--   0 kylin      (501) staff       (20)        0 2021-09-08 07:23:18.000000 mlgame-9.5.3.2a0/mlgame/view/__init__.py
--rw-r--r--   0 kylin      (501) staff       (20)     5667 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/view/decorator.py
--rw-r--r--   0 kylin      (501) staff       (20)    12806 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/view/view.py
--rw-r--r--   0 kylin      (501) staff       (20)     6601 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/mlgame/view/view_model.py
-drwxr-xr-x   0 kylin      (501) staff       (20)        0 2022-08-02 09:35:19.747944 mlgame-9.5.3.2a0/mlgame.egg-info/
--rw-r--r--   0 kylin      (501) staff       (20)     4022 2022-08-02 09:35:19.000000 mlgame-9.5.3.2a0/mlgame.egg-info/PKG-INFO
--rw-r--r--   0 kylin      (501) staff       (20)     3955 2022-08-02 09:35:19.000000 mlgame-9.5.3.2a0/mlgame.egg-info/SOURCES.txt
--rw-r--r--   0 kylin      (501) staff       (20)        1 2022-08-02 09:35:19.000000 mlgame-9.5.3.2a0/mlgame.egg-info/dependency_links.txt
--rw-r--r--   0 kylin      (501) staff       (20)       61 2022-08-02 09:35:19.000000 mlgame-9.5.3.2a0/mlgame.egg-info/requires.txt
--rw-r--r--   0 kylin      (501) staff       (20)        7 2022-08-02 09:35:19.000000 mlgame-9.5.3.2a0/mlgame.egg-info/top_level.txt
--rw-r--r--   0 kylin      (501) staff       (20)       84 2022-06-15 04:54:03.000000 mlgame-9.5.3.2a0/pyproject.toml
--rw-r--r--   0 kylin      (501) staff       (20)       38 2022-08-02 09:35:19.759300 mlgame-9.5.3.2a0/setup.cfg
--rw-r--r--   0 kylin      (501) staff       (20)     1159 2022-08-02 02:43:59.000000 mlgame-9.5.3.2a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-19 06:37:37.271104 mlgame-9.5.4.1b0/
+-rw-r--r--   0 root         (0) root         (0)      101 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4022 2022-08-19 06:37:37.271104 mlgame-9.5.4.1b0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3535 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-19 06:37:37.259103 mlgame-9.5.4.1b0/mlgame/
+-rw-r--r--   0 root         (0) root         (0)     1069 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/LICIENCE.txt
+-rw-r--r--   0 root         (0) root         (0)        2 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-19 06:37:37.263104 mlgame-9.5.4.1b0/mlgame/argument/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/argument/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3384 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/argument/cmd_argument.py
+-rw-r--r--   0 root         (0) root         (0)     7071 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/argument/game_argument.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/argument/model.py
+-rw-r--r--   0 root         (0) root         (0)      971 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/argument/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-19 06:37:37.263104 mlgame-9.5.4.1b0/mlgame/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11822 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/core/communication.py
+-rw-r--r--   0 root         (0) root         (0)       53 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/core/env.py
+-rw-r--r--   0 root         (0) root         (0)      300 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/core/errno.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/core/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    19178 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/core/executor.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/core/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-19 06:37:37.263104 mlgame-9.5.4.1b0/mlgame/crosslang/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/crosslang/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2945 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/crosslang/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-19 06:37:37.263104 mlgame-9.5.4.1b0/mlgame/crosslang/compile/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/crosslang/compile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-19 06:37:37.263104 mlgame-9.5.4.1b0/mlgame/crosslang/compile/cpp/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/crosslang/compile/cpp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/crosslang/compile/cpp/main.py
+-rw-r--r--   0 root         (0) root         (0)      649 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/crosslang/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      100 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/crosslang/ext_lang_map.py
+-rw-r--r--   0 root         (0) root         (0)      892 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/crosslang/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-19 06:37:37.267104 mlgame-9.5.4.1b0/mlgame/game/
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/game/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/game/generic.py
+-rw-r--r--   0 root         (0) root         (0)     3430 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/game/paia_game.py
+-rw-r--r--   0 root         (0) root         (0)     9792 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/game/physics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-19 06:37:37.267104 mlgame-9.5.4.1b0/mlgame/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      955 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/tests/test_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/tests/test_game_argument.py
+-rw-r--r--   0 root         (0) root         (0)      220 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/tests/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-19 06:37:37.267104 mlgame-9.5.4.1b0/mlgame/utils/
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      652 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/utils/enum.py
+-rw-r--r--   0 root         (0) root         (0)      325 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/utils/recorder.py
+-rw-r--r--   0 root         (0) root         (0)       25 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-19 06:37:37.267104 mlgame-9.5.4.1b0/mlgame/view/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/view/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5667 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/view/decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12806 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/view/view.py
+-rw-r--r--   0 root         (0) root         (0)     6601 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/mlgame/view/view_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-19 06:37:37.263104 mlgame-9.5.4.1b0/mlgame.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4022 2022-08-19 06:37:37.000000 mlgame-9.5.4.1b0/mlgame.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1344 2022-08-19 06:37:37.000000 mlgame-9.5.4.1b0/mlgame.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-19 06:37:37.000000 mlgame-9.5.4.1b0/mlgame.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2022-08-19 06:37:37.000000 mlgame-9.5.4.1b0/mlgame.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2022-08-19 06:37:37.000000 mlgame-9.5.4.1b0/mlgame.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-19 06:37:37.271104 mlgame-9.5.4.1b0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1159 2022-08-19 06:37:03.000000 mlgame-9.5.4.1b0/setup.py
```

### Comparing `mlgame-9.5.3.2a0/PKG-INFO` & `mlgame-9.5.4.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlgame
-Version: 9.5.3.2a0
+Version: 9.5.4.1b0
 Summary: A machine learning game framework based on Pygame
 Home-page: https://github.com/PAIA-Playful-AI-Arena/MLGame
 Author: PAIA
 Author-email: service@paia-tech.com
 Keywords: AI,machine learning,game,framework
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mlgame-9.5.3.2a0/README.md` & `mlgame-9.5.4.1b0/README.md`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/games/fake_game_with_error/src/game.py` & `mlgame-9.5.4.1b0/mlgame/view/view_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,189 +1,232 @@
-import time
-from os import path
-import pygame
-
-from mlgame.gamedev.game_interface import PaiaGame, GameResultState, GameStatus
-from mlgame.tests.test_decorator import check_game_progress, check_game_result
-from mlgame.view.view_model import create_text_view_data, create_asset_init_data, create_image_view_data, Scene, \
-    create_scene_progress_data
-from .game_object import Ball, Food
-
-ASSET_PATH = path.join(path.dirname(__file__), "../asset")
-
-
-class EasyGame(PaiaGame):
-    """
-    This is a Interface of a game
-    """
-
-    def __init__(self, time_to_play, total_point_count, score, color):
-        super().__init__()
-        self.game_result_state = GameResultState.FAIL
-        self.scene = Scene(width=800, height=600, color="#4FC3F7", bias_x=0, bias_y=0)
-        print(color)
-        self.ball = Ball("#" + color)
-        self.foods = pygame.sprite.Group()
-        self.score = 0
-        self.score_to_win = score
-        self._create_foods(total_point_count)
-        self._begin_time = time.time()
-        self._timer = 0
-        self.frame_count = 0
-        self.time_limit = time_to_play
-
-    def update(self, commands):
-        # handle command
-        ai_1p_cmd = commands[self.ai_clients()[0]["name"]][0]
-        # print(ai_1p_cmd)
-        self.ball.update(ai_1p_cmd)
-
-        # update sprite
-        self.foods.update()
-        if self.frame_count > 10:
-            ai_1p_cmd[100] = "1"
-
-        # handle collision
-        hits = pygame.sprite.spritecollide(self.ball, self.foods, True, pygame.sprite.collide_rect_ratio(0.8))
-        if hits:
-            self.score += len(hits)
-            self._create_foods(len(hits))
-        self._timer = round(time.time() - self._begin_time, 3)
+import random
 
-        self.frame_count += 1
-        # self.draw()
 
-        if not self.is_running:
-            return "QUIT"
-
-    def game_to_player_data(self):
-        """
-        send something to game AI
-        we could send different data to different ai
+class Scene:
+    def __init__(self, width: int, height: int, color: str = "#000000", bias_x=0, bias_y=0):
         """
-        to_players_data = {}
-        foods_data = []
-        for food in self.foods:
-            foods_data.append({"x": food.rect.x, "y": food.rect.y})
-        data_to_1p = {
-            "frame": self.frame_count,
-            "ball_x": self.ball.rect.centerx,
-            "ball_y": self.ball.rect.centery,
-            "foods": foods_data,
-            "score": self.score,
-            "status": self.get_game_status()
-        }
+        This is a value object
+        :param width:
+        :param height:
+        :param color:
+        """
+        self.width = width
+        self.height = height
+        self.color = color
+        self.bias_x = bias_x
+        self.bias_y = bias_y
+
+
+def create_asset_init_data(image_id: str, width: int, height: int, file_path: str, github_raw_url: str):
+    # assert file_path is valid
+    return {
+        "type": "image",
+        "image_id": image_id,
+        "width": width,
+        "height": height,
+        "file_path": file_path,
+        "url": github_raw_url
+    }
+
+
+def create_scene_view_data(width: int, height: int, color: str = "#000000"):
+    return {
+        "width": width,
+        "height": height,
+        "color": color
+    }
+
+
+def create_scene_progress_data(frame: int = 0, background=None, object_list=None,
+                               toggle=None, toggle_with_bias=None, foreground=None, user_info=None,
+                               game_sys_info=None):
+    if background is None:
+        background = []
+    if object_list is None:
+        object_list = []
+    if toggle is None:
+        toggle = []
+    if toggle_with_bias is None:
+        toggle_with_bias = []
+    if foreground is None:
+        foreground = []
+    if user_info is None:
+        user_info = []
+    if game_sys_info is None:
+        game_sys_info = {}
+    return {
+        # background view data will be draw first
+        "frame": frame,
+        "background": background,
+        # game object view data will be draw on screen by order , and it could be shifted by WASD
+        "object_list": object_list,
+        "toggle_with_bias": toggle_with_bias,
+        "toggle": toggle,
+        "foreground": foreground,
+        # other information to display on web
+        "user_info": user_info,
+        # other information to display on web
+        "game_sys_info": game_sys_info
+    }
 
-        for ai_client in self.ai_clients():
-            to_players_data[ai_client['name']] = data_to_1p
-        # should be equal to config. GAME_SETUP["ml_clients"][0]["name"]
-
-        return to_players_data
-
-    def get_game_status(self):
-
-        if self.is_running:
-            status = GameStatus.GAME_ALIVE
-        elif self.score > self.score_to_win:
-            status = GameStatus.GAME_PASS
-        else:
-            status = GameStatus.GAME_OVER
-        return status
-
-    def reset(self):
-        pass
-
-    @property
-    def is_running(self):
-        return self.frame_count < self.time_limit
 
-    def get_scene_init_data(self):
-        """
-        Get the initial scene and object information for drawing on the web
-        """
-        # TODO add music or sound
-        bg_path = path.join(ASSET_PATH, "img/background.jpg")
-        background = create_asset_init_data("background", 800, 600, bg_path, "url")
-        scene_init_data = {"scene": self.scene.__dict__,
-                           "assets": [
-                               background
-                           ],
-                           # "audios": {}
-                           }
-        return scene_init_data
+def create_image_view_data(image_id, x, y, width, height, angle=0):
+    """
+    這是一個用來繪製圖片的資料格式，
+    "type"表示不同的類型
+    "x" "y" 表示物體左上角的座標
+    "width" "height"表示其大小
+    "image_id"表示其圖片的識別號，需在
+    "angle"表示其順時針旋轉的角度
+    """
+    return {"type": "image",
+            "x": x,
+            "y": y,
+            "width": width,
+            "height": height,
+            "image_id": image_id,
+            "angle": angle}
 
-    @check_game_progress
-    def get_scene_progress_data(self):
-        """
-        Get the position of game objects for drawing on the web
-        """
-        foods_data = []
-        for food in self.foods:
-            foods_data.append(food.game_object_data)
-        game_obj_list = [self.ball.game_object_data]
-        game_obj_list.extend(foods_data)
-        backgrounds = [create_image_view_data("background", 0, 0, 800, 600)]
-        foregrounds = [create_text_view_data(f"Score = {str(self.score)}", 650, 50, "#FF0000", "24px Arial BOLD")]
-        toggle_objs = [create_text_view_data(f"Timer = {str(self._timer)} s", 650, 100, "#FFAA00", "24px Arial")]
-        scene_progress = create_scene_progress_data(frame=self.frame_count, background=backgrounds,
-                                                    object_list=game_obj_list,
-                                                    foreground=foregrounds, toggle=toggle_objs)
-        return scene_progress
 
-    @check_game_result
-    def get_game_result(self):
-        """
-        send game result
-        """
-        if self.get_game_status() == GameStatus.GAME_PASS:
-            self.game_result_state = GameResultState.FINISH
-        return {"frame_used": self.frame_count,
-                "state": self.game_result_state,
-                "attachment": [
-                    {
-                        "player": self.ai_clients()[0]["name"],
-                        "rank": 1,
-                        "score": self.score
-                    }
-                ]
+def create_rect_view_data(name: str, x: int, y: int, width: int, height: int, color: str, angle: int = 0):
+    # TODO angle
+    """
+    這是一個用來繪製矩形的資料格式，
+    "type"表示不同的類型
+    "name"用來描述這個物件
+    "x""y"表示其位置，位置表示物體左上角的座標
+    "size"表示其大小
+    "image"表示其圖片
+    "angle"表示其順時針旋轉的角度
+    "color"以字串表示
+    :return:
+    """
+    return {"type": "rect",
+            "name": name,
+            "x": x,
+            "y": y,
+            "angle": angle,
+            "width": width,
+            "height": height,
+            "color": color
+            }
 
-                }
 
-    def get_keyboard_command(self):
-        """
-        Define how your game will run by your keyboard
-        """
-        cmd_1p = []
-        key_pressed_list = pygame.key.get_pressed()
-        if key_pressed_list[pygame.K_UP]:
-            cmd_1p.append("UP")
-        elif key_pressed_list[pygame.K_DOWN]:
-            cmd_1p.append("DOWN")
-        elif key_pressed_list[pygame.K_LEFT]:
-            cmd_1p.append("LEFT")
-        elif key_pressed_list[pygame.K_RIGHT]:
-            cmd_1p.append("RIGHT")
-        else:
-            cmd_1p.append("NONE")
-        ai_1p = self.ai_clients()[0]["name"]
-        return {ai_1p: cmd_1p}
-
-    def _create_foods(self, count: int = 5):
-        for i in range(count):
-            # add food to group
-            food = Food(self.foods)
-        pass
+def create_line_view_data(name: str, x1: int, y1: int, x2: int, y2: int, color: str, width: int = 2):
+    """
+    這是一個用來繪製直線的資料格式，
+    "x1","y1"表示起點位置，位置表示物體左上角的座標
+    "x2","y2"表示終點位置，位置表示物體左上角的座標
+    "color"以字串表示
+    "width" 表示寬度
+    :return:
+    """
+    return {"type": "line",
+            "name": name,
+            "x1": x1,
+            "y1": y1,
+            "x2": x2,
+            "y2": y2,
+            "width": width,
+            "color": color
+            }
 
-    @staticmethod
-    def ai_clients():
-        """
-        let MLGame know how to parse your ai,
-        you can also use this names to get different cmd and send different data to each ai client
-        """
-        return [
-            {"name": "1P",
-             "args": ('a'),
-             "kwargs": {
-                 "kw1": "1"
-             }
-             },
-        ]
+
+def create_polygon_view_data(name: str, points: list, color: str):
+    """
+    這是一個用來繪製多邊形的資料格式，
+    points欄位至少三個 # [[100,101],[52.1,31.3],[53.1,12.3]]
+    :return:dict
+    """
+    assert len(points) >= 3
+    vertices = []
+    for p in points:
+        vertices.append({"x": p[0], "y": p[1]})
+    return {"type": "polygon",
+            "name": name,
+            "color": color,
+            "points": vertices
+            }
+
+
+def create_text_view_data(content: str, x: int, y: int, color: str, font_style="24px Arial"):
+    return {
+        "type": "text",
+        "content": content,
+        "color": color,
+        "x": x,
+        "y": y,
+        "font-style": font_style
+    }
+
+
+def get_scene_init_sample_data() -> dict:
+    """
+    :rtype: dict
+    :return:  遊戲場景初始化的資料
+    """
+
+    scene = Scene(800, 600)
+    assets = [
+        {
+            "type": "image",
+            "image_id": 'car_01',
+            "width": 50,
+            "height": 50,
+            "url": 'https://raw.githubusercontent.com/yen900611/Maze_Car/master/game_core/image/car_01.png'
+        }, {
+            "type": "image",
+            "image_id": 'car_02',
+            "width": 50,
+            "height": 50,
+            "url": 'https://raw.githubusercontent.com/yen900611/Maze_Car/master/game_core/image/car_02.png'
+        }
+    ]
+
+    return {"scene": scene.__dict__,
+            "assets": assets,
+            # "audios": {}
+            }
+
+
+def get_dummy_progress_data():
+    background = create_image_view_data("background", 0, 0, 800, 600)
+    score_text = create_text_view_data("Score = 1", 650, 50, "#FF0000")
+    rect = create_rect_view_data("dummy_rect", 200, 300, 100, 200, "#FFFAAA", 30)
+    line = create_line_view_data("dummy_line", 10, 30, 100, 300, "#AAAFFF", 5)
+    points = gen_points(5)
+    polygon = create_polygon_view_data("dummy_polygon", points, "#FFAAFF")
+
+    scene_progress = {
+        # background view data will be draw first
+        "frame":1,
+        "background": [
+            background,
+
+        ],
+        # game object view data will be draw on screen by order , and it could be shifted by WASD
+        "object_list": [
+            rect,
+            line
+        ],
+        "toggle": [
+            polygon
+        ],
+        "foreground": [
+            score_text
+        ],
+        # other information to display on web
+        "user_info": [],
+        # other information to display on web
+        "game_sys_info": {}
+    }
+    return scene_progress
+
+
+def gen_points(point_num: int = 4) -> list:
+    """
+    points should be [x,y] ex [100.3,300.231]
+    """
+    result = []
+    for i in range(point_num):
+        result.append([random.randint(0, 100), random.randint(0, 100)])
+    return result
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mlgame-9.5.3.2a0/mlgame/LICIENCE.txt` & `mlgame-9.5.4.1b0/mlgame/LICIENCE.txt`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/__main__.py` & `mlgame-9.5.4.1b0/mlgame/__main__.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/argument/cmd_argument.py` & `mlgame-9.5.4.1b0/mlgame/argument/cmd_argument.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/argument/game_argument.py` & `mlgame-9.5.4.1b0/mlgame/argument/game_argument.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/argument/model.py` & `mlgame-9.5.4.1b0/mlgame/argument/model.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/argument/tool.py` & `mlgame-9.5.4.1b0/mlgame/argument/tool.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/core/communication.py` & `mlgame-9.5.4.1b0/mlgame/core/communication.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/core/exceptions.py` & `mlgame-9.5.4.1b0/mlgame/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/core/executor.py` & `mlgame-9.5.4.1b0/mlgame/core/executor.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/core/process.py` & `mlgame-9.5.4.1b0/mlgame/core/process.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/crosslang/client.py` & `mlgame-9.5.4.1b0/mlgame/crosslang/client.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/crosslang/compile/cpp/main.py` & `mlgame-9.5.4.1b0/mlgame/crosslang/compile/cpp/main.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/crosslang/exceptions.py` & `mlgame-9.5.4.1b0/mlgame/crosslang/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/crosslang/main.py` & `mlgame-9.5.4.1b0/mlgame/crosslang/main.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/game/generic.py` & `mlgame-9.5.4.1b0/mlgame/game/generic.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/game/paia_game.py` & `mlgame-9.5.4.1b0/mlgame/game/paia_game.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/game/physics.py` & `mlgame-9.5.4.1b0/mlgame/game/physics.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/tests/test_decorator.py` & `mlgame-9.5.4.1b0/mlgame/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/tests/test_game_argument.py` & `mlgame-9.5.4.1b0/mlgame/tests/test_game_argument.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/tests/test_tools.py` & `mlgame-9.5.4.1b0/mlgame/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/utils/enum.py` & `mlgame-9.5.4.1b0/mlgame/utils/enum.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/utils/recorder.py` & `mlgame-9.5.4.1b0/mlgame/utils/recorder.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/view/decorator.py` & `mlgame-9.5.4.1b0/mlgame/view/decorator.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame/view/view.py` & `mlgame-9.5.4.1b0/mlgame/view/view.py`

 * *Files identical despite different names*

### Comparing `mlgame-9.5.3.2a0/mlgame.egg-info/PKG-INFO` & `mlgame-9.5.4.1b0/mlgame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlgame
-Version: 9.5.3.2a0
+Version: 9.5.4.1b0
 Summary: A machine learning game framework based on Pygame
 Home-page: https://github.com/PAIA-Playful-AI-Arena/MLGame
 Author: PAIA
 Author-email: service@paia-tech.com
 Keywords: AI,machine learning,game,framework
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mlgame-9.5.3.2a0/setup.py` & `mlgame-9.5.4.1b0/setup.py`

 * *Files identical despite different names*

