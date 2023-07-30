# Comparing `tmp/gymnasium_connect_four-1.2.2.tar.gz` & `tmp/gymnasium_connect_four-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_connect_four-1.2.2.tar", last modified: Sat Jul 29 17:32:22 2023, max compression
+gzip compressed data, was "gymnasium_connect_four-1.2.3.tar", last modified: Sun Jul 30 07:25:07 2023, max compression
```

## Comparing `gymnasium_connect_four-1.2.2.tar` & `gymnasium_connect_four-1.2.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 17:32:22.682506 gymnasium_connect_four-1.2.2/
--rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.2/LICENSE
--rw-rw-rw-   0        0        0      251 2023-07-29 17:32:22.682506 gymnasium_connect_four-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    10858 2023-07-29 17:13:55.000000 gymnasium_connect_four-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 17:32:22.670500 gymnasium_connect_four-1.2.2/connect_four_gymnasium/
--rw-rw-rw-   0        0        0     8813 2023-07-29 17:26:26.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/ConnectFourEnv.py
--rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:32:22.670500 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/
--rw-rw-rw-   0        0        0     4654 2023-07-29 17:00:12.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/AdultPlayer.py
--rw-rw-rw-   0        0        0     4378 2023-07-29 17:00:36.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/AdultSmarterPlayer.py
--rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/BabyPlayer.py
--rw-rw-rw-   0        0        0     1881 2023-07-29 14:17:29.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ChildPlayer.py
--rw-rw-rw-   0        0        0     2248 2023-07-29 17:00:55.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ChildSmarterPlayer.py
--rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ConsolePlayer.py
--rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ModelPlayer.py
--rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/Player.py
--rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/SimulatePlayer.py
--rw-rw-rw-   0        0        0     3163 2023-07-29 17:01:08.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/TeenagerPlayer.py
--rw-rw-rw-   0        0        0     4378 2023-07-29 17:01:22.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
--rw-rw-rw-   0        0        0      446 2023-07-29 10:59:21.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:32:22.682506 gymnasium_connect_four-1.2.2/connect_four_gymnasium/tools/
--rw-rw-rw-   0        0        0     3238 2023-07-29 14:40:52.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/tools/EloLeaderboard.py
--rw-rw-rw-   0        0        0     4744 2023-07-29 14:17:37.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/tools/Update_bot_elo.py
--rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:32:22.682506 gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/
--rw-rw-rw-   0        0        0      251 2023-07-29 17:32:22.000000 gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2023-07-29 17:32:22.000000 gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 17:32:22.000000 gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-29 17:32:22.000000 gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-29 17:32:22.000000 gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 17:32:22.682506 gymnasium_connect_four-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-07-29 17:32:08.000000 gymnasium_connect_four-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:32:22.682506 gymnasium_connect_four-1.2.2/test/
--rw-rw-rw-   0        0        0     4722 2023-07-29 17:17:01.000000 gymnasium_connect_four-1.2.2/test/test_no_opponant.py
--rw-rw-rw-   0        0        0    21564 2023-07-29 17:15:09.000000 gymnasium_connect_four-1.2.2/test/test_power_4_logic.py
--rw-rw-rw-   0        0        0     2372 2023-07-29 17:18:55.000000 gymnasium_connect_four-1.2.2/test/test_ppo_env.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:25:07.096603 gymnasium_connect_four-1.2.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-07-30 07:25:07.096603 gymnasium_connect_four-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11334 2023-07-30 07:23:29.000000 gymnasium_connect_four-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 07:25:07.071531 gymnasium_connect_four-1.2.3/connect_four_gymnasium/
+-rw-rw-rw-   0        0        0     9195 2023-07-30 07:21:16.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/ConnectFourEnv.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:25:07.084059 gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/
+-rw-rw-rw-   0        0        0     4654 2023-07-29 17:00:12.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/AdultPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-07-29 17:00:36.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/AdultSmarterPlayer.py
+-rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/BabyPlayer.py
+-rw-rw-rw-   0        0        0     1881 2023-07-29 14:17:29.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/ChildPlayer.py
+-rw-rw-rw-   0        0        0     2248 2023-07-29 17:00:55.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/ChildSmarterPlayer.py
+-rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/ConsolePlayer.py
+-rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/ModelPlayer.py
+-rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/Player.py
+-rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/SimulatePlayer.py
+-rw-rw-rw-   0        0        0     3163 2023-07-29 17:01:08.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/TeenagerPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-07-29 17:01:22.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
+-rw-rw-rw-   0        0        0      446 2023-07-29 10:59:21.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:25:07.087607 gymnasium_connect_four-1.2.3/connect_four_gymnasium/tools/
+-rw-rw-rw-   0        0        0     3238 2023-07-29 14:40:52.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/tools/EloLeaderboard.py
+-rw-rw-rw-   0        0        0     4744 2023-07-29 14:17:37.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/tools/Update_bot_elo.py
+-rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.3/connect_four_gymnasium/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:25:07.092595 gymnasium_connect_four-1.2.3/gymnasium_connect_four.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-07-30 07:25:06.000000 gymnasium_connect_four-1.2.3/gymnasium_connect_four.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2023-07-30 07:25:07.000000 gymnasium_connect_four-1.2.3/gymnasium_connect_four.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 07:25:06.000000 gymnasium_connect_four-1.2.3/gymnasium_connect_four.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-30 07:25:06.000000 gymnasium_connect_four-1.2.3/gymnasium_connect_four.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-30 07:25:06.000000 gymnasium_connect_four-1.2.3/gymnasium_connect_four.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 07:25:07.096603 gymnasium_connect_four-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-07-30 07:24:59.000000 gymnasium_connect_four-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:25:07.095595 gymnasium_connect_four-1.2.3/test/
+-rw-rw-rw-   0        0        0     4722 2023-07-29 17:17:01.000000 gymnasium_connect_four-1.2.3/test/test_no_opponant.py
+-rw-rw-rw-   0        0        0    21564 2023-07-29 17:15:09.000000 gymnasium_connect_four-1.2.3/test/test_power_4_logic.py
+-rw-rw-rw-   0        0        0     2372 2023-07-29 17:18:55.000000 gymnasium_connect_four-1.2.3/test/test_ppo_env.py
```

### Comparing `gymnasium_connect_four-1.2.2/LICENSE` & `gymnasium_connect_four-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/README.md` & `gymnasium_connect_four-1.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 ```
 
 ### Observation Space
 
 The observation space in the Connect Four environment is a 2D array representing the game board. Each cell in the array can have one of three possible values: 0 (empty), 1 (player's piece), or -1 (opponent's piece). The observation space is defined as follows:
 
 ```python
-self.observation_space = spaces.Box(low=0, high=2, shape=(self.ROWS_COUNT, self.COLUMNS_COUNT), dtype=np.int32)
+self.observation_space = spaces.Box(low=-1, high=1, shape=(self.ROWS_COUNT, self.COLUMNS_COUNT), dtype=np.int32)
 ```
 
 ### Rewards
 
 The reward system in the Connect Four environment is designed to encourage the AI model to learn how to win the game. The rewards are as follows:
 
 - A reward of +1 is given when the AI model wins the game by connecting four of its pieces in a row, either horizontally, vertically, or diagonally.
@@ -139,19 +139,19 @@
 ### Elo Ratings
 
 Here are the Elo ratings of the different algorithms:
 
 ```
 1.  AdultSmarterPlayer:    1790
 2.  AdultPlayer:           1654
-5.  TeenagerSmarterPlayer: 1647
-6.  TeenagerPlayer:        1639
-7.  ChildSmarterPlayer:    1571
-9.  ChildPlayer:           1222
-10. BabyPlayer:            1000
+3.  TeenagerSmarterPlayer: 1647
+4.  TeenagerPlayer:        1639
+5.  ChildSmarterPlayer:    1571
+6.  ChildPlayer:           1222
+7.  BabyPlayer:            1000
 ```
 
 In addition to the provided players, we also offer a tool to evaluate the Elo rating of your own AI model. This is extremely useful to have an "absolute" idea of the progress of your AI. For example, if an AI learns by fighting against itself, we know that it is getting stronger as it would be able to win against its older versions, but this is not enough to evaluate if it has learned a lot. This is where our tool comes in, which allows you to give an Elo rating to the AI.
 
 Here is how to use it in Python:
 
 ```python
@@ -162,14 +162,18 @@
 myModelPlayer = ModelPlayer(model,name="Your trained Model")
 
 your_model_elo = EloLeaderboard().get_elo([myModelPlayer], num_matches=100)
 ```
 
 You can find an example of how to use this tool in a Google Colab notebook [here](https://colab.research.google.com/github/lucasBertola/Connect-4-Gym-env-Reinforcement-learning/blob/main/exemples/Train_ppo_and_test.ipynb).
 
+## Detailed Documentation
+
+For a comprehensive overview of the methods and classes used in this environment, please refer to the [detailed documentation](https://github.com/lucasBertola/Connect-4-Gym-env-Reinforcement-learning/blob/main/DOCUMENTATION.md) available on the GitHub repository. This documentation provides in-depth explanations and examples to help you better understand the inner workings of the Connect Four environment and make the most of its features.
+
 ## Testing
 
 We believe in the importance of testing. That's why we have included a suite of tests in the `test` directory. To run the tests, simply use the command `pytest`.
 
 ## Contribute & Support
 
 We warmly welcome contributions from the community. If you have an idea for an improvement or found a bug, don't hesitate to open an issue or submit a pull request. Your input is greatly appreciated, and our project is made better by your participation!
```

#### html2text {}

```diff
@@ -68,15 +68,15 @@
 total of 7 possible actions. Each action corresponds to a column in the game
 board where a player can drop their piece. The action space is represented as
 follows: ```python self.action_space = spaces.Discrete(self.COLUMNS_COUNT) ```
 ### Observation Space The observation space in the Connect Four environment is
 a 2D array representing the game board. Each cell in the array can have one of
 three possible values: 0 (empty), 1 (player's piece), or -1 (opponent's piece).
 The observation space is defined as follows: ```python self.observation_space =
-spaces.Box(low=0, high=2, shape=(self.ROWS_COUNT, self.COLUMNS_COUNT),
+spaces.Box(low=-1, high=1, shape=(self.ROWS_COUNT, self.COLUMNS_COUNT),
 dtype=np.int32) ``` ### Rewards The reward system in the Connect Four
 environment is designed to encourage the AI model to learn how to win the game.
 The rewards are as follows: - A reward of +1 is given when the AI model wins
 the game by connecting four of its pieces in a row, either horizontally,
 vertically, or diagonally. - A reward of -1 is given when the AI model loses
 the game or plays an invalid action. - A reward of 0 is given for all other
 actions that do not result in a win or loss. ### Episode Termination An episode
@@ -106,31 +106,38 @@
 a move creates a line of three tokens with available spaces on both sides for
 the opponent. If so, it will play that move to block the opponent. -
 **AdultSmarterPlayer**: Same as AdultPlayer, but checks if a move allows to
 create multiple ways to win and plays that move. Also checks if a move allows
 the opponent to create multiple ways to win and plays that move to protect
 itself. - **ConsolePlayer**: Asks for moves to play in the console. Perfect for
 testing your own AI. ### Elo Ratings Here are the Elo ratings of the different
-algorithms: ``` 1. AdultSmarterPlayer: 1790 2. AdultPlayer: 1654 5.
-TeenagerSmarterPlayer: 1647 6. TeenagerPlayer: 1639 7. ChildSmarterPlayer: 1571
-9. ChildPlayer: 1222 10. BabyPlayer: 1000 ``` In addition to the provided
+algorithms: ``` 1. AdultSmarterPlayer: 1790 2. AdultPlayer: 1654 3.
+TeenagerSmarterPlayer: 1647 4. TeenagerPlayer: 1639 5. ChildSmarterPlayer: 1571
+6. ChildPlayer: 1222 7. BabyPlayer: 1000 ``` In addition to the provided
 players, we also offer a tool to evaluate the Elo rating of your own AI model.
 This is extremely useful to have an "absolute" idea of the progress of your AI.
 For example, if an AI learns by fighting against itself, we know that it is
 getting stronger as it would be able to win against its older versions, but
 this is not enough to evaluate if it has learned a lot. This is where our tool
 comes in, which allows you to give an Elo rating to the AI. Here is how to use
 it in Python: ```python env = ConnectFourEnv(opponent=BabyPlayer()) model = PPO
 ("MlpPolicy", env) model.learn(total_timesteps=10000) myModelPlayer =
 ModelPlayer(model,name="Your trained Model") your_model_elo = EloLeaderboard
 ().get_elo([myModelPlayer], num_matches=100) ``` You can find an example of how
 to use this tool in a Google Colab notebook [here](https://
 colab.research.google.com/github/lucasBertola/Connect-4-Gym-env-Reinforcement-
-learning/blob/main/exemples/Train_ppo_and_test.ipynb). ## Testing We believe in
-the importance of testing. That's why we have included a suite of tests in the
-`test` directory. To run the tests, simply use the command `pytest`. ##
-Contribute & Support We warmly welcome contributions from the community. If you
-have an idea for an improvement or found a bug, don't hesitate to open an issue
-or submit a pull request. Your input is greatly appreciated, and our project is
-made better by your participation! If you find this repository useful, please
-give it a star! ## License This project is licensed under the MIT License. See
-the `LICENSE` file for details.
+learning/blob/main/exemples/Train_ppo_and_test.ipynb). ## Detailed
+Documentation For a comprehensive overview of the methods and classes used in
+this environment, please refer to the [detailed documentation](https://
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

### Comparing `gymnasium_connect_four-1.2.2/connect_four_gymnasium/ConnectFourEnv.py` & `gymnasium_connect_four-1.2.3/connect_four_gymnasium/ConnectFourEnv.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     player_1_color = (224, 209, 18)
     player_2_color = (197, 7, 17)
     MIN_INDEX_TO_PLAY = 0
     INVALID_player = 0
     INVALID_opponent = 0
 
     def change_opponent(self, opponent):
-        self.opponent = opponent
+        self._opponent = opponent
 
     def __init__(self, opponent=None, render_mode=None, first_player=None):
-        self.opponent = opponent  # Define the opponent
+        self._opponent = opponent  # Define the opponent
         # Define the action and observation spaces
         self.action_space = spaces.Discrete(self.COLUMNS_COUNT)
 
         # 1 is you, -1 is the opponent
         self.observation_space = spaces.Box(low=-1, high=1, shape=(self.ROWS_COUNT, self.COLUMNS_COUNT), dtype=np.int32)
 
         # Check if the render mode is valid
@@ -34,99 +34,114 @@
         self.render_mode = render_mode
         self.last_render_time = None
         self.window = None
         self.first_player = first_player
 
     def reset(self, seed=None, options=None):
         super().reset(seed=seed)
-        self._board = np.zeros((self.ROWS_COUNT, self.COLUMNS_COUNT))
-        self.render_for_human()
+        self.board = np.zeros((self.ROWS_COUNT, self.COLUMNS_COUNT))
+        self._render_for_human()
 
         if self.first_player is None:
             self.next_player_to_play = np.random.choice([1, -1])
         else:
             self.next_player_to_play = self.first_player
 
-        if self.opponent is not None:
+        if self._opponent is not None:
             if self.next_player_to_play == -1:
-                opponent_action = self.opponent.play(self._board)
-                result, isFinish = self.play_action(opponent_action, self.next_player_to_play)
+                opponent_action = self._opponent.play(self.board)
+                result, isFinish = self._play_action(opponent_action, self.next_player_to_play)
                 if isFinish :
                     print('wtf')
                     print(opponent_action)
                     exit("The opponent played an invalid action in the first move!")
                 self.next_player_to_play = 1
 
-            self.render_for_human()
+            self._render_for_human()
 
-        return self._board, {}
+        return self.board, {}
 
-    def render_for_human(self):
+    def _render_for_human(self):
         if self.render_mode == "human":
             self._render_frame()
 
     def is_column_full(self, column):
-        return self._board[0, column] != 0
+        return self.board[0, column] != 0
 
     def is_action_valid(self, action):
         return action >= self.MIN_INDEX_TO_PLAY and action < self.COLUMNS_COUNT and not self.is_column_full(action)
 
-    def play_action(self, action, player):
+    def _play_action(self, action, player):
         if not self.is_action_valid(action):
             return -1, True
 
-        last_move_row = self.drop_piece(action, player)
+        last_move_row = self._drop_piece(action, player)
 
-        self.render_for_human()
+        self._render_for_human()
 
         if self.check_win_around_last_move(player, last_move_row, action):
             if self.render_mode == "human":
                 print("You won!")
                 time.sleep(5)
             return 1, True
         
         if self.board_is_full():
             return 0, True
 
         return 0, False
 
     def board_is_full(self):
-        return np.all(self._board != 0)
+        return np.all(self.board != 0)
     
     def inverse_player_position(self):
-        return -self._board
+        self.board = -self.board
 
     def switch_player(self):
         self.next_player_to_play = -1*self.next_player_to_play
-        
+        #because 1 is you and -1 is the opponent
+        self.inverse_player_position()
+    
+    def get_valid_actions(self):
+        valid_actions = []
+        for col in range(self.COLUMNS_COUNT):
+            if not self.is_column_full(col):
+                valid_actions.append(col)
+        return valid_actions
+    
+    def clone(self):
+        new_env = ConnectFourEnv(opponent=self._opponent, render_mode=self.render_mode, first_player=self.first_player)
+        new_env.next_player_to_play = self.next_player_to_play
+        return new_env
+
+    def clone_and_play(self, action):
+        newself = self.clone()
+        newBoard, result, IsFinish, isTruncated = newself.step(action)
+        return newBoard, result, IsFinish, isTruncated, newself
+
     def step(self, action, play_opponent=True):
         action = action.item() if isinstance(action, np.ndarray) else action
 
-        result, is_finish = self.play_action(action, self.next_player_to_play)
+        result, is_finish = self._play_action(action, 1)
+
         if is_finish:
-            return self._board, result, True, False, {}
-        
+            return self.board, result, True, False, {}
+
         self.switch_player()
 
-        if  play_opponent and self.opponent is not None:
-            # because 1 is you, -1 is the opponent
-            # you need to see the board as the opponent sees it
-            opponent_action = self.opponent.play(self.inverse_player_position())
+        if  play_opponent and self._opponent is not None:
+            opponent_action = self._opponent.play(self.board)
             opponent_result = self.step(opponent_action, play_opponent=False)
-            return opponent_result[0],-1* opponent_result[1], opponent_result[2], opponent_result[3], opponent_result[4]
-        elif self.opponent is None:
-            boardToReturn = self._board if self.next_player_to_play == 1 else self.inverse_player_position()
-            return boardToReturn, 0, False, False, {}
+            return self.board,-1* opponent_result[1], opponent_result[2], opponent_result[3], opponent_result[4]
             
-        return self._board, 0, False, False, {}
+        return self.board, 0, False, False, {}
 
-    def drop_piece(self, action, player):
+    def _drop_piece(self, action, player):
         for i in range(self.ROWS_COUNT - 1, -1, -1):
-            if self._board[i, action] == 0:
-                self._board[i, action] = player
+            if self.board[i, action] == 0:
+                self.board[i, action] = player
                 return i
         print('wtf', self.is_action_valid(action))
         exit("Someone played an invalid action!")
 
     def check_win_around_last_move(self, player, row, col):
         directions = [
             (1, 0),  # horizontal
@@ -135,28 +150,28 @@
             (1, -1)  # diagonal \
         ]
 
         for dr, dc in directions:
             count = 0
             for step in range(-3, 4):
                 r, c = row + step * dr, col + step * dc
-                if 0 <= r < self.ROWS_COUNT and 0 <= c < self.COLUMNS_COUNT and self._board[r, c] == player:
+                if 0 <= r < self.ROWS_COUNT and 0 <= c < self.COLUMNS_COUNT and self.board[r, c] == player:
                     count += 1
                     if count == 4:
                         return True
                 else:
                     count = 0
 
         return False
     
     def render(self):
         if self.render_mode == "rgb_array":
             return self._render_frame()
 
-    def wait_for_render(self):
+    def _wait_for_render(self):
         current_time = time.time()
         time_to_wait = 1 / self.FPS
         if self.last_render_time is not None and current_time - self.last_render_time < time_to_wait:
             time.sleep(1 - (current_time - self.last_render_time))
         self.last_render_time = time.time()
 
     def _render_frame(self):
@@ -168,15 +183,15 @@
         windows_width = (padding * 2) + (circle_radius * 2 * self.COLUMNS_COUNT) + padding_center * (self.COLUMNS_COUNT - 1)
         end_height_board = (padding * 2) + (circle_radius * 2 * self.ROWS_COUNT) + padding_center * (self.ROWS_COUNT - 1)
         windows_height = end_height_board + text_players_size
         
         pygame.font.init()
         # if render GUI, we want to limit the frame rate to X FPS for better visualization
         if self.render_mode == "human":
-            self.wait_for_render()
+            self._wait_for_render()
 
         if self.window is None and self.render_mode == "human":
             pygame.init()
             pygame.display.init()
             self.window = pygame.display.set_mode((windows_width, windows_height))
 
         canvas = pygame.Surface((windows_width, windows_height))
@@ -187,28 +202,28 @@
         circle_radius = 32
 
         i_position = padding
         for i in range(self.ROWS_COUNT):
             j_position = padding
             for j in range(self.COLUMNS_COUNT):
                 color = (245, 245, 245)
-                if self._board[i, j] == 1:
+                if self.board[i, j] == 1:
                     color = self.player_1_color
-                elif self._board[i, j] == -1:
+                elif self.board[i, j] == -1:
                     color = self.player_2_color
                 pygame.draw.circle(canvas, color, (j_position + circle_radius, i_position + circle_radius), circle_radius)
                 j_position += (circle_radius * 2) + padding_center
             i_position += (circle_radius * 2) + padding_center
 
         # Display opponent's color and name
         text_position_y_first_player = end_height_board
         pygame.draw.circle(canvas, self.player_2_color, (50, text_position_y_first_player + circle_radius / 4),
                            circle_radius / 2)
         font = pygame.font.Font(None, 36)
-        opponent_name = self.opponent.getName()
+        opponent_name = self._opponent.getName()
         text = font.render(f"{opponent_name}", 1, (10, 10, 10))
 
         canvas.blit(text, (80, text_position_y_first_player))
 
         # Display user's color
         text_position_y_second_player = text_position_y_first_player + 40
         pygame.draw.circle(canvas, self.player_1_color, (50, text_position_y_second_player + circle_radius / 4),
@@ -219,11 +234,11 @@
         if self.render_mode == "human":
             self.window.blit(canvas, canvas.get_rect())
             pygame.event.pump()
             pygame.display.update()
         else:
             return np.transpose(pygame.surfarray.array3d(canvas), (1, 0, 2))
         
-        def close(self):
-            if self.window is not None:
-                pygame.display.quit()
-                pygame.quit()
+    def close(self):
+        if self.window is not None:
+            pygame.display.quit()
+            pygame.quit()
```

### Comparing `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/AdultPlayer.py` & `gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/AdultPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/AdultSmarterPlayer.py` & `gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/AdultSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/BabyPlayer.py` & `gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/BabyPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ChildPlayer.py` & `gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/ChildPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ChildSmarterPlayer.py` & `gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/ChildSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ConsolePlayer.py` & `gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/ConsolePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ModelPlayer.py` & `gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/ModelPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/SimulatePlayer.py` & `gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/SimulatePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/TeenagerPlayer.py` & `gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/TeenagerPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/TeenagerSmarterPlayer.py` & `gymnasium_connect_four-1.2.3/connect_four_gymnasium/players/TeenagerSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/connect_four_gymnasium/tools/EloLeaderboard.py` & `gymnasium_connect_four-1.2.3/connect_four_gymnasium/tools/EloLeaderboard.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/connect_four_gymnasium/tools/Update_bot_elo.py` & `gymnasium_connect_four-1.2.3/connect_four_gymnasium/tools/Update_bot_elo.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/SOURCES.txt` & `gymnasium_connect_four-1.2.3/gymnasium_connect_four.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/setup.py` & `gymnasium_connect_four-1.2.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='gymnasium_connect_four',
-    version='1.2.2',
+    version='1.2.3',
     description='A connect 4 (connect four) environment for OpenAI Gym and Gymnasium',
     author='Lucas Bertola',
     url='https://github.com/lucasBertola/Connect-4-env',  
     # author_email='your.email@example.com',
     packages=find_packages(),
     install_requires=[
         'pygame==2.1.3',
```

### Comparing `gymnasium_connect_four-1.2.2/test/test_no_opponant.py` & `gymnasium_connect_four-1.2.3/test/test_no_opponant.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/test/test_power_4_logic.py` & `gymnasium_connect_four-1.2.3/test/test_power_4_logic.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.2/test/test_ppo_env.py` & `gymnasium_connect_four-1.2.3/test/test_ppo_env.py`

 * *Files identical despite different names*

