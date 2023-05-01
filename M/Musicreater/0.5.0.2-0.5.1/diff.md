# Comparing `tmp/Musicreater-0.5.0.2.tar.gz` & `tmp/Musicreater-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Musicreater-0.5.0.2.tar", last modified: Sun Apr 30 14:35:44 2023, max compression
+gzip compressed data, was "Musicreater-0.5.1.tar", last modified: Mon May  1 04:41:54 2023, max compression
```

## Comparing `Musicreater-0.5.0.2.tar` & `Musicreater-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 14:35:44.345693 Musicreater-0.5.0.2/
--rw-rw-rw-   0        0        0    13085 2023-02-05 09:39:58.000000 Musicreater-0.5.0.2/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-04-30 14:35:44.328693 Musicreater-0.5.0.2/Musicreater/
--rw-rw-rw-   0        0        0      892 2023-04-30 14:34:46.000000 Musicreater-0.5.0.2/Musicreater/__init__.py
--rw-rw-rw-   0        0        0     3197 2023-04-29 13:59:22.000000 Musicreater-0.5.0.2/Musicreater/exceptions.py
--rw-rw-rw-   0        0        0     5479 2023-04-29 11:13:55.000000 Musicreater-0.5.0.2/Musicreater/instConstants.py
--rw-rw-rw-   0        0        0    10696 2023-04-29 11:13:55.000000 Musicreater-0.5.0.2/Musicreater/magicmain.py
--rw-rw-rw-   0        0        0    80374 2023-04-30 14:34:46.000000 Musicreater-0.5.0.2/Musicreater/main.py
--rw-rw-rw-   0        0        0    13570 2023-04-30 14:34:46.000000 Musicreater-0.5.0.2/Musicreater/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-30 14:35:44.342693 Musicreater-0.5.0.2/Musicreater.egg-info/
--rw-rw-rw-   0        0        0     7618 2023-04-30 14:35:43.000000 Musicreater-0.5.0.2/Musicreater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-30 14:35:44.000000 Musicreater-0.5.0.2/Musicreater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 14:35:43.000000 Musicreater-0.5.0.2/Musicreater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-30 14:35:43.000000 Musicreater-0.5.0.2/Musicreater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-30 14:35:43.000000 Musicreater-0.5.0.2/Musicreater.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7618 2023-04-30 14:35:44.344693 Musicreater-0.5.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6547 2023-04-30 14:34:46.000000 Musicreater-0.5.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 14:35:44.345693 Musicreater-0.5.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1597 2023-04-29 13:59:22.000000 Musicreater-0.5.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 04:41:54.062459 Musicreater-0.5.1/
+-rw-rw-rw-   0        0        0    13085 2023-02-05 09:39:58.000000 Musicreater-0.5.1/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-05-01 04:41:54.049458 Musicreater-0.5.1/Musicreater/
+-rw-rw-rw-   0        0        0      890 2023-05-01 04:41:16.000000 Musicreater-0.5.1/Musicreater/__init__.py
+-rw-rw-rw-   0        0        0     3197 2023-04-29 13:59:22.000000 Musicreater-0.5.1/Musicreater/exceptions.py
+-rw-rw-rw-   0        0        0     5479 2023-04-29 11:13:55.000000 Musicreater-0.5.1/Musicreater/instConstants.py
+-rw-rw-rw-   0        0        0    10696 2023-04-29 11:13:55.000000 Musicreater-0.5.1/Musicreater/magicmain.py
+-rw-rw-rw-   0        0        0    79747 2023-05-01 04:41:16.000000 Musicreater-0.5.1/Musicreater/main.py
+-rw-rw-rw-   0        0        0    13516 2023-04-30 14:43:50.000000 Musicreater-0.5.1/Musicreater/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-01 04:41:54.059455 Musicreater-0.5.1/Musicreater.egg-info/
+-rw-rw-rw-   0        0        0     7718 2023-05-01 04:41:53.000000 Musicreater-0.5.1/Musicreater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-05-01 04:41:53.000000 Musicreater-0.5.1/Musicreater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 04:41:53.000000 Musicreater-0.5.1/Musicreater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-01 04:41:53.000000 Musicreater-0.5.1/Musicreater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 04:41:53.000000 Musicreater-0.5.1/Musicreater.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7718 2023-05-01 04:41:54.061458 Musicreater-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6649 2023-05-01 04:41:16.000000 Musicreater-0.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 04:41:54.062459 Musicreater-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1597 2023-04-29 13:59:22.000000 Musicreater-0.5.1/setup.py
```

### Comparing `Musicreater-0.5.0.2/LICENSE.md` & `Musicreater-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Musicreater-0.5.0.2/Musicreater/__init__.py` & `Musicreater-0.5.1/Musicreater/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 版权所有 金羿("Eilles Wan") & 诸葛亮与八卦阵("bgArray") & 鸣凤鸽子("MingFengPigeon")
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 from .main import *
 
-__version__ = "0.5.0.2"
+__version__ = "0.5.1"
 __all__ = []
 __author__ = (("金羿", "Eilles Wan"), ("诸葛亮与八卦阵", "bgArray"), ("鸣凤鸽子", "MingFengPigeon"))
```

### Comparing `Musicreater-0.5.0.2/Musicreater/exceptions.py` & `Musicreater-0.5.1/Musicreater/exceptions.py`

 * *Files identical despite different names*

### Comparing `Musicreater-0.5.0.2/Musicreater/instConstants.py` & `Musicreater-0.5.1/Musicreater/instConstants.py`

 * *Files identical despite different names*

### Comparing `Musicreater-0.5.0.2/Musicreater/magicmain.py` & `Musicreater-0.5.1/Musicreater/magicmain.py`

 * *Files identical despite different names*

### Comparing `Musicreater-0.5.0.2/Musicreater/main.py` & `Musicreater-0.5.1/Musicreater/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     r"▶ %%N [ %%s/%^s %%% __________ %%t|%^t ]",
     ("§e=§r", "§7=§r"),
 )
 
 
 class SingleNote:
     def __init__(
-            self, instrument: int, pitch: int, velocity: int, startTime: int, lastTime: int
+        self, instrument: int, pitch: int, velocity: int, startTime: int, lastTime: int
     ):
         """用于存储单个音符的类
         :param instrument 乐器编号
         :param pitch 音符编号
         :param velocity 力度/响度
         :param startTime 开始之时(ms)
             注：此处的时间是用从乐曲开始到当前的毫秒数
@@ -212,15 +212,15 @@
         """输出路径"""
         # 将self.midiFile的文件名，不含路径且不含后缀存入self.midiFileName
         self.mid_file_name = os.path.splitext(os.path.basename(self.midi_file))[0]
         """文件名，不含路径且不含后缀"""
 
     @staticmethod
     def __Inst2soundID_withX(
-            instrumentID: int,
+        instrumentID: int,
     ):
         """
         返回midi的乐器ID对应的我的世界乐器名，对于音域转换算法，如下：
         2**( ( msg.note - 60 - X ) / 12 ) 即为MC的音高，其中
         X的取值随乐器不同而变化：
         竖琴harp、电钢琴pling、班卓琴banjo、方波bit、颤音琴iron_xylophone 的时候为6
         吉他的时候为7
@@ -256,15 +256,15 @@
         Returns
         -------
         tuple(str我的世界乐器名, int转换算法中的X)
         """
         try:
             return percussion_instrument_list[instrumentID]
         except KeyError:
-            print("WARN", "无法使用打击乐器列表库，或者使用了不存在的乐器，打击乐器使用Dislink算法代替。{instrumentID}")
+            print("WARN", f"无法使用打击乐器列表库，或者使用了不存在的乐器，打击乐器使用Dislink算法代替。{instrumentID}")
             if instrumentID == 55:
                 return "note.cow_bell", 5
             elif instrumentID in [41, 43, 45]:
                 return "note.hat", 7
             elif instrumentID in [36, 37, 39]:
                 return "note.snare", 7
             else:
@@ -274,18 +274,18 @@
     def score2time(score: int):
         """
         将《我的世界》的计分（以游戏刻计）转为表示时间的字符串
         """
         return str(int(int(score / 20) / 60)) + ":" + str(int(int(score / 20) % 60))
 
     def __form_progress_bar(
-            self,
-            max_score: int,
-            scoreboard_name: str,
-            progressbar_style: tuple = DEFAULT_PROGRESSBAR_STYLE,
+        self,
+        max_score: int,
+        scoreboard_name: str,
+        progressbar_style: tuple = DEFAULT_PROGRESSBAR_STYLE,
     ) -> list:
         """
         生成进度条
 
         Parameters
         ----------
         maxscore: int
@@ -462,18 +462,18 @@
         if r"%%t" in pgs_style:
             result.append("scoreboard objectives remove {}TMinT".format(sbn_pc))
             result.append("scoreboard objectives remove {}TSecT".format(sbn_pc))
 
         return result
 
     def _toCmdList_m1(
-            self,
-            scoreboard_name: str = "mscplay",
-            MaxVolume: float = 1.0,
-            speed: float = 1.0,
+        self,
+        scoreboard_name: str = "mscplay",
+        MaxVolume: float = 1.0,
+        speed: float = 1.0,
     ) -> list:
         """
         使用Dislink Sforza的转换思路，将midi转换为我的世界命令列表
         :param scoreboard_name: 我的世界的计分板名称
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :return: tuple(命令列表, 命令个数, 计分板最大值)
         """
@@ -521,28 +521,28 @@
                         singleTrack.append(
                             "execute @a[scores={"
                             + str(scoreboard_name)
                             + "="
                             + str(nowscore)
                             + "}"
                             + f"] ~ ~ ~ playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg.velocity / 128} "
-                              f"{2 ** ((msg.note - 60 - _X) / 12)}"
+                            f"{2 ** ((msg.note - 60 - _X) / 12)}"
                         )
                         commands += 1
             if len(singleTrack) != 0:
                 tracks.append(singleTrack)
 
         return [tracks, commands, maxscore]
 
     # 原本这个算法的转换效果应该和上面的算法相似的
     def _toCmdList_m2(
-            self,
-            scoreboard_name: str = "mscplay",
-            MaxVolume: float = 1.0,
-            speed: float = 1.0,
+        self,
+        scoreboard_name: str = "mscplay",
+        MaxVolume: float = 1.0,
+        speed: float = 1.0,
     ) -> list:
         """
         使用神羽和金羿的转换思路，将midi转换为我的世界命令列表
         :param scoreboard_name: 我的世界的计分板名称
         :param MaxVolume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :return: tuple(命令列表, 命令个数, 计分板最大值)
@@ -593,15 +593,15 @@
 
                 elif msg.type == "note_on" and msg.velocity != 0:
                     channels[msg.channel].append(
                         ("NoteS", msg.note, msg.velocity, microseconds)
                     )
 
                 elif (msg.type == "note_on" and msg.velocity == 0) or (
-                        msg.type == "note_off"
+                    msg.type == "note_off"
                 ):
                     channels[msg.channel].append(("NoteE", msg.note, microseconds))
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
 
         1 切换乐器消息
@@ -656,29 +656,29 @@
                     nowTrack.append(
                         self.execute_cmd_head.format(
                             "@a[scores=({}={})]".format(scoreboard_name, score_now)
                             .replace("(", r"{")
                             .replace(")", r"}")
                         )
                         + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
-                          f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                        f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                     )
 
                     cmdAmount += 1
 
             if nowTrack:
                 tracks.append(nowTrack)
 
         return [tracks, cmdAmount, maxScore]
 
     def _toCmdList_m3(
-            self,
-            scoreboard_name: str = "mscplay",
-            MaxVolume: float = 1.0,
-            speed: float = 1.0,
+        self,
+        scoreboard_name: str = "mscplay",
+        MaxVolume: float = 1.0,
+        speed: float = 1.0,
     ) -> list:
         """
         使用金羿的转换思路，将midi转换为我的世界命令列表
         :param scoreboard_name: 我的世界的计分板名称
         :param MaxVolume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :return: tuple(命令列表, 命令个数, 计分板最大值)
@@ -716,26 +716,26 @@
         for track_no, track in enumerate(self.midi.tracks):
             microseconds = 0
 
             for msg in track:
                 if msg.time != 0:
                     try:
                         microseconds += (
-                                msg.time * tempo / self.midi.ticks_per_beat / 1000
+                            msg.time * tempo / self.midi.ticks_per_beat / 1000
                         )
                         # print(microseconds)
                     except NameError:
                         if self.debug_mode:
                             raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
                         else:
                             microseconds += (
-                                                    msg.time
-                                                    * mido.midifiles.midifiles.DEFAULT_TEMPO
-                                                    / self.midi.ticks_per_beat
-                                            ) / 1000
+                                msg.time
+                                * mido.midifiles.midifiles.DEFAULT_TEMPO
+                                / self.midi.ticks_per_beat
+                            ) / 1000
 
                 if msg.is_meta:
                     if msg.type == "set_tempo":
                         tempo = msg.tempo
                         if self.debug_mode:
                             self.prt(f"TEMPO更改：{tempo}（毫秒每拍）")
                 else:
@@ -755,15 +755,15 @@
 
                     elif msg.type == "note_on" and msg.velocity != 0:
                         channels[msg.channel][track_no].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
-                            msg.type == "note_off"
+                        msg.type == "note_off"
                     ):
                         channels[msg.channel][track_no].append(
                             ("NoteE", msg.note, microseconds)
                         )
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
@@ -821,30 +821,30 @@
                         nowTrack.append(
                             self.execute_cmd_head.format(
                                 "@a[scores=({}={})]".format(scoreboard_name, score_now)
                                 .replace("(", r"{")
                                 .replace(")", r"}")
                             )
                             + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
-                              f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                            f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                         )
 
                         cmdAmount += 1
 
                 if nowTrack:
                     tracks.append(nowTrack)
 
         return [tracks, cmdAmount, maxScore]
 
     # 简单的单音填充
     def _toCmdList_m4(
-            self,
-            scoreboard_name: str = "mscplay",
-            MaxVolume: float = 1.0,
-            speed: float = 1.0,
+        self,
+        scoreboard_name: str = "mscplay",
+        MaxVolume: float = 1.0,
+        speed: float = 1.0,
     ) -> list:
         """
         使用金羿的转换思路，将midi转换为我的世界命令列表，并使用完全填充算法优化音感
         :param scoreboard_name: 我的世界的计分板名称
         :param MaxVolume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :return: tuple(命令列表, 命令个数, 计分板最大值)
@@ -889,15 +889,15 @@
 
                     elif msg.type == "note_on" and msg.velocity != 0:
                         channels[msg.channel].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
-                            msg.type == "note_off"
+                        msg.type == "note_off"
                     ):
                         channels[msg.channel].append(("NoteE", msg.note, microseconds))
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
 
         1 切换乐器消息
@@ -1005,27 +1005,27 @@
                     nowTrack.append(
                         "execute @a[scores={"
                         + str(scoreboard_name)
                         + "="
                         + str(score_now)
                         + "}"
                         + f"] ~ ~ ~ playsound {soundID} @s ~ ~{1 / every_note[4] - 1} ~ "
-                          f"{note.velocity * (0.7 if CheckFirstChannel else 0.9)} {2 ** ((note.pitch - 60 - _X) / 12)}"
+                        f"{note.velocity * (0.7 if CheckFirstChannel else 0.9)} {2 ** ((note.pitch - 60 - _X) / 12)}"
                     )
 
                     cmdAmount += 1
             tracks.append(nowTrack)
 
         return [tracks, cmdAmount, maxScore]
 
     def _toCmdList_withDelay_m1(
-            self,
-            MaxVolume: float = 1.0,
-            speed: float = 1.0,
-            player: str = "@a",
+        self,
+        MaxVolume: float = 1.0,
+        speed: float = 1.0,
+        player: str = "@a",
     ) -> list:
         """
         使用Dislink Sforza的转换思路，将midi转换为我的世界命令列表，并输出每个音符之后的延迟
         :param MaxVolume: 最大播放音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :param player: 玩家选择器，默认为`@a`
         :return: 全部指令列表[ ( str指令, int距离上一个指令的延迟 ),...]
@@ -1057,26 +1057,27 @@
                             / ((self.midi.ticks_per_beat * float(speed)) * 50000)
                         )
                         soundID, _X = self.__Inst2soundID_withX(instrumentID)
                         try:
                             tracks[now_tick].append(
                                 self.execute_cmd_head.format(player)
                                 + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg.velocity / 128} "
-                                  f"{2 ** ((msg.note - 60 - _X) / 12)}"
+                                f"{2 ** ((msg.note - 60 - _X) / 12)}"
                             )
                         except KeyError:
                             tracks[now_tick] = [
                                 self.execute_cmd_head.format(player)
                                 + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg.velocity / 128} "
-                                  f"{2 ** ((msg.note - 60 - _X) / 12)}"
+                                f"{2 ** ((msg.note - 60 - _X) / 12)}"
                             ]
 
         results = []
 
         all_ticks = list(tracks.keys())
+        all_ticks.sort()
 
         for i in range(len(all_ticks)):
             if i != 0:
                 for j in range(len(tracks[all_ticks[i]])):
                     if j != 0:
                         results.append((tracks[all_ticks[i]][j], 0))
                     else:
@@ -1086,18 +1087,18 @@
             else:
                 for j in range(len(tracks[all_ticks[i]])):
                     results.append((tracks[all_ticks[i]][j], all_ticks[i]))
 
         return [results, max(all_ticks)]
 
     def _toCmdList_withDelay_m2(
-            self,
-            MaxVolume: float = 1.0,
-            speed: float = 1.0,
-            player: str = "@a",
+        self,
+        MaxVolume: float = 1.0,
+        speed: float = 1.0,
+        player: str = "@a",
     ) -> list:
         """
         使用神羽和金羿的转换思路，将midi转换为我的世界命令列表，并输出每个音符之后的延迟
         :param MaxVolume: 最大播放音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :param player: 玩家选择器，默认为`@a`
         :return: 全部指令列表[ ( str指令, int距离上一个指令的延迟 ),...]
@@ -1133,24 +1134,24 @@
 
         microseconds = 0
 
         # 我们来用通道统计音乐信息
         for msg in self.midi:
             try:
                 microseconds += (
-                        msg.time * 1000
+                    msg.time * 1000
                 )  # 任何人都tm不要动这里，这里循环方式不是track，所以，这里的计时方式不一样
 
                 # print(microseconds)
             except NameError:
                 if self.debug_mode:
                     raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
                 else:
                     microseconds += (
-                            msg.time * 1000
+                        msg.time * 1000
                     )  # 任何人都tm不要动这里，这里循环方式不是track，所以，这里的计时方式不一样
 
             if msg.is_meta:
                 if msg.type == "set_tempo":
                     tempo = msg.tempo
             else:
                 if self.debug_mode:
@@ -1165,15 +1166,15 @@
 
                 elif msg.type == "note_on" and msg.velocity != 0:
                     channels[msg.channel].append(
                         ("NoteS", msg.note, msg.velocity, microseconds)
                     )
 
                 elif (msg.type == "note_on" and msg.velocity == 0) or (
-                        msg.type == "note_off"
+                    msg.type == "note_off"
                 ):
                     channels[msg.channel].append(("NoteE", msg.note, microseconds))
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
 
         1 切换乐器消息
@@ -1219,24 +1220,25 @@
                             )
                     score_now = round(msg[-1] / float(speed) / 50)
 
                     try:
                         tracks[score_now].append(
                             self.execute_cmd_head.format(player)
                             + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
-                              f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                            f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                         )
                     except KeyError:
                         tracks[score_now] = [
                             self.execute_cmd_head.format(player)
                             + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
-                              f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                            f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                         ]
 
         all_ticks = list(tracks.keys())
+        all_ticks.sort()
 
         for i in range(len(all_ticks)):
             for j in range(len(tracks[all_ticks[i]])):
                 results.append(
                     (
                         tracks[all_ticks[i]][j],
                         (
@@ -1250,18 +1252,18 @@
                         ),
                     )
                 )
 
         return [results, max(all_ticks)]
 
     def _toCmdList_withDelay_m3(
-            self,
-            MaxVolume: float = 1.0,
-            speed: float = 1.0,
-            player: str = "@a",
+        self,
+        MaxVolume: float = 1.0,
+        speed: float = 1.0,
+        player: str = "@a",
     ) -> list:
         """
         使用金羿的转换思路，将midi转换为我的世界命令列表，并输出每个音符之后的延迟
         :param MaxVolume: 最大播放音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :param player: 玩家选择器，默认为`@a`
         :return: 全部指令列表[ ( str指令, int距离上一个指令的延迟 ),...]
@@ -1299,54 +1301,53 @@
         for track_no, track in enumerate(self.midi.tracks):
             microseconds = 0
 
             for msg in track:
                 if msg.time != 0:
                     try:
                         microseconds += (
-                                msg.time * tempo / self.midi.ticks_per_beat / 1000
+                            msg.time * tempo / self.midi.ticks_per_beat / 1000
                         )
                         # print(microseconds)
                     except NameError:
                         if self.debug_mode:
                             raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
                         else:
                             microseconds += (
-                                                    msg.time
-                                                    * mido.midifiles.midifiles.DEFAULT_TEMPO
-                                                    / self.midi.ticks_per_beat
-                                            ) / 1000
+                                msg.time
+                                * mido.midifiles.midifiles.DEFAULT_TEMPO
+                                / self.midi.ticks_per_beat
+                            ) / 1000
 
                 if msg.is_meta:
                     if msg.type == "set_tempo":
                         tempo = msg.tempo
                         if self.debug_mode:
                             self.prt(f"TEMPO更改：{tempo}（毫秒每拍）")
                 else:
-                    if self.debug_mode:
-                        try:
-                            if msg.channel > 15:
-                                raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
-                        except AttributeError:
-                            pass
+                    try:
+                        if msg.channel > 15 and self.debug_mode:
+                            raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
+                        if not track_no in channels[msg.channel].keys():
+                            channels[msg.channel][track_no] = []
+                    except AttributeError:
+                        pass
 
-                    if not track_no in channels[msg.channel].keys():
-                        channels[msg.channel][track_no] = []
                     if msg.type == "program_change":
                         channels[msg.channel][track_no].append(
                             ("PgmC", msg.program, microseconds)
                         )
 
                     elif msg.type == "note_on" and msg.velocity != 0:
                         channels[msg.channel][track_no].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
-                            msg.type == "note_off"
+                        msg.type == "note_off"
                     ):
                         channels[msg.channel][track_no].append(
                             ("NoteE", msg.note, microseconds)
                         )
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
@@ -1391,29 +1392,31 @@
                             else:
                                 soundID, _X = (
                                     self.__bitInst2ID_withX(-1)
                                     if SpecialBits
                                     else self.__Inst2soundID_withX(-1)
                                 )
                         score_now = round(msg[-1] / float(speed) / 50)
+                        # print(score_now)
 
                         try:
                             tracks[score_now].append(
                                 self.execute_cmd_head.format(player)
                                 + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
-                                  f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                                f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                             )
                         except KeyError:
                             tracks[score_now] = [
                                 self.execute_cmd_head.format(player)
                                 + f"playsound {soundID} @s ^ ^ ^{1 / MaxVolume - 1} {msg[2] / 128} "
-                                  f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                                f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                             ]
 
         all_ticks = list(tracks.keys())
+        all_ticks.sort()
         results = []
 
         for i in range(len(all_ticks)):
             for j in range(len(tracks[all_ticks[i]])):
                 results.append(
                     (
                         tracks[all_ticks[i]][j],
@@ -1428,21 +1431,21 @@
                         ),
                     )
                 )
 
         return [results, max(all_ticks)]
 
     def to_mcpack(
-            self,
-            method: int = 1,
-            volume: float = 1.0,
-            speed: float = 1.0,
-            progressbar: Union[bool, tuple] = None,
-            scoreboard_name: str = "mscplay",
-            isAutoReset: bool = False,
+        self,
+        method: int = 1,
+        volume: float = 1.0,
+        speed: float = 1.0,
+        progressbar: Union[bool, tuple] = None,
+        scoreboard_name: str = "mscplay",
+        isAutoReset: bool = False,
     ) -> tuple:
         """
         使用method指定的转换算法，将midi转换为我的世界mcpack格式的包
         :param method: 转换算法
         :param isAutoReset: 是否自动重置计分板
         :param progressbar: 进度条，（当此参数为True时使用默认进度条，为其他的值为真的参数时识别为进度条自定义参数，为其他值为假的时候不生成进度条）
         :param scoreboard_name: 我的世界的计分板名称
@@ -1462,15 +1465,15 @@
         if os.path.exists(f"{self.output_path}/temp/functions/"):
             shutil.rmtree(f"{self.output_path}/temp/functions/")
         os.makedirs(f"{self.output_path}/temp/functions/mscplay")
 
         # 写入manifest.json
         if not os.path.exists(f"{self.output_path}/temp/manifest.json"):
             with open(
-                    f"{self.output_path}/temp/manifest.json", "w", encoding="utf-8"
+                f"{self.output_path}/temp/manifest.json", "w", encoding="utf-8"
             ) as f:
                 f.write(
                     '{\n  "format_version": 1,\n  "header": {\n    "description": "'
                     + self.mid_file_name
                     + ' Pack : behavior pack",\n    "version": [ 0, 0, 1 ],\n    "name": "'
                     + self.mid_file_name
                     + 'Pack",\n    "uuid": "'
@@ -1479,15 +1482,15 @@
                     + f"the Player of the Music {self.mid_file_name}"
                     + '",\n      "type": "data",\n      "version": [ 0, 0, 1 ],\n      "uuid": "'
                     + str(uuid.uuid4())
                     + '"\n    }\n  ]\n}'
                 )
         else:
             with open(
-                    f"{self.output_path}/temp/manifest.json", "r", encoding="utf-8"
+                f"{self.output_path}/temp/manifest.json", "r", encoding="utf-8"
             ) as manifest:
                 data = json.loads(manifest.read())
                 data["header"][
                     "description"
                 ] = f"the Player of the Music {self.mid_file_name}"
                 data["header"]["name"] = self.mid_file_name
                 data["header"]["uuid"] = str(uuid.uuid4())
@@ -1503,57 +1506,57 @@
             f"{self.output_path}/temp/functions/index.mcfunction", "w", encoding="utf-8"
         )
         for track in cmdlist:
             index_file.write(
                 "function mscplay/track" + str(cmdlist.index(track) + 1) + "\n"
             )
             with open(
-                    f"{self.output_path}/temp/functions/mscplay/track{cmdlist.index(track) + 1}.mcfunction",
-                    "w",
-                    encoding="utf-8",
+                f"{self.output_path}/temp/functions/mscplay/track{cmdlist.index(track) + 1}.mcfunction",
+                "w",
+                encoding="utf-8",
             ) as f:
                 f.write("\n".join(track))
         index_file.writelines(
             (
                 "scoreboard players add @a[scores={"
                 + scoreboard_name
                 + "=1..}] "
                 + scoreboard_name
                 + " 1\n",
                 (
-                        "scoreboard players reset @a[scores={"
-                        + scoreboard_name
-                        + "="
-                        + str(maxscore + 20)
-                        + "..}]"
-                        + f" {scoreboard_name}\n"
+                    "scoreboard players reset @a[scores={"
+                    + scoreboard_name
+                    + "="
+                    + str(maxscore + 20)
+                    + "..}]"
+                    + f" {scoreboard_name}\n"
                 )
                 if isAutoReset
                 else "",
                 f"function mscplay/progressShow\n" if progressbar else "",
             )
         )
 
         if progressbar:
             # 此处是对于仅有 True 的参数和自定义参数的判断
             # 改这一行没🐎
             if progressbar is True:
                 with open(
-                        f"{self.output_path}/temp/functions/mscplay/progressShow.mcfunction",
-                        "w",
-                        encoding="utf-8",
+                    f"{self.output_path}/temp/functions/mscplay/progressShow.mcfunction",
+                    "w",
+                    encoding="utf-8",
                 ) as f:
                     f.writelines(
                         "\n".join(self.__form_progress_bar(maxscore, scoreboard_name))
                     )
             else:
                 with open(
-                        f"{self.output_path}/temp/functions/mscplay/progressShow.mcfunction",
-                        "w",
-                        encoding="utf-8",
+                    f"{self.output_path}/temp/functions/mscplay/progressShow.mcfunction",
+                    "w",
+                    encoding="utf-8",
                 ) as f:
                     f.writelines(
                         "\n".join(
                             self.__form_progress_bar(
                                 maxscore, scoreboard_name, progressbar
                             )
                         )
@@ -1569,34 +1572,34 @@
         )
 
         shutil.rmtree(f"{self.output_path}/temp/")
 
         return True, maxlen, maxscore
 
     def to_mcpack_with_delay(
-            self,
-            method: int = 1,
-            volume: float = 1.0,
-            speed: float = 1.0,
-            progressbar: Union[bool, tuple] = False,
-            player: str = "@a",
-            max_height: int = 64,
+        self,
+        method: int = 1,
+        volume: float = 1.0,
+        speed: float = 1.0,
+        progressbar: Union[bool, tuple] = False,
+        player: str = "@a",
+        max_height: int = 64,
     ):
         """
         使用method指定的转换算法，将midi转换为mcstructure结构文件后打包成mcpack文件
         :param method: 转换算法
         :param author: 作者名称
         :param progressbar: 进度条，（当此参数为True时使用默认进度条，为其他的值为真的参数时识别为进度条自定义参数，为其他值为假的时候不生成进度条）
         :param max_height: 生成结构最大高度
         :param volume: 音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放音频
         :param speed: 速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
         :param player: 玩家选择器，默认为`@a`
         :return 成功与否，成功返回(True,未经过压缩的源,结构占用大小)，失败返回(False,str失败原因)
         """
-        
+
         from TrimMCStruct import Structure
 
         if self.enable_old_exe_format:
             raise CommandFormatError("使用mcstructure结构文件导出时不支持旧版本的指令格式。")
 
         command_list, max_delay = self.methods_byDelay[method - 1](
             volume,
@@ -1644,22 +1647,22 @@
         # 将命令列表写入文件
         index_file = open(
             f"{self.output_path}/temp/functions/index.mcfunction", "w", encoding="utf-8"
         )
 
         struct, size, end_pos = commands_to_structure(command_list, max_height - 1)
         with open(
-                os.path.abspath(
-                    os.path.join(
-                        self.output_path,
-                        "temp/structures/",
-                        f"{self.mid_file_name}_main.mcstructure",
-                    )
-                ),
-                "wb+",
+            os.path.abspath(
+                os.path.join(
+                    self.output_path,
+                    "temp/structures/",
+                    f"{self.mid_file_name}_main.mcstructure",
+                )
+            ),
+            "wb+",
         ) as f:
             struct.dump(f)
 
         del struct
 
         if progressbar:
             scb_name = self.mid_file_name[:5] + "Pgb"
@@ -1673,77 +1676,79 @@
             struct_a.set_block(
                 (0, 0, 0),
                 form_command_block_in_NBT_struct(
                     r"scoreboard players add {} {} 1".format(player, scb_name),
                     (0, 0, 0),
                     1,
                     1,
+                    alwaysRun=False,
                     customName="显示进度条并加分",
                 ),
             )
 
             with open(
-                    os.path.abspath(
-                        os.path.join(
-                            self.output_path,
-                            "temp/structures/",
-                            f"{self.mid_file_name}_start.mcstructure",
-                        )
-                    ),
-                    "wb+",
+                os.path.abspath(
+                    os.path.join(
+                        self.output_path,
+                        "temp/structures/",
+                        f"{self.mid_file_name}_start.mcstructure",
+                    )
+                ),
+                "wb+",
             ) as f:
                 struct_a.dump(f)
 
             index_file.write(f"structure load {self.mid_file_name}_start ~ ~ ~1\n")
 
             pgb_struct, pgbSize, pgbNowPos = commands_to_structure(
                 [
                     (i, 0)
                     for i in self.__form_progress_bar(max_delay, scb_name, progressbar)
                 ],
                 max_height - 1,
             )
 
             with open(
-                    os.path.abspath(
-                        os.path.join(
-                            self.output_path,
-                            "temp/structures/",
-                            f"{self.mid_file_name}_pgb.mcstructure",
-                        )
-                    ),
-                    "wb+",
+                os.path.abspath(
+                    os.path.join(
+                        self.output_path,
+                        "temp/structures/",
+                        f"{self.mid_file_name}_pgb.mcstructure",
+                    )
+                ),
+                "wb+",
             ) as f:
                 pgb_struct.dump(f)
 
             index_file.write(f"structure load {self.mid_file_name}_pgb ~ ~1 ~1\n")
 
             struct_a = Structure(
                 (1, 1, 1),
             )
             struct_a.set_block(
                 (0, 0, 0),
                 form_command_block_in_NBT_struct(
                     r"scoreboard players reset {} {}".format(player, scb_name),
                     (0, 0, 0),
                     1,
-                    1,
+                    0,
+                    alwaysRun=False,
                     customName="重置进度条计分板",
                 ),
             )
 
             with open(
-                    os.path.abspath(
-                        os.path.join(
-                            self.output_path,
-                            "temp/structures/",
-                            f"{self.mid_file_name}_reset.mcstructure",
-                        )
-                    ),
-                    "wb+",
+                os.path.abspath(
+                    os.path.join(
+                        self.output_path,
+                        "temp/structures/",
+                        f"{self.mid_file_name}_reset.mcstructure",
+                    )
+                ),
+                "wb+",
             ) as f:
                 struct_a.dump(f)
 
             del struct_a, pgb_struct
 
             index_file.write(
                 f"structure load {self.mid_file_name}_reset ~{pgbSize[0] + 2} ~ ~1\n"
@@ -1766,20 +1771,20 @@
         )
 
         shutil.rmtree(f"{self.output_path}/temp/")
 
         return True, len(command_list), max_delay
 
     def to_mcstructure_file_with_delay(
-            self,
-            method: int = 1,
-            volume: float = 1.0,
-            speed: float = 1.0,
-            player: str = "@a",
-            max_height: int = 64,
+        self,
+        method: int = 1,
+        volume: float = 1.0,
+        speed: float = 1.0,
+        player: str = "@a",
+        max_height: int = 64,
     ):
         """
         使用method指定的转换算法，将midi转换为mcstructure结构文件
         :param method: 转换算法
         :param author: 作者名称
         :param progressbar: 进度条，（当此参数为True时使用默认进度条，为其他的值为真的参数时识别为进度条自定义参数，为其他值为假的时候不生成进度条）
         :param max_height: 生成结构最大高度
@@ -1800,33 +1805,33 @@
 
         if not os.path.exists(self.output_path):
             os.makedirs(self.output_path)
 
         struct, size, end_pos = commands_to_structure(cmd_list, max_height - 1)
 
         with open(
-                os.path.abspath(
-                    os.path.join(self.output_path, f"{self.mid_file_name}.mcstructure")
-                ),
-                "wb+",
+            os.path.abspath(
+                os.path.join(self.output_path, f"{self.mid_file_name}.mcstructure")
+            ),
+            "wb+",
         ) as f:
             struct.dump(f)
 
         return True, size, max_delay
 
     def to_BDX_file(
-            self,
-            method: int = 1,
-            volume: float = 1.0,
-            speed: float = 1.0,
-            progressbar: Union[bool, tuple] = False,
-            scoreboard_name: str = "mscplay",
-            isAutoReset: bool = False,
-            author: str = "Eilles",
-            max_height: int = 64,
+        self,
+        method: int = 1,
+        volume: float = 1.0,
+        speed: float = 1.0,
+        progressbar: Union[bool, tuple] = False,
+        scoreboard_name: str = "mscplay",
+        isAutoReset: bool = False,
+        author: str = "Eilles",
+        max_height: int = 64,
     ):
         """
         使用method指定的转换算法，将midi转换为BDX结构文件
         :param method: 转换算法
         :param author: 作者名称
         :param progressbar: 进度条，（当此参数为True时使用默认进度条，为其他的值为真的参数时识别为进度条自定义参数，为其他值为假的时候不生成进度条）
         :param max_height: 生成结构最大高度
@@ -1843,25 +1848,25 @@
         # except Exception as E:
         #     return (False, f"无法找到算法ID{method}对应的转换算法: {E}")
 
         if not os.path.exists(self.output_path):
             os.makedirs(self.output_path)
 
         with open(
-                os.path.abspath(
-                    os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
-                ),
-                "w+",
+            os.path.abspath(
+                os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
+            ),
+            "w+",
         ) as f:
             f.write("BD@")
 
         _bytes = (
-                b"BDX\x00"
-                + author.encode("utf-8")
-                + b" & Musicreater\x00\x01command_block\x00"
+            b"BDX\x00"
+            + author.encode("utf-8")
+            + b" & Musicreater\x00\x01command_block\x00"
         )
 
         commands = []
 
         for track in cmdlist:
             commands += track
 
@@ -1880,22 +1885,22 @@
         )
 
         if progressbar:
             pgbBytes, pgbSize, pgbNowPos = commands_to_BDX_bytes(
                 [
                     (i, 0)
                     for i in (
-                    self.__form_progress_bar(maxScore, scoreboard_name)
-                    # 此处是对于仅有 True 的参数和自定义参数的判断
-                    # 改这一行没🐎
-                    if progressbar is True
-                    else self.__form_progress_bar(
-                        maxScore, scoreboard_name, progressbar
+                        self.__form_progress_bar(maxScore, scoreboard_name)
+                        # 此处是对于仅有 True 的参数和自定义参数的判断
+                        # 改这一行没🐎
+                        if progressbar is True
+                        else self.__form_progress_bar(
+                            maxScore, scoreboard_name, progressbar
+                        )
                     )
-                )
                 ],
                 max_height - 1,
             )
             _bytes += pgbBytes
             _bytes += bdx_move(y, -pgbNowPos[1])
             _bytes += bdx_move(z, -pgbNowPos[2])
             _bytes += bdx_move(x, 2)
@@ -1903,32 +1908,32 @@
             size[0] += 2 + pgbSize[0]
             size[1] = max(size[1], pgbSize[1])
             size[2] = max(size[2], pgbSize[2])
 
         _bytes += cmdBytes
 
         with open(
-                os.path.abspath(
-                    os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
-                ),
-                "ab+",
+            os.path.abspath(
+                os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
+            ),
+            "ab+",
         ) as f:
             f.write(brotli.compress(_bytes + b"XE"))
 
         return True, total_count, maxScore, size, finalPos
 
     def to_BDX_file_with_delay(
-            self,
-            method: int = 1,
-            volume: float = 1.0,
-            speed: float = 1.0,
-            progressbar: Union[bool, tuple] = False,
-            player: str = "@a",
-            author: str = "Eilles",
-            max_height: int = 64,
+        self,
+        method: int = 1,
+        volume: float = 1.0,
+        speed: float = 1.0,
+        progressbar: Union[bool, tuple] = False,
+        player: str = "@a",
+        author: str = "Eilles",
+        max_height: int = 64,
     ):
         """
         使用method指定的转换算法，将midi转换为BDX结构文件
         :param method: 转换算法
         :param author: 作者名称
         :param progressbar: 进度条，（当此参数为True时使用默认进度条，为其他的值为真的参数时识别为进度条自定义参数，为其他值为假的时候不生成进度条）
         :param max_height: 生成结构最大高度
@@ -1947,25 +1952,25 @@
         # except Exception as E:
         #     return (False, f"无法找到算法ID{method}对应的转换算法\n{E}")
 
         if not os.path.exists(self.output_path):
             os.makedirs(self.output_path)
 
         with open(
-                os.path.abspath(
-                    os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
-                ),
-                "w+",
+            os.path.abspath(
+                os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
+            ),
+            "w+",
         ) as f:
             f.write("BD@")
 
         _bytes = (
-                b"BDX\x00"
-                + author.encode("utf-8")
-                + b" & Musicreater\x00\x01command_block\x00"
+            b"BDX\x00"
+            + author.encode("utf-8")
+            + b" & Musicreater\x00\x01command_block\x00"
         )
 
         # 此处是对于仅有 True 的参数和自定义参数的判断
         # 改这一行没🐎
         if progressbar is True:
             progressbar = DEFAULT_PROGRESSBAR_STYLE
 
@@ -2007,25 +2012,25 @@
             size[1] = max(size[1], pgbSize[1])
             size[2] = max(size[2], pgbSize[2])
 
         size[1] += 1
         _bytes += cmdBytes
 
         with open(
-                os.path.abspath(
-                    os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
-                ),
-                "ab+",
+            os.path.abspath(
+                os.path.join(self.output_path, f"{self.mid_file_name}.bdx")
+            ),
+            "ab+",
         ) as f:
             f.write(brotli.compress(_bytes + b"XE"))
 
         return True, len(cmdlist), max_delay, size, finalPos
 
     def toDICT(
-            self,
+        self,
     ) -> dict:
         """
         使用金羿的转换思路，将midi转换为字典
         :return: dict()
         """
 
         # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
@@ -2060,17 +2065,17 @@
                         microseconds += msg.time * tempo / self.midi.ticks_per_beat
                         # print(microseconds)
                     except NameError:
                         if self.debug_mode:
                             raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
                         else:
                             microseconds += (
-                                    msg.time
-                                    * mido.midifiles.midifiles.DEFAULT_TEMPO
-                                    / self.midi.ticks_per_beat
+                                msg.time
+                                * mido.midifiles.midifiles.DEFAULT_TEMPO
+                                / self.midi.ticks_per_beat
                             )
 
                 if msg.is_meta:
                     if msg.type == "set_tempo":
                         tempo = msg.tempo
                         if self.debug_mode:
                             self.prt(f"TEMPO更改：{tempo}（毫秒每拍）")
@@ -2091,15 +2096,15 @@
 
                     elif msg.type == "note_on" and msg.velocity != 0:
                         channels[msg.channel][track_no].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
-                            msg.type == "note_off"
+                        msg.type == "note_off"
                     ):
                         channels[msg.channel][track_no].append(
                             ("NoteE", msg.note, microseconds)
                         )
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
```

### Comparing `Musicreater-0.5.0.2/Musicreater/utils.py` & `Musicreater-0.5.1/Musicreater/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import math
 import os
 
-
 bdx_key = {
     "x": [b"\x0f", b"\x0e", b"\x1c", b"\x14", b"\x15"],
     "y": [b"\x11", b"\x10", b"\x1d", b"\x16", b"\x17"],
     "z": [b"\x13", b"\x12", b"\x1e", b"\x18", b"\x19"],
 }
 """key存储了方块移动指令的数据，其中可以用key[x|y|z][0|1]来表示xyz的减或增
 而key[][2+]是用来增加指定数目的"""
@@ -261,20 +260,18 @@
     )
 
 
 def form_repeater_in_NBT_struct(
         delay: int, facing: int
 ):
     """生成中继器方块
-    :param powered:
-    :param locked:
     :param facing:
     :param delay: 1~4
     :return Block()"""
-    
+
     from TrimMCStruct import Block
 
     return Block(
         "minecraft",
         "unpowered_repeater",
         {
             "repeater_delay": delay,
@@ -336,15 +333,14 @@
         首刻执行(循环指令方块是否激活后立即执行，若为False，则从激活时起延迟后第一次执行)
     :param trackOutput: `bool`
         是否输出
 
     :return:str
     """
 
-    
     from TrimMCStruct import Block, TAG_Long
 
     return Block(
         "minecraft",
         "command_block"
         if impluse == 0
         else ("repeating_command_block" if impluse == 1 else "chain_command_block"),
@@ -385,15 +381,14 @@
 ):
     """
     :param commands: 指令列表(指令, 延迟)
     :param max_height: 生成结构最大高度
     :return 成功与否，成功返回(结构类,结构占用大小)，失败返回(False,str失败原因)
     """
 
-    
     from TrimMCStruct import Structure
 
     _sideLength = bottem_side_length_of_smallest_square_bottom_box(
         len(commands), max_height
     )
 
     struct = Structure(
```

### Comparing `Musicreater-0.5.0.2/Musicreater.egg-info/PKG-INFO` & `Musicreater-0.5.1/Musicreater.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 0.5.0.2
+Version: 0.5.1
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
@@ -107,15 +107,15 @@
 本致谢列表排名无顺序。
 
 - 感谢 **昀梦**\<QQ1515399885\> 找出指令生成错误bug并指正
 - 感谢由 **Charlie_Ping “查理平”** 带来的BDX文件转换参考，以及MIDI-我的世界对应乐器参考表格
 - 感谢由 **[CMA_2401PT](https://github.com/CMA2401PT)** 为我们的软件开发的一些方面进行指导，同时我们参考了他的BDXworkshop作为BDX结构编辑的参考
 - 感谢由 **[Dislink Sforza](https://github.com/Dislink) “断联·斯福尔扎”**\<QQ1600515314\> 带来的midi音色解析以及转换指令的算法，我们将其改编并应用；同时，感谢他的[网页版转换器](https://dislink.github.io/midi2bdx/)给我们的开发与更新带来巨大的压力和动力，让我们在原本一骑绝尘的摸鱼道路上转向开发，希望他能考上一个理想的大学！
 - 感谢 **Touch “偷吃”**\<QQ1793537164\> 提供的BDX导入测试支持，并对程序的改进提供了丰富的意见；同时也感谢他的不断尝试新的内容，使我们的排错更进一步
-- 感谢 **Mono**\<QQ738893087\> 反馈安装时的问题，辅助我们找到了视窗操作系统下的兼容性问题
+- 感谢 **Mono**\<QQ738893087\> 反馈安装时的问题，辅助我们找到了视窗操作系统下的兼容性问题；感谢其反馈延迟播放器出现的重大问题，让我们得以修改全部延迟播放错误
 - 感谢 **Ammelia “艾米利亚”**\<QQ2838334637\> 敦促我们进行新的功能开发，并为新功能提出了非常优秀的大量建议，以及提供的BDX导入测试支持，为我们的新结构生成算法提供了大量的实际理论支持
 - 感谢 **[神羽](https://gitee.com/snowykami) “[SnowyKami](https://github.com/snowyfirefly)”** 对我们项目的支持与宣传，希望他能考的一所优秀的大学！
 - 感谢 **指令师_苦力怕 playjuice123**\<QQ240667197\>为我们的程序找出错误，并提醒我们修复一个一直存在的大bug。
 - 感谢 **雷霆**\<QQ3555268519\>为我们的程序找出错误，并提醒修复bug。
 
 >	感谢广大群友为此程序提供的测试等支持
 >
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Musicreater Version: 0.5.0.2 Summary:
+Metadata-Version: 2.1 Name: Musicreater Version: 0.5.1 Summary:
 ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã midé³ä¹è½¬æ¢åºã Home-page:
 https://github.com/TriM-Organization/Musicreater Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: Chinese (Simplified) Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -60,15 +60,15 @@
 âæ­èÂ·æ¯ç¦å°æâ**\>
 å¸¦æ¥çmidié³è²è§£æä»¥åè½¬æ¢æä»¤çç®æ³ï¼æä»¬å°å¶æ¹ç¼å¹¶åºç¨ï¼åæ¶ï¼æè°¢ä»ç
 [ç½é¡µçè½¬æ¢å¨](https://dislink.github.io/midi2bdx/
 )ç»æä»¬çå¼åä¸æ´æ°å¸¦æ¥å·¨å¤§çåååå¨åï¼è®©æä»¬å¨åæ¬ä¸éªç»å°çæ¸é±¼éè·¯ä¸è½¬åå¼åï¼å¸æä»è½èä¸ä¸ä¸ªçæ³çå¤§å­¦ï¼
 - æè°¢ **Touch âå·åâ**\>
 æä¾çBDXå¯¼å¥æµè¯æ¯æï¼å¹¶å¯¹ç¨åºçæ¹è¿æä¾äºä¸°å¯çæè§ï¼åæ¶ä¹æè°¢ä»çä¸æ­å°è¯æ°çåå®¹ï¼ä½¿æä»¬çæéæ´è¿ä¸æ­¥
 - æè°¢ **Mono**\>
-åé¦å®è£æ¶çé®é¢ï¼è¾å©æä»¬æ¾å°äºè§çªæä½ç³»ç»ä¸çå¼å®¹æ§é®é¢
+åé¦å®è£æ¶çé®é¢ï¼è¾å©æä»¬æ¾å°äºè§çªæä½ç³»ç»ä¸çå¼å®¹æ§é®é¢ï¼æè°¢å¶åé¦å»¶è¿æ­æ¾å¨åºç°çéå¤§é®é¢ï¼è®©æä»¬å¾ä»¥ä¿®æ¹å¨é¨å»¶è¿æ­æ¾éè¯¯
 - æè°¢ **Ammelia âè¾ç±³å©äºâ**\>
 æ¦ä¿æä»¬è¿è¡æ°çåè½å¼åï¼å¹¶ä¸ºæ°åè½æåºäºéå¸¸ä¼ç§çå¤§éå»ºè®®ï¼ä»¥åæä¾çBDXå¯¼å¥æµè¯æ¯æï¼ä¸ºæä»¬çæ°ç»æçæç®æ³æä¾äºå¤§éçå®éçè®ºæ¯æ
 - æè°¢ **[ç¥ç¾½](https://gitee.com/snowykami) â[SnowyKami](https://
 github.com/snowyfirefly)â**
 å¯¹æä»¬é¡¹ç®çæ¯æä¸å®£ä¼ ï¼å¸æä»è½èçä¸æä¼ç§çå¤§å­¦ï¼
 - æè°¢ **æä»¤å¸_è¦åæ
 playjuice123**\>ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéæä»¬ä¿®å¤ä¸ä¸ªä¸ç´å­å¨çå¤§bugã
```

### Comparing `Musicreater-0.5.0.2/PKG-INFO` & `Musicreater-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 0.5.0.2
+Version: 0.5.1
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
@@ -107,15 +107,15 @@
 本致谢列表排名无顺序。
 
 - 感谢 **昀梦**\<QQ1515399885\> 找出指令生成错误bug并指正
 - 感谢由 **Charlie_Ping “查理平”** 带来的BDX文件转换参考，以及MIDI-我的世界对应乐器参考表格
 - 感谢由 **[CMA_2401PT](https://github.com/CMA2401PT)** 为我们的软件开发的一些方面进行指导，同时我们参考了他的BDXworkshop作为BDX结构编辑的参考
 - 感谢由 **[Dislink Sforza](https://github.com/Dislink) “断联·斯福尔扎”**\<QQ1600515314\> 带来的midi音色解析以及转换指令的算法，我们将其改编并应用；同时，感谢他的[网页版转换器](https://dislink.github.io/midi2bdx/)给我们的开发与更新带来巨大的压力和动力，让我们在原本一骑绝尘的摸鱼道路上转向开发，希望他能考上一个理想的大学！
 - 感谢 **Touch “偷吃”**\<QQ1793537164\> 提供的BDX导入测试支持，并对程序的改进提供了丰富的意见；同时也感谢他的不断尝试新的内容，使我们的排错更进一步
-- 感谢 **Mono**\<QQ738893087\> 反馈安装时的问题，辅助我们找到了视窗操作系统下的兼容性问题
+- 感谢 **Mono**\<QQ738893087\> 反馈安装时的问题，辅助我们找到了视窗操作系统下的兼容性问题；感谢其反馈延迟播放器出现的重大问题，让我们得以修改全部延迟播放错误
 - 感谢 **Ammelia “艾米利亚”**\<QQ2838334637\> 敦促我们进行新的功能开发，并为新功能提出了非常优秀的大量建议，以及提供的BDX导入测试支持，为我们的新结构生成算法提供了大量的实际理论支持
 - 感谢 **[神羽](https://gitee.com/snowykami) “[SnowyKami](https://github.com/snowyfirefly)”** 对我们项目的支持与宣传，希望他能考的一所优秀的大学！
 - 感谢 **指令师_苦力怕 playjuice123**\<QQ240667197\>为我们的程序找出错误，并提醒我们修复一个一直存在的大bug。
 - 感谢 **雷霆**\<QQ3555268519\>为我们的程序找出错误，并提醒修复bug。
 
 >	感谢广大群友为此程序提供的测试等支持
 >
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Musicreater Version: 0.5.0.2 Summary:
+Metadata-Version: 2.1 Name: Musicreater Version: 0.5.1 Summary:
 ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã midé³ä¹è½¬æ¢åºã Home-page:
 https://github.com/TriM-Organization/Musicreater Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: Chinese (Simplified) Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -60,15 +60,15 @@
 âæ­èÂ·æ¯ç¦å°æâ**\>
 å¸¦æ¥çmidié³è²è§£æä»¥åè½¬æ¢æä»¤çç®æ³ï¼æä»¬å°å¶æ¹ç¼å¹¶åºç¨ï¼åæ¶ï¼æè°¢ä»ç
 [ç½é¡µçè½¬æ¢å¨](https://dislink.github.io/midi2bdx/
 )ç»æä»¬çå¼åä¸æ´æ°å¸¦æ¥å·¨å¤§çåååå¨åï¼è®©æä»¬å¨åæ¬ä¸éªç»å°çæ¸é±¼éè·¯ä¸è½¬åå¼åï¼å¸æä»è½èä¸ä¸ä¸ªçæ³çå¤§å­¦ï¼
 - æè°¢ **Touch âå·åâ**\>
 æä¾çBDXå¯¼å¥æµè¯æ¯æï¼å¹¶å¯¹ç¨åºçæ¹è¿æä¾äºä¸°å¯çæè§ï¼åæ¶ä¹æè°¢ä»çä¸æ­å°è¯æ°çåå®¹ï¼ä½¿æä»¬çæéæ´è¿ä¸æ­¥
 - æè°¢ **Mono**\>
-åé¦å®è£æ¶çé®é¢ï¼è¾å©æä»¬æ¾å°äºè§çªæä½ç³»ç»ä¸çå¼å®¹æ§é®é¢
+åé¦å®è£æ¶çé®é¢ï¼è¾å©æä»¬æ¾å°äºè§çªæä½ç³»ç»ä¸çå¼å®¹æ§é®é¢ï¼æè°¢å¶åé¦å»¶è¿æ­æ¾å¨åºç°çéå¤§é®é¢ï¼è®©æä»¬å¾ä»¥ä¿®æ¹å¨é¨å»¶è¿æ­æ¾éè¯¯
 - æè°¢ **Ammelia âè¾ç±³å©äºâ**\>
 æ¦ä¿æä»¬è¿è¡æ°çåè½å¼åï¼å¹¶ä¸ºæ°åè½æåºäºéå¸¸ä¼ç§çå¤§éå»ºè®®ï¼ä»¥åæä¾çBDXå¯¼å¥æµè¯æ¯æï¼ä¸ºæä»¬çæ°ç»æçæç®æ³æä¾äºå¤§éçå®éçè®ºæ¯æ
 - æè°¢ **[ç¥ç¾½](https://gitee.com/snowykami) â[SnowyKami](https://
 github.com/snowyfirefly)â**
 å¯¹æä»¬é¡¹ç®çæ¯æä¸å®£ä¼ ï¼å¸æä»è½èçä¸æä¼ç§çå¤§å­¦ï¼
 - æè°¢ **æä»¤å¸_è¦åæ
 playjuice123**\>ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéæä»¬ä¿®å¤ä¸ä¸ªä¸ç´å­å¨çå¤§bugã
```

### Comparing `Musicreater-0.5.0.2/README.md` & `Musicreater-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 本致谢列表排名无顺序。
 
 - 感谢 **昀梦**\<QQ1515399885\> 找出指令生成错误bug并指正
 - 感谢由 **Charlie_Ping “查理平”** 带来的BDX文件转换参考，以及MIDI-我的世界对应乐器参考表格
 - 感谢由 **[CMA_2401PT](https://github.com/CMA2401PT)** 为我们的软件开发的一些方面进行指导，同时我们参考了他的BDXworkshop作为BDX结构编辑的参考
 - 感谢由 **[Dislink Sforza](https://github.com/Dislink) “断联·斯福尔扎”**\<QQ1600515314\> 带来的midi音色解析以及转换指令的算法，我们将其改编并应用；同时，感谢他的[网页版转换器](https://dislink.github.io/midi2bdx/)给我们的开发与更新带来巨大的压力和动力，让我们在原本一骑绝尘的摸鱼道路上转向开发，希望他能考上一个理想的大学！
 - 感谢 **Touch “偷吃”**\<QQ1793537164\> 提供的BDX导入测试支持，并对程序的改进提供了丰富的意见；同时也感谢他的不断尝试新的内容，使我们的排错更进一步
-- 感谢 **Mono**\<QQ738893087\> 反馈安装时的问题，辅助我们找到了视窗操作系统下的兼容性问题
+- 感谢 **Mono**\<QQ738893087\> 反馈安装时的问题，辅助我们找到了视窗操作系统下的兼容性问题；感谢其反馈延迟播放器出现的重大问题，让我们得以修改全部延迟播放错误
 - 感谢 **Ammelia “艾米利亚”**\<QQ2838334637\> 敦促我们进行新的功能开发，并为新功能提出了非常优秀的大量建议，以及提供的BDX导入测试支持，为我们的新结构生成算法提供了大量的实际理论支持
 - 感谢 **[神羽](https://gitee.com/snowykami) “[SnowyKami](https://github.com/snowyfirefly)”** 对我们项目的支持与宣传，希望他能考的一所优秀的大学！
 - 感谢 **指令师_苦力怕 playjuice123**\<QQ240667197\>为我们的程序找出错误，并提醒我们修复一个一直存在的大bug。
 - 感谢 **雷霆**\<QQ3555268519\>为我们的程序找出错误，并提醒修复bug。
 
 >	感谢广大群友为此程序提供的测试等支持
 >
```

#### html2text {}

```diff
@@ -45,15 +45,15 @@
 âæ­èÂ·æ¯ç¦å°æâ**\>
 å¸¦æ¥çmidié³è²è§£æä»¥åè½¬æ¢æä»¤çç®æ³ï¼æä»¬å°å¶æ¹ç¼å¹¶åºç¨ï¼åæ¶ï¼æè°¢ä»ç
 [ç½é¡µçè½¬æ¢å¨](https://dislink.github.io/midi2bdx/
 )ç»æä»¬çå¼åä¸æ´æ°å¸¦æ¥å·¨å¤§çåååå¨åï¼è®©æä»¬å¨åæ¬ä¸éªç»å°çæ¸é±¼éè·¯ä¸è½¬åå¼åï¼å¸æä»è½èä¸ä¸ä¸ªçæ³çå¤§å­¦ï¼
 - æè°¢ **Touch âå·åâ**\>
 æä¾çBDXå¯¼å¥æµè¯æ¯æï¼å¹¶å¯¹ç¨åºçæ¹è¿æä¾äºä¸°å¯çæè§ï¼åæ¶ä¹æè°¢ä»çä¸æ­å°è¯æ°çåå®¹ï¼ä½¿æä»¬çæéæ´è¿ä¸æ­¥
 - æè°¢ **Mono**\>
-åé¦å®è£æ¶çé®é¢ï¼è¾å©æä»¬æ¾å°äºè§çªæä½ç³»ç»ä¸çå¼å®¹æ§é®é¢
+åé¦å®è£æ¶çé®é¢ï¼è¾å©æä»¬æ¾å°äºè§çªæä½ç³»ç»ä¸çå¼å®¹æ§é®é¢ï¼æè°¢å¶åé¦å»¶è¿æ­æ¾å¨åºç°çéå¤§é®é¢ï¼è®©æä»¬å¾ä»¥ä¿®æ¹å¨é¨å»¶è¿æ­æ¾éè¯¯
 - æè°¢ **Ammelia âè¾ç±³å©äºâ**\>
 æ¦ä¿æä»¬è¿è¡æ°çåè½å¼åï¼å¹¶ä¸ºæ°åè½æåºäºéå¸¸ä¼ç§çå¤§éå»ºè®®ï¼ä»¥åæä¾çBDXå¯¼å¥æµè¯æ¯æï¼ä¸ºæä»¬çæ°ç»æçæç®æ³æä¾äºå¤§éçå®éçè®ºæ¯æ
 - æè°¢ **[ç¥ç¾½](https://gitee.com/snowykami) â[SnowyKami](https://
 github.com/snowyfirefly)â**
 å¯¹æä»¬é¡¹ç®çæ¯æä¸å®£ä¼ ï¼å¸æä»è½èçä¸æä¼ç§çå¤§å­¦ï¼
 - æè°¢ **æä»¤å¸_è¦åæ
 playjuice123**\>ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéæä»¬ä¿®å¤ä¸ä¸ªä¸ç´å­å¨çå¤§bugã
```

### Comparing `Musicreater-0.5.0.2/setup.py` & `Musicreater-0.5.1/setup.py`

 * *Files identical despite different names*

