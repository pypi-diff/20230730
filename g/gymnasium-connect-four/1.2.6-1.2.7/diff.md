# Comparing `tmp/gymnasium_connect_four-1.2.6.tar.gz` & `tmp/gymnasium_connect_four-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_connect_four-1.2.6.tar", last modified: Sun Jul 30 17:30:03 2023, max compression
+gzip compressed data, was "gymnasium_connect_four-1.2.7.tar", last modified: Sun Jul 30 17:35:50 2023, max compression
```

## Comparing `gymnasium_connect_four-1.2.6.tar` & `gymnasium_connect_four-1.2.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 17:30:03.683437 gymnasium_connect_four-1.2.6/
--rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.6/LICENSE
--rw-rw-rw-   0        0        0      251 2023-07-30 17:30:03.682439 gymnasium_connect_four-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    11473 2023-07-30 16:53:38.000000 gymnasium_connect_four-1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 17:30:03.658962 gymnasium_connect_four-1.2.6/connect_four_gymnasium/
--rw-rw-rw-   0        0        0     9241 2023-07-30 08:06:17.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/ConnectFourEnv.py
--rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 17:30:03.670983 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/
--rw-rw-rw-   0        0        0     4654 2023-07-30 16:49:29.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/AdultPlayer.py
--rw-rw-rw-   0        0        0     4378 2023-07-30 16:49:19.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/AdultSmarterPlayer.py
--rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/BabyPlayer.py
--rw-rw-rw-   0        0        0      649 2023-07-30 17:27:29.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/BabySmarterPlayer.py
--rw-rw-rw-   0        0        0     1920 2023-07-30 16:50:55.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ChildPlayer.py
--rw-rw-rw-   0        0        0     2248 2023-07-30 16:50:49.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ChildSmarterPlayer.py
--rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ConsolePlayer.py
--rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ModelPlayer.py
--rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/Player.py
--rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/SimulatePlayer.py
--rw-rw-rw-   0        0        0     3163 2023-07-30 16:49:44.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/TeenagerPlayer.py
--rw-rw-rw-   0        0        0     4378 2023-07-30 16:49:36.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
--rw-rw-rw-   0        0        0      496 2023-07-30 16:31:44.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 17:30:03.673983 gymnasium_connect_four-1.2.6/connect_four_gymnasium/tools/
--rw-rw-rw-   0        0        0     4173 2023-07-30 17:28:44.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/tools/EloLeaderboard.py
--rw-rw-rw-   0        0        0     4805 2023-07-30 16:46:39.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/tools/Update_bot_elo.py
--rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 17:30:03.677983 gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/
--rw-rw-rw-   0        0        0      251 2023-07-30 17:30:03.000000 gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1166 2023-07-30 17:30:03.000000 gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 17:30:03.000000 gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-30 17:30:03.000000 gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-30 17:30:03.000000 gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 17:30:03.683437 gymnasium_connect_four-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-07-30 17:29:37.000000 gymnasium_connect_four-1.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 17:30:03.681438 gymnasium_connect_four-1.2.6/test/
--rw-rw-rw-   0        0        0     4722 2023-07-29 17:17:01.000000 gymnasium_connect_four-1.2.6/test/test_no_opponant.py
--rw-rw-rw-   0        0        0    21564 2023-07-29 17:15:09.000000 gymnasium_connect_four-1.2.6/test/test_power_4_logic.py
--rw-rw-rw-   0        0        0     2372 2023-07-29 17:18:55.000000 gymnasium_connect_four-1.2.6/test/test_ppo_env.py
+drwxrwxrwx   0        0        0        0 2023-07-30 17:35:50.079176 gymnasium_connect_four-1.2.7/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-07-30 17:35:50.077672 gymnasium_connect_four-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11454 2023-07-30 17:35:07.000000 gymnasium_connect_four-1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 17:35:50.052651 gymnasium_connect_four-1.2.7/connect_four_gymnasium/
+-rw-rw-rw-   0        0        0     9241 2023-07-30 08:06:17.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/ConnectFourEnv.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 17:35:50.066160 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/
+-rw-rw-rw-   0        0        0     4654 2023-07-30 16:49:29.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/AdultPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-07-30 16:49:19.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/AdultSmarterPlayer.py
+-rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/BabyPlayer.py
+-rw-rw-rw-   0        0        0      649 2023-07-30 17:27:29.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/BabySmarterPlayer.py
+-rw-rw-rw-   0        0        0     1920 2023-07-30 16:50:55.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ChildPlayer.py
+-rw-rw-rw-   0        0        0     2248 2023-07-30 16:50:49.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ChildSmarterPlayer.py
+-rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ConsolePlayer.py
+-rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ModelPlayer.py
+-rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/Player.py
+-rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/SimulatePlayer.py
+-rw-rw-rw-   0        0        0     3163 2023-07-30 16:49:44.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/TeenagerPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-07-30 16:49:36.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
+-rw-rw-rw-   0        0        0      496 2023-07-30 16:31:44.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 17:35:50.069668 gymnasium_connect_four-1.2.7/connect_four_gymnasium/tools/
+-rw-rw-rw-   0        0        0     4082 2023-07-30 17:34:52.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/tools/EloLeaderboard.py
+-rw-rw-rw-   0        0        0     4805 2023-07-30 16:46:39.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/tools/Update_bot_elo.py
+-rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 17:35:50.074673 gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-07-30 17:35:49.000000 gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1166 2023-07-30 17:35:50.000000 gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 17:35:49.000000 gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-30 17:35:49.000000 gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-30 17:35:49.000000 gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 17:35:50.079176 gymnasium_connect_four-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-07-30 17:35:43.000000 gymnasium_connect_four-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 17:35:50.077672 gymnasium_connect_four-1.2.7/test/
+-rw-rw-rw-   0        0        0     4722 2023-07-29 17:17:01.000000 gymnasium_connect_four-1.2.7/test/test_no_opponant.py
+-rw-rw-rw-   0        0        0    21564 2023-07-29 17:15:09.000000 gymnasium_connect_four-1.2.7/test/test_power_4_logic.py
+-rw-rw-rw-   0        0        0     2372 2023-07-29 17:18:55.000000 gymnasium_connect_four-1.2.7/test/test_ppo_env.py
```

### Comparing `gymnasium_connect_four-1.2.6/LICENSE` & `gymnasium_connect_four-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/README.md` & `gymnasium_connect_four-1.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 ```python
 env = ConnectFourEnv(opponent=BabyPlayer())
 model = PPO("MlpPolicy", env)
 model.learn(total_timesteps=10000)
 
 myModelPlayer = ModelPlayer(model,name="Your trained Model")
 
-your_model_elo = EloLeaderboard().get_elo([myModelPlayer], num_matches=100)
+your_model_elo = EloLeaderboard().get_elo(myModelPlayer)
 ```
 
 You can find an example of how to use this tool in a Google Colab notebook [here](https://colab.research.google.com/github/lucasBertola/Connect-4-Gym-env-Reinforcement-learning/blob/main/exemples/Train_ppo_and_test.ipynb).
 
 ## Detailed Documentation
 
 For a comprehensive overview of the methods and classes used in this environment, please refer to the [detailed documentation](https://github.com/lucasBertola/Connect-4-Gym-env-Reinforcement-learning/blob/main/DOCUMENTATION.md) available on the GitHub repository. This documentation provides in-depth explanations and examples to help you better understand the inner workings of the Connect Four environment and make the most of its features.
```

#### html2text {}

```diff
@@ -119,26 +119,26 @@
 have an "absolute" idea of the progress of your AI. For example, if an AI
 learns by fighting against itself, we know that it is getting stronger as it
 would be able to win against its older versions, but this is not enough to
 evaluate if it has learned a lot. This is where our tool comes in, which allows
 you to give an Elo rating to the AI. Here is how to use it in Python: ```python
 env = ConnectFourEnv(opponent=BabyPlayer()) model = PPO("MlpPolicy", env)
 model.learn(total_timesteps=10000) myModelPlayer = ModelPlayer(model,name="Your
-trained Model") your_model_elo = EloLeaderboard().get_elo([myModelPlayer],
-num_matches=100) ``` You can find an example of how to use this tool in a
-Google Colab notebook [here](https://colab.research.google.com/github/
-lucasBertola/Connect-4-Gym-env-Reinforcement-learning/blob/main/exemples/
-Train_ppo_and_test.ipynb). ## Detailed Documentation For a comprehensive
-overview of the methods and classes used in this environment, please refer to
-the [detailed documentation](https://github.com/lucasBertola/Connect-4-Gym-env-
-Reinforcement-learning/blob/main/DOCUMENTATION.md) available on the GitHub
-repository. This documentation provides in-depth explanations and examples to
-help you better understand the inner workings of the Connect Four environment
-and make the most of its features. ## Testing We believe in the importance of
-testing. That's why we have included a suite of tests in the `test` directory.
-To run the tests, simply use the command `pytest`. ## Contribute & Support We
-warmly welcome contributions from the community. If you have an idea for an
-improvement or found a bug, don't hesitate to open an issue or submit a pull
-request. Your input is greatly appreciated, and our project is made better by
-your participation! If you find this repository useful, please give it a star!
-## License This project is licensed under the MIT License. See the `LICENSE`
-file for details.
+trained Model") your_model_elo = EloLeaderboard().get_elo(myModelPlayer) ```
+You can find an example of how to use this tool in a Google Colab notebook
+[here](https://colab.research.google.com/github/lucasBertola/Connect-4-Gym-env-
+Reinforcement-learning/blob/main/exemples/Train_ppo_and_test.ipynb). ##
+Detailed Documentation For a comprehensive overview of the methods and classes
+used in this environment, please refer to the [detailed documentation](https://
+github.com/lucasBertola/Connect-4-Gym-env-Reinforcement-learning/blob/main/
+DOCUMENTATION.md) available on the GitHub repository. This documentation
+provides in-depth explanations and examples to help you better understand the
+inner workings of the Connect Four environment and make the most of its
+features. ## Testing We believe in the importance of testing. That's why we
+have included a suite of tests in the `test` directory. To run the tests,
+simply use the command `pytest`. ## Contribute & Support We warmly welcome
+contributions from the community. If you have an idea for an improvement or
+found a bug, don't hesitate to open an issue or submit a pull request. Your
+input is greatly appreciated, and our project is made better by your
+participation! If you find this repository useful, please give it a star! ##
+License This project is licensed under the MIT License. See the `LICENSE` file
+for details.
```

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/ConnectFourEnv.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/ConnectFourEnv.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/AdultPlayer.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/AdultPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/AdultSmarterPlayer.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/AdultSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/BabyPlayer.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/BabyPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/BabySmarterPlayer.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/BabySmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ChildPlayer.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ChildPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ChildSmarterPlayer.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ChildSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ConsolePlayer.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ConsolePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ModelPlayer.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ModelPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/SimulatePlayer.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/SimulatePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/TeenagerPlayer.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/TeenagerPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/TeenagerSmarterPlayer.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/TeenagerSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/tools/EloLeaderboard.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/tools/EloLeaderboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import math
 import sys
 import random
-import time
 sys.path.append('../../')
 
 from connect_four_gymnasium.ConnectFourEnv import ConnectFourEnv
 from connect_four_gymnasium.players import (
     BabyPlayer,
     BabySmarterPlayer,
     ChildPlayer,
@@ -55,26 +54,25 @@
             scores = self.get_scores(player, closest_opponents)
             for opponent, score in zip(closest_opponents, scores):
                 player_won = score > 0
                 draw = score == 0
                 match_results.append((player_won, draw, opponent.getElo()))
                 k_factor = 400 / (1 + (gamePlayed))
                 actualElo = self.update_elo(actualElo, opponent.getElo(), player_won, k_factor, draw)
-                print(f"{player.getName()} vs {opponent.getName()}: {score} - {actualElo}")
                 gamePlayed += 1
 
         for _ in range(2000):
             for player_won, draw, opponent_elo in match_results:
                 k_factor = 400 / (1 + (gamePlayed))
                 actualElo = self.update_elo(actualElo, opponent_elo, player_won, k_factor, draw)
                 gamePlayed += 1
 
         return actualElo
 
-    def get_elo(self, player, num_matches=400):
+    def get_elo(self, player, num_matches=100):
         actualElo = player.getElo() if player.getElo() is not None else 1400
         actualElo = 1400
         return self.play_rounds(player, actualElo, num_matches)
 
     def get_scores(self, player, opponents):
         envs = [ConnectFourEnv(opponent=opponent) for opponent in opponents]
         obs_list = [obs for obs, _ in [env.reset() for env in envs]]
@@ -96,13 +94,13 @@
 
             remaining_indices = new_remaining_indices
 
         return scores
 
 
 if __name__ == "__main__":
-
+    import time
     elo_leaderboard = EloLeaderboard()
     start_time = time.time()
     print(elo_leaderboard.get_elo(BabySmarterPlayer(), num_matches=20))
     end_time = time.time()
     print(f"Time elapsed: {end_time - start_time} seconds")
```

### Comparing `gymnasium_connect_four-1.2.6/connect_four_gymnasium/tools/Update_bot_elo.py` & `gymnasium_connect_four-1.2.7/connect_four_gymnasium/tools/Update_bot_elo.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/SOURCES.txt` & `gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/setup.py` & `gymnasium_connect_four-1.2.7/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='gymnasium_connect_four',
-    version='1.2.6',
+    version='1.2.7',
     description='A connect 4 (connect four) environment for OpenAI Gym and Gymnasium',
     author='Lucas Bertola',
     url='https://github.com/lucasBertola/Connect-4-env',  
     # author_email='your.email@example.com',
     packages=find_packages(),
     install_requires=[
         'pygame==2.1.3',
```

### Comparing `gymnasium_connect_four-1.2.6/test/test_no_opponant.py` & `gymnasium_connect_four-1.2.7/test/test_no_opponant.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/test/test_power_4_logic.py` & `gymnasium_connect_four-1.2.7/test/test_power_4_logic.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.6/test/test_ppo_env.py` & `gymnasium_connect_four-1.2.7/test/test_ppo_env.py`

 * *Files identical despite different names*

