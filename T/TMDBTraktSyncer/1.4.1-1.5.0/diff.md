# Comparing `tmp/TMDBTraktSyncer-1.4.1.tar.gz` & `tmp/TMDBTraktSyncer-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.4.1.tar", last modified: Sat Jul  1 01:06:16 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.5.0.tar", last modified: Sun Jul 30 04:51:09 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.4.1.tar` & `TMDBTraktSyncer-1.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 01:06:16.512729 TMDBTraktSyncer-1.4.1/
--rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.4.1/LICENSE
--rw-rw-rw-   0        0        0    10839 2023-07-01 01:06:16.511728 TMDBTraktSyncer-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0    10091 2023-07-01 01:05:25.000000 TMDBTraktSyncer-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 01:06:16.480728 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0    18069 2023-06-28 04:01:34.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4548 2023-06-27 07:34:14.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0    10181 2023-06-27 07:45:31.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1669 2023-06-27 07:34:28.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0     4058 2023-06-27 07:33:19.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/tmdbData.py
--rw-rw-rw-   0        0        0     7120 2023-06-27 07:33:10.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     8014 2023-06-27 07:36:59.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-07-01 01:06:16.509728 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    10839 2023-07-01 01:06:16.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-07-01 01:06:16.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 01:06:16.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-01 01:06:16.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 01:06:16.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-01 01:06:16.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 01:06:16.512729 TMDBTraktSyncer-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-07-01 01:02:52.000000 TMDBTraktSyncer-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 04:51:09.508399 TMDBTraktSyncer-1.5.0/
+-rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0    11433 2023-07-30 04:51:09.508399 TMDBTraktSyncer-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10684 2023-07-30 04:50:28.000000 TMDBTraktSyncer-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 04:51:09.474401 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    19953 2023-07-30 04:45:49.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4548 2023-06-27 07:34:14.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0    10181 2023-06-27 07:45:31.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2023-06-27 07:34:28.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0     4231 2023-07-30 04:14:15.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/tmdbData.py
+-rw-rw-rw-   0        0        0     7319 2023-07-30 04:07:44.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     8014 2023-06-27 07:36:59.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-07-30 04:51:09.506415 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    11433 2023-07-30 04:51:09.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-07-30 04:51:09.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 04:51:09.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-30 04:51:09.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 04:51:09.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-30 04:51:09.000000 TMDBTraktSyncer-1.5.0/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 04:51:09.509400 TMDBTraktSyncer-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-07-30 04:50:17.000000 TMDBTraktSyncer-1.5.0/setup.py
```

### Comparing `TMDBTraktSyncer-1.4.1/LICENSE` & `TMDBTraktSyncer-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/PKG-INFO` & `TMDBTraktSyncer-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.4.1
+Version: 1.5.0
 Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -17,26 +17,26 @@
 # TMDB-Trakt-Syncer
 
 This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings and watchlist sync are both optional. The user will be prompted to enter their settings and api keys on first run.
 
 The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/TMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions:
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later). During installation, tick the box for adding Python to your PATH variable.
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
    - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
+   - Application summary: `Use TMDB API and Trakt API to sync user watchlists and ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run the script by running `TMDBTraktSyncer` in the command line.
 6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
-7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/TMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## Installing the Script:
 ```
 python -m pip install TMDBTraktSyncer
 ```
 _Run in your operating system's native command line._
 ## Running the Script:
@@ -58,26 +58,26 @@
 ## Installing a Specific Version:
 ```
 python -m pip install TMDBTraktSyncer==VERSION_NUMBER
 ```
 _Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) (e.g. 1.0.1) and run in your operating system's native command line._
 
 ## Alternative Manual Installation Method (without pip install):
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later). During installation, tick the box for adding Python to your PATH variable.
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
    - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
+   - Application summary: `Use TMDB API and Trakt API to sync user watchlists and ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
 6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
-7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/TMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## For Setting Up Automation See the Following Wiki Pages:
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
@@ -110,25 +110,26 @@
 
 | Project Name | Description |
 |--------------|-------------|
 | [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
 | [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
 | [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
 | [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
+| [Casvt / AudioSubChanger](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/audio_sub_changer.py) | A script with advanced options for changing audio & subtitle tracks in Plex. |
 | [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
 | [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
 | [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
 | [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
 | [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
 | [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
 | [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
 | [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
 | [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
 | [Plex Media Server](https://www.plex.tv/media-server-downloads/#plex-app) | A media server software to organize and stream your personal media collection. |
 | [Radarr](https://github.com/Radarr/Radarr) | A movie collection manager and downloader for various platforms. |
 | [Sonarr](https://github.com/Sonarr/Sonarr) | A TV show collection manager and downloader for various platforms. |
 | [Jackett](https://github.com/Jackett/Jackett) | A proxy server that provides API support for various torrent trackers commonly used with Radarr and Sonarr. |
 | [qBittorrent](https://github.com/qbittorrent/qBittorrent) | A free and open-source BitTorrent client. |
-| [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) | An open-source VPN client for Mullvad VPN service with port forwarding support. Great VPN for torrents. |
+| [AirVPN](https://airvpn.org/) | A VPN client with port forwarding support. Great VPN for torrents. |
 | [Overseerr](https://github.com/sct/overseerr) | A request management and media discovery tool for your home media server. |
 | [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | A reverse proxy solution to bypass Cloudflare protection and access websites commonly used with Jackett. |
 | [youtube-dl](https://github.com/ytdl-org/youtube-dl) | A command-line program to download videos from YouTube and other sites. |
```

### Comparing `TMDBTraktSyncer-1.4.1/README.md` & `TMDBTraktSyncer-1.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # TMDB-Trakt-Syncer
 
 This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings and watchlist sync are both optional. The user will be prompted to enter their settings and api keys on first run.
 
 The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/TMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions:
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later). During installation, tick the box for adding Python to your PATH variable.
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
    - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
+   - Application summary: `Use TMDB API and Trakt API to sync user watchlists and ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run the script by running `TMDBTraktSyncer` in the command line.
 6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
-7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/TMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## Installing the Script:
 ```
 python -m pip install TMDBTraktSyncer
 ```
 _Run in your operating system's native command line._
 ## Running the Script:
@@ -42,26 +42,26 @@
 ## Installing a Specific Version:
 ```
 python -m pip install TMDBTraktSyncer==VERSION_NUMBER
 ```
 _Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) (e.g. 1.0.1) and run in your operating system's native command line._
 
 ## Alternative Manual Installation Method (without pip install):
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later). During installation, tick the box for adding Python to your PATH variable.
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
    - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
+   - Application summary: `Use TMDB API and Trakt API to sync user watchlists and ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
 6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
-7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/TMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## For Setting Up Automation See the Following Wiki Pages:
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
@@ -94,25 +94,26 @@
 
 | Project Name | Description |
 |--------------|-------------|
 | [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
 | [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
 | [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
 | [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
+| [Casvt / AudioSubChanger](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/audio_sub_changer.py) | A script with advanced options for changing audio & subtitle tracks in Plex. |
 | [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
 | [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
 | [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
 | [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
 | [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
 | [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
 | [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
 | [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
 | [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
 | [Plex Media Server](https://www.plex.tv/media-server-downloads/#plex-app) | A media server software to organize and stream your personal media collection. |
 | [Radarr](https://github.com/Radarr/Radarr) | A movie collection manager and downloader for various platforms. |
 | [Sonarr](https://github.com/Sonarr/Sonarr) | A TV show collection manager and downloader for various platforms. |
 | [Jackett](https://github.com/Jackett/Jackett) | A proxy server that provides API support for various torrent trackers commonly used with Radarr and Sonarr. |
 | [qBittorrent](https://github.com/qbittorrent/qBittorrent) | A free and open-source BitTorrent client. |
-| [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) | An open-source VPN client for Mullvad VPN service with port forwarding support. Great VPN for torrents. |
+| [AirVPN](https://airvpn.org/) | A VPN client with port forwarding support. Great VPN for torrents. |
 | [Overseerr](https://github.com/sct/overseerr) | A request management and media discovery tool for your home media server. |
 | [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | A reverse proxy solution to bypass Cloudflare protection and access websites commonly used with Jackett. |
 | [youtube-dl](https://github.com/ytdl-org/youtube-dl) | A command-line program to download videos from YouTube and other sites. |
```

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import requests
 import time
+from datetime import datetime
 try:
     from TMDBTraktSyncer import verifyCredentials as VC
     from TMDBTraktSyncer import traktData
     from TMDBTraktSyncer import tmdbData
     from TMDBTraktSyncer import errorHandling as EH
     from TMDBTraktSyncer import errorLogger as EL
 except ImportError:
@@ -15,27 +16,59 @@
     import errorLogger as EL
 
 
 def main():
     try:
             
         trakt_watchlist, trakt_ratings, watched_content = traktData.getTraktData()
-        tmdb_watchlist, tmdb_ratings = tmdbData.getTMDBRatings()
+        tmdb_watchlist, tmdb_ratings = tmdbData.getTMDBData()
 
         #Get trakt and tmdb ratings and filter out trakt ratings with missing tmdb id
         trakt_ratings = [rating for rating in trakt_ratings if rating['TMDB_ID'] is not None]
         tmdb_ratings = [rating for rating in tmdb_ratings if rating['TMDB_ID'] is not None]
         trakt_watchlist = [item for item in trakt_watchlist if item['TMDB_ID'] is not None]
         tmdb_watchlist = [item for item in tmdb_watchlist if item['TMDB_ID'] is not None]
         #Filter out ratings already set
         tmdb_ratings_to_set = [rating for rating in trakt_ratings if rating['TMDB_ID'] not in [tmdb_rating['TMDB_ID'] for tmdb_rating in tmdb_ratings]]
         trakt_ratings_to_set = [rating for rating in tmdb_ratings if rating['TMDB_ID'] not in [trakt_rating['TMDB_ID'] for trakt_rating in trakt_ratings]]
         tmdb_watchlist_to_set = [item for item in trakt_watchlist if item['TMDB_ID'] not in [tmdb_item['TMDB_ID'] for tmdb_item in tmdb_watchlist]]
         trakt_watchlist_to_set = [item for item in tmdb_watchlist if item['TMDB_ID'] not in [trakt_item['TMDB_ID'] for trakt_item in trakt_watchlist]]
         
+        # Filter ratings to update
+        tmdb_ratings_to_update = []
+        trakt_ratings_to_update = []
+
+        # Dictionary to store TMDB_IDs and their corresponding ratings for TMDB and Trakt
+        tmdb_ratings_dict = {rating['TMDB_ID']: rating for rating in tmdb_ratings}
+        trakt_ratings_dict = {rating['TMDB_ID']: rating for rating in trakt_ratings}
+
+        # Include only items with the same TMDB_ID and different ratings and prefer the most recent rating
+        for tmdb_id, tmdb_rating in tmdb_ratings_dict.items():
+            if tmdb_id in trakt_ratings_dict:
+                trakt_rating = trakt_ratings_dict[tmdb_id]
+                # Convert ratings to float before comparing
+                tmdb_rating_value = float(tmdb_rating['Rating'])
+                trakt_rating_value = float(trakt_rating['Rating'])
+                
+                if tmdb_rating_value != trakt_rating_value:
+                    # Check if both tmdb_rating and trakt_rating have Date_Added values
+                    if tmdb_rating['Date_Added'] is not None and trakt_rating['Date_Added'] is not None:
+                        tmdb_date_added = datetime.fromisoformat(tmdb_rating['Date_Added'])
+                        trakt_date_added = datetime.fromisoformat(trakt_rating['Date_Added'])
+                    
+                        # If TMDB rating is more recent, add the Trakt rating to the update list, and vice versa
+                        if tmdb_date_added > trakt_date_added:
+                            trakt_ratings_to_update.append(tmdb_rating)
+                        else:
+                            tmdb_ratings_to_update.append(trakt_rating)
+
+        # Update ratings_to_set
+        tmdb_ratings_to_set.extend(tmdb_ratings_to_update)
+        trakt_ratings_to_set.extend(trakt_ratings_to_update)
+        
         # If remove_watched_from_watchlists_value is true
         if VC.remove_watched_from_watchlists_value:        
             # Get the IDs from watched_content
             watched_content_ids = set(item['TMDB_ID'] for item in watched_content if item['TMDB_ID'])
                     
             # Filter out watched content from trakt_watchlist_to_set
             trakt_watchlist_to_set = [item for item in trakt_watchlist_to_set if item['TMDB_ID'] not in watched_content_ids]
```

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/errorLogger.py` & `TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/tmdbData.py` & `TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/tmdbData.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     response = EH.make_tmdb_request(url)
     json_data = json.loads(response.text)
     results = json_data['results']
     total_pages = json_data['total_pages']
     current_page = json_data['page']
     return results, total_pages, current_page
 
-def getTMDBRatings():
+def getTMDBData():
     print('Processing TMDB Data')
 
     # Fetch Account ID
     response = EH.make_tmdb_request('https://api.themoviedb.org/3/account')
     json_data = json.loads(response.text)
     account_id = json_data['id']
     
@@ -56,33 +56,33 @@
 
     # Fetch Movie Ratings
     movie_ratings = []
     page = 1
     total_pages = 1
 
     while page <= total_pages:
-        url = f'https://api.themoviedb.org/3/account/{account_id}/rated/movies?page={page}'
+        url = f'https://api.themoviedb.org/4/account/{account_id}/movie/rated?page={page}'
         results, total_pages, _ = fetch_data(url)
         
         for movie in results:
-            movie_ratings.append({'Title': movie['title'], 'Year': movie['release_date'][:4], 'Rating': movie['rating'], 'TMDB_ID': movie['id'], 'Type': 'movie'})
+            movie_ratings.append({'Title': movie['title'], 'Year': movie['release_date'][:4], 'Rating': movie['account_rating']['value'], 'TMDB_ID': movie['id'], 'Date_Added': movie['account_rating']['created_at'], 'Type': 'movie'})
         
         page += 1
 
     # Fetch TV Show Ratings
     show_ratings = []
     page = 1
     total_pages = 1
 
     while page <= total_pages:
-        url = f'https://api.themoviedb.org/3/account/{account_id}/rated/tv?page={page}'
+        url = f'https://api.themoviedb.org/4/account/{account_id}/tv/rated?page={page}'
         results, total_pages, _ = fetch_data(url)
         
         for show in results:
-            show_ratings.append({'Title': show['name'], 'Year': show['first_air_date'][:4], 'Rating': show['rating'], 'TMDB_ID': show['id'], 'Type': 'show'})
+            show_ratings.append({'Title': show['name'], 'Year': show['first_air_date'][:4], 'Rating': show['account_rating']['value'], 'TMDB_ID': show['id'], 'Date_Added': movie['account_rating']['created_at'], 'Type': 'show'})
         
         page += 1
 
     # Fetch Episode Ratings
     episode_ratings = []
     page = 1
     total_pages = 1
@@ -101,14 +101,15 @@
                 'Title': episode_title,
                 'Year': episode.get('air_date', '')[:4],
                 'Rating': episode.get('rating'),
                 'TMDB_ID': episode.get('id'),
                 'Season': episode.get('season_number'),
                 'Episode': episode.get('episode_number'),
                 'ShowID': show_id,
+                'Date_Added': None,
                 'Type': 'episode'
             })
             
             page += 1
 
     tmdb_ratings = movie_ratings + show_ratings + episode_ratings
```

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/traktData.py` & `TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/traktData.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,38 +25,38 @@
     trakt_watchlist = []
 
     for item in json_data:
         if item['type'] == 'movie':
             movie = item.get('movie')
             tmdb_movie_id = movie.get('ids', {}).get('tmdb')
             trakt_movie_id = movie.get('ids', {}).get('trakt')
-            trakt_watchlist.append({'Title': movie.get('title'), 'Year': movie.get('year'), "TMDB_ID": tmdb_movie_id, 'TraktID': trakt_movie_id, 'Type': 'movie'})
+            trakt_watchlist.append({'Title': movie.get('title'), 'Year': movie.get('year'), "TMDB_ID": tmdb_movie_id, 'TraktID': trakt_movie_id, 'Date_Added': item.get('listed_at'), 'Type': 'movie'})
         elif item['type'] == 'show':
             show = item.get('show')
             tmdb_show_id = show.get('ids', {}).get('tmdb')
             trakt_show_id = show.get('ids', {}).get('trakt')
-            trakt_watchlist.append({'Title': show.get('title'), 'Year': show.get('year'), "TMDB_ID": tmdb_show_id, 'TraktID': trakt_show_id, 'Type': 'show'})
+            trakt_watchlist.append({'Title': show.get('title'), 'Year': show.get('year'), "TMDB_ID": tmdb_show_id, 'TraktID': trakt_show_id, 'Date_Added': item.get('listed_at'), 'Type': 'show'})
 
     # Get Trakt Ratings
     response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/ratings')
     json_data = json.loads(response.text)
 
     movie_ratings = []
     show_ratings = []
     episode_ratings = []
 
     for item in json_data:
         if item['type'] == 'movie':
             movie = item.get('movie')
             movie_id = movie.get('ids', {}).get('tmdb')
-            movie_ratings.append({'Title': movie.get('title'), 'Year': movie.get('year'), 'Rating': item.get('rating'), "TMDB_ID": movie_id, 'Type': 'movie'})
+            movie_ratings.append({'Title': movie.get('title'), 'Year': movie.get('year'), 'Rating': item.get('rating'), "TMDB_ID": movie_id, 'Date_Added': item.get('rated_at'), 'Type': 'movie'})
         elif item['type'] == 'show':
             show = item.get('show')
             show_id = show.get('ids', {}).get('tmdb')
-            show_ratings.append({'Title': show.get('title'), 'Year': show.get('year'), 'Rating': item.get('rating'), "TMDB_ID": show_id, 'Type': 'show'})
+            show_ratings.append({'Title': show.get('title'), 'Year': show.get('year'), 'Rating': item.get('rating'), "TMDB_ID": show_id, 'Date_Added': item.get('rated_at'), 'Type': 'show'})
         elif item['type'] == 'episode':
             show = item.get('show')
             show_title = show.get('title')
             show_tmdb_id = show.get('ids', {}).get('tmdb') if show and 'ids' in show else None
             episode = item.get('episode')
             episode_id = episode.get('ids', {}).get('tmdb')
             episode_title = f'{show_title}: {episode.get("title")}'
@@ -64,14 +64,15 @@
                 'Title': episode_title,
                 'Year': episode.get('year'),
                 'Rating': item.get('rating'),
                 "TMDB_ID": episode_id,
                 'Season': episode.get('season'),
                 'Episode': episode.get('number'),
                 'TMDB_ShowID': show_tmdb_id,
+                'Date_Added': item.get('rated_at'),
                 'Type': 'episode'
             })
 
     trakt_ratings = movie_ratings + show_ratings + episode_ratings
     
     # Get Trakt Watch History
     response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/history?limit=100')
```

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.5.0/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.5.0/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.4.1
+Version: 1.5.0
 Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -17,26 +17,26 @@
 # TMDB-Trakt-Syncer
 
 This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings and watchlist sync are both optional. The user will be prompted to enter their settings and api keys on first run.
 
 The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/TMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions:
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later). During installation, tick the box for adding Python to your PATH variable.
 2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
    - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
+   - Application summary: `Use TMDB API and Trakt API to sync user watchlists and ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run the script by running `TMDBTraktSyncer` in the command line.
 6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
-7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/TMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## Installing the Script:
 ```
 python -m pip install TMDBTraktSyncer
 ```
 _Run in your operating system's native command line._
 ## Running the Script:
@@ -58,26 +58,26 @@
 ## Installing a Specific Version:
 ```
 python -m pip install TMDBTraktSyncer==VERSION_NUMBER
 ```
 _Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) (e.g. 1.0.1) and run in your operating system's native command line._
 
 ## Alternative Manual Installation Method (without pip install):
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later). During installation, tick the box for adding Python to your PATH variable.
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
    - Type of use: `Personal`
    - Application name: `TMDB-Trakt-Sync`
    - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
+   - Application summary: `Use TMDB API and Trakt API to sync user watchlists and ratings between platforms.`
    - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
 5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
 6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
-7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/TMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## For Setting Up Automation See the Following Wiki Pages:
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
@@ -110,25 +110,26 @@
 
 | Project Name | Description |
 |--------------|-------------|
 | [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
 | [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
 | [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
 | [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
+| [Casvt / AudioSubChanger](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/audio_sub_changer.py) | A script with advanced options for changing audio & subtitle tracks in Plex. |
 | [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
 | [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
 | [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
 | [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
 | [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
 | [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
 | [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
 | [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
 | [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
 | [Plex Media Server](https://www.plex.tv/media-server-downloads/#plex-app) | A media server software to organize and stream your personal media collection. |
 | [Radarr](https://github.com/Radarr/Radarr) | A movie collection manager and downloader for various platforms. |
 | [Sonarr](https://github.com/Sonarr/Sonarr) | A TV show collection manager and downloader for various platforms. |
 | [Jackett](https://github.com/Jackett/Jackett) | A proxy server that provides API support for various torrent trackers commonly used with Radarr and Sonarr. |
 | [qBittorrent](https://github.com/qbittorrent/qBittorrent) | A free and open-source BitTorrent client. |
-| [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) | An open-source VPN client for Mullvad VPN service with port forwarding support. Great VPN for torrents. |
+| [AirVPN](https://airvpn.org/) | A VPN client with port forwarding support. Great VPN for torrents. |
 | [Overseerr](https://github.com/sct/overseerr) | A request management and media discovery tool for your home media server. |
 | [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | A reverse proxy solution to bypass Cloudflare protection and access websites commonly used with Jackett. |
 | [youtube-dl](https://github.com/ytdl-org/youtube-dl) | A command-line program to download videos from YouTube and other sites. |
```

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/SOURCES.txt` & `TMDBTraktSyncer-1.5.0/TMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/setup.py` & `TMDBTraktSyncer-1.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.4.1'
+VERSION = '1.5.0'
 DESCRIPTION = 'A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

