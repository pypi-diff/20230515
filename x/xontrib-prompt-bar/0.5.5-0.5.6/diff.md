# Comparing `tmp/xontrib-prompt-bar-0.5.5.tar.gz` & `tmp/xontrib-prompt-bar-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xontrib-prompt-bar-0.5.5.tar", last modified: Thu Mar 23 11:47:33 2023, max compression
+gzip compressed data, was "xontrib-prompt-bar-0.5.6.tar", last modified: Mon May 15 14:30:53 2023, max compression
```

## Comparing `xontrib-prompt-bar-0.5.5.tar` & `xontrib-prompt-bar-0.5.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:47:33.537171 xontrib-prompt-bar-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-23 11:47:22.000000 xontrib-prompt-bar-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-23 11:47:22.000000 xontrib-prompt-bar-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-03-23 11:47:33.537171 xontrib-prompt-bar-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-03-23 11:47:22.000000 xontrib-prompt-bar-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 11:47:33.537171 xontrib-prompt-bar-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-23 11:47:22.000000 xontrib-prompt-bar-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:47:33.537171 xontrib-prompt-bar-0.5.5/xontrib/
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-03-23 11:47:22.000000 xontrib-prompt-bar-0.5.5/xontrib/prompt_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:47:33.537171 xontrib-prompt-bar-0.5.5/xontrib_prompt_bar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-03-23 11:47:33.000000 xontrib-prompt-bar-0.5.5/xontrib_prompt_bar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-23 11:47:33.000000 xontrib-prompt-bar-0.5.5/xontrib_prompt_bar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 11:47:33.000000 xontrib-prompt-bar-0.5.5/xontrib_prompt_bar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-23 11:47:33.000000 xontrib-prompt-bar-0.5.5/xontrib_prompt_bar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:30:53.608808 xontrib-prompt-bar-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-15 14:30:43.000000 xontrib-prompt-bar-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 14:30:43.000000 xontrib-prompt-bar-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-05-15 14:30:53.608808 xontrib-prompt-bar-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-05-15 14:30:43.000000 xontrib-prompt-bar-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 14:30:53.608808 xontrib-prompt-bar-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-15 14:30:43.000000 xontrib-prompt-bar-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:30:53.608808 xontrib-prompt-bar-0.5.6/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-15 14:30:43.000000 xontrib-prompt-bar-0.5.6/xontrib/prompt_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:30:53.608808 xontrib-prompt-bar-0.5.6/xontrib_prompt_bar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-05-15 14:30:53.000000 xontrib-prompt-bar-0.5.6/xontrib_prompt_bar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-15 14:30:53.000000 xontrib-prompt-bar-0.5.6/xontrib_prompt_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:30:53.000000 xontrib-prompt-bar-0.5.6/xontrib_prompt_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 14:30:53.000000 xontrib-prompt-bar-0.5.6/xontrib_prompt_bar.egg-info/top_level.txt
```

### Comparing `xontrib-prompt-bar-0.5.5/LICENSE` & `xontrib-prompt-bar-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xontrib-prompt-bar-0.5.5/PKG-INFO` & `xontrib-prompt-bar-0.5.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-prompt-bar
-Version: 0.5.5
+Version: 0.5.6
 Summary: The bar theme for xonsh shell.
 Home-page: https://github.com/anki-code/xontrib-prompt-bar
 Author: anki
 Author-email: author@example.com
 License: BSD
 Project-URL: Documentation, https://github.com/anki-code/xontrib-prompt-bar/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xontrib-prompt-bar
@@ -58,15 +58,15 @@
 ```
 
 ## Default theme
 
 ```python
 $XONTRIB_PROMPT_BAR_THEME = {
     'left': '{hostname}{user}{cwd_abs#accent}',
-    'right': '{curr_branch#section}{env_name#strip_brackets#section}{date_time_tz}',
+    'right': '{hist_status#section}{curr_branch#section}{env_name#strip_brackets#section}{date_time_tz}',
     'bar_bg': '{BACKGROUND_#323232}',
     'bar_fg': '{#AAA}',
     'section_bg': '{BACKGROUND_#444}',
     'section_fg': '{#CCC}',
     'accent_fg': '{BOLD_#DDD}',
 }
 xontrib load prompt_bar
@@ -77,14 +77,15 @@
 ### Customize the fields
 
 Supported fields:
 * [xonsh default fields and colors notation](https://xon.sh/tutorial.html#customizing-the-prompt)
 * `screens` - list of the windows that created by [screen window manager](https://www.gnu.org/software/screen/manual/screen.html#Overview) i.e. `screen -S mywin`.
 * `cwd_abs` - current absolute path (`~` disabled).
 * `date_time_tz` - date and time with timezone i.e. `21-12-25 18:00:00-01`.
+* `hist_status` - show `hist off` if history disabled by [`history off`](https://xon.sh/tutorial_hist.html#off-action) command.
 
 To customize the appearance of the fields on the bar you can use wrappers and chaining them:
 ```python
 $XONTRIB_PROMPT_BAR_RIGHT = '{hostname#accent#section} {date_time_tz#nocolorx}'
 xontrib load prompt_bar
 ```
 Builtin wrappers:
@@ -162,15 +163,15 @@
 
 ### Using [xontrib-cmd-durations](https://github.com/jnoortheen/xontrib-cmd-durations)
 
 The [xontrib-cmd-durations](https://github.com/jnoortheen/xontrib-cmd-durations) is to send notification once long-running command is finished and also show the execution time. Usage example:
 
 ```python
 # Add `{long_cmd_duration}` section
-$XONTRIB_PROMPT_BAR_RIGHT = '{long_cmd_duration}{screens#section}{env_name#strip_brackets#section}{date_time_tz}'
+$XONTRIB_PROMPT_BAR_RIGHT = '{long_cmd_duration}{curr_branch#section}{screens#section}{env_name#strip_brackets#section}{date_time_tz}'
 xontrib load cmd_done
 ```
 
 ### Hide return code in special cases
 
 Sometimes it's needed to hide the return code. In this case you can use `-8888` return code i.e.:
 
@@ -187,15 +188,15 @@
 * [xonsh default fields and colors notation](https://xon.sh/tutorial.html#customizing-the-prompt)
 * [Meaning of git status symbols](https://xon.sh/envvars.html#xonsh-gitstatus) (●×+⚑✓↑↓)
 * [Awesome example of rewriting the theme from Jonathan Slenders](https://github.com/prompt-toolkit/python-prompt-toolkit/blob/master/examples/prompts/fancy-zsh-prompt.py)
 * [Customization the colors in the input line](https://github.com/xonsh/xonsh/pull/3878#issuecomment-707982828)
 
 ## Environment variables
 
-* `$XONTRIB_PROMPT_BAR_SHOW_RETURN = True` - show return code.
+* `$XONTRIB_PROMPT_BAR_SHOW_RETURN` - show return code. Default `True`.
 
 ## Known issues
 ### Spaces in the copied and pasted command line
 Please update [prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit) 
 to 3.0.7+ version via `python -m pip install -U prompt_toolkit`.
 
 ## Credits
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xontrib-prompt-bar Version: 0.5.5 Summary: The bar
+Metadata-Version: 2.1 Name: xontrib-prompt-bar Version: 0.5.6 Summary: The bar
 theme for xonsh shell. Home-page: https://github.com/anki-code/xontrib-prompt-
 bar Author: anki Author-email: author@example.com License: BSD Project-URL:
 Documentation, https://github.com/anki-code/xontrib-prompt-bar/blob/master/
 README.md Project-URL: Code, https://github.com/anki-code/xontrib-prompt-bar
 Project-URL: Issue tracker, https://github.com/anki-code/xontrib-prompt-bar/
 issues Platform: any Classifier: Environment :: Console Classifier: Intended
 Audience :: End Users/Desktop Classifier: Operating System :: OS Independent
@@ -20,24 +20,26 @@
 command beginning has fixed position to have a large command line every time
 and avoid mess of attention. * The sections placed to right but not in the same
 line as command and it allows you to copy the command and output without
 environmental disclosure. * Full customization. Change colors, add sections
 with info you need easily with Python. ## Install ```python xpip install -
 U xontrib-prompt-bar echo 'xontrib load prompt_bar' >> ~/.xonshrc # Reload
 xonsh ``` ## Default theme ```python $XONTRIB_PROMPT_BAR_THEME = { 'left': '
-{hostname}{user}{cwd_abs#accent}', 'right': '{curr_branch#section}
-{env_name#strip_brackets#section}{date_time_tz}', 'bar_bg': '
-{BACKGROUND_#323232}', 'bar_fg': '{#AAA}', 'section_bg': '{BACKGROUND_#444}',
-'section_fg': '{#CCC}', 'accent_fg': '{BOLD_#DDD}', } xontrib load prompt_bar
-``` ## Use cases ### Customize the fields Supported fields: * [xonsh default
-fields and colors notation](https://xon.sh/tutorial.html#customizing-the-
-prompt) * `screens` - list of the windows that created by [screen window
-manager](https://www.gnu.org/software/screen/manual/screen.html#Overview) i.e.
-`screen -S mywin`. * `cwd_abs` - current absolute path (`~` disabled). *
-`date_time_tz` - date and time with timezone i.e. `21-12-25 18:00:00-01`. To
+{hostname}{user}{cwd_abs#accent}', 'right': '{hist_status#section}
+{curr_branch#section}{env_name#strip_brackets#section}{date_time_tz}',
+'bar_bg': '{BACKGROUND_#323232}', 'bar_fg': '{#AAA}', 'section_bg': '
+{BACKGROUND_#444}', 'section_fg': '{#CCC}', 'accent_fg': '{BOLD_#DDD}', }
+xontrib load prompt_bar ``` ## Use cases ### Customize the fields Supported
+fields: * [xonsh default fields and colors notation](https://xon.sh/
+tutorial.html#customizing-the-prompt) * `screens` - list of the windows that
+created by [screen window manager](https://www.gnu.org/software/screen/manual/
+screen.html#Overview) i.e. `screen -S mywin`. * `cwd_abs` - current absolute
+path (`~` disabled). * `date_time_tz` - date and time with timezone i.e. `21-
+12-25 18:00:00-01`. * `hist_status` - show `hist off` if history disabled by
+[`history off`](https://xon.sh/tutorial_hist.html#off-action) command. To
 customize the appearance of the fields on the bar you can use wrappers and
 chaining them: ```python $XONTRIB_PROMPT_BAR_RIGHT = '{hostname#accent#section}
 {date_time_tz#nocolorx}' xontrib load prompt_bar ``` Builtin wrappers: *
 `section` - add backlight for the text. * `accent` - bold font and lighter
 color. * `noesc` - remove the ANSI escape characters (colors). * `strip` -
 remove the white spaces in the begin and end. * `strip_brackets` - remove the
 white spaces in the begin and end and then remove the brackets `()[]{}` if the
@@ -71,31 +73,32 @@
 $XONTRIB_PROMPT_BAR_RIGHT = '{starship_right#noesc#nonl#strip}' xontrib load
 prompt_starship prompt_bar ``` Result: [Prompt bar with starship sections.] ###
 Using [xontrib-cmd-durations](https://github.com/jnoortheen/xontrib-cmd-
 durations) The [xontrib-cmd-durations](https://github.com/jnoortheen/xontrib-
 cmd-durations) is to send notification once long-running command is finished
 and also show the execution time. Usage example: ```python # Add `
 {long_cmd_duration}` section $XONTRIB_PROMPT_BAR_RIGHT = '{long_cmd_duration}
-{screens#section}{env_name#strip_brackets#section}{date_time_tz}' xontrib load
-cmd_done ``` ### Hide return code in special cases Sometimes it's needed to
-hide the return code. In this case you can use `-8888` return code i.e.: ```xsh
-aliases['cdls'] = "cd @($arg0) && @(lambda: -8888 if len(g`./*`) > 100 else 0)
-&& ls --group-directories-first -A --color" cdls / # return code is 0 and `ls`
-command was executed and return code is not shown cdls /usr/sbin # return code
-is -8888 and `ls` command was NOT executed and return code is not shown ``` ###
-Additional links * [Asynchronous section rendering](https://xon.sh/
-envvars.html#enable-async-prompt) * [xonsh default fields and colors notation]
-(https://xon.sh/tutorial.html#customizing-the-prompt) * [Meaning of git status
-symbols](https://xon.sh/envvars.html#xonsh-gitstatus) (âÃ+ââââ) *
-[Awesome example of rewriting the theme from Jonathan Slenders](https://
-github.com/prompt-toolkit/python-prompt-toolkit/blob/master/examples/prompts/
-fancy-zsh-prompt.py) * [Customization the colors in the input line](https://
-github.com/xonsh/xonsh/pull/3878#issuecomment-707982828) ## Environment
-variables * `$XONTRIB_PROMPT_BAR_SHOW_RETURN = True` - show return code. ##
-Known issues ### Spaces in the copied and pasted command line Please update
-[prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit) to
-3.0.7+ version via `python -m pip install -U prompt_toolkit`. ## Credits * This
-package is the part of [rc-awesome](https://github.com/anki-code/xontrib-rc-
-awesome) - awesome snippets of code for xonshrc in xonsh shell. * This package
-is the part of [ergopack](https://github.com/anki-code/xontrib-ergopack) - the
-pack of ergonomic xontribs. * This package was created with [xontrib
-cookiecutter template](https://github.com/xonsh/xontrib-cookiecutter).
+{curr_branch#section}{screens#section}{env_name#strip_brackets#section}
+{date_time_tz}' xontrib load cmd_done ``` ### Hide return code in special cases
+Sometimes it's needed to hide the return code. In this case you can use `-8888`
+return code i.e.: ```xsh aliases['cdls'] = "cd @($arg0) && @(lambda: -8888 if
+len(g`./*`) > 100 else 0) && ls --group-directories-first -A --color" cdls / #
+return code is 0 and `ls` command was executed and return code is not shown
+cdls /usr/sbin # return code is -8888 and `ls` command was NOT executed and
+return code is not shown ``` ### Additional links * [Asynchronous section
+rendering](https://xon.sh/envvars.html#enable-async-prompt) * [xonsh default
+fields and colors notation](https://xon.sh/tutorial.html#customizing-the-
+prompt) * [Meaning of git status symbols](https://xon.sh/envvars.html#xonsh-
+gitstatus) (âÃ+ââââ) * [Awesome example of rewriting the theme from
+Jonathan Slenders](https://github.com/prompt-toolkit/python-prompt-toolkit/
+blob/master/examples/prompts/fancy-zsh-prompt.py) * [Customization the colors
+in the input line](https://github.com/xonsh/xonsh/pull/3878#issuecomment-
+707982828) ## Environment variables * `$XONTRIB_PROMPT_BAR_SHOW_RETURN` - show
+return code. Default `True`. ## Known issues ### Spaces in the copied and
+pasted command line Please update [prompt_toolkit](https://github.com/prompt-
+toolkit/python-prompt-toolkit) to 3.0.7+ version via `python -m pip install -
+U prompt_toolkit`. ## Credits * This package is the part of [rc-awesome](https:
+//github.com/anki-code/xontrib-rc-awesome) - awesome snippets of code for
+xonshrc in xonsh shell. * This package is the part of [ergopack](https://
+github.com/anki-code/xontrib-ergopack) - the pack of ergonomic xontribs. * This
+package was created with [xontrib cookiecutter template](https://github.com/
+xonsh/xontrib-cookiecutter).
```

### Comparing `xontrib-prompt-bar-0.5.5/README.md` & `xontrib-prompt-bar-0.5.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ```
 
 ## Default theme
 
 ```python
 $XONTRIB_PROMPT_BAR_THEME = {
     'left': '{hostname}{user}{cwd_abs#accent}',
-    'right': '{curr_branch#section}{env_name#strip_brackets#section}{date_time_tz}',
+    'right': '{hist_status#section}{curr_branch#section}{env_name#strip_brackets#section}{date_time_tz}',
     'bar_bg': '{BACKGROUND_#323232}',
     'bar_fg': '{#AAA}',
     'section_bg': '{BACKGROUND_#444}',
     'section_fg': '{#CCC}',
     'accent_fg': '{BOLD_#DDD}',
 }
 xontrib load prompt_bar
@@ -51,14 +51,15 @@
 ### Customize the fields
 
 Supported fields:
 * [xonsh default fields and colors notation](https://xon.sh/tutorial.html#customizing-the-prompt)
 * `screens` - list of the windows that created by [screen window manager](https://www.gnu.org/software/screen/manual/screen.html#Overview) i.e. `screen -S mywin`.
 * `cwd_abs` - current absolute path (`~` disabled).
 * `date_time_tz` - date and time with timezone i.e. `21-12-25 18:00:00-01`.
+* `hist_status` - show `hist off` if history disabled by [`history off`](https://xon.sh/tutorial_hist.html#off-action) command.
 
 To customize the appearance of the fields on the bar you can use wrappers and chaining them:
 ```python
 $XONTRIB_PROMPT_BAR_RIGHT = '{hostname#accent#section} {date_time_tz#nocolorx}'
 xontrib load prompt_bar
 ```
 Builtin wrappers:
@@ -136,15 +137,15 @@
 
 ### Using [xontrib-cmd-durations](https://github.com/jnoortheen/xontrib-cmd-durations)
 
 The [xontrib-cmd-durations](https://github.com/jnoortheen/xontrib-cmd-durations) is to send notification once long-running command is finished and also show the execution time. Usage example:
 
 ```python
 # Add `{long_cmd_duration}` section
-$XONTRIB_PROMPT_BAR_RIGHT = '{long_cmd_duration}{screens#section}{env_name#strip_brackets#section}{date_time_tz}'
+$XONTRIB_PROMPT_BAR_RIGHT = '{long_cmd_duration}{curr_branch#section}{screens#section}{env_name#strip_brackets#section}{date_time_tz}'
 xontrib load cmd_done
 ```
 
 ### Hide return code in special cases
 
 Sometimes it's needed to hide the return code. In this case you can use `-8888` return code i.e.:
 
@@ -161,15 +162,15 @@
 * [xonsh default fields and colors notation](https://xon.sh/tutorial.html#customizing-the-prompt)
 * [Meaning of git status symbols](https://xon.sh/envvars.html#xonsh-gitstatus) (●×+⚑✓↑↓)
 * [Awesome example of rewriting the theme from Jonathan Slenders](https://github.com/prompt-toolkit/python-prompt-toolkit/blob/master/examples/prompts/fancy-zsh-prompt.py)
 * [Customization the colors in the input line](https://github.com/xonsh/xonsh/pull/3878#issuecomment-707982828)
 
 ## Environment variables
 
-* `$XONTRIB_PROMPT_BAR_SHOW_RETURN = True` - show return code.
+* `$XONTRIB_PROMPT_BAR_SHOW_RETURN` - show return code. Default `True`.
 
 ## Known issues
 ### Spaces in the copied and pasted command line
 Please update [prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit) 
 to 3.0.7+ version via `python -m pip install -U prompt_toolkit`.
 
 ## Credits
```

#### html2text {}

```diff
@@ -7,24 +7,26 @@
 command beginning has fixed position to have a large command line every time
 and avoid mess of attention. * The sections placed to right but not in the same
 line as command and it allows you to copy the command and output without
 environmental disclosure. * Full customization. Change colors, add sections
 with info you need easily with Python. ## Install ```python xpip install -
 U xontrib-prompt-bar echo 'xontrib load prompt_bar' >> ~/.xonshrc # Reload
 xonsh ``` ## Default theme ```python $XONTRIB_PROMPT_BAR_THEME = { 'left': '
-{hostname}{user}{cwd_abs#accent}', 'right': '{curr_branch#section}
-{env_name#strip_brackets#section}{date_time_tz}', 'bar_bg': '
-{BACKGROUND_#323232}', 'bar_fg': '{#AAA}', 'section_bg': '{BACKGROUND_#444}',
-'section_fg': '{#CCC}', 'accent_fg': '{BOLD_#DDD}', } xontrib load prompt_bar
-``` ## Use cases ### Customize the fields Supported fields: * [xonsh default
-fields and colors notation](https://xon.sh/tutorial.html#customizing-the-
-prompt) * `screens` - list of the windows that created by [screen window
-manager](https://www.gnu.org/software/screen/manual/screen.html#Overview) i.e.
-`screen -S mywin`. * `cwd_abs` - current absolute path (`~` disabled). *
-`date_time_tz` - date and time with timezone i.e. `21-12-25 18:00:00-01`. To
+{hostname}{user}{cwd_abs#accent}', 'right': '{hist_status#section}
+{curr_branch#section}{env_name#strip_brackets#section}{date_time_tz}',
+'bar_bg': '{BACKGROUND_#323232}', 'bar_fg': '{#AAA}', 'section_bg': '
+{BACKGROUND_#444}', 'section_fg': '{#CCC}', 'accent_fg': '{BOLD_#DDD}', }
+xontrib load prompt_bar ``` ## Use cases ### Customize the fields Supported
+fields: * [xonsh default fields and colors notation](https://xon.sh/
+tutorial.html#customizing-the-prompt) * `screens` - list of the windows that
+created by [screen window manager](https://www.gnu.org/software/screen/manual/
+screen.html#Overview) i.e. `screen -S mywin`. * `cwd_abs` - current absolute
+path (`~` disabled). * `date_time_tz` - date and time with timezone i.e. `21-
+12-25 18:00:00-01`. * `hist_status` - show `hist off` if history disabled by
+[`history off`](https://xon.sh/tutorial_hist.html#off-action) command. To
 customize the appearance of the fields on the bar you can use wrappers and
 chaining them: ```python $XONTRIB_PROMPT_BAR_RIGHT = '{hostname#accent#section}
 {date_time_tz#nocolorx}' xontrib load prompt_bar ``` Builtin wrappers: *
 `section` - add backlight for the text. * `accent` - bold font and lighter
 color. * `noesc` - remove the ANSI escape characters (colors). * `strip` -
 remove the white spaces in the begin and end. * `strip_brackets` - remove the
 white spaces in the begin and end and then remove the brackets `()[]{}` if the
@@ -58,31 +60,32 @@
 $XONTRIB_PROMPT_BAR_RIGHT = '{starship_right#noesc#nonl#strip}' xontrib load
 prompt_starship prompt_bar ``` Result: [Prompt bar with starship sections.] ###
 Using [xontrib-cmd-durations](https://github.com/jnoortheen/xontrib-cmd-
 durations) The [xontrib-cmd-durations](https://github.com/jnoortheen/xontrib-
 cmd-durations) is to send notification once long-running command is finished
 and also show the execution time. Usage example: ```python # Add `
 {long_cmd_duration}` section $XONTRIB_PROMPT_BAR_RIGHT = '{long_cmd_duration}
-{screens#section}{env_name#strip_brackets#section}{date_time_tz}' xontrib load
-cmd_done ``` ### Hide return code in special cases Sometimes it's needed to
-hide the return code. In this case you can use `-8888` return code i.e.: ```xsh
-aliases['cdls'] = "cd @($arg0) && @(lambda: -8888 if len(g`./*`) > 100 else 0)
-&& ls --group-directories-first -A --color" cdls / # return code is 0 and `ls`
-command was executed and return code is not shown cdls /usr/sbin # return code
-is -8888 and `ls` command was NOT executed and return code is not shown ``` ###
-Additional links * [Asynchronous section rendering](https://xon.sh/
-envvars.html#enable-async-prompt) * [xonsh default fields and colors notation]
-(https://xon.sh/tutorial.html#customizing-the-prompt) * [Meaning of git status
-symbols](https://xon.sh/envvars.html#xonsh-gitstatus) (âÃ+ââââ) *
-[Awesome example of rewriting the theme from Jonathan Slenders](https://
-github.com/prompt-toolkit/python-prompt-toolkit/blob/master/examples/prompts/
-fancy-zsh-prompt.py) * [Customization the colors in the input line](https://
-github.com/xonsh/xonsh/pull/3878#issuecomment-707982828) ## Environment
-variables * `$XONTRIB_PROMPT_BAR_SHOW_RETURN = True` - show return code. ##
-Known issues ### Spaces in the copied and pasted command line Please update
-[prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit) to
-3.0.7+ version via `python -m pip install -U prompt_toolkit`. ## Credits * This
-package is the part of [rc-awesome](https://github.com/anki-code/xontrib-rc-
-awesome) - awesome snippets of code for xonshrc in xonsh shell. * This package
-is the part of [ergopack](https://github.com/anki-code/xontrib-ergopack) - the
-pack of ergonomic xontribs. * This package was created with [xontrib
-cookiecutter template](https://github.com/xonsh/xontrib-cookiecutter).
+{curr_branch#section}{screens#section}{env_name#strip_brackets#section}
+{date_time_tz}' xontrib load cmd_done ``` ### Hide return code in special cases
+Sometimes it's needed to hide the return code. In this case you can use `-8888`
+return code i.e.: ```xsh aliases['cdls'] = "cd @($arg0) && @(lambda: -8888 if
+len(g`./*`) > 100 else 0) && ls --group-directories-first -A --color" cdls / #
+return code is 0 and `ls` command was executed and return code is not shown
+cdls /usr/sbin # return code is -8888 and `ls` command was NOT executed and
+return code is not shown ``` ### Additional links * [Asynchronous section
+rendering](https://xon.sh/envvars.html#enable-async-prompt) * [xonsh default
+fields and colors notation](https://xon.sh/tutorial.html#customizing-the-
+prompt) * [Meaning of git status symbols](https://xon.sh/envvars.html#xonsh-
+gitstatus) (âÃ+ââââ) * [Awesome example of rewriting the theme from
+Jonathan Slenders](https://github.com/prompt-toolkit/python-prompt-toolkit/
+blob/master/examples/prompts/fancy-zsh-prompt.py) * [Customization the colors
+in the input line](https://github.com/xonsh/xonsh/pull/3878#issuecomment-
+707982828) ## Environment variables * `$XONTRIB_PROMPT_BAR_SHOW_RETURN` - show
+return code. Default `True`. ## Known issues ### Spaces in the copied and
+pasted command line Please update [prompt_toolkit](https://github.com/prompt-
+toolkit/python-prompt-toolkit) to 3.0.7+ version via `python -m pip install -
+U prompt_toolkit`. ## Credits * This package is the part of [rc-awesome](https:
+//github.com/anki-code/xontrib-rc-awesome) - awesome snippets of code for
+xonshrc in xonsh shell. * This package is the part of [ergopack](https://
+github.com/anki-code/xontrib-ergopack) - the pack of ergonomic xontribs. * This
+package was created with [xontrib cookiecutter template](https://github.com/
+xonsh/xontrib-cookiecutter).
```

### Comparing `xontrib-prompt-bar-0.5.5/setup.py` & `xontrib-prompt-bar-0.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 except (IOError, OSError):
     long_description = ''
 
 setup(
     name='xontrib-prompt-bar',
-    version='0.5.5',
+    version='0.5.6',
     license='BSD',
     author='anki',
     author_email='author@example.com',
     description="The bar theme for xonsh shell.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
```

### Comparing `xontrib-prompt-bar-0.5.5/xontrib/prompt_bar.py` & `xontrib-prompt-bar-0.5.6/xontrib/prompt_bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """
 Themes:
  * Supported colors: https://xon.sh/tutorial.html#customizing-the-prompt
 """
 _pb_themes = {
     'default': {
         'left': '{hostname}{user}{cwd_abs#accent}',
-        'right': '{curr_branch#section}{env_name#strip#strip_brackets#section}{date_time_tz}',
+        'right': '{hist_status#section}{curr_branch#section}{env_name#strip#strip_brackets#section}{date_time_tz}',
         'bar_bg': '{BACKGROUND_#323232}',
         'bar_fg': '{#AAA}',
         'section_bg': '{BACKGROUND_#444}',
         'section_fg': '{#CCC}',
         'accent_fg': '{BOLD_#DDD}',
     }
 }
@@ -61,14 +61,16 @@
 def _field_date_time_tz():
     t = time.strftime('%y-%m-%d %H:%M:%S%z', time.localtime())
     return t[:-2] if t[-2:] == '00' else t
 
 __xonsh__.env['PROMPT_FIELDS']['prompt_end_xonsh'] = "#" if is_superuser() else "@"
 __xonsh__.env['PROMPT_FIELDS']['cwd_abs'] = lambda: str(Path(__xonsh__.env['PROMPT_FIELDS']['cwd']()).expanduser())
 __xonsh__.env['PROMPT_FIELDS']['date_time_tz'] = _field_date_time_tz
+__xonsh__.env['PROMPT_FIELDS']['hist_status'] = lambda: '' if __xonsh__.history.remember_history else 'hist off'
+
 
 def _screens():
     line = []
     sty = None
     for l in __xonsh__.subproc_captured_stdout(['bash', '-c', 'screen -ls; exit 0']).splitlines():  # bash is to fix https://github.com/xonsh/xonsh/issues/4912 
         if '\t' in l:
             screen_name = l.split('\t')[1].split('.')[1]
```

### Comparing `xontrib-prompt-bar-0.5.5/xontrib_prompt_bar.egg-info/PKG-INFO` & `xontrib-prompt-bar-0.5.6/xontrib_prompt_bar.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-prompt-bar
-Version: 0.5.5
+Version: 0.5.6
 Summary: The bar theme for xonsh shell.
 Home-page: https://github.com/anki-code/xontrib-prompt-bar
 Author: anki
 Author-email: author@example.com
 License: BSD
 Project-URL: Documentation, https://github.com/anki-code/xontrib-prompt-bar/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xontrib-prompt-bar
@@ -58,15 +58,15 @@
 ```
 
 ## Default theme
 
 ```python
 $XONTRIB_PROMPT_BAR_THEME = {
     'left': '{hostname}{user}{cwd_abs#accent}',
-    'right': '{curr_branch#section}{env_name#strip_brackets#section}{date_time_tz}',
+    'right': '{hist_status#section}{curr_branch#section}{env_name#strip_brackets#section}{date_time_tz}',
     'bar_bg': '{BACKGROUND_#323232}',
     'bar_fg': '{#AAA}',
     'section_bg': '{BACKGROUND_#444}',
     'section_fg': '{#CCC}',
     'accent_fg': '{BOLD_#DDD}',
 }
 xontrib load prompt_bar
@@ -77,14 +77,15 @@
 ### Customize the fields
 
 Supported fields:
 * [xonsh default fields and colors notation](https://xon.sh/tutorial.html#customizing-the-prompt)
 * `screens` - list of the windows that created by [screen window manager](https://www.gnu.org/software/screen/manual/screen.html#Overview) i.e. `screen -S mywin`.
 * `cwd_abs` - current absolute path (`~` disabled).
 * `date_time_tz` - date and time with timezone i.e. `21-12-25 18:00:00-01`.
+* `hist_status` - show `hist off` if history disabled by [`history off`](https://xon.sh/tutorial_hist.html#off-action) command.
 
 To customize the appearance of the fields on the bar you can use wrappers and chaining them:
 ```python
 $XONTRIB_PROMPT_BAR_RIGHT = '{hostname#accent#section} {date_time_tz#nocolorx}'
 xontrib load prompt_bar
 ```
 Builtin wrappers:
@@ -162,15 +163,15 @@
 
 ### Using [xontrib-cmd-durations](https://github.com/jnoortheen/xontrib-cmd-durations)
 
 The [xontrib-cmd-durations](https://github.com/jnoortheen/xontrib-cmd-durations) is to send notification once long-running command is finished and also show the execution time. Usage example:
 
 ```python
 # Add `{long_cmd_duration}` section
-$XONTRIB_PROMPT_BAR_RIGHT = '{long_cmd_duration}{screens#section}{env_name#strip_brackets#section}{date_time_tz}'
+$XONTRIB_PROMPT_BAR_RIGHT = '{long_cmd_duration}{curr_branch#section}{screens#section}{env_name#strip_brackets#section}{date_time_tz}'
 xontrib load cmd_done
 ```
 
 ### Hide return code in special cases
 
 Sometimes it's needed to hide the return code. In this case you can use `-8888` return code i.e.:
 
@@ -187,15 +188,15 @@
 * [xonsh default fields and colors notation](https://xon.sh/tutorial.html#customizing-the-prompt)
 * [Meaning of git status symbols](https://xon.sh/envvars.html#xonsh-gitstatus) (●×+⚑✓↑↓)
 * [Awesome example of rewriting the theme from Jonathan Slenders](https://github.com/prompt-toolkit/python-prompt-toolkit/blob/master/examples/prompts/fancy-zsh-prompt.py)
 * [Customization the colors in the input line](https://github.com/xonsh/xonsh/pull/3878#issuecomment-707982828)
 
 ## Environment variables
 
-* `$XONTRIB_PROMPT_BAR_SHOW_RETURN = True` - show return code.
+* `$XONTRIB_PROMPT_BAR_SHOW_RETURN` - show return code. Default `True`.
 
 ## Known issues
 ### Spaces in the copied and pasted command line
 Please update [prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit) 
 to 3.0.7+ version via `python -m pip install -U prompt_toolkit`.
 
 ## Credits
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xontrib-prompt-bar Version: 0.5.5 Summary: The bar
+Metadata-Version: 2.1 Name: xontrib-prompt-bar Version: 0.5.6 Summary: The bar
 theme for xonsh shell. Home-page: https://github.com/anki-code/xontrib-prompt-
 bar Author: anki Author-email: author@example.com License: BSD Project-URL:
 Documentation, https://github.com/anki-code/xontrib-prompt-bar/blob/master/
 README.md Project-URL: Code, https://github.com/anki-code/xontrib-prompt-bar
 Project-URL: Issue tracker, https://github.com/anki-code/xontrib-prompt-bar/
 issues Platform: any Classifier: Environment :: Console Classifier: Intended
 Audience :: End Users/Desktop Classifier: Operating System :: OS Independent
@@ -20,24 +20,26 @@
 command beginning has fixed position to have a large command line every time
 and avoid mess of attention. * The sections placed to right but not in the same
 line as command and it allows you to copy the command and output without
 environmental disclosure. * Full customization. Change colors, add sections
 with info you need easily with Python. ## Install ```python xpip install -
 U xontrib-prompt-bar echo 'xontrib load prompt_bar' >> ~/.xonshrc # Reload
 xonsh ``` ## Default theme ```python $XONTRIB_PROMPT_BAR_THEME = { 'left': '
-{hostname}{user}{cwd_abs#accent}', 'right': '{curr_branch#section}
-{env_name#strip_brackets#section}{date_time_tz}', 'bar_bg': '
-{BACKGROUND_#323232}', 'bar_fg': '{#AAA}', 'section_bg': '{BACKGROUND_#444}',
-'section_fg': '{#CCC}', 'accent_fg': '{BOLD_#DDD}', } xontrib load prompt_bar
-``` ## Use cases ### Customize the fields Supported fields: * [xonsh default
-fields and colors notation](https://xon.sh/tutorial.html#customizing-the-
-prompt) * `screens` - list of the windows that created by [screen window
-manager](https://www.gnu.org/software/screen/manual/screen.html#Overview) i.e.
-`screen -S mywin`. * `cwd_abs` - current absolute path (`~` disabled). *
-`date_time_tz` - date and time with timezone i.e. `21-12-25 18:00:00-01`. To
+{hostname}{user}{cwd_abs#accent}', 'right': '{hist_status#section}
+{curr_branch#section}{env_name#strip_brackets#section}{date_time_tz}',
+'bar_bg': '{BACKGROUND_#323232}', 'bar_fg': '{#AAA}', 'section_bg': '
+{BACKGROUND_#444}', 'section_fg': '{#CCC}', 'accent_fg': '{BOLD_#DDD}', }
+xontrib load prompt_bar ``` ## Use cases ### Customize the fields Supported
+fields: * [xonsh default fields and colors notation](https://xon.sh/
+tutorial.html#customizing-the-prompt) * `screens` - list of the windows that
+created by [screen window manager](https://www.gnu.org/software/screen/manual/
+screen.html#Overview) i.e. `screen -S mywin`. * `cwd_abs` - current absolute
+path (`~` disabled). * `date_time_tz` - date and time with timezone i.e. `21-
+12-25 18:00:00-01`. * `hist_status` - show `hist off` if history disabled by
+[`history off`](https://xon.sh/tutorial_hist.html#off-action) command. To
 customize the appearance of the fields on the bar you can use wrappers and
 chaining them: ```python $XONTRIB_PROMPT_BAR_RIGHT = '{hostname#accent#section}
 {date_time_tz#nocolorx}' xontrib load prompt_bar ``` Builtin wrappers: *
 `section` - add backlight for the text. * `accent` - bold font and lighter
 color. * `noesc` - remove the ANSI escape characters (colors). * `strip` -
 remove the white spaces in the begin and end. * `strip_brackets` - remove the
 white spaces in the begin and end and then remove the brackets `()[]{}` if the
@@ -71,31 +73,32 @@
 $XONTRIB_PROMPT_BAR_RIGHT = '{starship_right#noesc#nonl#strip}' xontrib load
 prompt_starship prompt_bar ``` Result: [Prompt bar with starship sections.] ###
 Using [xontrib-cmd-durations](https://github.com/jnoortheen/xontrib-cmd-
 durations) The [xontrib-cmd-durations](https://github.com/jnoortheen/xontrib-
 cmd-durations) is to send notification once long-running command is finished
 and also show the execution time. Usage example: ```python # Add `
 {long_cmd_duration}` section $XONTRIB_PROMPT_BAR_RIGHT = '{long_cmd_duration}
-{screens#section}{env_name#strip_brackets#section}{date_time_tz}' xontrib load
-cmd_done ``` ### Hide return code in special cases Sometimes it's needed to
-hide the return code. In this case you can use `-8888` return code i.e.: ```xsh
-aliases['cdls'] = "cd @($arg0) && @(lambda: -8888 if len(g`./*`) > 100 else 0)
-&& ls --group-directories-first -A --color" cdls / # return code is 0 and `ls`
-command was executed and return code is not shown cdls /usr/sbin # return code
-is -8888 and `ls` command was NOT executed and return code is not shown ``` ###
-Additional links * [Asynchronous section rendering](https://xon.sh/
-envvars.html#enable-async-prompt) * [xonsh default fields and colors notation]
-(https://xon.sh/tutorial.html#customizing-the-prompt) * [Meaning of git status
-symbols](https://xon.sh/envvars.html#xonsh-gitstatus) (âÃ+ââââ) *
-[Awesome example of rewriting the theme from Jonathan Slenders](https://
-github.com/prompt-toolkit/python-prompt-toolkit/blob/master/examples/prompts/
-fancy-zsh-prompt.py) * [Customization the colors in the input line](https://
-github.com/xonsh/xonsh/pull/3878#issuecomment-707982828) ## Environment
-variables * `$XONTRIB_PROMPT_BAR_SHOW_RETURN = True` - show return code. ##
-Known issues ### Spaces in the copied and pasted command line Please update
-[prompt_toolkit](https://github.com/prompt-toolkit/python-prompt-toolkit) to
-3.0.7+ version via `python -m pip install -U prompt_toolkit`. ## Credits * This
-package is the part of [rc-awesome](https://github.com/anki-code/xontrib-rc-
-awesome) - awesome snippets of code for xonshrc in xonsh shell. * This package
-is the part of [ergopack](https://github.com/anki-code/xontrib-ergopack) - the
-pack of ergonomic xontribs. * This package was created with [xontrib
-cookiecutter template](https://github.com/xonsh/xontrib-cookiecutter).
+{curr_branch#section}{screens#section}{env_name#strip_brackets#section}
+{date_time_tz}' xontrib load cmd_done ``` ### Hide return code in special cases
+Sometimes it's needed to hide the return code. In this case you can use `-8888`
+return code i.e.: ```xsh aliases['cdls'] = "cd @($arg0) && @(lambda: -8888 if
+len(g`./*`) > 100 else 0) && ls --group-directories-first -A --color" cdls / #
+return code is 0 and `ls` command was executed and return code is not shown
+cdls /usr/sbin # return code is -8888 and `ls` command was NOT executed and
+return code is not shown ``` ### Additional links * [Asynchronous section
+rendering](https://xon.sh/envvars.html#enable-async-prompt) * [xonsh default
+fields and colors notation](https://xon.sh/tutorial.html#customizing-the-
+prompt) * [Meaning of git status symbols](https://xon.sh/envvars.html#xonsh-
+gitstatus) (âÃ+ââââ) * [Awesome example of rewriting the theme from
+Jonathan Slenders](https://github.com/prompt-toolkit/python-prompt-toolkit/
+blob/master/examples/prompts/fancy-zsh-prompt.py) * [Customization the colors
+in the input line](https://github.com/xonsh/xonsh/pull/3878#issuecomment-
+707982828) ## Environment variables * `$XONTRIB_PROMPT_BAR_SHOW_RETURN` - show
+return code. Default `True`. ## Known issues ### Spaces in the copied and
+pasted command line Please update [prompt_toolkit](https://github.com/prompt-
+toolkit/python-prompt-toolkit) to 3.0.7+ version via `python -m pip install -
+U prompt_toolkit`. ## Credits * This package is the part of [rc-awesome](https:
+//github.com/anki-code/xontrib-rc-awesome) - awesome snippets of code for
+xonshrc in xonsh shell. * This package is the part of [ergopack](https://
+github.com/anki-code/xontrib-ergopack) - the pack of ergonomic xontribs. * This
+package was created with [xontrib cookiecutter template](https://github.com/
+xonsh/xontrib-cookiecutter).
```

