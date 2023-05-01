# Comparing `tmp/media_tools-0.4.0.tar.gz` & `tmp/media_tools-0.4.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media_tools-0.4.0.tar", max compression
+gzip compressed data, was "media_tools-0.4.2a0.tar", max compression
```

## Comparing `media_tools-0.4.0.tar` & `media_tools-0.4.2a0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    13091 2023-01-04 16:33:51.314113 media_tools-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-01-04 16:33:51.314113 media_tools-0.4.0/media_tools/__init__.py
--rw-r--r--   0        0        0     1990 2023-01-04 16:33:51.314113 media_tools-0.4.0/media_tools/backup_lastfm_data.py
--rw-r--r--   0        0        0     3403 2023-01-04 16:33:51.314113 media_tools-0.4.0/media_tools/buy_most_played.py
--rwxr-xr-x   0        0        0     4954 2023-01-04 16:33:51.314113 media_tools-0.4.0/media_tools/clean_filenames.py
--rwxr-xr-x   0        0        0     3991 2023-01-04 16:33:51.314113 media_tools-0.4.0/media_tools/copy_from_playlist.py
--rw-r--r--   0        0        0     7704 2023-01-04 16:33:51.314113 media_tools-0.4.0/media_tools/mixcloud_upload.py
--rw-r--r--   0        0        0     5569 2023-01-04 16:33:51.314113 media_tools-0.4.0/media_tools/print_length.py
--rw-r--r--   0        0        0      579 2023-01-04 16:33:51.314113 media_tools-0.4.0/media_tools/util/__init__.py
--rw-r--r--   0        0        0     3612 2023-01-04 16:33:51.314113 media_tools-0.4.0/media_tools/util/audacious_tools.py
--rw-r--r--   0        0        0      758 2023-01-04 16:33:51.314113 media_tools-0.4.0/media_tools/util/base_filename_cleaner.py
--rw-r--r--   0        0        0       51 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/buying/__init__.py
--rw-r--r--   0        0        0     1486 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/buying/distributor.py
--rw-r--r--   0        0        0     2725 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/buying/last_fm.py
--rw-r--r--   0        0        0     1181 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/buying/retry_http.py
--rw-r--r--   0        0        0     2180 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/buying/track.py
--rw-r--r--   0        0        0     1098 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/buying/trackdb.py
--rw-r--r--   0        0        0     1526 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/command.py
--rw-r--r--   0        0        0     1116 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/dump_data.py
--rw-r--r--   0        0        0     2630 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/duplicate_string_remover.py
--rw-r--r--   0        0        0     2156 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/junk_remover.py
--rw-r--r--   0        0        0      828 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/lastfm_user.py
--rw-r--r--   0        0        0     1907 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/length_reader.py
--rw-r--r--   0        0        0      489 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/logging.py
--rw-r--r--   0        0        0      418 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/mixcloud/__init__.py
--rw-r--r--   0        0        0      100 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/mixcloud/authorization_error.py
--rw-r--r--   0        0        0      560 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/mixcloud/constants.py
--rw-r--r--   0        0        0     6555 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/mixcloud/create_api_token.py
--rw-r--r--   0        0        0     1910 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/mixcloud/globals.py
--rw-r--r--   0        0        0     9467 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/mixcloud/mix.py
--rw-r--r--   0        0        0     1722 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/mixcloud/mix_path.py
--rw-r--r--   0        0        0     2405 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/mixcloud/multi_mix.py
--rw-r--r--   0        0        0     3528 2023-01-04 16:33:51.315113 media_tools-0.4.0/media_tools/util/mixcloud/oauth_parameter_receiver.py
--rw-r--r--   0        0        0     5324 2023-01-04 16:33:51.316113 media_tools-0.4.0/media_tools/util/numbering_fixer.py
--rw-r--r--   0        0        0     2996 2023-01-04 16:33:51.316113 media_tools-0.4.0/media_tools/util/playlist_copier.py
--rw-r--r--   0        0        0     3825 2023-01-04 16:33:51.316113 media_tools-0.4.0/media_tools/util/scrobbles.py
--rw-r--r--   0        0        0     2242 2023-01-04 16:33:51.316113 media_tools-0.4.0/media_tools/util/symlink_fixer.py
--rw-r--r--   0        0        0      702 2023-01-04 16:33:51.316113 media_tools-0.4.0/media_tools/util/undo_commands.py
--rw-r--r--   0        0        0     1080 2023-01-04 16:33:51.316113 media_tools-0.4.0/media_tools/util/util.py
--rw-r--r--   0        0        0     1434 2023-01-04 16:33:51.317113 media_tools-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    14998 1970-01-01 00:00:00.000000 media_tools-0.4.0/setup.py
--rw-r--r--   0        0        0    14233 1970-01-01 00:00:00.000000 media_tools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-01 19:12:46.948397 media_tools-0.4.2a0/LICENSE
+-rw-r--r--   0        0        0    13066 2023-05-01 19:12:46.948397 media_tools-0.4.2a0/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 19:12:46.948397 media_tools-0.4.2a0/media_tools/__init__.py
+-rw-r--r--   0        0        0     1990 2023-05-01 19:12:46.948397 media_tools-0.4.2a0/media_tools/backup_lastfm_data.py
+-rw-r--r--   0        0        0     3403 2023-05-01 19:12:46.948397 media_tools-0.4.2a0/media_tools/buy_most_played.py
+-rwxr-xr-x   0        0        0     4954 2023-05-01 19:12:46.948397 media_tools-0.4.2a0/media_tools/clean_filenames.py
+-rwxr-xr-x   0        0        0     3991 2023-05-01 19:12:46.948397 media_tools-0.4.2a0/media_tools/copy_from_playlist.py
+-rw-r--r--   0        0        0     7703 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/mixcloud_upload.py
+-rw-r--r--   0        0        0     5569 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/print_length.py
+-rw-r--r--   0        0        0      579 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/__init__.py
+-rw-r--r--   0        0        0     3630 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/audacious_tools.py
+-rw-r--r--   0        0        0      758 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/base_filename_cleaner.py
+-rw-r--r--   0        0        0       51 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/buying/__init__.py
+-rw-r--r--   0        0        0     1486 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/buying/distributor.py
+-rw-r--r--   0        0        0     2725 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/buying/last_fm.py
+-rw-r--r--   0        0        0     1181 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/buying/retry_http.py
+-rw-r--r--   0        0        0     2180 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/buying/track.py
+-rw-r--r--   0        0        0     1098 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/buying/trackdb.py
+-rw-r--r--   0        0        0     1526 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/command.py
+-rw-r--r--   0        0        0     1124 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/dump_data.py
+-rw-r--r--   0        0        0     2630 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/duplicate_string_remover.py
+-rw-r--r--   0        0        0     2156 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/junk_remover.py
+-rw-r--r--   0        0        0      828 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/lastfm_user.py
+-rw-r--r--   0        0        0     1907 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/length_reader.py
+-rw-r--r--   0        0        0      489 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/logging.py
+-rw-r--r--   0        0        0      418 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/mixcloud/__init__.py
+-rw-r--r--   0        0        0      100 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/mixcloud/authorization_error.py
+-rw-r--r--   0        0        0      599 2023-05-01 19:12:46.949397 media_tools-0.4.2a0/media_tools/util/mixcloud/constants.py
+-rw-r--r--   0        0        0     6555 2023-05-01 19:12:46.950397 media_tools-0.4.2a0/media_tools/util/mixcloud/create_api_token.py
+-rw-r--r--   0        0        0     1910 2023-05-01 19:12:46.950397 media_tools-0.4.2a0/media_tools/util/mixcloud/globals.py
+-rw-r--r--   0        0        0    10343 2023-05-01 19:12:46.950397 media_tools-0.4.2a0/media_tools/util/mixcloud/mix.py
+-rw-r--r--   0        0        0     1720 2023-05-01 19:12:46.950397 media_tools-0.4.2a0/media_tools/util/mixcloud/mix_path.py
+-rw-r--r--   0        0        0     2405 2023-05-01 19:12:46.950397 media_tools-0.4.2a0/media_tools/util/mixcloud/multi_mix.py
+-rw-r--r--   0        0        0     3528 2023-05-01 19:12:46.950397 media_tools-0.4.2a0/media_tools/util/mixcloud/oauth_parameter_receiver.py
+-rw-r--r--   0        0        0     5324 2023-05-01 19:12:46.950397 media_tools-0.4.2a0/media_tools/util/numbering_fixer.py
+-rw-r--r--   0        0        0     2996 2023-05-01 19:12:46.950397 media_tools-0.4.2a0/media_tools/util/playlist_copier.py
+-rw-r--r--   0        0        0     3847 2023-05-01 19:12:46.950397 media_tools-0.4.2a0/media_tools/util/scrobbles.py
+-rw-r--r--   0        0        0     2242 2023-05-01 19:12:46.950397 media_tools-0.4.2a0/media_tools/util/symlink_fixer.py
+-rw-r--r--   0        0        0      702 2023-05-01 19:12:46.950397 media_tools-0.4.2a0/media_tools/util/undo_commands.py
+-rw-r--r--   0        0        0     1080 2023-05-01 19:12:46.950397 media_tools-0.4.2a0/media_tools/util/util.py
+-rw-r--r--   0        0        0     1576 2023-05-01 19:12:46.951397 media_tools-0.4.2a0/pyproject.toml
+-rw-r--r--   0        0        0    14160 1970-01-01 00:00:00.000000 media_tools-0.4.2a0/PKG-INFO
```

### Comparing `media_tools-0.4.0/README.md` & `media_tools-0.4.2a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 Installation
 ============
 
 ``` {.bash}
 $ pip install media-tools
 ```
-This will install the commands `mixcloud`, `buy_most_played`, `clean_filenames`, 
+This will install the commands `mixcloud`, `buy_most_played`, `clean_filenames`,
 `backup_lastfm_data`, `copy_from_playlist` and `print_length`.
 
 Usage
 =====
 
 `mixcloud`
 -----------------
@@ -63,62 +63,62 @@
     |-- description.txt
     |-- tags.txt
 
 ``` {.shell}
 $ mixcloud upload -d "10 - My awesome mix"
 ```
 will upload this mix to Mixcloud under the name "My awesome mix" with track 01 to 04 in that order.
-Prefixing the tracks with numbers is not necessary, but helpful to ensure the tracks are in the 
+Prefixing the tracks with numbers is not necessary, but helpful to ensure the tracks are in the
 desired order.
 
 #### Options
 
-- `-d DIRECTORY`, `--directory DIRECTORY`: Specify the folder containing the mix, as seen in the 
+- `-d DIRECTORY`, `--directory DIRECTORY`: Specify the folder containing the mix, as seen in the
     example above
-- `-e EXTENSION [EXTENSION ...]`, `--extensions EXTENSION [EXTENSION ...]`: List of file extensions 
+- `-e EXTENSION [EXTENSION ...]`, `--extensions EXTENSION [EXTENSION ...]`: List of file extensions
     to consider as audio files for the mix. Per default, files ending in `.mp3`, `.MP3`, `.flac`,
-    `.m4a` and `.ogg` are treated as audio and added to the mix. Change this list if any of your 
-    audio files have extensions that are not part of this list, or if you want to exclude any of 
+    `.m4a` and `.ogg` are treated as audio and added to the mix. Change this list if any of your
+    audio files have extensions that are not part of this list, or if you want to exclude any of
     these extensions.
 - `-q`, `--quiet`: Only errors are printed. Usually you want to omit `-q`, since the entire
-    generating and uploading process takes several minutes, so you want to be informed of what is 
+    generating and uploading process takes several minutes, so you want to be informed of what is
     going on.
 - `-s`, `--strict`: Do not upload the mix if any of these conditions are met:
     -   There is no picture, no `descriptions.txt` or no `tags.txt` in the upload folder
     -   Any of the audio tracks in the folder is missing the ID3 tag for title or artist. These tags
         are needed to generate the tracklist for the mix.
 - `-c CROSSFADE_MS`, `--crossfade-ms CROSSFADE_MS`: Number of milliseconds to use for crossfading
     between two tracks. Currently, there can only be one global value which is used between all
     tracks.
 - `-r MAX_RETRY`, `--max-retry MAX_RETRY`: Maximum number of retries for failing uploads. Uploads
     can fail for a number of reasons, such as rate limiting on the Mixcloud side, or because of a
     bad internet connection. The default number of retries is set to 100, set this to a lower number
     if you want to give up earlier.
-- `-a TOKEN_FILE`, `--auth-token-file TOKEN_FILE`: explicitly specify the file containing the 
+- `-a TOKEN_FILE`, `--auth-token-file TOKEN_FILE`: explicitly specify the file containing the
     Mixcloud authorization token.
-- `-t TOKEN_STRING`, `--auth-token-string TOKEN_STRING`: explicitly specify the Mixcloud 
+- `-t TOKEN_STRING`, `--auth-token-string TOKEN_STRING`: explicitly specify the Mixcloud
     authorization token as a string.
 - `--description-file DESCRIPTION_FILE` The description that goes with the mix on its Mixcloud page
 -   in a file
-- `--description DESCRIPTION_STRING` The description that goes with the mix on its Mixcloud page as 
+- `--description DESCRIPTION_STRING` The description that goes with the mix on its Mixcloud page as
 -   a string
 - `--tags-file TAGS_FILE` Tags for the mix, in a newline-separated file
 - `--tags TAG_STRING [TAG_STRING ...]` Tags for the mix, space-separated
 - `--picture-file PICTURE_FILE` Picture for the mix
 
 ### `mixcloud create-auth`: Create authorization with the Mixcloud API
 
-This process takes three steps. You will need to generate an application on Mixcloud for your 
-Mixcloud account, authorize it to get an OAuth token and ose the OAuth token get an API access 
-token, as described in the 
-[Mixcloud API Documentation](https://www.mixcloud.com/developers/#authorization). The 
+This process takes three steps. You will need to generate an application on Mixcloud for your
+Mixcloud account, authorize it to get an OAuth token and ose the OAuth token get an API access
+token, as described in the
+[Mixcloud API Documentation](https://www.mixcloud.com/developers/#authorization). The
 `mixcloud create-auth` command guides you through the process as follows:
 
 #### Step 1: Create a Mixcloud app
-Before you start this step, ensure that you are logged in to Mixcloud on your system browser, 
+Before you start this step, ensure that you are logged in to Mixcloud on your system browser,
 because you need to fill in the form that is going to open in your browser.
 
 Then enter:
 ``` {.shell}
 $ mixcloud create-auth --create-app
 ```
 A window will open in your browser. Follow the instructions printed in your terminal - click on the
@@ -131,28 +131,28 @@
 ```
 Again a browser window will open with a page displaying an "Authorize" button. Click it and you will
 be taken to a page displaying a so-called OAuth code. Copy the code to use it in step 3.
 
 #### Step 3: Create the Mixcloud API token
 Use the code from step 2 to run
 ``` {.shell}
-$ mixcloud create-auth --create-token --client-id CLIENT_ID \ 
+$ mixcloud create-auth --create-token --client-id CLIENT_ID \
                                       --client-secret CLIENT_SECRET \
                                       --oauth-code OAUTH_CODE
 ```
 This will open yet another browser window showing you a token (in JSON format). Copy only the string
-inside the quotes to use as token - either directly (here called <TOKEN>) or written (without any 
+inside the quotes to use as token - either directly (here called <TOKEN>) or written (without any
 extra spaces or newlines) to a file (here called <TOKEN_FILE>).
 
 Afterwards you can use the generated token to upload mixes to Mixcloud with:
 ``` {.shell}
 $ mixcloud upload --auth-token-string <TOKEN> ...
 $ mixcloud upload --auth-token-file <TOKEN_FILE> ...
 ```
-If you store this access token as `.mixcloud_access_token` in either the current directory, your 
+If you store this access token as `.mixcloud_access_token` in either the current directory, your
 user's `$HOME` directory or under `$HOME/.config/media-tools`, that token will be used without
 specifying `--auth-token-string` or `--auth-token-file`.
 
 ### Configuration options
 
 `clean_filenames`
 -----------------
@@ -264,53 +264,53 @@
 
 ### Options
 - `-u USER`, `--user USER`: Last.FM username
 - `-k API_KEY`, `--api-key API_KEY`: Last.FM API key
 - `-l LIMIT`, `--limit LIMIT`: Maximum number of tracks to display
 - `-m MIN_PLAYS`, `--min-plays MIN_PLAYS`: Minimum number of plays per track to consider buying it
 - `--buy-up-to BUY_UP_TO`: When specified, repeat until this may tracks have been bought
-- `-p PERIOD`, `--period PERIOD`: Period (`{overall,7day,1month,3month,6month,12month}`) from which 
+- `-p PERIOD`, `--period PERIOD`: Period (`{overall,7day,1month,3month,6month,12month}`) from which
   to choose favorite tracks
-- `-f FROM_DATE`, `--from-date FROM_DATE`: Start date of period in which most played tracks are 
+- `-f FROM_DATE`, `--from-date FROM_DATE`: Start date of period in which most played tracks are
   considered
 - `-t TO_DATE`, `--to-date TO_DATE`: End date of period in which most played tracks are considered
 - `-d TRACK_DB`, `--track-db TRACK_DB`: Name of the file storing already bought tracks
 
 
 `backup_lastfm_data`
 --------------------
 
 Back up Last.FM scrobbles. Output is saved in JSON format.
 
 ### Options
-- `--limit N`, `-l N`: maximum number of scrobbles (most recent scrobbles first) and other entities 
+- `--limit N`, `-l N`: maximum number of scrobbles (most recent scrobbles first) and other entities
   (top `N` items) to back up
 - `--year YEAR`, `-y YEAR`: year the data is requested for (empty for all Last.FM scrobbles)
 - `--output FILE`, `-o FILE`: output file name
-- `--max-retry-wait SECS`, `-m SECS`: maximum seconds to wait between requests to avoid rate 
+- `--max-retry-wait SECS`, `-m SECS`: maximum seconds to wait between requests to avoid rate
   limiting
 - `--lastfm-user USER`: Last.FM user name for scrobbles to be read (defaults to environment variable
   `$PYLAST_USERNAME`)
 - `--lastfm-api-key`: Last.FM API key (defaults to environment variable `PYLAST_API_KEY`)
 - `--lastfm-api-secret`: Last.FM API secret (defaults to environment variable `PYLAST_API_SECRET`)
 
 
 `print_length`
 --------------
 
-Given a directory of audio files, print the total playing time of that directory, optionally broken 
+Given a directory of audio files, print the total playing time of that directory, optionally broken
 down by subdirectory.
 
 ```shell
 $ print_length [OPTIONS] TARGET_DIRECTORY
 ```
 
 ### Options
-- `-r`/`--recursive`: print the playing time of each subdirectory, recursively descending 
-  subdirectories, sorted by directory playing time 
+- `-r`/`--recursive`: print the playing time of each subdirectory, recursively descending
+  subdirectories, sorted by directory playing time
 - `--debug`: print lots of internal info for debugging
 - `--max-debug-items N`: limit debugging output to the `N` shortest items
 
 
 Development
 ===========
```

### Comparing `media_tools-0.4.0/media_tools/backup_lastfm_data.py` & `media_tools-0.4.2a0/media_tools/backup_lastfm_data.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/buy_most_played.py` & `media_tools-0.4.2a0/media_tools/buy_most_played.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/clean_filenames.py` & `media_tools-0.4.2a0/media_tools/clean_filenames.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/copy_from_playlist.py` & `media_tools-0.4.2a0/media_tools/copy_from_playlist.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/mixcloud_upload.py` & `media_tools-0.4.2a0/media_tools/mixcloud_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         if not check(path):
             raise ValueError(f'{arg} is of wrong type')
         return path
     return inner
 
 
 def parse_commandline(args: List[str]) -> Namespace:
-    exit_on_error = dict(exit_on_error=False) if sys.version_info >= (3, 9) else {}
+    exit_on_error = {'exit_on_error': False} if sys.version_info >= (3, 9) else {}
     parser = ArgumentParser(
         description='Interface to the Mixcloud API to create mixes',
         **exit_on_error  # type: ignore
     )
     subparsers = parser.add_subparsers(
         title='subcommands', required=True
     )
```

### Comparing `media_tools-0.4.0/media_tools/print_length.py` & `media_tools-0.4.2a0/media_tools/print_length.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/__init__.py` & `media_tools-0.4.2a0/media_tools/util/__init__.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/audacious_tools.py` & `media_tools-0.4.2a0/media_tools/util/audacious_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = 'Lene Preuss <lene.preuss@gmail.com>'
 
 import os
-from subprocess import check_output
+from subprocess import check_output  # nosec
 from typing import List, Optional
 from urllib.parse import unquote
 
 DEFAULT_AUDACIOUS_CONFIG_DIR = os.path.join(
     os.environ['HOME'], '.config', 'audacious'
 )
 
@@ -77,15 +77,15 @@
                 self._file_base_dir, unquote(line[len(AudaciousTools.FILE_LINE_PREFIX):]).strip()
             )
             for line in lines if line.startswith(AudaciousTools.FILE_LINE_PREFIX)
         ]
 
     @staticmethod
     def _currently_playing_playlist_number() -> int:
-        return int(check_output(['audtool', 'current-playlist']))
+        return int(check_output(['audtool', 'current-playlist']))  # nosec
 
 
 def find_first_dir(name: str, path: str) -> Optional[str]:
     for root, dirs, _ in os.walk(path):
         if name in dirs:
             return os.path.join(root, name)
     return None
```

### Comparing `media_tools-0.4.0/media_tools/util/base_filename_cleaner.py` & `media_tools-0.4.2a0/media_tools/util/base_filename_cleaner.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/buying/distributor.py` & `media_tools-0.4.2a0/media_tools/util/buying/distributor.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/buying/last_fm.py` & `media_tools-0.4.2a0/media_tools/util/buying/last_fm.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/buying/retry_http.py` & `media_tools-0.4.2a0/media_tools/util/buying/retry_http.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/buying/track.py` & `media_tools-0.4.2a0/media_tools/util/buying/track.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/buying/trackdb.py` & `media_tools-0.4.2a0/media_tools/util/buying/trackdb.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/command.py` & `media_tools-0.4.2a0/media_tools/util/command.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/dump_data.py` & `media_tools-0.4.2a0/media_tools/util/dump_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 __author__ = 'Lene Preuss <lene.preuss@gmail.com>'
 
 import json
-import pickle
+import pickle  # nosec
 from bz2 import open as bzopen
 from gzip import open as gzopen
 from lzma import open as xzopen
 from typing import Callable, Dict
 
 OPEN_FUNCTIONS: Dict[str, Callable] = {
     'bz2': bzopen,
     'gz': gzopen,
     'xz': xzopen,
 }
 DUMP_PARAMS: Dict[str, Dict] = {
-    'json': {'dump': json.dump, 'mode': 'wt', 'kwargs': dict(default=str)},
+    'json': {'dump': json.dump, 'mode': 'wt', 'kwargs': {'default': str}},
     'pickle': {'dump': pickle.dump, 'mode': 'wb', 'kwargs': {}}
 }
 
 
 def open_function(extension: str) -> Callable:
     return OPEN_FUNCTIONS.get(extension, open)
```

### Comparing `media_tools-0.4.0/media_tools/util/duplicate_string_remover.py` & `media_tools-0.4.2a0/media_tools/util/duplicate_string_remover.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/junk_remover.py` & `media_tools-0.4.2a0/media_tools/util/junk_remover.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/lastfm_user.py` & `media_tools-0.4.2a0/media_tools/util/lastfm_user.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/length_reader.py` & `media_tools-0.4.2a0/media_tools/util/length_reader.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/mixcloud/constants.py` & `media_tools-0.4.2a0/media_tools/util/mixcloud/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 
 
 MIXCLOUD_MAX_FILESIZE = 512 * 1024 * 1024
 MIXCLOUD_MAX_TAGS = 5
 MIXCLOUD_API_UPLOAD_URL = 'https://api.mixcloud.com/upload'
 DEFAULT_CROSSFADE_MS = 1000
 DEFAULT_MAX_RETRY = 20
+ALLOWED_TRACKS_PER_ARTIST = 4
 DEFAULT_AUDIO_FILE_TYPES = ['flac', 'MP3', 'mp3', 'ogg', 'm4a']
 # Mixcloud app:
 # https://www.mixcloud.com/developers/Q29uc3VtZXI6MzY3Nw%253D%253D/
-ACCESS_TOKEN_FILE = '.mixcloud_access_token'
+ACCESS_TOKEN_FILE = '.mixcloud_access_token'  # nosec
 ACCESS_TOKEN_SEARCH_PATH = (Path('.'), Path.home(), Path.home() / '.config' / 'media-tools')
 MP3_KBIT_RATE = 128
```

### Comparing `media_tools-0.4.0/media_tools/util/mixcloud/create_api_token.py` & `media_tools-0.4.2a0/media_tools/util/mixcloud/create_api_token.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/mixcloud/globals.py` & `media_tools-0.4.2a0/media_tools/util/mixcloud/globals.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/mixcloud/mix.py` & `media_tools-0.4.2a0/media_tools/util/mixcloud/mix.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 __author__ = 'Lene Preuss <lene.preuss@gmail.com>'
 
 import logging
 import sys
+from collections import defaultdict
 from pathlib import Path
 from time import sleep
 from typing import List, Dict, Optional
 
 import requests
 from pydub import AudioSegment
 from tinytag import TinyTag
 
 from media_tools.util.mixcloud.constants import (
     DEFAULT_CROSSFADE_MS, DEFAULT_MAX_RETRY, MP3_KBIT_RATE, MIXCLOUD_API_UPLOAD_URL,
-    MIXCLOUD_MAX_TAGS
+    MIXCLOUD_MAX_TAGS, ALLOWED_TRACKS_PER_ARTIST
 )
 from media_tools.util.mixcloud.mix_path import MixPath
 
 
 class Mix:  # pylint: disable=too-many-instance-attributes
 
     def __init__(
@@ -48,20 +49,23 @@
         return not self._incomplete
 
     @property
     def tags(self) -> List[str]:
         tags = self._mix_path.tags
         error = self.check_tag_validity(tags)
         if error:
-            self._incomplete = True
-            logging.warning(str(error))
-            if self._strict:
-                raise ValueError(error)
+            self.raise_error(error)
         return tags
 
+    def raise_error(self, error: str) -> None:
+        self._incomplete = True
+        if self._strict:
+            raise ValueError(error)
+        logging.warning(error)
+
     @staticmethod
     def check_tag_validity(tags: List[str]) -> str:
         if len(tags) > MIXCLOUD_MAX_TAGS:
             return f'Max. {MIXCLOUD_MAX_TAGS} tags allowed, found {len(tags)}: {tags}'
         if not tags:
             return 'No tags found'
         return ''
@@ -74,77 +78,85 @@
         return f"Test - don't bother playing ({title})" if self._incomplete else title
 
     @property
     def description(self) -> str:
         description = self._mix_path.description
         if description:
             return description
-        if self._strict:
-            raise ValueError('No description found')
-        logging.warning('No description found')
-        self._incomplete = True
+        self.raise_error('No description found')
         return ''
 
     @property
     def picture(self) -> Optional[Path]:
         """Currently just returns the first JPEG or PNG. Room for improvement!"""
         try:
             return self._mix_path.picture
-        except StopIteration as error:
-            if self._strict:
-                raise ValueError(f'No picture in {self._mix_path.basedir}') from error
-            logging.warning('No picture found')
-            self._incomplete = True
+        except StopIteration:
+            self.raise_error(f'No picture in {self._mix_path.basedir}')
             return None
 
     def _import_audio(self, audio_files: List[Path]) -> AudioSegment:
         part_name = '' if self._part is None else f'_{self._part}'
         mix_file = self._mix_path.file(Path(f'mix{part_name}.mp3'))
         self._track_info = [self._get_track_info(audio_file) for audio_file in audio_files]
+        self._check_tracks_per_artist_limit()
         if mix_file.exists():
+            logging.info('Reading present %s', mix_file)
             return AudioSegment.from_file(mix_file)
 
         audio = AudioSegment.empty()
         for i, audio_file in enumerate(audio_files):
-            logging.info('%s - %s', i + 1, audio_file.name)
+            logging.info(
+                '%s: %s (%s - %s)',
+                i + 1, audio_file.name, self._track_info[i]['artist'], self._track_info[i]['title']
+            )
             audio = audio.append(
                 self._read_track(audio_file),
                 crossfade=self._crossfade_ms if len(audio) > self._crossfade_ms else len(audio)
             )
 
         return audio
 
+    def _check_tracks_per_artist_limit(self) -> None:
+        artists: Dict[str, int] = defaultdict(int)
+        for track in self._track_info:
+            artists[track['artist']] += 1
+        if artists and max(artists.values()) > ALLOWED_TRACKS_PER_ARTIST:
+            artists_with_too_many_tracks = ', '.join([
+                a for a, num in artists.items() if num > ALLOWED_TRACKS_PER_ARTIST
+            ])
+            self.raise_error(
+                f'More than {ALLOWED_TRACKS_PER_ARTIST} tracks by: {artists_with_too_many_tracks}')
+
     @staticmethod
     def _read_track(audio_file):
         track = AudioSegment.from_file(audio_file)
         if track.sample_width != 2:
             track = track.set_sample_width(2)
         if track.frame_rate != 44100:
             track = track.set_frame_rate(44100)
         return track.normalize()
 
     def _get_track_info(self, audio_file: Path) -> Dict:
         tags = TinyTag.get(str(audio_file))
         if tags.artist is None or tags.title is None:
-            if self._strict:
-                raise ValueError(f'Incomplete tags for {audio_file}')
-            logging.warning('Incomplete tags for %s', audio_file)
-            self._incomplete = True
+            self.raise_error(f'Incomplete tags for {audio_file}')
             return {
                 'artist': tags.artist or '???', 'title': tags.title or '???',
                 'length': tags.duration
             }
         return {
             'artist': tags.artist, 'title': tags.title, 'length': tags.duration,
             'filename': audio_file.name
         }
 
     def export(self, name: Path = Path('mix.mp3')) -> None:
         mix_file = self._mix_path.file(name)
         if mix_file.exists():
+            logging.info('Mix already exported as %s', mix_file)
             return
         audio_format = name.suffix[1:]
         logging.info(
             'Exporting %s audio to %s with bitrate %s kbps',
             self.mix_length(), mix_file, MP3_KBIT_RATE
         )
         self._audio.export(
@@ -152,15 +164,15 @@
         )
 
     def upload(self, name: Path = Path('mix.mp3'), max_retry: int = DEFAULT_MAX_RETRY) -> None:
         mix_file = self._mix_path.file(name)
         if not mix_file.exists():
             raise FileNotFoundError(mix_file)
         files = {
-            'mp3': ('mix.mp3', mix_file.open('rb'), 'audio/mpeg'),
+            'mp3': (str(name), mix_file.open('rb'), 'audio/mpeg'),
         }
         if self.picture:
             picture_type = self.picture.suffix
             files['picture'] = (
                 'picture' + picture_type, self.picture.open('rb'),
                 f'image/{"png" if picture_type == ".png" else "jpeg"}'
             )
@@ -184,19 +196,27 @@
 
     def _do_upload(self, name: Path, files: Dict, data: Dict, max_retry: int):
         if max_retry < 0:
             logging.error('out of retries, aborting upload attempt')
             sys.exit(1)
 
         url = MIXCLOUD_API_UPLOAD_URL + '/?access_token=' + self._access_token
-        logging.info('uploading to %s, max. %s retries', url, max_retry)
+        logging.info(
+            'uploading to %s, max. %s retries',
+            url.replace(self._access_token, '<REDACTED>'), max_retry
+        )
         try:
-            response = requests.post(url, files=files, data=data)
+            upload_timeout = 3600  # it can take quite a long time
+            response = requests.post(url, files=files, data=data, timeout=upload_timeout)
         except requests.exceptions.ConnectionError as error:
-            logging.warning(self.connection_error_message(error, max_retry))
+            logging.warning(
+                self.connection_error_message(error, max_retry).replace(
+                    self._access_token, '<REDACTED>'
+                )
+            )
             self._do_upload(name, files=files, data=data, max_retry=max_retry - 1)
         else:
             if self.is_rate_limited(response):
                 logging.info(self.response_message(response))
                 sleep(int(response.json().get('error', {}).get('retry_after', 60)))
                 self._do_upload(name, files=files, data=data, max_retry=max_retry - 1)
             elif response.status_code == 200:
@@ -229,15 +249,15 @@
 
     @staticmethod
     def error_args_message(error: requests.exceptions.ConnectionError) -> str:
         if not error.args:
             return ''
         if error.args[0].args and len(error.args[0].args) > 1:
             return f'{error.args[0].args[1].args[1]}: {error.args[0].args[0]} '
-        return str(error.args)
+        return ', '.join(str(arg) for arg in error.args)
 
     def _add_tags(self, data: Dict) -> None:
         for i, tag in enumerate(self.tags):
             data[f'tags-{i}-tag'] = tag
 
     def _add_track_info(self, data: Dict) -> None:
         start_time = 0
```

### Comparing `media_tools-0.4.0/media_tools/util/mixcloud/mix_path.py` & `media_tools-0.4.2a0/media_tools/util/mixcloud/mix_path.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def from_files(self, files: Tuple[Path, ...]):
         return MixPath(self.basedir, tuple(file.name for file in files))
 
     def file(self, filename: Path) -> Path:
         return self.basedir / filename
 
     def scan(self) -> Tuple[List[str], int]:
-        length = sum([TinyTag.get(str(audio_file)).duration for audio_file in self.audio_files])
+        length = sum(TinyTag.get(str(audio_file)).duration for audio_file in self.audio_files)
         return [f.name for f in self.audio_files], int(length)
 
     @property
     def tags(self) -> List[str]:
         if (self.basedir / 'tags.txt').exists():
             with (self.basedir / 'tags.txt').open() as file:
                 return list(line for line in (line.strip() for line in file) if line)
```

### Comparing `media_tools-0.4.0/media_tools/util/mixcloud/multi_mix.py` & `media_tools-0.4.2a0/media_tools/util/mixcloud/multi_mix.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/mixcloud/oauth_parameter_receiver.py` & `media_tools-0.4.2a0/media_tools/util/mixcloud/oauth_parameter_receiver.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/numbering_fixer.py` & `media_tools-0.4.2a0/media_tools/util/numbering_fixer.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/playlist_copier.py` & `media_tools-0.4.2a0/media_tools/util/playlist_copier.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/scrobbles.py` & `media_tools-0.4.2a0/media_tools/util/scrobbles.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,24 +40,24 @@
             play_count = self.user.get_playcount()
             tracks = self.get_and_wait(tracks, self.user.get_recent_tracks, wait_time, **year_dates)
             loved = self.get_and_wait(loved, self.user.get_loved_tracks, wait_time)
             top_tracks = self.get_and_wait(top_tracks, self.user.get_top_tracks, wait_time)
             top_artists = self.get_and_wait(None, self.user.get_top_artists, wait_time)
             top_albums = self.get_and_wait(None, self.user.get_top_albums, wait_time)
             top_tags = self.user.get_top_tags(limit=self.limit)
-            return dict(
-                time=datetime.now(),
-                play_count=play_count,
-                tracks=tracks,
-                loved=loved,
-                top_tracks=top_tracks,
-                top_artists=top_artists,
-                top_albums=top_albums,
-                top_tags=top_tags,
-            )
+            return {
+                'time': datetime.now(),
+                'play_count': play_count,
+                'tracks': tracks,
+                'loved': loved,
+                'top_tracks': top_tracks,
+                'top_artists': top_artists,
+                'top_albums': top_albums,
+                'top_tags': top_tags,
+            }
         # pylast has a feature to deal with rate limiting, but it doesn't seem to work reliably
         except PyLastError as error:
             logging.info('%s: %s', type(error).__name__, str(error))
             next_wait_time = 1 if wait_time == 0 else 2 * wait_time
             if next_wait_time <= self.max_retry_wait:
                 logging.warning(
                     '%s, retrying with %ss wait time', type(error).__name__, next_wait_time
@@ -88,8 +88,8 @@
 def from_datetime(convert_datetime: datetime) -> int:
     return timegm(convert_datetime.utctimetuple())
 
 
 def year_range(year: Optional[int]) -> Dict[str, int]:
     start = None if year is None else from_datetime(datetime(year, 1, 1, 0, 0, 0))
     end = None if year is None else from_datetime(datetime(year, 12, 31, 23, 59, 59, 999999))
-    return dict(time_from=start, time_to=end)
+    return {'time_from': start, 'time_to': end}
```

### Comparing `media_tools-0.4.0/media_tools/util/symlink_fixer.py` & `media_tools-0.4.2a0/media_tools/util/symlink_fixer.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/undo_commands.py` & `media_tools-0.4.2a0/media_tools/util/undo_commands.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/media_tools/util/util.py` & `media_tools-0.4.2a0/media_tools/util/util.py`

 * *Files identical despite different names*

### Comparing `media_tools-0.4.0/pyproject.toml` & `media_tools-0.4.2a0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "media-tools"
-version = "0.4.0"
+version = "0.4.2a"
 description = "Creating and managing playlists, and managing the filenames and directory structure for large numbers of music files."
 authors = ["Lene Preuss <lene.preuss@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lilacashes/music-library-tools"
 repository = "https://gitlab.com/lilacashes/music-library-tools.git"
 keywords = ["music", "audio"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 lxml = ">=4.8.0"
 tinytag = ">=1.8.1"
 pydub = ">=0.24.1"
 requests = ">=2.27.1"
 pylast = ">=5.0.0"
 python-magic = ">=0.4.25"
 audioread = ">=2.1.9"
@@ -31,19 +31,26 @@
 py-spy = "^0.3.11"
 requests-mock = "^1.8.0"
 types-requests = ">=2.27.16"
 pytest = ">=7.1.1"
 pytest-cov = ">=3.0.0"
 ptpython = "^3.0.20"
 pytest-xdist = "^2.5.0"
+eyed3 = ">=0.9.7"
+soundfile = "<0.12" # version 0.12 breaks pydub
+pre-commit = "^3.2.1"
+bandit = "^1.7.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.bandit]
+exclude = ["tests"]
+
 [tool.poetry.scripts]
 mixcloud = "media_tools.mixcloud_upload:main"
 buy_most_played = "media_tools.buy_most_played:main"
 clean_filenames = "media_tools.clean_filenames:main"
 backup_lastfm_data = "media_tools.backup_lastfm_data:entry"
 copy_from_playlist = "media_tools.copy_from_playlist:main"
 print_length = "media_tools.print_length:main"
```

### Comparing `media_tools-0.4.0/PKG-INFO` & `media_tools-0.4.2a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: media-tools
-Version: 0.4.0
+Version: 0.4.2a0
 Summary: Creating and managing playlists, and managing the filenames and directory structure for large numbers of music files.
 Home-page: https://gitlab.com/lilacashes/music-library-tools
 License: MIT
 Keywords: music,audio
 Author: Lene Preuss
 Author-email: lene.preuss@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: audioread (>=2.1.9)
 Requires-Dist: coloredlogs (>=15.0.1)
 Requires-Dist: lxml (>=4.8.0)
@@ -55,15 +54,15 @@
 
 Installation
 ============
 
 ``` {.bash}
 $ pip install media-tools
 ```
-This will install the commands `mixcloud`, `buy_most_played`, `clean_filenames`, 
+This will install the commands `mixcloud`, `buy_most_played`, `clean_filenames`,
 `backup_lastfm_data`, `copy_from_playlist` and `print_length`.
 
 Usage
 =====
 
 `mixcloud`
 -----------------
@@ -92,62 +91,62 @@
     |-- description.txt
     |-- tags.txt
 
 ``` {.shell}
 $ mixcloud upload -d "10 - My awesome mix"
 ```
 will upload this mix to Mixcloud under the name "My awesome mix" with track 01 to 04 in that order.
-Prefixing the tracks with numbers is not necessary, but helpful to ensure the tracks are in the 
+Prefixing the tracks with numbers is not necessary, but helpful to ensure the tracks are in the
 desired order.
 
 #### Options
 
-- `-d DIRECTORY`, `--directory DIRECTORY`: Specify the folder containing the mix, as seen in the 
+- `-d DIRECTORY`, `--directory DIRECTORY`: Specify the folder containing the mix, as seen in the
     example above
-- `-e EXTENSION [EXTENSION ...]`, `--extensions EXTENSION [EXTENSION ...]`: List of file extensions 
+- `-e EXTENSION [EXTENSION ...]`, `--extensions EXTENSION [EXTENSION ...]`: List of file extensions
     to consider as audio files for the mix. Per default, files ending in `.mp3`, `.MP3`, `.flac`,
-    `.m4a` and `.ogg` are treated as audio and added to the mix. Change this list if any of your 
-    audio files have extensions that are not part of this list, or if you want to exclude any of 
+    `.m4a` and `.ogg` are treated as audio and added to the mix. Change this list if any of your
+    audio files have extensions that are not part of this list, or if you want to exclude any of
     these extensions.
 - `-q`, `--quiet`: Only errors are printed. Usually you want to omit `-q`, since the entire
-    generating and uploading process takes several minutes, so you want to be informed of what is 
+    generating and uploading process takes several minutes, so you want to be informed of what is
     going on.
 - `-s`, `--strict`: Do not upload the mix if any of these conditions are met:
     -   There is no picture, no `descriptions.txt` or no `tags.txt` in the upload folder
     -   Any of the audio tracks in the folder is missing the ID3 tag for title or artist. These tags
         are needed to generate the tracklist for the mix.
 - `-c CROSSFADE_MS`, `--crossfade-ms CROSSFADE_MS`: Number of milliseconds to use for crossfading
     between two tracks. Currently, there can only be one global value which is used between all
     tracks.
 - `-r MAX_RETRY`, `--max-retry MAX_RETRY`: Maximum number of retries for failing uploads. Uploads
     can fail for a number of reasons, such as rate limiting on the Mixcloud side, or because of a
     bad internet connection. The default number of retries is set to 100, set this to a lower number
     if you want to give up earlier.
-- `-a TOKEN_FILE`, `--auth-token-file TOKEN_FILE`: explicitly specify the file containing the 
+- `-a TOKEN_FILE`, `--auth-token-file TOKEN_FILE`: explicitly specify the file containing the
     Mixcloud authorization token.
-- `-t TOKEN_STRING`, `--auth-token-string TOKEN_STRING`: explicitly specify the Mixcloud 
+- `-t TOKEN_STRING`, `--auth-token-string TOKEN_STRING`: explicitly specify the Mixcloud
     authorization token as a string.
 - `--description-file DESCRIPTION_FILE` The description that goes with the mix on its Mixcloud page
 -   in a file
-- `--description DESCRIPTION_STRING` The description that goes with the mix on its Mixcloud page as 
+- `--description DESCRIPTION_STRING` The description that goes with the mix on its Mixcloud page as
 -   a string
 - `--tags-file TAGS_FILE` Tags for the mix, in a newline-separated file
 - `--tags TAG_STRING [TAG_STRING ...]` Tags for the mix, space-separated
 - `--picture-file PICTURE_FILE` Picture for the mix
 
 ### `mixcloud create-auth`: Create authorization with the Mixcloud API
 
-This process takes three steps. You will need to generate an application on Mixcloud for your 
-Mixcloud account, authorize it to get an OAuth token and ose the OAuth token get an API access 
-token, as described in the 
-[Mixcloud API Documentation](https://www.mixcloud.com/developers/#authorization). The 
+This process takes three steps. You will need to generate an application on Mixcloud for your
+Mixcloud account, authorize it to get an OAuth token and ose the OAuth token get an API access
+token, as described in the
+[Mixcloud API Documentation](https://www.mixcloud.com/developers/#authorization). The
 `mixcloud create-auth` command guides you through the process as follows:
 
 #### Step 1: Create a Mixcloud app
-Before you start this step, ensure that you are logged in to Mixcloud on your system browser, 
+Before you start this step, ensure that you are logged in to Mixcloud on your system browser,
 because you need to fill in the form that is going to open in your browser.
 
 Then enter:
 ``` {.shell}
 $ mixcloud create-auth --create-app
 ```
 A window will open in your browser. Follow the instructions printed in your terminal - click on the
@@ -160,28 +159,28 @@
 ```
 Again a browser window will open with a page displaying an "Authorize" button. Click it and you will
 be taken to a page displaying a so-called OAuth code. Copy the code to use it in step 3.
 
 #### Step 3: Create the Mixcloud API token
 Use the code from step 2 to run
 ``` {.shell}
-$ mixcloud create-auth --create-token --client-id CLIENT_ID \ 
+$ mixcloud create-auth --create-token --client-id CLIENT_ID \
                                       --client-secret CLIENT_SECRET \
                                       --oauth-code OAUTH_CODE
 ```
 This will open yet another browser window showing you a token (in JSON format). Copy only the string
-inside the quotes to use as token - either directly (here called <TOKEN>) or written (without any 
+inside the quotes to use as token - either directly (here called <TOKEN>) or written (without any
 extra spaces or newlines) to a file (here called <TOKEN_FILE>).
 
 Afterwards you can use the generated token to upload mixes to Mixcloud with:
 ``` {.shell}
 $ mixcloud upload --auth-token-string <TOKEN> ...
 $ mixcloud upload --auth-token-file <TOKEN_FILE> ...
 ```
-If you store this access token as `.mixcloud_access_token` in either the current directory, your 
+If you store this access token as `.mixcloud_access_token` in either the current directory, your
 user's `$HOME` directory or under `$HOME/.config/media-tools`, that token will be used without
 specifying `--auth-token-string` or `--auth-token-file`.
 
 ### Configuration options
 
 `clean_filenames`
 -----------------
@@ -293,53 +292,53 @@
 
 ### Options
 - `-u USER`, `--user USER`: Last.FM username
 - `-k API_KEY`, `--api-key API_KEY`: Last.FM API key
 - `-l LIMIT`, `--limit LIMIT`: Maximum number of tracks to display
 - `-m MIN_PLAYS`, `--min-plays MIN_PLAYS`: Minimum number of plays per track to consider buying it
 - `--buy-up-to BUY_UP_TO`: When specified, repeat until this may tracks have been bought
-- `-p PERIOD`, `--period PERIOD`: Period (`{overall,7day,1month,3month,6month,12month}`) from which 
+- `-p PERIOD`, `--period PERIOD`: Period (`{overall,7day,1month,3month,6month,12month}`) from which
   to choose favorite tracks
-- `-f FROM_DATE`, `--from-date FROM_DATE`: Start date of period in which most played tracks are 
+- `-f FROM_DATE`, `--from-date FROM_DATE`: Start date of period in which most played tracks are
   considered
 - `-t TO_DATE`, `--to-date TO_DATE`: End date of period in which most played tracks are considered
 - `-d TRACK_DB`, `--track-db TRACK_DB`: Name of the file storing already bought tracks
 
 
 `backup_lastfm_data`
 --------------------
 
 Back up Last.FM scrobbles. Output is saved in JSON format.
 
 ### Options
-- `--limit N`, `-l N`: maximum number of scrobbles (most recent scrobbles first) and other entities 
+- `--limit N`, `-l N`: maximum number of scrobbles (most recent scrobbles first) and other entities
   (top `N` items) to back up
 - `--year YEAR`, `-y YEAR`: year the data is requested for (empty for all Last.FM scrobbles)
 - `--output FILE`, `-o FILE`: output file name
-- `--max-retry-wait SECS`, `-m SECS`: maximum seconds to wait between requests to avoid rate 
+- `--max-retry-wait SECS`, `-m SECS`: maximum seconds to wait between requests to avoid rate
   limiting
 - `--lastfm-user USER`: Last.FM user name for scrobbles to be read (defaults to environment variable
   `$PYLAST_USERNAME`)
 - `--lastfm-api-key`: Last.FM API key (defaults to environment variable `PYLAST_API_KEY`)
 - `--lastfm-api-secret`: Last.FM API secret (defaults to environment variable `PYLAST_API_SECRET`)
 
 
 `print_length`
 --------------
 
-Given a directory of audio files, print the total playing time of that directory, optionally broken 
+Given a directory of audio files, print the total playing time of that directory, optionally broken
 down by subdirectory.
 
 ```shell
 $ print_length [OPTIONS] TARGET_DIRECTORY
 ```
 
 ### Options
-- `-r`/`--recursive`: print the playing time of each subdirectory, recursively descending 
-  subdirectories, sorted by directory playing time 
+- `-r`/`--recursive`: print the playing time of each subdirectory, recursively descending
+  subdirectories, sorted by directory playing time
 - `--debug`: print lots of internal info for debugging
 - `--max-debug-items N`: limit debugging output to the `N` shortest items
 
 
 Development
 ===========
```

