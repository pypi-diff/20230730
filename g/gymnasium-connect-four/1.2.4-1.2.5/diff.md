# Comparing `tmp/gymnasium_connect_four-1.2.4.tar.gz` & `tmp/gymnasium_connect_four-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_connect_four-1.2.4.tar", last modified: Sun Jul 30 08:02:12 2023, max compression
+gzip compressed data, was "gymnasium_connect_four-1.2.5.tar", last modified: Sun Jul 30 08:06:43 2023, max compression
```

## Comparing `gymnasium_connect_four-1.2.4.tar` & `gymnasium_connect_four-1.2.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 08:02:12.127942 gymnasium_connect_four-1.2.4/
--rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.4/LICENSE
--rw-rw-rw-   0        0        0      251 2023-07-30 08:02:12.127942 gymnasium_connect_four-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    11334 2023-07-30 07:23:29.000000 gymnasium_connect_four-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 08:02:12.099884 gymnasium_connect_four-1.2.4/connect_four_gymnasium/
--rw-rw-rw-   0        0        0     9238 2023-07-30 08:01:03.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/ConnectFourEnv.py
--rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:02:12.115886 gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/
--rw-rw-rw-   0        0        0     4654 2023-07-29 17:00:12.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/AdultPlayer.py
--rw-rw-rw-   0        0        0     4378 2023-07-29 17:00:36.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/AdultSmarterPlayer.py
--rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/BabyPlayer.py
--rw-rw-rw-   0        0        0     1881 2023-07-29 14:17:29.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/ChildPlayer.py
--rw-rw-rw-   0        0        0     2248 2023-07-29 17:00:55.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/ChildSmarterPlayer.py
--rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/ConsolePlayer.py
--rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/ModelPlayer.py
--rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/Player.py
--rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/SimulatePlayer.py
--rw-rw-rw-   0        0        0     3163 2023-07-29 17:01:08.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/TeenagerPlayer.py
--rw-rw-rw-   0        0        0     4378 2023-07-29 17:01:22.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
--rw-rw-rw-   0        0        0      446 2023-07-29 10:59:21.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:02:12.119416 gymnasium_connect_four-1.2.4/connect_four_gymnasium/tools/
--rw-rw-rw-   0        0        0     3238 2023-07-29 14:40:52.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/tools/EloLeaderboard.py
--rw-rw-rw-   0        0        0     4744 2023-07-29 14:17:37.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/tools/Update_bot_elo.py
--rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.4/connect_four_gymnasium/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:02:12.124418 gymnasium_connect_four-1.2.4/gymnasium_connect_four.egg-info/
--rw-rw-rw-   0        0        0      251 2023-07-30 08:02:12.000000 gymnasium_connect_four-1.2.4/gymnasium_connect_four.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2023-07-30 08:02:12.000000 gymnasium_connect_four-1.2.4/gymnasium_connect_four.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 08:02:12.000000 gymnasium_connect_four-1.2.4/gymnasium_connect_four.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-30 08:02:12.000000 gymnasium_connect_four-1.2.4/gymnasium_connect_four.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-30 08:02:12.000000 gymnasium_connect_four-1.2.4/gymnasium_connect_four.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 08:02:12.127942 gymnasium_connect_four-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-07-30 08:02:04.000000 gymnasium_connect_four-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:02:12.126427 gymnasium_connect_four-1.2.4/test/
--rw-rw-rw-   0        0        0     4722 2023-07-29 17:17:01.000000 gymnasium_connect_four-1.2.4/test/test_no_opponant.py
--rw-rw-rw-   0        0        0    21564 2023-07-29 17:15:09.000000 gymnasium_connect_four-1.2.4/test/test_power_4_logic.py
--rw-rw-rw-   0        0        0     2372 2023-07-29 17:18:55.000000 gymnasium_connect_four-1.2.4/test/test_ppo_env.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:06:43.298202 gymnasium_connect_four-1.2.5/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-07-30 08:06:43.298202 gymnasium_connect_four-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    11334 2023-07-30 07:23:29.000000 gymnasium_connect_four-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 08:06:43.279785 gymnasium_connect_four-1.2.5/connect_four_gymnasium/
+-rw-rw-rw-   0        0        0     9241 2023-07-30 08:06:17.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/ConnectFourEnv.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:06:43.288302 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/
+-rw-rw-rw-   0        0        0     4654 2023-07-29 17:00:12.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/AdultPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-07-29 17:00:36.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/AdultSmarterPlayer.py
+-rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/BabyPlayer.py
+-rw-rw-rw-   0        0        0     1881 2023-07-29 14:17:29.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ChildPlayer.py
+-rw-rw-rw-   0        0        0     2248 2023-07-29 17:00:55.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ChildSmarterPlayer.py
+-rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ConsolePlayer.py
+-rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ModelPlayer.py
+-rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/Player.py
+-rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/SimulatePlayer.py
+-rw-rw-rw-   0        0        0     3163 2023-07-29 17:01:08.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/TeenagerPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-07-29 17:01:22.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
+-rw-rw-rw-   0        0        0      446 2023-07-29 10:59:21.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:06:43.295688 gymnasium_connect_four-1.2.5/connect_four_gymnasium/tools/
+-rw-rw-rw-   0        0        0     3238 2023-07-29 14:40:52.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/tools/EloLeaderboard.py
+-rw-rw-rw-   0        0        0     4744 2023-07-29 14:17:37.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/tools/Update_bot_elo.py
+-rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:06:43.298202 gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-07-30 08:06:43.000000 gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2023-07-30 08:06:43.000000 gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 08:06:43.000000 gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-30 08:06:43.000000 gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-30 08:06:43.000000 gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 08:06:43.298202 gymnasium_connect_four-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-07-30 08:06:26.000000 gymnasium_connect_four-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:06:43.298202 gymnasium_connect_four-1.2.5/test/
+-rw-rw-rw-   0        0        0     4722 2023-07-29 17:17:01.000000 gymnasium_connect_four-1.2.5/test/test_no_opponant.py
+-rw-rw-rw-   0        0        0    21564 2023-07-29 17:15:09.000000 gymnasium_connect_four-1.2.5/test/test_power_4_logic.py
+-rw-rw-rw-   0        0        0     2372 2023-07-29 17:18:55.000000 gymnasium_connect_four-1.2.5/test/test_ppo_env.py
```

### Comparing `gymnasium_connect_four-1.2.4/LICENSE` & `gymnasium_connect_four-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/README.md` & `gymnasium_connect_four-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/connect_four_gymnasium/ConnectFourEnv.py` & `gymnasium_connect_four-1.2.5/connect_four_gymnasium/ConnectFourEnv.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         new_env = ConnectFourEnv(opponent=self._opponent, render_mode=self.render_mode, first_player=self.first_player)
         new_env.next_player_to_play = self.next_player_to_play
         new_env.board = self.board.copy()
         return new_env
 
     def clone_and_play(self, action):
         newself = self.clone()
-        newBoard, result, IsFinish, isTruncated = newself.step(action)
+        newBoard, result, IsFinish, isTruncated, _ = newself.step(action)
         return newBoard, result, IsFinish, isTruncated, newself
 
     def step(self, action, play_opponent=True):
         action = action.item() if isinstance(action, np.ndarray) else action
 
         result, is_finish = self._play_action(action, 1)
```

### Comparing `gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/AdultPlayer.py` & `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/AdultPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/AdultSmarterPlayer.py` & `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/AdultSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/BabyPlayer.py` & `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/BabyPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/ChildPlayer.py` & `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ChildPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/ChildSmarterPlayer.py` & `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ChildSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/ConsolePlayer.py` & `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ConsolePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/ModelPlayer.py` & `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ModelPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/SimulatePlayer.py` & `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/SimulatePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/TeenagerPlayer.py` & `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/TeenagerPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/connect_four_gymnasium/players/TeenagerSmarterPlayer.py` & `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/TeenagerSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/connect_four_gymnasium/tools/EloLeaderboard.py` & `gymnasium_connect_four-1.2.5/connect_four_gymnasium/tools/EloLeaderboard.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/connect_four_gymnasium/tools/Update_bot_elo.py` & `gymnasium_connect_four-1.2.5/connect_four_gymnasium/tools/Update_bot_elo.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/gymnasium_connect_four.egg-info/SOURCES.txt` & `gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/setup.py` & `gymnasium_connect_four-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='gymnasium_connect_four',
-    version='1.2.4',
+    version='1.2.5',
     description='A connect 4 (connect four) environment for OpenAI Gym and Gymnasium',
     author='Lucas Bertola',
     url='https://github.com/lucasBertola/Connect-4-env',  
     # author_email='your.email@example.com',
     packages=find_packages(),
     install_requires=[
         'pygame==2.1.3',
```

### Comparing `gymnasium_connect_four-1.2.4/test/test_no_opponant.py` & `gymnasium_connect_four-1.2.5/test/test_no_opponant.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/test/test_power_4_logic.py` & `gymnasium_connect_four-1.2.5/test/test_power_4_logic.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.4/test/test_ppo_env.py` & `gymnasium_connect_four-1.2.5/test/test_ppo_env.py`

 * *Files identical despite different names*

