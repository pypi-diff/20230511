# Comparing `tmp/mahjong-utils-0.5.0.post1.tar.gz` & `tmp/mahjong-utils-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mahjong-utils-0.5.0.post1.tar", last modified: Wed May 10 11:15:57 2023, max compression
+gzip compressed data, was "mahjong-utils-0.5.1.tar", last modified: Thu May 11 15:23:50 2023, max compression
```

## Comparing `mahjong-utils-0.5.0.post1.tar` & `mahjong-utils-0.5.1.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/
--rw-rw-rw-   0        0        0       61 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/MANIFEST.in
--rw-rw-rw-   0        0        0     9243 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/PKG-INFO
--rw-rw-rw-   0        0        0     8982 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/
--rw-rw-rw-   0        0        0       27 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/.git
--rw-rw-rw-   0        0        0     2272 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/.gitignore
--rw-rw-rw-   0        0        0     1085 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/LICENSE
--rw-rw-rw-   0        0        0     7412 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/build-scripts/
--rw-rw-rw-   0        0        0      219 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/build-scripts/build.gradle.kts
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.580586 mahjong-utils-0.5.0.post1/kt/build-scripts/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.580586 mahjong-utils-0.5.0.post1/kt/build-scripts/src/main/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/build-scripts/src/main/kotlin/
--rw-rw-rw-   0        0        0     3528 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/build-scripts/src/main/kotlin/build.publication.gradle.kts
--rw-rw-rw-   0        0        0     1341 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/build.gradle.kts
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.580586 mahjong-utils-0.5.0.post1/kt/gradle/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/gradle/wrapper/
--rw-rw-rw-   0        0        0    59821 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/gradle/wrapper/gradle-wrapper.jar
--rw-rw-rw-   0        0        0      207 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/gradle/wrapper/gradle-wrapper.properties
--rw-rw-rw-   0        0        0      160 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/gradle.properties
--rw-rw-rw-   0        0        0     8304 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/gradlew
--rwxrwxrwx   0        0        0     2763 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/gradlew.bat
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/kotlin-js-store/
--rw-rw-rw-   0        0        0   104679 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/kotlin-js-store/yarn.lock
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/
--rw-rw-rw-   0        0        0     2247 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/build.gradle.kts
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0      765 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Coders.kt
--rw-rw-rw-   0        0        0     3589 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Entry.kt
--rw-rw-rw-   0        0        0     2402 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Main.kt
--rw-rw-rw-   0        0        0     1098 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Models.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsMain/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsMain/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0     1468 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/Main.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsTest/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsTest/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0     6239 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/TestEntry.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeMain/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeMain/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0     1243 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/Main.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeTest/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeTest/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/
--rw-rw-rw-   0        0        0     5972 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/TestEntry.kt
--rw-rw-rw-   0        0        0      102 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/settings.gradle.kts
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/commonMain/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/common/
--rw-rw-rw-   0        0        0     5458 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/common/HandPatternUtils.kt
--rw-rw-rw-   0        0        0     7595 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/common/RegularHandSearcher.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hanhu/
--rw-rw-rw-   0        0        0     3866 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hanhu/PointByHanHu.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hora/
--rw-rw-rw-   0        0        0     6458 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hora/Hora.kt
--rw-rw-rw-   0        0        0     8108 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hora/HoraHandPattern.kt
--rw-rw-rw-   0        0        0      442 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hora/HoraInfo.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/
--rw-rw-rw-   0        0        0     3780 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Furo.kt
--rw-rw-rw-   0        0        0     4359 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Mentsu.kt
--rw-rw-rw-   0        0        0     6033 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Tatsu.kt
--rw-rw-rw-   0        0        0     8193 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Tile.kt
--rw-rw-rw-   0        0        0      308 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Wind.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/hand/
--rw-rw-rw-   0        0        0      412 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/hand/Hand.kt
--rw-rw-rw-   0        0        0     3482 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/hand/HandPattern.kt
--rw-rw-rw-   0        0        0      303 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/hand/IHasFuro.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.611836 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/
--rw-rw-rw-   0        0        0     3755 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/ChitoiShanten.kt
--rw-rw-rw-   0        0        0     6200 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/FuroChanceShanten.kt
--rw-rw-rw-   0        0        0     4268 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/KokushiShanten.kt
--rw-rw-rw-   0        0        0     4904 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/Models.kt
--rw-rw-rw-   0        0        0    10782 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/RegularShanten.kt
--rw-rw-rw-   0        0        0     6362 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/Shanten.kt
--rw-rw-rw-   0        0        0     3285 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/Utils.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/
--rw-rw-rw-   0        0        0     7774 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/CheckerFactory.kt
--rw-rw-rw-   0        0        0     1683 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/Yaku.kt
--rw-rw-rw-   0        0        0    10647 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/Yakus.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/jvmTest/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.596209 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/hanhu/
--rw-rw-rw-   0        0        0     2194 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/hanhu/TestPointByHanHu.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/hora/
--rw-rw-rw-   0        0        0     5806 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/hora/TestHora.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/shanten/
--rw-rw-rw-   0        0        0     2656 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestFuroChanceShanten.kt
--rw-rw-rw-   0        0        0    44661 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestShanten.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/
--rw-rw-rw-   0        0        0     9674 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYaku.kt
--rw-rw-rw-   0        0        0     6902 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYakuman.kt
--rw-rw-rw-   0        0        0      573 2023-05-10 11:14:19.000000 mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/Tester.kt
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/mahjong_utils/
--rw-rw-rw-   0        0        0      116 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/mahjong_utils/hora/
--rw-rw-rw-   0        0        0       44 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/hora/__init__.py
--rw-rw-rw-   0        0        0     2714 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/hora/hora.py
--rw-rw-rw-   0        0        0     6263 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/hora/models.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/mahjong_utils/lib/
--rw-rw-rw-   0        0        0     2209 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/lib/__init__.py
--rw-rw-rw-   0        0        0    22878 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/lib/libmahjongutils_api.i
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/mahjong_utils/models/
--rw-rw-rw-   0        0        0      176 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/__init__.py
--rw-rw-rw-   0        0        0     2765 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/furo.py
--rw-rw-rw-   0        0        0     1360 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/hand.py
--rw-rw-rw-   0        0        0     6769 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/hand_pattern.py
--rw-rw-rw-   0        0        0     3136 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/mentsu.py
--rw-rw-rw-   0        0        0     4718 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/tatsu.py
--rw-rw-rw-   0        0        0     6600 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/tile.py
--rw-rw-rw-   0        0        0      618 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/tile_type.py
--rw-rw-rw-   0        0        0      367 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/models/wind.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/mahjong_utils/point_by_han_hu/
--rw-rw-rw-   0        0        0       55 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/point_by_han_hu/__init__.py
--rw-rw-rw-   0        0        0      605 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/point_by_han_hu/models.py
--rw-rw-rw-   0        0        0      924 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/point_by_han_hu/point_by_han_hu.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/mahjong_utils/shanten/
--rw-rw-rw-   0        0        0       47 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/shanten/__init__.py
--rw-rw-rw-   0        0        0    12099 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/shanten/models.py
--rw-rw-rw-   0        0        0     4024 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/shanten/shanten.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/
--rw-rw-rw-   0        0        0      172 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/__init__.py
--rw-rw-rw-   0        0        0      543 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/all_yaku.py
--rw-rw-rw-   0        0        0     1353 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/common.py
--rw-rw-rw-   0        0        0      649 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/extra.py
--rw-rw-rw-   0        0        0      168 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/yaku.py
--rw-rw-rw-   0        0        0     1156 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/mahjong_utils/yaku/yakuman.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.627460 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/
--rw-rw-rw-   0        0        0     9243 2023-05-10 11:15:57.000000 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3932 2023-05-10 11:15:57.000000 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 11:15:57.000000 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-10 11:15:57.000000 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-05-10 11:15:57.000000 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-10 11:15:57.000000 mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/setup.cfg
--rw-rw-rw-   0        0        0     5025 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:15:57.643085 mahjong-utils-0.5.0.post1/tests/
--rw-rw-rw-   0        0        0     1221 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/tests/test_han_hu.py
--rw-rw-rw-   0        0        0     5422 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/tests/test_hora.py
--rw-rw-rw-   0        0        0      297 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/tests/test_lib.py
--rw-rw-rw-   0        0        0     8938 2023-05-10 11:14:18.000000 mahjong-utils-0.5.0.post1/tests/test_shanten.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.091980 mahjong-utils-0.5.1/
+-rw-rw-rw-   0        0        0       61 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     9237 2023-05-11 15:23:50.091980 mahjong-utils-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8982 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.014006 mahjong-utils-0.5.1/kt/
+-rw-rw-rw-   0        0        0       27 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/.git
+-rw-rw-rw-   0        0        0     2272 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/.gitignore
+-rw-rw-rw-   0        0        0     1085 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/LICENSE
+-rw-rw-rw-   0        0        0     7412 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.014006 mahjong-utils-0.5.1/kt/build-scripts/
+-rw-rw-rw-   0        0        0      219 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/build-scripts/build.gradle.kts
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/build-scripts/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/build-scripts/src/main/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.014006 mahjong-utils-0.5.1/kt/build-scripts/src/main/kotlin/
+-rw-rw-rw-   0        0        0     3528 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/build-scripts/src/main/kotlin/build.publication.gradle.kts
+-rw-rw-rw-   0        0        0     1341 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/build.gradle.kts
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/gradle/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.014006 mahjong-utils-0.5.1/kt/gradle/wrapper/
+-rw-rw-rw-   0        0        0    59821 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/gradle/wrapper/gradle-wrapper.jar
+-rw-rw-rw-   0        0        0      207 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/gradle/wrapper/gradle-wrapper.properties
+-rw-rw-rw-   0        0        0      160 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/gradle.properties
+-rw-rw-rw-   0        0        0     8304 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/gradlew
+-rwxrwxrwx   0        0        0     2763 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/gradlew.bat
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.014006 mahjong-utils-0.5.1/kt/kotlin-js-store/
+-rw-rw-rw-   0        0        0   104679 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/kotlin-js-store/yarn.lock
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.014006 mahjong-utils-0.5.1/kt/mahjong-utils-entry/
+-rw-rw-rw-   0        0        0     2247 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/mahjong-utils-entry/build.gradle.kts
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/commonMain/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/commonMain/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.014006 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0      765 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Coders.kt
+-rw-rw-rw-   0        0        0     3589 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Entry.kt
+-rw-rw-rw-   0        0        0     2402 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Main.kt
+-rw-rw-rw-   0        0        0     1098 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Models.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/jsMain/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/jsMain/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.014006 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0     1468 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/Main.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/jsTest/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/jsTest/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.014006 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0     6239 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/TestEntry.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/nativeMain/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/nativeMain/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.014006 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0     1243 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/Main.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/nativeTest/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/nativeTest/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.014006 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/
+-rw-rw-rw-   0        0        0     5972 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/TestEntry.kt
+-rw-rw-rw-   0        0        0      102 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/settings.gradle.kts
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/src/commonMain/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.029549 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/common/
+-rw-rw-rw-   0        0        0     5458 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/common/HandPatternUtils.kt
+-rw-rw-rw-   0        0        0     7595 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/common/RegularHandSearcher.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.030060 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/hanhu/
+-rw-rw-rw-   0        0        0     3866 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/hanhu/PointByHanHu.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.030060 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/hora/
+-rw-rw-rw-   0        0        0     6458 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/hora/Hora.kt
+-rw-rw-rw-   0        0        0     8108 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/hora/HoraHandPattern.kt
+-rw-rw-rw-   0        0        0      442 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/hora/HoraInfo.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.030060 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/
+-rw-rw-rw-   0        0        0     3780 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/Furo.kt
+-rw-rw-rw-   0        0        0     4359 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/Mentsu.kt
+-rw-rw-rw-   0        0        0     6033 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/Tatsu.kt
+-rw-rw-rw-   0        0        0     8193 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/Tile.kt
+-rw-rw-rw-   0        0        0      308 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/Wind.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.030060 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/hand/
+-rw-rw-rw-   0        0        0      412 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/hand/Hand.kt
+-rw-rw-rw-   0        0        0     3482 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/hand/HandPattern.kt
+-rw-rw-rw-   0        0        0      303 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/hand/IHasFuro.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.030060 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/
+-rw-rw-rw-   0        0        0     3755 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/ChitoiShanten.kt
+-rw-rw-rw-   0        0        0     6200 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/FuroChanceShanten.kt
+-rw-rw-rw-   0        0        0     4268 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/KokushiShanten.kt
+-rw-rw-rw-   0        0        0     5443 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/Models.kt
+-rw-rw-rw-   0        0        0    11574 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/RegularShanten.kt
+-rw-rw-rw-   0        0        0     6527 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/Shanten.kt
+-rw-rw-rw-   0        0        0     3706 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/Utils.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.045073 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/yaku/
+-rw-rw-rw-   0        0        0     7774 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/yaku/CheckerFactory.kt
+-rw-rw-rw-   0        0        0     1683 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/yaku/Yaku.kt
+-rw-rw-rw-   0        0        0    10647 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/yaku/Yakus.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/src/jvmTest/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.982468 mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:49.998093 mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.045073 mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/hanhu/
+-rw-rw-rw-   0        0        0     2194 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/hanhu/TestPointByHanHu.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.045073 mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/hora/
+-rw-rw-rw-   0        0        0     5806 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/hora/TestHora.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.045073 mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/shanten/
+-rw-rw-rw-   0        0        0     2657 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestFuroChanceShanten.kt
+-rw-rw-rw-   0        0        0    60157 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestShanten.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.045073 mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/yaku/
+-rw-rw-rw-   0        0        0     9674 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYaku.kt
+-rw-rw-rw-   0        0        0     6902 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYakuman.kt
+-rw-rw-rw-   0        0        0      573 2023-05-11 15:20:45.000000 mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/yaku/Tester.kt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.045073 mahjong-utils-0.5.1/mahjong_utils/
+-rw-rw-rw-   0        0        0      116 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.061270 mahjong-utils-0.5.1/mahjong_utils/hora/
+-rw-rw-rw-   0        0        0       44 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/hora/__init__.py
+-rw-rw-rw-   0        0        0     2714 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/hora/hora.py
+-rw-rw-rw-   0        0        0     6263 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/hora/models.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.061270 mahjong-utils-0.5.1/mahjong_utils/lib/
+-rw-rw-rw-   0        0        0     2209 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/lib/__init__.py
+-rw-rw-rw-   0        0        0    22878 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/lib/libmahjongutils_api.i
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.076342 mahjong-utils-0.5.1/mahjong_utils/models/
+-rw-rw-rw-   0        0        0      176 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/models/__init__.py
+-rw-rw-rw-   0        0        0     2765 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/models/furo.py
+-rw-rw-rw-   0        0        0     1360 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/models/hand.py
+-rw-rw-rw-   0        0        0     6769 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/models/hand_pattern.py
+-rw-rw-rw-   0        0        0     3136 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/models/mentsu.py
+-rw-rw-rw-   0        0        0     4718 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/models/tatsu.py
+-rw-rw-rw-   0        0        0     6600 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/models/tile.py
+-rw-rw-rw-   0        0        0      618 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/models/tile_type.py
+-rw-rw-rw-   0        0        0      367 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/models/wind.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.076342 mahjong-utils-0.5.1/mahjong_utils/point_by_han_hu/
+-rw-rw-rw-   0        0        0       55 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/point_by_han_hu/__init__.py
+-rw-rw-rw-   0        0        0      605 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/point_by_han_hu/models.py
+-rw-rw-rw-   0        0        0      924 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/point_by_han_hu/point_by_han_hu.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.076342 mahjong-utils-0.5.1/mahjong_utils/shanten/
+-rw-rw-rw-   0        0        0       47 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/shanten/__init__.py
+-rw-rw-rw-   0        0        0    13179 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/shanten/models.py
+-rw-rw-rw-   0        0        0     4024 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/shanten/shanten.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.076342 mahjong-utils-0.5.1/mahjong_utils/yaku/
+-rw-rw-rw-   0        0        0      172 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/yaku/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/yaku/all_yaku.py
+-rw-rw-rw-   0        0        0     1353 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/yaku/common.py
+-rw-rw-rw-   0        0        0      649 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/yaku/extra.py
+-rw-rw-rw-   0        0        0      168 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/yaku/yaku.py
+-rw-rw-rw-   0        0        0     1156 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/mahjong_utils/yaku/yakuman.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.061270 mahjong-utils-0.5.1/mahjong_utils.egg-info/
+-rw-rw-rw-   0        0        0     9237 2023-05-11 15:23:49.000000 mahjong-utils-0.5.1/mahjong_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3932 2023-05-11 15:23:49.000000 mahjong-utils-0.5.1/mahjong_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 15:23:49.000000 mahjong-utils-0.5.1/mahjong_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-11 15:23:49.000000 mahjong-utils-0.5.1/mahjong_utils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-05-11 15:23:49.000000 mahjong-utils-0.5.1/mahjong_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-11 15:23:49.000000 mahjong-utils-0.5.1/mahjong_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-11 15:23:50.091980 mahjong-utils-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     5019 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:23:50.091980 mahjong-utils-0.5.1/tests/
+-rw-rw-rw-   0        0        0     1221 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/tests/test_han_hu.py
+-rw-rw-rw-   0        0        0     5422 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/tests/test_hora.py
+-rw-rw-rw-   0        0        0      297 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/tests/test_lib.py
+-rw-rw-rw-   0        0        0     8938 2023-05-11 15:20:43.000000 mahjong-utils-0.5.1/tests/test_shanten.py
```

### Comparing `mahjong-utils-0.5.0.post1/PKG-INFO` & `mahjong-utils-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mahjong-utils
-Version: 0.5.0.post1
+Version: 0.5.1
 Summary: 日麻小工具
 Home-page: https://github.com/ssttkkl/mahjong-utils
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `mahjong-utils-0.5.0.post1/README.md` & `mahjong-utils-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/.gitignore` & `mahjong-utils-0.5.1/kt/.gitignore`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/LICENSE` & `mahjong-utils-0.5.1/kt/LICENSE`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/README.md` & `mahjong-utils-0.5.1/kt/README.md`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/build-scripts/src/main/kotlin/build.publication.gradle.kts` & `mahjong-utils-0.5.1/kt/build-scripts/src/main/kotlin/build.publication.gradle.kts`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/build.gradle.kts` & `mahjong-utils-0.5.1/kt/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/gradle/wrapper/gradle-wrapper.jar` & `mahjong-utils-0.5.1/kt/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/gradlew` & `mahjong-utils-0.5.1/kt/gradlew`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/gradlew.bat` & `mahjong-utils-0.5.1/kt/gradlew.bat`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/kotlin-js-store/yarn.lock` & `mahjong-utils-0.5.1/kt/kotlin-js-store/yarn.lock`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/build.gradle.kts` & `mahjong-utils-0.5.1/kt/mahjong-utils-entry/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Coders.kt` & `mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Coders.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Entry.kt` & `mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Entry.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Main.kt` & `mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Main.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Models.kt` & `mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/commonMain/kotlin/mahjongutils/Models.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/Main.kt` & `mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/jsMain/kotlin/mahjongutils/Main.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/TestEntry.kt` & `mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/jsTest/kotlin/mahjongutils/TestEntry.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/Main.kt` & `mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/nativeMain/kotlin/mahjongutils/Main.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/TestEntry.kt` & `mahjong-utils-0.5.1/kt/mahjong-utils-entry/src/nativeTest/kotlin/mahjongutils/TestEntry.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/common/HandPatternUtils.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/common/HandPatternUtils.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/common/RegularHandSearcher.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/common/RegularHandSearcher.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hanhu/PointByHanHu.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/hanhu/PointByHanHu.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hora/Hora.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/hora/Hora.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/hora/HoraHandPattern.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/hora/HoraHandPattern.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Furo.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/Furo.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Mentsu.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/Mentsu.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Tatsu.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/Tatsu.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/Tile.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/Tile.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/models/hand/HandPattern.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/models/hand/HandPattern.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/ChitoiShanten.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/ChitoiShanten.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/FuroChanceShanten.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/FuroChanceShanten.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/KokushiShanten.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/KokushiShanten.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/Models.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/Models.kt`

 * *Files 3% similar despite different names*

```diff
@@ -67,20 +67,31 @@
      */
     @EncodeDefault val goodShapeAdvanceNum: Int? = if (shantenNum == 1) 0 else null,
     /**
      * 改良张（能让听牌数目增加的牌）
      * 对于每种改良张，只计算能让进张最多的打法
      * 仅当听牌时进行计算
      */
-    @EncodeDefault val improvement: Map<Tile, Set<Improvement>>? = if (shantenNum == 0) emptyMap() else null,
+    @EncodeDefault val improvement: Map<Tile, List<Improvement>>? = if (shantenNum == 0) emptyMap() else null,
     /**
      * 改良张数（能让听牌数目增加的牌）
      * 仅当听牌时进行计算
      */
-    @EncodeDefault val improvementNum: Int? = if (shantenNum == 0) 0 else null
+    @EncodeDefault val improvementNum: Int? = if (shantenNum == 0) 0 else null,
+    /**
+     * 好型改良张（能让听牌数目增加到大于4张的牌）
+     * 对于每种改良张，只计算能让进张最多的打法
+     * 仅当听牌时进行计算
+     */
+    @EncodeDefault val goodShapeImprovement: Map<Tile, List<Improvement>>? = if (shantenNum == 0) emptyMap() else null,
+    /**
+     * 好型改良张数（能让听牌数目增加到大于4张的牌）
+     * 仅当听牌时进行计算
+     */
+    @EncodeDefault val goodShapeImprovementNum: Int? = if (shantenNum == 0) 0 else null,
 ) : CommonShanten
 
 /**
  * 摸牌的手牌的向听信息
  */
 @Serializable
 @SerialName("ShantenWithGot")
```

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/RegularShanten.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/RegularShanten.kt`

 * *Files 4% similar despite different names*

```diff
@@ -35,33 +35,33 @@
             if (maxAdvAfterAdv.advanceNum > 4) {
                 add(adv)
             }
         }
     }
 }
 
-private fun getImprovement(
+private fun ShantenWithoutGot.fillImprovement(
     tiles: List<Tile>,
     furo: List<Furo>,
     remaining: IntArray,
     shantenNum: Int,
     advanceMoreThan: Int,
     tryAllTile: Boolean = false
-): Map<Tile, Set<Improvement>> {
+): ShantenWithoutGot {
     val zone = if (!tryAllTile) {
         // 解空间为所有数牌的靠张
         tiles.filter { it.type !== TileType.Z }
             .flatMap { TILE_CLING[it] ?: emptyList() }
             .toSet()
             .filter { remaining[it.code] > 0 }
     } else {
         Tile.allExcludeAkaDora
     }
 
-    return zone.mapNotNull { t ->
+    val improvement = zone.mapNotNull { t ->
         // 摸上这张牌之后的向听信息
         val (shantenAfterGot, _) = handleRegularShantenWithGot(
             tiles + t, furo,
             bestShantenOnly = true,
             calcImprovement = false,
             calcGoodShapeAdvance = false,
             allowAnkan = false
@@ -80,26 +80,33 @@
             // 此时还未计算advanceNum
             val advanceNum = improvedShanten.advance.sumOf { remaining[it.code] }
             if (advanceNum > maxAdvanceNum) {
                 improvement = mutableListOf()
                 maxAdvanceNum = advanceNum
             }
             if (advanceNum == maxAdvanceNum) {
-                improvement.add(Improvement(discard, improvedShanten.advance))
+                improvement.add(Improvement(discard, improvedShanten.advance, advanceNum))
             }
         }
 
         remaining[t.code] += 1
 
+        // 保证顺序（为了单测）
+        improvement.sortBy { it.discard }
+
         if (maxAdvanceNum != advanceMoreThan) {
-            Pair(t, improvement.toSet())
+            Pair(t, improvement)
         } else {
             null
         }
     }.associate { it }
+
+    val goodShapeImprovement = improvement.filterValues { it.first().advanceNum >= 5 }
+
+    return copy(improvement = improvement, goodShapeImprovement = goodShapeImprovement)
 }
 
 private fun handleRegularShantenWithoutGot(
     tiles: List<Tile>, furo: List<Furo>,
     calcGoodShapeAdvance: Boolean = true,
     calcImprovement: Boolean = true
 ): Pair<ShantenWithoutGot, Collection<RegularHandPattern>> {
@@ -114,29 +121,37 @@
     // 一向听时计算好型进张
     val goodShape = if (calcGoodShapeAdvance && bestShanten == 1) {
         getGoodShapeAdvance(tiles, furo, remaining, advance)
     } else {
         null
     }
 
-    // 听牌时计算改良张
-    val improvement = if (calcImprovement && bestShanten == 0) {
-        val advanceNum = advance.sumOf { remaining[it.code] }
-        val tryAllTile = bestPatterns.any { it.remaining.isNotEmpty() }  // 如果有单吊听牌就计算换听
-        getImprovement(tiles, furo, remaining, bestShanten, advanceNum, tryAllTile)
-    } else {
-        null
-    }
-
-    val shanten = ShantenWithoutGot(
+    var shanten = ShantenWithoutGot(
         shantenNum = bestShanten,
         advance = advance,
-        goodShapeAdvance = goodShape,
-        improvement = improvement
+        goodShapeAdvance = goodShape
     )
+
+    // 听牌时计算改良张
+    if (bestShanten == 0) {
+        shanten = if (calcImprovement) {
+            val advanceNum = advance.sumOf { remaining[it.code] }
+            val tryAllTile = bestPatterns.any { it.remaining.isNotEmpty() }  // 如果有单吊听牌就计算换听
+
+            shanten.fillImprovement(tiles, furo, remaining, bestShanten, advanceNum, tryAllTile)
+        } else {
+            shanten.copy(
+                improvement = null,
+                improvementNum = null,
+                goodShapeImprovement = null,
+                goodShapeImprovementNum = null
+            )
+        }
+    }
+
     return Pair(shanten, bestPatterns)
 }
 
 private fun handleRegularShantenWithGot(
     tiles: List<Tile>, furo: List<Furo>,
     calcGoodShapeAdvance: Boolean = true,
     bestShantenOnly: Boolean = false,
@@ -173,29 +188,38 @@
             // 一向听时计算好型进张
             val goodShape = if (calcGoodShapeAdvance && bestShanten == 1) {
                 getGoodShapeAdvance(tiles - discard, furo, remaining, advance)
             } else {
                 null
             }
 
-            // 听牌时计算改良张
-            val improvement = if (calcImprovement && bestShanten == 0) {
-                val advanceNum = advance.sumOf { remaining[it.code] }
-                val tryAllTile = bestPatterns.any { it.remaining.any { it != discard } }  // 如果有单吊听牌就计算换听
-                getImprovement(tiles - discard, furo, remaining, bestShanten, advanceNum, tryAllTile)
-            } else {
-                null
-            }
-
-            this[discard] = ShantenWithoutGot(
+            var shanten = ShantenWithoutGot(
                 shantenNum = bestShanten,
                 advance = advance,
-                goodShapeAdvance = goodShape,
-                improvement = improvement
+                goodShapeAdvance = goodShape
             )
+
+            // 听牌时计算改良张
+            if (bestShanten == 0) {
+                shanten = if (calcImprovement) {
+                    val advanceNum = advance.sumOf { remaining[it.code] }
+                    val tryAllTile = bestPatterns.any { it.remaining.any { it != discard } }  // 如果有单吊听牌就计算换听
+
+                    shanten.fillImprovement(tiles - discard, furo, remaining, bestShanten, advanceNum, tryAllTile)
+                } else {
+                    shanten.copy(
+                        improvement = null,
+                        improvementNum = null,
+                        goodShapeImprovement = null,
+                        goodShapeImprovementNum = null
+                    )
+                }
+            }
+
+            this[discard] = shanten
         }
 
         this
     }
 
     // 再计算退向的打法
     if (!bestShantenOnly) {
```

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/Shanten.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/Shanten.kt`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,16 @@
         mergeIntoWithoutGot(shantenNum, advance, goodShapeAdvance, patterns, chitoi)
         mergeIntoWithoutGot(shantenNum, advance, goodShapeAdvance, patterns, kokushi)
 
         ShantenWithoutGot(
             shantenNum, advance,
             goodShapeAdvance = if (shantenNum == 1) goodShapeAdvance else null,
             improvement = (regular.shantenInfo as ShantenWithoutGot).improvement
+                ?: (if (shantenNum == 0) emptyMap() else null),
+            goodShapeImprovement = (regular.shantenInfo as ShantenWithoutGot).goodShapeImprovement
                 ?: (if (shantenNum == 0) emptyMap() else null)
         )
     } else {
         val discardToAdvance = HashMap<Tile, ShantenWithoutGot>()
 
         mergeIntoWithGot(shantenNum, discardToAdvance, patterns, regular, bestShantenOnly)
         mergeIntoWithGot(shantenNum, discardToAdvance, patterns, chitoi, bestShantenOnly)
```

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/shanten/Utils.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/shanten/Utils.kt`

 * *Files 4% similar despite different names*

```diff
@@ -76,20 +76,28 @@
     return when (this) {
         is ShantenWithoutGot -> {
             copy(
                 advanceNum = advance.sumOf { remaining[it.code] },
                 goodShapeAdvanceNum = goodShapeAdvance?.sumOf { remaining[it.code] },
                 improvement = improvement?.mapValues { (k, v) ->
                     remaining[k.code] -= 1
-                    val v = v.map { imp -> imp.copy(advanceNum = imp.advance.sumOf { remaining[it.code] }) }.toSet()
+                    val v = v.map { imp -> imp.copy(advanceNum = imp.advance.sumOf { remaining[it.code] }) }
                     remaining[k.code] += 1
 
                     v
                 },
-                improvementNum = improvement?.keys?.sumOf { remaining[it.code] }
+                goodShapeImprovement = goodShapeImprovement?.mapValues { (k, v) ->
+                    remaining[k.code] -= 1
+                    val v = v.map { imp -> imp.copy(advanceNum = imp.advance.sumOf { remaining[it.code] }) }
+                    remaining[k.code] += 1
+
+                    v
+                },
+                improvementNum = improvement?.keys?.sumOf { remaining[it.code] },
+                goodShapeImprovementNum = goodShapeImprovement?.keys?.sumOf { remaining[it.code] },
             ) as T
         }
 
         is ShantenWithGot -> {
             copy(
                 discardToAdvance = discardToAdvance.mapValues { (_, v) -> v.fillNumByRemaining(remaining) },
                 ankanToAdvance = ankanToAdvance.mapValues { (_, v) -> v.fillNumByRemaining(remaining) },
```

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/CheckerFactory.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/yaku/CheckerFactory.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/Yaku.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/yaku/Yaku.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/commonMain/kotlin/mahjongutils/yaku/Yakus.kt` & `mahjong-utils-0.5.1/kt/src/commonMain/kotlin/mahjongutils/yaku/Yakus.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/hanhu/TestPointByHanHu.kt` & `mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/hanhu/TestPointByHanHu.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/hora/TestHora.kt` & `mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/hora/TestHora.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestFuroChanceShanten.kt` & `mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestFuroChanceShanten.kt`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                 shantenNum = 0,
                 discardToAdvance = mapOf(
                     Tile.get("8m") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = setOf(),
                         advanceNum = 0,
                         improvement = Tile.allExcludeAkaDora.filter { it !== Tile.get("9m") }.associateWith {
-                            setOf(
+                            listOf(
                                 Improvement(
                                     discard = Tile.get("9m"),
                                     advance = setOf(it),
                                     advanceNum = if (it == Tile.get("8m")) 2 else 3
                                 )
                             )
                         },
```

### Comparing `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestShanten.kt` & `mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/shanten/TestShanten.kt`

 * *Files 16% similar despite different names*

```diff
@@ -118,58 +118,103 @@
         )
         tester(
             "22s23455666p345m", ShantenWithoutGot(
                 shantenNum = 0,
                 advance = Tile.parseTiles("5p2s").toSet(),
                 advanceNum = 4,
                 improvement = mapOf(
-                    Tile.get("1p") to setOf(
+                    Tile.get("1p") to listOf(
                         Improvement(
                             discard = Tile.Companion.get("6p"),
                             advance = Tile.parseTiles("47p").toSet(),
                             advanceNum = 7
                         )
                     ),
-                    Tile.get("3p") to setOf(
+                    Tile.get("3p") to listOf(
                         Improvement(
                             discard = Tile.Companion.get("5p"),
                             advance = Tile.parseTiles("14p").toSet(),
                             advanceNum = 7
                         )
                     ),
-                    Tile.get("4p") to setOf(
+                    Tile.get("4p") to listOf(
                         Improvement(
                             discard = Tile.Companion.get("6p"),
                             advance = Tile.parseTiles("147p").toSet(),
                             advanceNum = 10
                         )
                     ),
-                    Tile.get("6p") to setOf(
+                    Tile.get("6p") to listOf(
                         Improvement(
                             discard = Tile.Companion.get("5p"),
                             advance = Tile.parseTiles("147p").toSet(),
                             advanceNum = 11
                         )
                     ),
-                    Tile.get("7p") to setOf(
+                    Tile.get("7p") to listOf(
                         Improvement(
                             discard = Tile.Companion.get("6p"),
                             advance = Tile.parseTiles("147p").toSet(),
                             advanceNum = 10
                         )
                     ),
-                    Tile.get("3s") to setOf(
+                    Tile.get("3s") to listOf(
                         Improvement(
                             discard = Tile.Companion.get("2s"),
                             advance = Tile.parseTiles("14s").toSet(),
                             advanceNum = 8
                         )
                     ),
                 ),
-                improvementNum = 19
+                improvementNum = 19,
+                goodShapeImprovement = mapOf(
+                    Tile.get("1p") to listOf(
+                        Improvement(
+                            discard = Tile.Companion.get("6p"),
+                            advance = Tile.parseTiles("47p").toSet(),
+                            advanceNum = 7
+                        )
+                    ),
+                    Tile.get("3p") to listOf(
+                        Improvement(
+                            discard = Tile.Companion.get("5p"),
+                            advance = Tile.parseTiles("14p").toSet(),
+                            advanceNum = 7
+                        )
+                    ),
+                    Tile.get("4p") to listOf(
+                        Improvement(
+                            discard = Tile.Companion.get("6p"),
+                            advance = Tile.parseTiles("147p").toSet(),
+                            advanceNum = 10
+                        )
+                    ),
+                    Tile.get("6p") to listOf(
+                        Improvement(
+                            discard = Tile.Companion.get("5p"),
+                            advance = Tile.parseTiles("147p").toSet(),
+                            advanceNum = 11
+                        )
+                    ),
+                    Tile.get("7p") to listOf(
+                        Improvement(
+                            discard = Tile.Companion.get("6p"),
+                            advance = Tile.parseTiles("147p").toSet(),
+                            advanceNum = 10
+                        )
+                    ),
+                    Tile.get("3s") to listOf(
+                        Improvement(
+                            discard = Tile.Companion.get("2s"),
+                            advance = Tile.parseTiles("14s").toSet(),
+                            advanceNum = 8
+                        )
+                    ),
+                ),
+                goodShapeImprovementNum = 19
             )
         )
         tester(
             "1112345678999p", ShantenWithoutGot(
                 shantenNum = 0,
                 advance = Tile.parseTiles("123456789p").toSet(),
                 advanceNum = 23,
@@ -234,196 +279,359 @@
                         advanceNum = 11
                     ),
                     Tile.get("2s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("1357s").toSet(),
                         advanceNum = 9,
                         improvement = mapOf(
-                            Tile.get("2s") to setOf(
+                            Tile.get("2s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 11
+                                )
+                            ),
+                            Tile.get("6s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("12567s").toSet(),
+                                    advanceNum = 12
+                                )
+                            ),
+                        ),
+                        improvementNum = 5,
+                        goodShapeImprovement = mapOf(
+                            Tile.get("2s") to listOf(
                                 Improvement(
                                     discard = Tile.get("3s"),
                                     advance = Tile.parseTiles("1567s").toSet(),
                                     advanceNum = 11
                                 )
                             ),
-                            Tile.get("6s") to setOf(
+                            Tile.get("6s") to listOf(
                                 Improvement(
                                     discard = Tile.get("3s"),
                                     advance = Tile.parseTiles("12567s").toSet(),
                                     advanceNum = 12
                                 )
                             ),
                         ),
-                        improvementNum = 5
+                        goodShapeImprovementNum = 5
                     ),
                     Tile.get("5s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("17s").toSet(),
                         advanceNum = 7,
                         improvement = mapOf(
-                            Tile.get("2s") to setOf(
+                            Tile.get("2s") to listOf(
                                 Improvement(
                                     discard = Tile.get("1s"),
                                     advance = Tile.parseTiles("23567s").toSet(),
                                     advanceNum = 10
                                 )
                             ),
-                            Tile.get("3s") to setOf(
+                            Tile.get("3s") to listOf(
                                 Improvement(
                                     discard = Tile.get("1s"),
                                     advance = Tile.parseTiles("267s").toSet(),
                                     advanceNum = 9
                                 ),
                                 Improvement(
                                     discard = Tile.get("5s"),
                                     advance = Tile.parseTiles("127s").toSet(),
                                     advanceNum = 9
                                 ),
                             ),
-                            Tile.get("5s") to setOf(
+                            Tile.get("5s") to listOf(
                                 Improvement(
                                     discard = Tile.get("3s"),
                                     advance = Tile.parseTiles("1567s").toSet(),
                                     advanceNum = 10
                                 )
                             ),
-                            Tile.get("6s") to setOf(
+                            Tile.get("6s") to listOf(
                                 Improvement(
                                     discard = Tile.get("3s"),
                                     advance = Tile.parseTiles("1567s").toSet(),
                                     advanceNum = 10
                                 )
                             ),
                         ),
-                        improvementNum = 7
+                        improvementNum = 7,
+                        goodShapeImprovement = mapOf(
+                            Tile.get("2s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("1s"),
+                                    advance = Tile.parseTiles("23567s").toSet(),
+                                    advanceNum = 10
+                                )
+                            ),
+                            Tile.get("3s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("1s"),
+                                    advance = Tile.parseTiles("267s").toSet(),
+                                    advanceNum = 9
+                                ),
+                                Improvement(
+                                    discard = Tile.get("5s"),
+                                    advance = Tile.parseTiles("127s").toSet(),
+                                    advanceNum = 9
+                                ),
+                            ),
+                            Tile.get("5s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 10
+                                )
+                            ),
+                            Tile.get("6s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 10
+                                )
+                            ),
+                        ),
+                        goodShapeImprovementNum = 7
                     ),
                     Tile.get("6s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("1235s").toSet(),
                         advanceNum = 7,
                         improvement = mapOf(
-                            Tile.get("6s") to setOf(
+                            Tile.get("6s") to listOf(
                                 Improvement(
                                     discard = Tile.get("3s"),
                                     advance = Tile.parseTiles("1567s").toSet(),
                                     advanceNum = 10
                                 )
                             )
                         ),
-                        improvementNum = 3
+                        improvementNum = 3,
+                        goodShapeImprovement = mapOf(
+                            Tile.get("6s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 10
+                                )
+                            )
+                        ),
+                        goodShapeImprovementNum = 3
                     ),
                     Tile.get("1s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("25s").toSet(),
                         advanceNum = 3,
                         improvement = mapOf(
-                            Tile.get("1s") to setOf(
+                            Tile.get("1s") to listOf(
                                 Improvement(
                                     discard = Tile.get("3s"),
                                     advance = Tile.parseTiles("1567s").toSet(),
                                     advanceNum = 10
                                 )
                             ),
-                            Tile.get("3s") to setOf(
+                            Tile.get("3s") to listOf(
                                 Improvement(
                                     discard = Tile.get("2s"),
                                     advance = Tile.parseTiles("1567s").toSet(),
                                     advanceNum = 11
                                 )
                             ),
-                            Tile.get("4s") to setOf(
+                            Tile.get("4s") to listOf(
                                 Improvement(
                                     discard = Tile.get("3s"),
                                     advance = Tile.parseTiles("12567s").toSet(),
                                     advanceNum = 13
                                 ),
                                 Improvement(
                                     discard = Tile.get("5s"),
                                     advance = Tile.parseTiles("12367s").toSet(),
                                     advanceNum = 13
                                 )
                             ),
-                            Tile.get("6s") to setOf(
+                            Tile.get("6s") to listOf(
                                 Improvement(
                                     discard = Tile.get("5s"),
                                     advance = Tile.parseTiles("2367s").toSet(),
                                     advanceNum = 9
                                 )
                             ),
-                            Tile.get("7s") to setOf(
+                            Tile.get("7s") to listOf(
                                 Improvement(
                                     discard = Tile.get("2s"),
                                     advance = Tile.parseTiles("13578s").toSet(),
                                     advanceNum = 12
                                 ),
                                 Improvement(
                                     discard = Tile.get("5s"),
                                     advance = Tile.parseTiles("12367s").toSet(),
                                     advanceNum = 12
                                 ),
                             ),
-                            Tile.get("8s") to setOf(
+                            Tile.get("8s") to listOf(
                                 Improvement(
                                     discard = Tile.get("2s"),
                                     advance = Tile.parseTiles("78s").toSet(),
                                     advanceNum = 7
                                 )
                             ),
                         ),
-                        improvementNum = 15
+                        improvementNum = 15,
+                        goodShapeImprovement = mapOf(
+                            Tile.get("1s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 10
+                                )
+                            ),
+                            Tile.get("3s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("2s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 11
+                                )
+                            ),
+                            Tile.get("4s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("12567s").toSet(),
+                                    advanceNum = 13
+                                ),
+                                Improvement(
+                                    discard = Tile.get("5s"),
+                                    advance = Tile.parseTiles("12367s").toSet(),
+                                    advanceNum = 13
+                                )
+                            ),
+                            Tile.get("6s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("5s"),
+                                    advance = Tile.parseTiles("2367s").toSet(),
+                                    advanceNum = 9
+                                )
+                            ),
+                            Tile.get("7s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("2s"),
+                                    advance = Tile.parseTiles("13578s").toSet(),
+                                    advanceNum = 12
+                                ),
+                                Improvement(
+                                    discard = Tile.get("5s"),
+                                    advance = Tile.parseTiles("12367s").toSet(),
+                                    advanceNum = 12
+                                ),
+                            ),
+                            Tile.get("8s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("2s"),
+                                    advance = Tile.parseTiles("78s").toSet(),
+                                    advanceNum = 7
+                                )
+                            ),
+                        ),
+                        goodShapeImprovementNum = 15
                     ),
                     Tile.get("4s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("25s").toSet(),
                         advanceNum = 3,
                         improvement = mapOf(
-                            Tile.get("1s") to setOf(
+                            Tile.get("1s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("124567s").toSet(),
+                                    advanceNum = 12
+                                )
+                            ),
+                            Tile.get("3s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("2s"),
+                                    advance = Tile.parseTiles("4567s").toSet(),
+                                    advanceNum = 8
+                                )
+                            ),
+                            Tile.get("4s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("1567s").toSet(),
+                                    advanceNum = 11
+                                )
+                            ),
+                            Tile.get("6s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("3s"),
+                                    advance = Tile.parseTiles("12456s").toSet(),
+                                    advanceNum = 8
+                                )
+                            ),
+                            Tile.get("7s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("2s"),
+                                    advance = Tile.parseTiles("134578s").toSet(),
+                                    advanceNum = 12
+                                )
+                            ),
+                            Tile.get("8s") to listOf(
+                                Improvement(
+                                    discard = Tile.get("2s"),
+                                    advance = Tile.parseTiles("78s").toSet(),
+                                    advanceNum = 7
+                                )
+                            ),
+                        ),
+                        improvementNum = 15,
+                        goodShapeImprovement = mapOf(
+                            Tile.get("1s") to listOf(
                                 Improvement(
                                     discard = Tile.get("3s"),
                                     advance = Tile.parseTiles("124567s").toSet(),
                                     advanceNum = 12
                                 )
                             ),
-                            Tile.get("3s") to setOf(
+                            Tile.get("3s") to listOf(
                                 Improvement(
                                     discard = Tile.get("2s"),
                                     advance = Tile.parseTiles("4567s").toSet(),
                                     advanceNum = 8
                                 )
                             ),
-                            Tile.get("4s") to setOf(
+                            Tile.get("4s") to listOf(
                                 Improvement(
                                     discard = Tile.get("3s"),
                                     advance = Tile.parseTiles("1567s").toSet(),
                                     advanceNum = 11
                                 )
                             ),
-                            Tile.get("6s") to setOf(
+                            Tile.get("6s") to listOf(
                                 Improvement(
                                     discard = Tile.get("3s"),
                                     advance = Tile.parseTiles("12456s").toSet(),
                                     advanceNum = 8
                                 )
                             ),
-                            Tile.get("7s") to setOf(
+                            Tile.get("7s") to listOf(
                                 Improvement(
                                     discard = Tile.get("2s"),
                                     advance = Tile.parseTiles("134578s").toSet(),
                                     advanceNum = 12
                                 )
                             ),
-                            Tile.get("8s") to setOf(
+                            Tile.get("8s") to listOf(
                                 Improvement(
                                     discard = Tile.get("2s"),
                                     advance = Tile.parseTiles("78s").toSet(),
                                     advanceNum = 7
                                 )
                             ),
                         ),
-                        improvementNum = 15
+                        goodShapeImprovementNum = 15
                     ),
                 ), ankanToAdvance = mapOf(
                     Tile.get("4s") to ShantenWithoutGot(
                         shantenNum = 1,
                         advance = Tile.parseTiles("1235678s").toSet(),
                         advanceNum = 18,
                         goodShapeAdvance = Tile.parseTiles("1237s").toSet(),
@@ -556,36 +764,44 @@
             "1112345678999s1z", ShantenWithGot(
                 shantenNum = 0, discardToAdvance = mapOf(
                     Tile.get("2s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("1z").toSet(),
                         advanceNum = 3,
                         improvement = null,
-                        improvementNum = null
+                        improvementNum = null,
+                        goodShapeImprovement = null,
+                        goodShapeImprovementNum = null
                     ),
                     Tile.get("5s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("1z").toSet(),
                         advanceNum = 3,
                         improvement = null,
-                        improvementNum = null
+                        improvementNum = null,
+                        goodShapeImprovement = null,
+                        goodShapeImprovementNum = null
                     ),
                     Tile.get("8s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("1z").toSet(),
                         advanceNum = 3,
                         improvement = null,
-                        improvementNum = null
+                        improvementNum = null,
+                        goodShapeImprovement = null,
+                        goodShapeImprovementNum = null
                     ),
                     Tile.get("1z") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("123456789s").toSet(),
                         advanceNum = 23,
                         improvement = null,
-                        improvementNum = null
+                        improvementNum = null,
+                        goodShapeImprovement = null,
+                        goodShapeImprovementNum = null
                     ),
                     Tile.get("1s") to ShantenWithoutGot(
                         shantenNum = 1,
                         advance = Tile.parseTiles("123456789s1z").toSet(),
                         advanceNum = 26,
                         goodShapeAdvance = Tile.parseTiles("1234679s1z").toSet(),
                         goodShapeAdvanceNum = 20
@@ -756,36 +972,44 @@
                 shantenNum = 0,
                 discardToAdvance = mapOf(
                     Tile.get("1p") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("14s").toSet(),
                         advanceNum = 7,
                         improvement = null,
-                        improvementNum = null
+                        improvementNum = null,
+                        goodShapeImprovement = null,
+                        goodShapeImprovementNum = null
                     ),
                     Tile.get("1s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("23s").toSet(),
                         advanceNum = 4,
                         improvement = null,
-                        improvementNum = null
+                        improvementNum = null,
+                        goodShapeImprovement = null,
+                        goodShapeImprovementNum = null
                     ),
                     Tile.get("2s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("3s").toSet(),
                         advanceNum = 2,
                         improvement = null,
-                        improvementNum = null
+                        improvementNum = null,
+                        goodShapeImprovement = null,
+                        goodShapeImprovementNum = null
                     ),
                     Tile.get("3s") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("2s").toSet(),
                         advanceNum = 2,
                         improvement = null,
-                        improvementNum = null
+                        improvementNum = null,
+                        goodShapeImprovement = null,
+                        goodShapeImprovementNum = null
                     )
                 )
             ),
             bestShantenOnly = true,
             calcImprovement = false
         )
         tester(
@@ -793,97 +1017,176 @@
                 shantenNum = 0,
                 discardToAdvance = mapOf(
                     Tile.get("4m") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("457p").toSet(),
                         advanceNum = 9,
                         improvement = mapOf(
-                            Tile.get("2p") to setOf(
+                            Tile.get("2p") to listOf(
                                 Improvement(
                                     discard = Tile.get("5p"),
                                     advance = Tile.parseTiles("1247p").toSet(),
                                     advanceNum = 14
                                 )
                             )
                         ),
-                        improvementNum = 4
+                        improvementNum = 4,
+                        goodShapeImprovement = mapOf(
+                            Tile.get("2p") to listOf(
+                                Improvement(
+                                    discard = Tile.get("5p"),
+                                    advance = Tile.parseTiles("1247p").toSet(),
+                                    advanceNum = 14
+                                )
+                            )
+                        ),
+                        goodShapeImprovementNum = 4
                     ),
                     Tile.get("5p") to ShantenWithoutGot(
                         shantenNum = 0,
                         advance = Tile.parseTiles("47m").toSet(),
                         advanceNum = 6,
                         improvement = mapOf(
-                            Tile.get("3m") to setOf(
+                            Tile.get("3m") to listOf(
                                 Improvement(
-                                    discard = Tile.get("6p"),
+                                    discard = Tile.get("3p"),
                                     advance = Tile.parseTiles("25m").toSet(),
                                     advanceNum = 7
                                 ),
                                 Improvement(
-                                    discard = Tile.get("3p"),
+                                    discard = Tile.get("6p"),
                                     advance = Tile.parseTiles("25m").toSet(),
                                     advanceNum = 7
                                 ),
                             ),
-                            Tile.get("5m") to setOf(
+                            Tile.get("5m") to listOf(
+                                Improvement(
+                                    discard = Tile.get("3p"),
+                                    advance = Tile.parseTiles("36m").toSet(),
+                                    advanceNum = 7
+                                ),
                                 Improvement(
                                     discard = Tile.get("6p"),
                                     advance = Tile.parseTiles("36m").toSet(),
                                     advanceNum = 7
                                 ),
+                            ),
+                            Tile.get("1p") to listOf(
+                                Improvement(
+                                    discard = Tile.get("4m"),
+                                    advance = Tile.parseTiles("12p").toSet(),
+                                    advanceNum = 7
+                                )
+                            ),
+                            Tile.get("2p") to listOf(
+                                Improvement(
+                                    discard = Tile.get("4m"),
+                                    advance = Tile.parseTiles("1247p").toSet(),
+                                    advanceNum = 14
+                                )
+                            ),
+                            Tile.get("4p") to listOf(
+                                Improvement(
+                                    discard = Tile.get("4m"),
+                                    advance = Tile.parseTiles("2457p").toSet(),
+                                    advanceNum = 12
+                                )
+                            ),
+                            Tile.get("5p") to listOf(
+                                Improvement(
+                                    discard = Tile.get("4m"),
+                                    advance = Tile.parseTiles("457p").toSet(),
+                                    advanceNum = 8
+                                )
+                            ),
+                            Tile.get("7p") to listOf(
+                                Improvement(
+                                    discard = Tile.get("4m"),
+                                    advance = Tile.parseTiles("24578p").toSet(),
+                                    advanceNum = 16
+                                )
+                            ),
+                            Tile.get("8p") to listOf(
+                                Improvement(
+                                    discard = Tile.get("4m"),
+                                    advance = Tile.parseTiles("78p").toSet(),
+                                    advanceNum = 7
+                                )
+                            ),
+                        ),
+                        improvementNum = 28,
+                        goodShapeImprovement = mapOf(
+                            Tile.get("3m") to listOf(
+                                Improvement(
+                                    discard = Tile.get("3p"),
+                                    advance = Tile.parseTiles("25m").toSet(),
+                                    advanceNum = 7
+                                ),
+                                Improvement(
+                                    discard = Tile.get("6p"),
+                                    advance = Tile.parseTiles("25m").toSet(),
+                                    advanceNum = 7
+                                ),
+                            ),
+                            Tile.get("5m") to listOf(
                                 Improvement(
                                     discard = Tile.get("3p"),
                                     advance = Tile.parseTiles("36m").toSet(),
                                     advanceNum = 7
                                 ),
+                                Improvement(
+                                    discard = Tile.get("6p"),
+                                    advance = Tile.parseTiles("36m").toSet(),
+                                    advanceNum = 7
+                                ),
                             ),
-                            Tile.get("1p") to setOf(
+                            Tile.get("1p") to listOf(
                                 Improvement(
                                     discard = Tile.get("4m"),
                                     advance = Tile.parseTiles("12p").toSet(),
                                     advanceNum = 7
                                 )
                             ),
-                            Tile.get("2p") to setOf(
+                            Tile.get("2p") to listOf(
                                 Improvement(
                                     discard = Tile.get("4m"),
                                     advance = Tile.parseTiles("1247p").toSet(),
                                     advanceNum = 14
                                 )
                             ),
-                            Tile.get("4p") to setOf(
+                            Tile.get("4p") to listOf(
                                 Improvement(
                                     discard = Tile.get("4m"),
                                     advance = Tile.parseTiles("2457p").toSet(),
                                     advanceNum = 12
                                 )
                             ),
-                            Tile.get("5p") to setOf(
+                            Tile.get("5p") to listOf(
                                 Improvement(
                                     discard = Tile.get("4m"),
                                     advance = Tile.parseTiles("457p").toSet(),
                                     advanceNum = 8
                                 )
                             ),
-                            Tile.get("7p") to setOf(
+                            Tile.get("7p") to listOf(
                                 Improvement(
                                     discard = Tile.get("4m"),
                                     advance = Tile.parseTiles("24578p").toSet(),
                                     advanceNum = 16
                                 )
                             ),
-                            Tile.get("8p") to setOf(
+                            Tile.get("8p") to listOf(
                                 Improvement(
                                     discard = Tile.get("4m"),
                                     advance = Tile.parseTiles("78p").toSet(),
                                     advanceNum = 7
                                 )
                             ),
                         ),
-                        improvementNum = 28
+                        goodShapeImprovementNum = 28
                     ),
                 )
             ),
             bestShantenOnly = true
         )
         tester(
             "35m11223399p7799s", ShantenWithGot(
```

### Comparing `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYaku.kt` & `mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYaku.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYakuman.kt` & `mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/yaku/TestYakuman.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/kt/src/jvmTest/kotlin/mahjongutils/yaku/Tester.kt` & `mahjong-utils-0.5.1/kt/src/jvmTest/kotlin/mahjongutils/yaku/Tester.kt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/hora/hora.py` & `mahjong-utils-0.5.1/mahjong_utils/hora/hora.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/hora/models.py` & `mahjong-utils-0.5.1/mahjong_utils/hora/models.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/lib/__init__.py` & `mahjong-utils-0.5.1/mahjong_utils/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/lib/libmahjongutils_api.i` & `mahjong-utils-0.5.1/mahjong_utils/lib/libmahjongutils_api.i`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/models/furo.py` & `mahjong-utils-0.5.1/mahjong_utils/models/furo.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/models/hand.py` & `mahjong-utils-0.5.1/mahjong_utils/models/hand.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/models/hand_pattern.py` & `mahjong-utils-0.5.1/mahjong_utils/models/hand_pattern.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/models/mentsu.py` & `mahjong-utils-0.5.1/mahjong_utils/models/mentsu.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/models/tatsu.py` & `mahjong-utils-0.5.1/mahjong_utils/models/tatsu.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/models/tile.py` & `mahjong-utils-0.5.1/mahjong_utils/models/tile.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/models/tile_type.py` & `mahjong-utils-0.5.1/mahjong_utils/models/tile_type.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/point_by_han_hu/models.py` & `mahjong-utils-0.5.1/mahjong_utils/point_by_han_hu/models.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/point_by_han_hu/point_by_han_hu.py` & `mahjong-utils-0.5.1/mahjong_utils/point_by_han_hu/point_by_han_hu.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/shanten/models.py` & `mahjong-utils-0.5.1/mahjong_utils/shanten/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,62 +53,73 @@
         return Improvement(
             discard=Tile.__decode__(data["discard"]),
             advance=set(Tile.__decode__(x) for x in data["advance"]),
             advance_num=data["advanceNum"]
         )
 
 
+def _encode_improvement_dict(improvement: Dict[Tile, List[Improvement]]):
+    d = dict()
+    for t in improvement:
+        d[t.__encode__()] = [x.__encode__() for x in improvement[t]]
+    return d
+
+
+def _decode_improvement_dict(improvement: dict) -> Dict[Tile, List[Improvement]]:
+    d = dict()
+    for t in improvement:
+        d[Tile.__decode__(t)] = [Improvement.__decode__(x) for x in improvement[t]]
+    return d
+
+
 class ShantenWithoutGot(CommonShanten):
     advance: Set[Tile]
     advance_num: int
     good_shape_advance: Optional[Set[Tile]]
     good_shape_advance_num: Optional[int]
     improvement: Optional[Dict[Tile, List[Improvement]]]
     improvement_num: Optional[int]
+    good_shape_improvement: Optional[Dict[Tile, List[Improvement]]]
+    good_shape_improvement_num: Optional[int]
 
     def __encode__(self) -> dict:
-        improvement = None
-
-        if self.improvement is not None:
-            improvement = dict()
-            for t in self.improvement:
-                improvement[t.__encode__()] = [x.__encode__() for x in self.improvement[t]]
-
         return dict(
             type="ShantenWithoutGot",
             shantenNum=self.shanten,
             advance=[t.__encode__() for t in self.advance],
             advanceNum=self.advance_num,
             goodShapeAdvance=[t.__encode__() for t in self.good_shape_advance]
             if self.good_shape_advance is not None else None,
             goodShapeAdvanceNum=self.good_shape_advance_num,
-            improvement=improvement,
+            improvement=_encode_improvement_dict(self.improvement)
+            if self.improvement is not None else None,
             improvementNum=self.improvement_num,
+            goodShapeImprovement=_encode_improvement_dict(self.good_shape_improvement)
+            if self.good_shape_improvement is not None else None,
+            goodShapeImprovementNum=self.good_shape_improvement_num,
         )
 
     @classmethod
     def __decode__(cls, data: dict) -> "ShantenWithoutGot":
-        improvement = None
-
-        if data["improvement"] is not None:
-            improvement = dict()
-            for t in data["improvement"]:
-                improvement[Tile.__decode__(t)] = [Improvement.__decode__(x) for x in data["improvement"][t]]
-
         return ShantenWithoutGot(
             shanten=data["shantenNum"],
             advance=set(Tile.__decode__(x) for x in data["advance"]),
             advance_num=data["advanceNum"],
             good_shape_advance=set(Tile.__decode__(x) for x in data["goodShapeAdvance"])
             if data["goodShapeAdvance"] is not None else None,
             good_shape_advance_num=data["goodShapeAdvanceNum"]
             if data["goodShapeAdvanceNum"] is not None else None,
-            improvement=improvement,
+            improvement=_decode_improvement_dict(data["improvement"])
+            if data["improvement"] is not None else None,
             improvement_num=data["improvementNum"]
             if data["improvementNum"] is not None else None,
+            good_shape_improvement=_decode_improvement_dict(data["goodShapeImprovement"])
+            if data["goodShapeImprovement"] is not None else None,
+            good_shape_improvement_num=data["goodShapeImprovementNum"]
+            if data["goodShapeImprovementNum"] is not None else None,
         )
 
 
 class ShantenWithGot(CommonShanten):
     discard_to_advance: Dict[Tile, ShantenWithoutGot]
     ankan_to_advance: Dict[Tile, ShantenWithoutGot]
 
@@ -211,14 +222,22 @@
         return getattr(self.shanten_info, "improvement", None)
 
     @property
     def improvement_num(self) -> Optional[int]:
         return getattr(self.shanten_info, "improvement_num", None)
 
     @property
+    def good_shape_improvement(self) -> Optional[Dict[Tile, List[Improvement]]]:
+        return getattr(self.shanten_info, "good_shape_improvement", None)
+
+    @property
+    def good_shape_improvement_num(self) -> Optional[int]:
+        return getattr(self.shanten_info, "good_shape_improvement_num", None)
+
+    @property
     def discard_to_advance(self) -> Optional[Dict[Tile, ShantenWithoutGot]]:
         return getattr(self.shanten_info, "discard_to_advance", None)
 
     @property
     def ankan_to_advance(self) -> Optional[Dict[Tile, ShantenWithoutGot]]:
         return getattr(self.shanten_info, "ankan_to_advance", None)
```

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/shanten/shanten.py` & `mahjong-utils-0.5.1/mahjong_utils/shanten/shanten.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/yaku/all_yaku.py` & `mahjong-utils-0.5.1/mahjong_utils/yaku/all_yaku.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/yaku/common.py` & `mahjong-utils-0.5.1/mahjong_utils/yaku/common.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/yaku/extra.py` & `mahjong-utils-0.5.1/mahjong_utils/yaku/extra.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils/yaku/yakuman.py` & `mahjong-utils-0.5.1/mahjong_utils/yaku/yakuman.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/PKG-INFO` & `mahjong-utils-0.5.1/mahjong_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mahjong-utils
-Version: 0.5.0.post1
+Version: 0.5.1
 Summary: 日麻小工具
 Home-page: https://github.com/ssttkkl/mahjong-utils
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `mahjong-utils-0.5.0.post1/mahjong_utils.egg-info/SOURCES.txt` & `mahjong-utils-0.5.1/mahjong_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/setup.py` & `mahjong-utils-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mahjong-utils",
-    version="0.5.0.post1",
+    version="0.5.1",
     author="ssttkkl",
     author_email="huang.wen.long@hotmail.com",
     license="MIT",
     url="https://github.com/ssttkkl/mahjong-utils",
     description="日麻小工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mahjong-utils-0.5.0.post1/tests/test_han_hu.py` & `mahjong-utils-0.5.1/tests/test_han_hu.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/tests/test_hora.py` & `mahjong-utils-0.5.1/tests/test_hora.py`

 * *Files identical despite different names*

### Comparing `mahjong-utils-0.5.0.post1/tests/test_shanten.py` & `mahjong-utils-0.5.1/tests/test_shanten.py`

 * *Files identical despite different names*

