# Comparing `tmp/TMDBTraktSyncer-1.4.1.tar.gz` & `tmp/TMDBTraktSyncer-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.4.1.tar", last modified: Sat Jul  1 01:06:16 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.5.1.tar", last modified: Sun Jul 30 07:04:21 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.4.1.tar` & `TMDBTraktSyncer-1.5.1.tar`

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
+drwxrwxrwx   0        0        0        0 2023-07-30 07:04:21.456208 TMDBTraktSyncer-1.5.1/
+-rw-rw-rw-   0        0        0     1079 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0    11433 2023-07-30 07:04:21.455197 TMDBTraktSyncer-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10684 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 07:04:21.420200 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    18069 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4548 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0    10181 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0     4058 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/tmdbData.py
+-rw-rw-rw-   0        0        0     7120 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     8014 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:04:21.453207 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    11433 2023-07-30 07:04:21.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-07-30 07:04:21.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 07:04:21.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-30 07:04:21.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 07:04:21.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-30 07:04:21.000000 TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 07:04:21.457198 TMDBTraktSyncer-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1343 2023-07-30 05:03:26.000000 TMDBTraktSyncer-1.5.1/setup.py
```

### Comparing `TMDBTraktSyncer-1.4.1/LICENSE` & `TMDBTraktSyncer-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/PKG-INFO` & `TMDBTraktSyncer-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.4.1
+Version: 1.5.1
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

### Comparing `TMDBTraktSyncer-1.4.1/README.md` & `TMDBTraktSyncer-1.5.1/README.md`

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

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/errorLogger.py` & `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/tmdbData.py` & `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/tmdbData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/traktData.py` & `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.4.1
+Version: 1.5.1
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

### Comparing `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/SOURCES.txt` & `TMDBTraktSyncer-1.5.1/TMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.1/setup.py` & `TMDBTraktSyncer-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.4.1'
+VERSION = '1.5.1'
 DESCRIPTION = 'A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
@@ -33,8 +33,8 @@
     ],
     entry_points={
         'console_scripts': [
             'TMDBTraktSyncer = TMDBTraktSyncer.TMDBTraktSyncer:main'
         ]
     },
     python_requires='>=3.6'
-)
+)
```

