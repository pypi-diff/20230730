# Comparing `tmp/describealign-0.1.2.tar.gz` & `tmp/describealign-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "describealign-0.1.2.tar", last modified: Fri Jul 28 02:57:41 2023, max compression
+gzip compressed data, was "describealign-0.1.3.tar", last modified: Sun Jul 30 07:55:37 2023, max compression
```

## Comparing `describealign-0.1.2.tar` & `describealign-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 02:57:41.915980 describealign-0.1.2/
--rw-rw-rw-   0        0        0    35149 2023-07-26 20:20:51.000000 describealign-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      807 2023-07-28 02:57:41.914980 describealign-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-07-26 19:29:21.000000 describealign-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 02:57:41.913980 describealign-0.1.2/describealign.egg-info/
--rw-rw-rw-   0        0        0      807 2023-07-28 02:57:41.000000 describealign-0.1.2/describealign.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-28 02:57:41.000000 describealign-0.1.2/describealign.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 02:57:41.000000 describealign-0.1.2/describealign.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-07-28 02:57:41.000000 describealign-0.1.2/describealign.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      117 2023-07-28 02:57:41.000000 describealign-0.1.2/describealign.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-28 02:57:41.000000 describealign-0.1.2/describealign.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    40156 2023-07-27 07:05:59.000000 describealign-0.1.2/describealign.py
--rw-rw-rw-   0        0        0      950 2023-07-28 02:55:44.000000 describealign-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 02:57:41.915980 describealign-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 07:55:37.572422 describealign-0.1.3/
+-rw-rw-rw-   0        0        0    35149 2023-07-26 20:20:51.000000 describealign-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      807 2023-07-30 07:55:37.571422 describealign-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-26 19:29:21.000000 describealign-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 07:55:37.571422 describealign-0.1.3/describealign.egg-info/
+-rw-rw-rw-   0        0        0      807 2023-07-30 07:55:37.000000 describealign-0.1.3/describealign.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-30 07:55:37.000000 describealign-0.1.3/describealign.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 07:55:37.000000 describealign-0.1.3/describealign.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-30 07:55:37.000000 describealign-0.1.3/describealign.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      117 2023-07-30 07:55:37.000000 describealign-0.1.3/describealign.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-30 07:55:37.000000 describealign-0.1.3/describealign.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    41720 2023-07-30 07:08:16.000000 describealign-0.1.3/describealign.py
+-rw-rw-rw-   0        0        0      950 2023-07-30 07:16:49.000000 describealign-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-30 07:55:37.572422 describealign-0.1.3/setup.cfg
```

### Comparing `describealign-0.1.2/LICENSE` & `describealign-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `describealign-0.1.2/PKG-INFO` & `describealign-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: describealign
-Version: 0.1.2
+Version: 0.1.3
 Summary: Combines videos with matching audio files (e.g. audio descriptions)
 Author-email: Julian Brown <julbean@proton.me>
 Project-URL: Homepage, https://github.com/julbean/describealign
 Project-URL: Bug Tracker, https://github.com/julbean/describealign/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `describealign-0.1.2/describealign.egg-info/PKG-INFO` & `describealign-0.1.3/describealign.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: describealign
-Version: 0.1.2
+Version: 0.1.3
 Summary: Combines videos with matching audio files (e.g. audio descriptions)
 Author-email: Julian Brown <julbean@proton.me>
 Project-URL: Homepage, https://github.com/julbean/describealign
 Project-URL: Bug Tracker, https://github.com/julbean/describealign/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `describealign-0.1.2/describealign.py` & `describealign-0.1.3/describealign.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 '''
 
 VIDEO_EXTENSIONS = set(['mp4', 'mkv', 'avi', 'mov', 'webm', 'mkv', 'm4v', 'flv', 'vob'])
 AUDIO_EXTENSIONS = set(['mp3', 'm4a', 'opus', 'wav', 'aac', 'flac', 'ac3', 'mka'])
 OUTPUT_FILE_PREPEND_TEXT = "ad_"
 OUTPUT_DIR = "videos_with_ad"
 PLOT_DIR = "alignment_plots"
+EXTERNAL_FILES_FOLDER = "resources"
 PLOT_ALIGNMENT_TO_FILE = True
 
 TIMESTEP_SIZE_SECONDS = .16
 TIMESTEP_OVERLAP_RATIO = .5
 AUDIO_SAMPLE_RATE = 44100
 MEL_COEFFS_PER_TIMESTEP = 25
 DITHER_PERIOD_STEPS = 60
@@ -68,38 +69,40 @@
 
 def ensure_folders_exist(dirs):
   for dir in dirs:
     if not os.path.isdir(dir):
       print("Directory not found, creating it:", dir)
       os.makedirs(dir)
 
-def get_sorted_filenames(path, extensions):
+def get_sorted_filenames(path, extensions, alt_extensions=set([])):
   path = os.path.abspath(path)
   if os.path.isdir(path):
     files = glob.glob(path + "/*")
   else:
     if not os.path.isfile(path):
       print("No file found at:", path)
       raise RuntimeError("No valid file found at input path.")
     files = [path]
-  files = [file for file in files if os.path.splitext(file)[1][1:] in extensions]
+  files = [file for file in files if os.path.splitext(file)[1][1:] in extensions | alt_extensions]
   if len(files) == 0:
     print("Not enough files with valid extensions present at:", path)
     print("Did you accidentally put the audio filepath before the video filepath?")
     print("The video path should be the first positional input, audio second.")
     print("Or maybe you need to add a new extension to this script's regex?")
     raise RuntimeError("No valid files found at input path.")
-  return sorted(files)
+  files = sorted(files)
+  file_types = [0 if os.path.splitext(file)[1][1:] in extensions else 1 for file in files]
+  return files, file_types
 
 # read audio from file with ffmpeg and convert to numpy array
 def parse_audio_from_file(media_file):
   media_stream, _ = (ffmpeg
     .input(media_file)
     .output('-', format='s16le', acodec='pcm_s16le', ac=2, ar=AUDIO_SAMPLE_RATE, loglevel='fatal')
-    .run(capture_stdout=True, cmd=imageio_ffmpeg.get_ffmpeg_exe())
+    .run(capture_stdout=True, cmd=get_ffmpeg())
   )
   media_arr = np.frombuffer(media_stream, np.int16).astype(np.float32).reshape((-1,2)).T
   return media_arr
 
 # tokenize audio by transforming with a mel-frequency cepstrum (MFC)
 def tokenize_audio(media_arr, rate=1):
   step_size_samples = psf.sigproc.round_half_up(TIMESTEP_SIZE_SECONDS * rate * AUDIO_SAMPLE_RATE)
@@ -253,15 +256,15 @@
     # correlations are between -1 and 1, as all tokens have unit norm
     token_correlation = np.dot(audio_desc_spec[node[0]],video_spec[node[1]])
     fisher_info = min(max(0, get_fisher_info(node)), 10)
     return max(0, token_correlation - MIN_CORR_FOR_TOKEN_MATCH) * (fisher_info / 5)
   
   # filter out low match quality nodes from LCS path
   quals = [get_match_quality(node) for node in path]
-  if max(quals) <= 0:
+  if len(quals) == 0 or max(quals) <= 0:
     raise RuntimeError("Rough alignment failed, are the input files mismatched?")
   path, quals = zip(*[(path, qual) for (path, qual) in zip(path, quals) if qual > 0])
   
   # convert units of path nodes from timesteps to seconds
   path = [(audio_desc_timings[i], video_timings[j]) for (i,j) in path]
   
   return path, quals
@@ -398,17 +401,22 @@
 def plot_alignment(plot_filename, path, smooth_path, quals, runs, bad_clips, ad_timings):
   scatter_color = [.2,.4,.8]
   lcs_rgba = np.zeros((len(quals),4))
   lcs_rgba[:,:3] = np.array(scatter_color)[None,:]
   lcs_rgba[:,3] = np.minimum(1, np.array(quals) * 500. / len(quals))
   audio_times, video_times = np.array(path).T.reshape((2,-1))
   audio_offsets = audio_times - video_times
-  plt.xlim((0, np.max(video_times) / 60.))
-  plt.ylim((np.min(audio_offsets) - TIMESTEP_SIZE_SECONDS / 2.,
-            np.max(audio_offsets) + TIMESTEP_SIZE_SECONDS / 2.))
+  def expand_limits(start, end, ratio=.01):
+    average = (end + start) / 2.
+    half_diff = (end - start) / 2.
+    half_diff *= (1 + ratio)
+    return (average - half_diff, average + half_diff)
+  plt.xlim(expand_limits(*(0, np.max(video_times) / 60.)))
+  plt.ylim(expand_limits(*(np.min(audio_offsets) - TIMESTEP_SIZE_SECONDS / 2.,
+                          np.max(audio_offsets) + TIMESTEP_SIZE_SECONDS / 2.)))
   plt.scatter(video_times / 60., audio_offsets, s=3, c=lcs_rgba, label='LCS Matches')
   audio_times, video_times = np.array(smooth_path).T.reshape((2,-1))
   audio_offsets = audio_times - video_times
   if ad_timings is None:
     plt.plot(video_times / 60., audio_offsets, 'r-', lw=.5, label='Replaced Audio')
     bad_path = []
     for clip in bad_clips:
@@ -621,55 +629,74 @@
   speech_sample_mask = token_mask_to_sample_mask(speech_mask)
   boost_sample_mask = token_mask_to_sample_mask(boost_mask)
   ad_timings = video_timings.copy()
   ad_timings[~speech_mask] = np.inf
   
   return speech_sample_mask, boost_sample_mask, ad_timings
 
-# outputs a new video file with the replaced audio (which includes audio descriptions)
-def write_replaced_media_to_disk(output_filename, video_file, video_arr):
-  video_arr_pipe = ffmpeg.input('pipe:', format='s16le', acodec='pcm_s16le',
+# check whether ffmpeg is available locally before checking for an installed version
+def get_ffmpeg():
+  if os.path.isdir(EXTERNAL_FILES_FOLDER):
+    files = glob.glob(EXTERNAL_FILES_FOLDER + "/ffmpeg*")
+    if len(files) > 0:
+      return files[0]
+  return imageio_ffmpeg.get_ffmpeg_exe()
+
+# outputs a new media file with the replaced audio (which includes audio descriptions)
+def write_replaced_media_to_disk(output_filename, media_arr, video_file=None):
+  media_arr_pipe = ffmpeg.input('pipe:', format='s16le', acodec='pcm_s16le',
                                 ac=2, ar=AUDIO_SAMPLE_RATE)
   original_video = ffmpeg.input(video_file, an=None)
-  # "-max_interleave_delta 0" is sometimes necessary to fix an .mkv bug that freezes audio/video:
-  #   ffmpeg bug warning: [matroska @ 0000000002c814c0] Starting new cluster due to timestamp
-  # more info about the bug and fix: https://reddit.com/r/ffmpeg/comments/efddfs/
-  write_command = ffmpeg.output(video_arr_pipe, original_video, output_filename,
-                                acodec='aac', vcodec='copy', scodec='copy',
-                                max_interleave_delta='0', loglevel='fatal')
-  ffmpeg_caller = write_command.run_async(pipe_stdin=True, cmd=imageio_ffmpeg.get_ffmpeg_exe())
-  ffmpeg_caller.stdin.write(video_arr.astype(np.int16).T.tobytes())
+  if video_file is None:
+    write_command = ffmpeg.output(media_arr_pipe, output_filename, loglevel='fatal')
+  else:
+    # "-max_interleave_delta 0" is sometimes necessary to fix an .mkv bug that freezes audio/video:
+    #   ffmpeg bug warning: [matroska @ 0000000002c814c0] Starting new cluster due to timestamp
+    # more info about the bug and fix: https://reddit.com/r/ffmpeg/comments/efddfs/
+    write_command = ffmpeg.output(media_arr_pipe, original_video, output_filename,
+                                  acodec='aac', vcodec='copy', scodec='copy',
+                                  max_interleave_delta='0', loglevel='fatal')
+  ffmpeg_caller = write_command.run_async(pipe_stdin=True, cmd=get_ffmpeg())
+  ffmpeg_caller.stdin.write(media_arr.astype(np.int16).T.tobytes())
   ffmpeg_caller.stdin.close()
   ffmpeg_caller.wait()
 
 # combines videos with matching audio files (e.g. audio descriptions)
 # this is the main function of this script, it calls the other functions in order
 def combine(video, audio, smoothness=50, keep_non_ad=False, boost=0,
-            ad_detect_sensitivity=.6, boost_sensitivity=.4):
-  video_files = get_sorted_filenames(video, VIDEO_EXTENSIONS)
-  audio_desc_files = get_sorted_filenames(audio, AUDIO_EXTENSIONS)
+            ad_detect_sensitivity=.6, boost_sensitivity=.4, yes=False):
+  video_files, video_file_types = get_sorted_filenames(video, VIDEO_EXTENSIONS, AUDIO_EXTENSIONS)
+  if yes == False and sum(video_file_types) > 0:
+    print("")
+    print("One or more audio files found in video input. Was this intentional?")
+    print("If not, press ctrl+c to kill this script.")
+    input("If this was intended, press Enter to continue...")
+    print("")
+  audio_desc_files, _ = get_sorted_filenames(audio, AUDIO_EXTENSIONS)
   if len(video_files) != len(audio_desc_files):
     raise RuntimeError("Number of valid files in input directories are not the same.")
   
   ensure_folders_exist([OUTPUT_DIR])
   if PLOT_ALIGNMENT_TO_FILE:
     ensure_folders_exist([PLOT_DIR])
   
   print("")
   for (video_file, audio_desc_file) in zip(video_files, audio_desc_files):
     print(os.path.split(video_file)[1])
     print(os.path.split(audio_desc_file)[1])
     print("")
-  print("Are the above input file pairings correct?")
-  print("If not, press ctrl+c to kill this script.")
-  input("If they are correct, press Enter to continue...")
-  print("")
+  if yes == False:
+    print("Are the above input file pairings correct?")
+    print("If not, press ctrl+c to kill this script.")
+    input("If they are correct, press Enter to continue...")
+    print("")
   print("Processing files:")
   
-  for (video_file, audio_desc_file) in zip(video_files, audio_desc_files):
+  for (video_file, audio_desc_file, video_filetype) in zip(video_files, audio_desc_files,
+                                                           video_file_types):
     output_filename = os.path.join(OUTPUT_DIR, OUTPUT_FILE_PREPEND_TEXT + \
                                                os.path.split(video_file)[1])
     print(" ", output_filename)
     
     if os.path.exists(output_filename):
       print("   ", "output file already exists, skipping...")
       continue
@@ -712,16 +739,18 @@
     
     # prevent peaking by rescaling to within +/- 16,382
     video_arr *= (2**15 - 2.) / np.max(np.abs(video_arr))
     
     if PLOT_ALIGNMENT_TO_FILE:
       plot_filename = os.path.join(PLOT_DIR, os.path.splitext(os.path.split(video_file)[1])[0] + '.png')
       plot_alignment(plot_filename, path, smooth_path, quals, runs, bad_clips, ad_timings)
-    
-    write_replaced_media_to_disk(output_filename, video_file, video_arr)
+    if video_filetype == 0:
+      write_replaced_media_to_disk(output_filename, video_arr, video_file)
+    else:
+      write_replaced_media_to_disk(output_filename, video_arr)
     del video_arr
 
 # Entry point for command line interaction, for example:
 # > describealign video.mp4 audio_desc.mp3
 def command_line_interface():
   parser = argparse.ArgumentParser(description="Replaces a video's sound with an audio description.",
                                    usage="python ADsync.py video_file.mp4 audio_file.mp3")
@@ -739,18 +768,20 @@
                            '-3 makes the describer about 2x quieter, while 3 makes them 2x louder.')
   parser.add_argument('--ad_detect_sensitivity', type=float, default=.6,
                       help='Audio description detection sensitivity ratio. Higher values make ' + \
                            '--keep_non_ad more likely to replace aligned audio. Default is 0.6')
   parser.add_argument('--boost_sensitivity', type=float, default=.4,
                       help='Higher values make --boost less likely to miss a description, but ' + \
                            'also make it more likely to boost non-description audio. Default is 0.4')
+  parser.add_argument('--yes', action='store_true',
+                      help='Auto-skips user prompts asking to verify information.')
   args = parser.parse_args()
   
   combine(args.video, args.audio, args.smoothness, args.keep_non_ad, args.boost,
-          args.ad_detect_sensitivity, args.boost_sensitivity)
+          args.ad_detect_sensitivity, args.boost_sensitivity, args.yes)
 
 # allows the script to be run on its own, rather than through the package, for example:
 # python3 describealign.py video.mp4 audio_desc.mp3
 if __name__ == "__main__":
   command_line_interface()
```

### Comparing `describealign-0.1.2/pyproject.toml` & `describealign-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "describealign"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Julian Brown", email="julbean@proton.me" },
 ]
 description = "Combines videos with matching audio files (e.g. audio descriptions)"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

