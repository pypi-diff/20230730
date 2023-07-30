# Comparing `tmp/gymnasium_connect_four-1.2.5.tar.gz` & `tmp/gymnasium_connect_four-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_connect_four-1.2.5.tar", last modified: Sun Jul 30 08:06:43 2023, max compression
+gzip compressed data, was "gymnasium_connect_four-1.2.6.tar", last modified: Sun Jul 30 17:30:03 2023, max compression
```

## Comparing `gymnasium_connect_four-1.2.5.tar` & `gymnasium_connect_four-1.2.6.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 08:06:43.298202 gymnasium_connect_four-1.2.5/
--rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.5/LICENSE
--rw-rw-rw-   0        0        0      251 2023-07-30 08:06:43.298202 gymnasium_connect_four-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    11334 2023-07-30 07:23:29.000000 gymnasium_connect_four-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 08:06:43.279785 gymnasium_connect_four-1.2.5/connect_four_gymnasium/
--rw-rw-rw-   0        0        0     9241 2023-07-30 08:06:17.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/ConnectFourEnv.py
--rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:06:43.288302 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/
--rw-rw-rw-   0        0        0     4654 2023-07-29 17:00:12.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/AdultPlayer.py
--rw-rw-rw-   0        0        0     4378 2023-07-29 17:00:36.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/AdultSmarterPlayer.py
--rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/BabyPlayer.py
--rw-rw-rw-   0        0        0     1881 2023-07-29 14:17:29.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ChildPlayer.py
--rw-rw-rw-   0        0        0     2248 2023-07-29 17:00:55.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ChildSmarterPlayer.py
--rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ConsolePlayer.py
--rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ModelPlayer.py
--rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/Player.py
--rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/SimulatePlayer.py
--rw-rw-rw-   0        0        0     3163 2023-07-29 17:01:08.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/TeenagerPlayer.py
--rw-rw-rw-   0        0        0     4378 2023-07-29 17:01:22.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
--rw-rw-rw-   0        0        0      446 2023-07-29 10:59:21.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:06:43.295688 gymnasium_connect_four-1.2.5/connect_four_gymnasium/tools/
--rw-rw-rw-   0        0        0     3238 2023-07-29 14:40:52.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/tools/EloLeaderboard.py
--rw-rw-rw-   0        0        0     4744 2023-07-29 14:17:37.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/tools/Update_bot_elo.py
--rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.5/connect_four_gymnasium/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:06:43.298202 gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/
--rw-rw-rw-   0        0        0      251 2023-07-30 08:06:43.000000 gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2023-07-30 08:06:43.000000 gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 08:06:43.000000 gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-30 08:06:43.000000 gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-30 08:06:43.000000 gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 08:06:43.298202 gymnasium_connect_four-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-07-30 08:06:26.000000 gymnasium_connect_four-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:06:43.298202 gymnasium_connect_four-1.2.5/test/
--rw-rw-rw-   0        0        0     4722 2023-07-29 17:17:01.000000 gymnasium_connect_four-1.2.5/test/test_no_opponant.py
--rw-rw-rw-   0        0        0    21564 2023-07-29 17:15:09.000000 gymnasium_connect_four-1.2.5/test/test_power_4_logic.py
--rw-rw-rw-   0        0        0     2372 2023-07-29 17:18:55.000000 gymnasium_connect_four-1.2.5/test/test_ppo_env.py
+drwxrwxrwx   0        0        0        0 2023-07-30 17:30:03.683437 gymnasium_connect_four-1.2.6/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-07-30 17:30:03.682439 gymnasium_connect_four-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11473 2023-07-30 16:53:38.000000 gymnasium_connect_four-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 17:30:03.658962 gymnasium_connect_four-1.2.6/connect_four_gymnasium/
+-rw-rw-rw-   0        0        0     9241 2023-07-30 08:06:17.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/ConnectFourEnv.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 17:30:03.670983 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/
+-rw-rw-rw-   0        0        0     4654 2023-07-30 16:49:29.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/AdultPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-07-30 16:49:19.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/AdultSmarterPlayer.py
+-rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/BabyPlayer.py
+-rw-rw-rw-   0        0        0      649 2023-07-30 17:27:29.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/BabySmarterPlayer.py
+-rw-rw-rw-   0        0        0     1920 2023-07-30 16:50:55.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ChildPlayer.py
+-rw-rw-rw-   0        0        0     2248 2023-07-30 16:50:49.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ChildSmarterPlayer.py
+-rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ConsolePlayer.py
+-rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ModelPlayer.py
+-rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/Player.py
+-rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/SimulatePlayer.py
+-rw-rw-rw-   0        0        0     3163 2023-07-30 16:49:44.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/TeenagerPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-07-30 16:49:36.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
+-rw-rw-rw-   0        0        0      496 2023-07-30 16:31:44.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 17:30:03.673983 gymnasium_connect_four-1.2.6/connect_four_gymnasium/tools/
+-rw-rw-rw-   0        0        0     4173 2023-07-30 17:28:44.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/tools/EloLeaderboard.py
+-rw-rw-rw-   0        0        0     4805 2023-07-30 16:46:39.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/tools/Update_bot_elo.py
+-rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.6/connect_four_gymnasium/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 17:30:03.677983 gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-07-30 17:30:03.000000 gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1166 2023-07-30 17:30:03.000000 gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 17:30:03.000000 gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-30 17:30:03.000000 gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-30 17:30:03.000000 gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 17:30:03.683437 gymnasium_connect_four-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-07-30 17:29:37.000000 gymnasium_connect_four-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 17:30:03.681438 gymnasium_connect_four-1.2.6/test/
+-rw-rw-rw-   0        0        0     4722 2023-07-29 17:17:01.000000 gymnasium_connect_four-1.2.6/test/test_no_opponant.py
+-rw-rw-rw-   0        0        0    21564 2023-07-29 17:15:09.000000 gymnasium_connect_four-1.2.6/test/test_power_4_logic.py
+-rw-rw-rw-   0        0        0     2372 2023-07-29 17:18:55.000000 gymnasium_connect_four-1.2.6/test/test_ppo_env.py
```

### Comparing `gymnasium_connect_four-1.2.5/LICENSE` & `gymnasium_connect_four-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.5/README.md` & `gymnasium_connect_four-1.2.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,17 @@
 env = ConnectFourEnv(opponent=BabyPlayer())
 ```
 
 ### Player Descriptions
 
 - **BabyPlayer**: Plays random moves.
 
-- **ChildPlayer**: Plays random moves, but if there is a winning move, it will play it.
+- **BabySmarterPlayer**: Plays random legal moves, ensuring it doesn't play on a column when it's full.
+
+- **ChildPlayer**: Same as BabySmarterPlayer, but if there is a winning move, it will play it.
 
 - **ChildSmarterPlayer**: Same as ChildPlayer, but if there is a move that would make the opponent win, it will play that move to block the opponent.
 
 - **TeenagerPlayer**: Same as ChildSmarterPlayer, but excludes moves that would allow the opponent to win if they play on top of it.
 
 - **TeenagerSmarterPlayer**: Same as TeenagerPlayer, but checks if a move creates a line of three tokens with available spaces on both sides. If so, it will play that move.
 
@@ -137,21 +139,22 @@
 - **ConsolePlayer**: Asks for moves to play in the console. Perfect for testing your own AI.
 
 ### Elo Ratings
 
 Here are the Elo ratings of the different algorithms:
 
 ```
-1.  AdultSmarterPlayer:    1790
-2.  AdultPlayer:           1654
-3.  TeenagerSmarterPlayer: 1647
-4.  TeenagerPlayer:        1639
-5.  ChildSmarterPlayer:    1571
-6.  ChildPlayer:           1222
-7.  BabyPlayer:            1000
+1. AdultSmarterPlayer:    1802
+2. AdultPlayer:           1666
+3. TeenagerSmarterPlayer: 1658
+4. TeenagerPlayer:        1655
+5. ChildSmarterPlayer:    1571
+6. ChildPlayer:           1272
+7. BabySmarterPlayer:     1060
+8. BabyPlayer:            1000
 ```
 
 In addition to the provided players, we also offer a tool to evaluate the Elo rating of your own AI model. This is extremely useful to have an "absolute" idea of the progress of your AI. For example, if an AI learns by fighting against itself, we know that it is getting stronger as it would be able to win against its older versions, but this is not enough to evaluate if it has learned a lot. This is where our tool comes in, which allows you to give an Elo rating to the AI.
 
 Here is how to use it in Python:
 
 ```python
```

#### html2text {}

```diff
@@ -91,53 +91,54 @@
 as: - **Learning by playing against them**: You can improve your AI model by
 playing against these bots, which range from beginner to advanced levels. -
 **Comparing the level of self-learning models**: By playing against these bots,
 you can evaluate the performance of your self-learning model and position it in
 terms of skill level and elo. You can integrate players as opponents in your
 gym environment like this: ```python env = ConnectFourEnv(opponent=BabyPlayer
 ()) ``` ### Player Descriptions - **BabyPlayer**: Plays random moves. -
-**ChildPlayer**: Plays random moves, but if there is a winning move, it will
-play it. - **ChildSmarterPlayer**: Same as ChildPlayer, but if there is a move
-that would make the opponent win, it will play that move to block the opponent.
-- **TeenagerPlayer**: Same as ChildSmarterPlayer, but excludes moves that would
-allow the opponent to win if they play on top of it. -
-**TeenagerSmarterPlayer**: Same as TeenagerPlayer, but checks if a move creates
-a line of three tokens with available spaces on both sides. If so, it will play
-that move. - **AdultPlayer**: Same as TeenagerSmarterPlayer, but also checks if
-a move creates a line of three tokens with available spaces on both sides for
-the opponent. If so, it will play that move to block the opponent. -
-**AdultSmarterPlayer**: Same as AdultPlayer, but checks if a move allows to
-create multiple ways to win and plays that move. Also checks if a move allows
-the opponent to create multiple ways to win and plays that move to protect
-itself. - **ConsolePlayer**: Asks for moves to play in the console. Perfect for
-testing your own AI. ### Elo Ratings Here are the Elo ratings of the different
-algorithms: ``` 1. AdultSmarterPlayer: 1790 2. AdultPlayer: 1654 3.
-TeenagerSmarterPlayer: 1647 4. TeenagerPlayer: 1639 5. ChildSmarterPlayer: 1571
-6. ChildPlayer: 1222 7. BabyPlayer: 1000 ``` In addition to the provided
-players, we also offer a tool to evaluate the Elo rating of your own AI model.
-This is extremely useful to have an "absolute" idea of the progress of your AI.
-For example, if an AI learns by fighting against itself, we know that it is
-getting stronger as it would be able to win against its older versions, but
-this is not enough to evaluate if it has learned a lot. This is where our tool
-comes in, which allows you to give an Elo rating to the AI. Here is how to use
-it in Python: ```python env = ConnectFourEnv(opponent=BabyPlayer()) model = PPO
-("MlpPolicy", env) model.learn(total_timesteps=10000) myModelPlayer =
-ModelPlayer(model,name="Your trained Model") your_model_elo = EloLeaderboard
-().get_elo([myModelPlayer], num_matches=100) ``` You can find an example of how
-to use this tool in a Google Colab notebook [here](https://
-colab.research.google.com/github/lucasBertola/Connect-4-Gym-env-Reinforcement-
-learning/blob/main/exemples/Train_ppo_and_test.ipynb). ## Detailed
-Documentation For a comprehensive overview of the methods and classes used in
-this environment, please refer to the [detailed documentation](https://
-github.com/lucasBertola/Connect-4-Gym-env-Reinforcement-learning/blob/main/
-DOCUMENTATION.md) available on the GitHub repository. This documentation
-provides in-depth explanations and examples to help you better understand the
-inner workings of the Connect Four environment and make the most of its
-features. ## Testing We believe in the importance of testing. That's why we
-have included a suite of tests in the `test` directory. To run the tests,
-simply use the command `pytest`. ## Contribute & Support We warmly welcome
-contributions from the community. If you have an idea for an improvement or
-found a bug, don't hesitate to open an issue or submit a pull request. Your
-input is greatly appreciated, and our project is made better by your
-participation! If you find this repository useful, please give it a star! ##
-License This project is licensed under the MIT License. See the `LICENSE` file
-for details.
+**BabySmarterPlayer**: Plays random legal moves, ensuring it doesn't play on a
+column when it's full. - **ChildPlayer**: Same as BabySmarterPlayer, but if
+there is a winning move, it will play it. - **ChildSmarterPlayer**: Same as
+ChildPlayer, but if there is a move that would make the opponent win, it will
+play that move to block the opponent. - **TeenagerPlayer**: Same as
+ChildSmarterPlayer, but excludes moves that would allow the opponent to win if
+they play on top of it. - **TeenagerSmarterPlayer**: Same as TeenagerPlayer,
+but checks if a move creates a line of three tokens with available spaces on
+both sides. If so, it will play that move. - **AdultPlayer**: Same as
+TeenagerSmarterPlayer, but also checks if a move creates a line of three tokens
+with available spaces on both sides for the opponent. If so, it will play that
+move to block the opponent. - **AdultSmarterPlayer**: Same as AdultPlayer, but
+checks if a move allows to create multiple ways to win and plays that move.
+Also checks if a move allows the opponent to create multiple ways to win and
+plays that move to protect itself. - **ConsolePlayer**: Asks for moves to play
+in the console. Perfect for testing your own AI. ### Elo Ratings Here are the
+Elo ratings of the different algorithms: ``` 1. AdultSmarterPlayer: 1802 2.
+AdultPlayer: 1666 3. TeenagerSmarterPlayer: 1658 4. TeenagerPlayer: 1655 5.
+ChildSmarterPlayer: 1571 6. ChildPlayer: 1272 7. BabySmarterPlayer: 1060 8.
+BabyPlayer: 1000 ``` In addition to the provided players, we also offer a tool
+to evaluate the Elo rating of your own AI model. This is extremely useful to
+have an "absolute" idea of the progress of your AI. For example, if an AI
+learns by fighting against itself, we know that it is getting stronger as it
+would be able to win against its older versions, but this is not enough to
+evaluate if it has learned a lot. This is where our tool comes in, which allows
+you to give an Elo rating to the AI. Here is how to use it in Python: ```python
+env = ConnectFourEnv(opponent=BabyPlayer()) model = PPO("MlpPolicy", env)
+model.learn(total_timesteps=10000) myModelPlayer = ModelPlayer(model,name="Your
+trained Model") your_model_elo = EloLeaderboard().get_elo([myModelPlayer],
+num_matches=100) ``` You can find an example of how to use this tool in a
+Google Colab notebook [here](https://colab.research.google.com/github/
+lucasBertola/Connect-4-Gym-env-Reinforcement-learning/blob/main/exemples/
+Train_ppo_and_test.ipynb). ## Detailed Documentation For a comprehensive
+overview of the methods and classes used in this environment, please refer to
+the [detailed documentation](https://github.com/lucasBertola/Connect-4-Gym-env-
+Reinforcement-learning/blob/main/DOCUMENTATION.md) available on the GitHub
+repository. This documentation provides in-depth explanations and examples to
+help you better understand the inner workings of the Connect Four environment
+and make the most of its features. ## Testing We believe in the importance of
+testing. That's why we have included a suite of tests in the `test` directory.
+To run the tests, simply use the command `pytest`. ## Contribute & Support We
+warmly welcome contributions from the community. If you have an idea for an
+improvement or found a bug, don't hesitate to open an issue or submit a pull
+request. Your input is greatly appreciated, and our project is made better by
+your participation! If you find this repository useful, please give it a star!
+## License This project is licensed under the MIT License. See the `LICENSE`
+file for details.
```

### Comparing `gymnasium_connect_four-1.2.5/connect_four_gymnasium/ConnectFourEnv.py` & `gymnasium_connect_four-1.2.6/connect_four_gymnasium/ConnectFourEnv.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/AdultPlayer.py` & `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/AdultPlayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         else:
             return self.play_single(obs)
 
     def getName(self):
         return "AdultPlayer"
 
     def getElo(self):
-        return 1654
+        return 1666
     
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
```

### Comparing `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/AdultSmarterPlayer.py` & `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/AdultSmarterPlayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,11 +106,11 @@
 
         return False
 
     def getName(self):
         return "AdultSmarterPlayer"
     
     def getElo(self):
-        return 1790
+        return 1802
     
     def isDeterministic(self):
         return False
```

### Comparing `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/BabyPlayer.py` & `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/BabyPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ChildPlayer.py` & `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ChildPlayer.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 from .Player import Player
 
 class ChildPlayer(Player):
 
     def __init__(self, _=""):
         pass
 
-    def random_move(self):
-        return np.random.choice(range(7))
-
     def play(self, observation):
         if isinstance(observation, list):
             return [self.play_single(obs) for obs in observation]
         else:
             return self.play_single(observation)
 
     def play_single(self, observation):
         # Check if a winning move is available for the player
         for move in range(7):
             if observation[0, move] == 0:
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if self.check_win_around_last_move(new_board, 1, row, col):
                     return move
 
-        return self.random_move()
+        # Play a random move
+        valid_moves = [c for c in range(7) if observation[0, c] == 0]
+        return np.random.choice(valid_moves)
 
     def getName(self):
         return "ChildPlayer"
     
     def getElo(self):
-        return 1222
+        return 1272
     
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
```

### Comparing `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ChildSmarterPlayer.py` & `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ChildSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ConsolePlayer.py` & `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ConsolePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/ModelPlayer.py` & `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/ModelPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/SimulatePlayer.py` & `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/SimulatePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/TeenagerPlayer.py` & `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/TeenagerPlayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         else:
             return self.play_single(obs)
 
     def getName(self):
         return "TeenagerPlayer"
 
     def getElo(self):
-        return 1639
+        return 1655
 
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
```

### Comparing `gymnasium_connect_four-1.2.5/connect_four_gymnasium/players/TeenagerSmarterPlayer.py` & `gymnasium_connect_four-1.2.6/connect_four_gymnasium/players/TeenagerSmarterPlayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         else:
             return self.play_single(obs)
 
     def getName(self):
         return "TeenagerSmarterPlayer"
 
     def getElo(self):
-        return 1647
+        return 1658
     
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
```

### Comparing `gymnasium_connect_four-1.2.5/connect_four_gymnasium/tools/Update_bot_elo.py` & `gymnasium_connect_four-1.2.6/connect_four_gymnasium/tools/Update_bot_elo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import math
 import sys
 sys.path.append('../../')
 
 from connect_four_gymnasium.ConnectFourEnv import ConnectFourEnv
 from connect_four_gymnasium.players import (
     BabyPlayer,
+    BabySmarterPlayer,
     ChildPlayer,
     ChildSmarterPlayer,
     TeenagerPlayer,
     TeenagerSmarterPlayer,
     AdultPlayer,
     AdultSmarterPlayer,
 )
 
 
 class EloLeaderboard:
     def __init__(self):
         # Initialize the list of players
         self.players = [
             BabyPlayer(),
+            BabySmarterPlayer(),
             ChildPlayer(),
             ChildSmarterPlayer(),
             TeenagerPlayer(),
             TeenagerSmarterPlayer(),
             AdultPlayer(),
             AdultSmarterPlayer()
         ]
@@ -66,15 +68,15 @@
         # Add new players to the leaderboard
         self.players.extend(new_players)
         for player in new_players:
             self.elo_rankings[player.getName()] = player.getElo() if player.getElo() is not None else 1500
 
         # Play the specified number of matches
         for i in range(num_matches):
-            k_factor = 2 / (1 + i / 10)
+            k_factor = 0.05 / (1 + 1 / 10)
             self.play_round(k_factor, move_elo_already_known)
             if display_log:
                 print(f"Elo rankings after {i+1} matches:")
                 self.display_rankings()
                 print("\n")
 
         # Return the updated Elo ratings for the new players
```

### Comparing `gymnasium_connect_four-1.2.5/gymnasium_connect_four.egg-info/SOURCES.txt` & `gymnasium_connect_four-1.2.6/gymnasium_connect_four.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 connect_four_gymnasium/ConnectFourEnv.py
 connect_four_gymnasium/__init__.py
 connect_four_gymnasium/players/AdultPlayer.py
 connect_four_gymnasium/players/AdultSmarterPlayer.py
 connect_four_gymnasium/players/BabyPlayer.py
+connect_four_gymnasium/players/BabySmarterPlayer.py
 connect_four_gymnasium/players/ChildPlayer.py
 connect_four_gymnasium/players/ChildSmarterPlayer.py
 connect_four_gymnasium/players/ConsolePlayer.py
 connect_four_gymnasium/players/ModelPlayer.py
 connect_four_gymnasium/players/Player.py
 connect_four_gymnasium/players/SimulatePlayer.py
 connect_four_gymnasium/players/TeenagerPlayer.py
```

### Comparing `gymnasium_connect_four-1.2.5/setup.py` & `gymnasium_connect_four-1.2.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='gymnasium_connect_four',
-    version='1.2.5',
+    version='1.2.6',
     description='A connect 4 (connect four) environment for OpenAI Gym and Gymnasium',
     author='Lucas Bertola',
     url='https://github.com/lucasBertola/Connect-4-env',  
     # author_email='your.email@example.com',
     packages=find_packages(),
     install_requires=[
         'pygame==2.1.3',
```

### Comparing `gymnasium_connect_four-1.2.5/test/test_no_opponant.py` & `gymnasium_connect_four-1.2.6/test/test_no_opponant.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.5/test/test_power_4_logic.py` & `gymnasium_connect_four-1.2.6/test/test_power_4_logic.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.5/test/test_ppo_env.py` & `gymnasium_connect_four-1.2.6/test/test_ppo_env.py`

 * *Files identical despite different names*

