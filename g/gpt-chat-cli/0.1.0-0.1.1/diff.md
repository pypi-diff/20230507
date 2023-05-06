# Comparing `tmp/gpt-chat-cli-0.1.0.tar.gz` & `tmp/gpt-chat-cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-chat-cli-0.1.0.tar", last modified: Sat May  6 21:46:14 2023, max compression
+gzip compressed data, was "gpt-chat-cli-0.1.1.tar", last modified: Sat May  6 22:06:28 2023, max compression
```

## Comparing `gpt-chat-cli-0.1.0.tar` & `gpt-chat-cli-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 21:46:14.234665 gpt-chat-cli-0.1.0/
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     1052 2023-05-04 23:39:54.000000 gpt-chat-cli-0.1.0/LICENSE
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10547 2023-05-06 21:46:14.234665 gpt-chat-cli-0.1.0/PKG-INFO
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10018 2023-05-06 21:42:48.000000 gpt-chat-cli-0.1.0/README.md
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      587 2023-05-06 10:51:01.000000 gpt-chat-cli-0.1.0/pyproject.toml
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       38 2023-05-06 21:46:14.234665 gpt-chat-cli-0.1.0/setup.cfg
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      441 2023-05-06 10:51:17.000000 gpt-chat-cli-0.1.0/setup.py
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 21:46:14.231331 gpt-chat-cli-0.1.0/src/
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 21:46:14.231331 gpt-chat-cli-0.1.0/src/gpt_chat_cli/
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-05 05:27:20.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/__init__.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10360 2023-05-06 20:06:24.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/argparsing.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     5690 2023-05-06 10:40:40.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/chat_colorizer.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     1979 2023-05-06 19:56:25.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/color.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     8587 2023-05-06 19:57:38.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/gcli.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     2873 2023-05-06 21:24:43.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/openai_wrappers.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     9556 2023-05-06 10:41:58.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/streaming_lexer.py
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       18 2023-05-06 10:50:51.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli/version.py
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 21:46:14.234665 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10547 2023-05-06 21:46:14.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/PKG-INFO
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      559 2023-05-06 21:46:14.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/SOURCES.txt
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)        1 2023-05-06 21:46:14.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/dependency_links.txt
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       56 2023-05-06 21:46:14.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/entry_points.txt
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       43 2023-05-06 21:46:14.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/requires.txt
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       13 2023-05-06 21:46:14.000000 gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/top_level.txt
-drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 21:46:14.234665 gpt-chat-cli-0.1.0/tests/
--rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     5409 2023-05-06 07:11:24.000000 gpt-chat-cli-0.1.0/tests/test_streaming_lexer.py
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 22:06:28.691866 gpt-chat-cli-0.1.1/
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     1052 2023-05-04 23:39:54.000000 gpt-chat-cli-0.1.1/LICENSE
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10705 2023-05-06 22:06:28.691866 gpt-chat-cli-0.1.1/PKG-INFO
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10176 2023-05-06 22:03:39.000000 gpt-chat-cli-0.1.1/README.md
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      587 2023-05-06 22:05:07.000000 gpt-chat-cli-0.1.1/pyproject.toml
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       38 2023-05-06 22:06:28.691866 gpt-chat-cli-0.1.1/setup.cfg
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      441 2023-05-06 22:05:13.000000 gpt-chat-cli-0.1.1/setup.py
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 22:06:28.688532 gpt-chat-cli-0.1.1/src/
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 22:06:28.688532 gpt-chat-cli-0.1.1/src/gpt_chat_cli/
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-05 05:27:20.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/__init__.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10360 2023-05-06 20:06:24.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/argparsing.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     5690 2023-05-06 10:40:40.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/chat_colorizer.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     1979 2023-05-06 19:56:25.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/color.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     8587 2023-05-06 19:57:38.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/gcli.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     2873 2023-05-06 21:24:43.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/openai_wrappers.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     9556 2023-05-06 10:41:58.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/streaming_lexer.py
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       18 2023-05-06 22:05:24.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli/version.py
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 22:06:28.691866 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)    10705 2023-05-06 22:06:28.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/PKG-INFO
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)      559 2023-05-06 22:06:28.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)        1 2023-05-06 22:06:28.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       56 2023-05-06 22:06:28.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/entry_points.txt
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       43 2023-05-06 22:06:28.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/requires.txt
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)       13 2023-05-06 22:06:28.000000 gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/top_level.txt
+drwxr-xr-x   0 flu0r1ne  (1000) flu0r1ne  (1000)        0 2023-05-06 22:06:28.691866 gpt-chat-cli-0.1.1/tests/
+-rw-r--r--   0 flu0r1ne  (1000) flu0r1ne  (1000)     5409 2023-05-06 07:11:24.000000 gpt-chat-cli-0.1.1/tests/test_streaming_lexer.py
```

### Comparing `gpt-chat-cli-0.1.0/LICENSE` & `gpt-chat-cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.0/PKG-INFO` & `gpt-chat-cli-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-chat-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple ChatGPT terminal CLI
 Author: Flu0r1ne
 Author-email: Flu0r1ne <flu0r1ne@flu0r1ne.net>
 Project-URL: Homepage, https://github.com/flu0r1ne/gpt-chat-cli
 Project-URL: Bug Tracker, https://github.com/flu0r1ne/gpt-chat-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,71 +12,71 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 gpt-chat-cli: a simple yet powerful ChatGPT CLI
 -----------------------------------------------
 
-## Intro
+## Introduction
 
-`gpt-chat-cli` is a simple, general purpose ChatGPT CLI. It brings the power of ChatGPT to the command line. It aims to be easy to use and configurable.
+`gpt-chat-cli` is a simple, general purpose ChatGPT CLI. It brings the power of ChatGPT to the command line. It aims to be easy to use and highly configurable.
 
 Some of the features include:
-- Streaming, real-time output
-- Interactive sessions with color and adornments
-- Support for any model which can be called through OpenAI's chat completions API.
+- Streaming, real-time output.
+- Interactive sessions with color and adornments.
+- Support for any model that can be called through OpenAI's chat completions API.
   [See model endpoint compatibility.](https://platform.openai.com/docs/models/model-endpoint-compatibility)
-- Modify model parameters including temperature, frequency penalty, presence penalty, top p, and the maximum number of tokens emitted
-- Dynamic code syntax highlighting
-- List available models
-- Respects unix norms. Input can be gathered from pipes, heredoc, files, and arbitrary file descriptors.
+- Ability to modify model parameters including temperature, frequency penalty, presence penalty, top p, and the maximum number of tokens emitted.
+- Dynamic code syntax highlighting.
+- List the available models.
+- Respects Unix norms. Input can be gathered from pipes, heredoc, files, and arbitrary file descriptors.
 
 ![gpt-chat-cli Completion Demo](./assets/images/gpt.gif)
 
 ### Installation
 
 ```bash
 pip install gpt-chat-cli
 ```
 
-The OpenAI API uses API keys for authentication. Visit your [API Keys page](https://platform.openai.com/account/api-keys) to retrieve the API key you'll use in your requests. 
+The OpenAI API uses API keys for authentication. Visit your [API Keys page](https://platform.openai.com/account/api-keys) to retrieve the API key you'll use in your requests:
 ```bash
 export OPENAI_API_KEY="INSERT_SECRET_KEY"
 ```
 
-Then, source the `OPENAI_API_KEY` environmental variable in your shell's configuration file. (That is, `~/.bashrc` or `~/.zshrc` for the Bash or Zsh shell, respectively.)
+Then, source the `OPENAI_API_KEY` environmental variable in your shell's configuration file. (That is, `~/.bashrc` or `~/.zshrc` for the Bash or Zsh shell, respectively):
 
 ```bash
 source ~/.bashrc
 ```
 
-### User guide
+### User Guide
 
 #### Basic Usage
 
 Without additional arguments, `gpt-chat-cli` will drop the user into an interactive shell:
 
 ```text
 $ gpt-chat-cli
 GPT Chat CLI version 0.1.0
 Press Control-D to exit
 [#] Hello!
 [gpt-3.5-turbo-0301] Hello! How can I assist you today?
 ```
 
-For a single completion, an initial message can be specified as the first positional:
+For a single completion, an initial message can be specified as the first positional argument:
 
 ```text
 $ gpt-chat-cli "In one sentence, who is Joseph Weizenbaum?"
 [gpt-3.5-turbo-0301] Joseph Weizenbaum was a German-American computer scientist
 and philosopher who is known for creating the ELIZA program, one of the first 
 natural language processing programs.
 ```
 
-Or, specify the inital message and drop into an interactive shell with `-i`:
+Alternatively, you can specify the initial message and drop into an interactive shell with `-i`:
 
 ```text
 $ gpt-chat-cli -i "What linux command prints a list of all open TCP sockets on port 8080?"
 GPT Chat CLI version 0.1.0
 Press Control-D to exit
 [#] What linux command prints a list of all open TCP sockets on port 8080?
 [gpt-3.5-turbo-0301] You can use the `lsof` (list open files) command to list all
@@ -86,15 +86,15 @@
 
 [#] Can do do this with ss?
 [gpt-3.5-turbo-0301] Yes, you can also use the `ss` (socket statistics) command to
 list all open TCP sockets on port 8080. The command to list all open TCP sockets
 on port 8080 using `ss` is `sudo ss -tlnp 'sport = :8080'`
 ```
 
-`gpt-chat-cli` respects pipes and redirects:
+`gpt-chat-cli` respects pipes and redirects, so you can use it in combination with other command-line tools:
 
 ```text
 $ printf "What is smmsp in /etc/group?\n$(cat /etc/group | head)" | gpt-chat-cli
 [gpt-3.5-turbo-0301] `smmsp` is a system user and group used by the Sendmail mail transfer agent (MTA)
 for sending mail. The `smmsp` group is used to provide access to the Sendmail queue directory and
 other Sendmail-related files. Members of this group are allowed to read and write to the Sendmail
 queue directory and other Sendmail-related files.
@@ -112,15 +112,15 @@
     let average = sum / count as i32;
     println!("The average is {}", average);
 }
 
 This code creates a vector of numbers, calculates the sum of the numbers using the `iter()` method and the `sum()` method, counts the number of elements in the vector using the `len()` method, and then calculates the average by dividing the sum by the count. Finally, it prints the average to the console.
 ```
 
-List available models:
+To list all available models, use the following command:
 
 ```text
 $ gpt-chat-cli --list-models
 gpt-3.5-turbo
 gpt-3.5-turbo-0301
 gpt-4
 gpt-4-0314
@@ -176,31 +176,31 @@
 | Environmental Variable | Controls | Default Value |
 | --- | --- | --- |
 | `GPT_CLI_MODEL` | ID of the model to use | "gpt-3.5-turbo" |
 | `GPT_CLI_TEMPERATURE` | Sampling temperature to use, between 0 and 2 | 0.5 |
 | `GPT_CLI_FREQUENCY_PENALTY` | Number between -2.0 and 2.0. Positive values penalize new tokens based on their existing frequency in the text so far | 0 |
 | `GPT_CLI_PRESENCE_PENALTY` | Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the text so far | 0 |
 | `GPT_CLI_MAX_TOKENS` | The maximum number of tokens to generate in the chat completion | 2048 |
-| `GPT_CLI_TOP_P` | An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass | 1 |
+| `GPT_CLI_TOP_P` | An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with `top_p` probability mass | 1 |
 | `GPT_CLI_N_COMPLETIONS` | How many chat completion choices to generate for each input message | 1 |
 | `GPT_CLI_SYSTEM_MESSAGE` | Specify an alternative system message | [See this section](#system-message) |
 
 #### System Message
 
 The default [system message](https://platform.openai.com/docs/guides/chat/instructing-chat-models) is:
 
 ```text
 The current date and time is 2023-05-06 15:55:56.619232. When emitting code or producing markdown, ensure to label fenced code blocks with the language in use.'
 ```
 
-This can be overridden. GPT 3.5 seems to sometime forget to emit labels for fenced code blocks which prevents the syntax highlighting from taking effect. Thus, a reminder in the system message is recommended.
+This can be overridden. GPT 3.5 sometimes forgets to emit labels for fenced code blocks, which prevents the syntax highlighting from taking effect. Thus, a reminder in the system message is recommended.
 
 #### Tricks
 
-You can use heredoc in bash to create a prompt with includes a file:
+You can use heredoc in `bash` to create a prompt with includes a file:
 
 ```text
 $ gpt-chat-cli -i --prompt-from-fd 3 3<<EOF
 heredoc> Can you review this code:
 heredoc> $(cat quicksort.c)
 heredoc> EOF
 [#] Can you review this code:
@@ -219,17 +219,18 @@
 
 1. Naming: The function name `quicksort` is not very descriptive. It would be better to name it something like `quicksort_entries_by_access_time` to make it clear what it does.
 
 ...
 [#]
 ```
 
-#### Known issues
+#### Known Issues
 
 There are a couple known issues. PRs are accepted:
 
 1. `gpt-chat-cli` lacks shell completion
 2. `gpt-chat-cli` does not track token usage. Ideally, it should gracefully handle long messages and remove messages from the chat history if the number of tokens in the context is exceeded. If the tokens exceed the model's context, the following error will occur:
 
 ```text
 openai.error.InvalidRequestError: This model's maximum context length is 4097 tokens. However, your messages resulted in 9758 tokens. Please reduce the length of the messages.
 ```
+
```

### Comparing `gpt-chat-cli-0.1.0/README.md` & `gpt-chat-cli-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 gpt-chat-cli: a simple yet powerful ChatGPT CLI
 -----------------------------------------------
 
-## Intro
+## Introduction
 
-`gpt-chat-cli` is a simple, general purpose ChatGPT CLI. It brings the power of ChatGPT to the command line. It aims to be easy to use and configurable.
+`gpt-chat-cli` is a simple, general purpose ChatGPT CLI. It brings the power of ChatGPT to the command line. It aims to be easy to use and highly configurable.
 
 Some of the features include:
-- Streaming, real-time output
-- Interactive sessions with color and adornments
-- Support for any model which can be called through OpenAI's chat completions API.
+- Streaming, real-time output.
+- Interactive sessions with color and adornments.
+- Support for any model that can be called through OpenAI's chat completions API.
   [See model endpoint compatibility.](https://platform.openai.com/docs/models/model-endpoint-compatibility)
-- Modify model parameters including temperature, frequency penalty, presence penalty, top p, and the maximum number of tokens emitted
-- Dynamic code syntax highlighting
-- List available models
-- Respects unix norms. Input can be gathered from pipes, heredoc, files, and arbitrary file descriptors.
+- Ability to modify model parameters including temperature, frequency penalty, presence penalty, top p, and the maximum number of tokens emitted.
+- Dynamic code syntax highlighting.
+- List the available models.
+- Respects Unix norms. Input can be gathered from pipes, heredoc, files, and arbitrary file descriptors.
 
 ![gpt-chat-cli Completion Demo](./assets/images/gpt.gif)
 
 ### Installation
 
 ```bash
 pip install gpt-chat-cli
 ```
 
-The OpenAI API uses API keys for authentication. Visit your [API Keys page](https://platform.openai.com/account/api-keys) to retrieve the API key you'll use in your requests. 
+The OpenAI API uses API keys for authentication. Visit your [API Keys page](https://platform.openai.com/account/api-keys) to retrieve the API key you'll use in your requests:
 ```bash
 export OPENAI_API_KEY="INSERT_SECRET_KEY"
 ```
 
-Then, source the `OPENAI_API_KEY` environmental variable in your shell's configuration file. (That is, `~/.bashrc` or `~/.zshrc` for the Bash or Zsh shell, respectively.)
+Then, source the `OPENAI_API_KEY` environmental variable in your shell's configuration file. (That is, `~/.bashrc` or `~/.zshrc` for the Bash or Zsh shell, respectively):
 
 ```bash
 source ~/.bashrc
 ```
 
-### User guide
+### User Guide
 
 #### Basic Usage
 
 Without additional arguments, `gpt-chat-cli` will drop the user into an interactive shell:
 
 ```text
 $ gpt-chat-cli
 GPT Chat CLI version 0.1.0
 Press Control-D to exit
 [#] Hello!
 [gpt-3.5-turbo-0301] Hello! How can I assist you today?
 ```
 
-For a single completion, an initial message can be specified as the first positional:
+For a single completion, an initial message can be specified as the first positional argument:
 
 ```text
 $ gpt-chat-cli "In one sentence, who is Joseph Weizenbaum?"
 [gpt-3.5-turbo-0301] Joseph Weizenbaum was a German-American computer scientist
 and philosopher who is known for creating the ELIZA program, one of the first 
 natural language processing programs.
 ```
 
-Or, specify the inital message and drop into an interactive shell with `-i`:
+Alternatively, you can specify the initial message and drop into an interactive shell with `-i`:
 
 ```text
 $ gpt-chat-cli -i "What linux command prints a list of all open TCP sockets on port 8080?"
 GPT Chat CLI version 0.1.0
 Press Control-D to exit
 [#] What linux command prints a list of all open TCP sockets on port 8080?
 [gpt-3.5-turbo-0301] You can use the `lsof` (list open files) command to list all
@@ -71,15 +71,15 @@
 
 [#] Can do do this with ss?
 [gpt-3.5-turbo-0301] Yes, you can also use the `ss` (socket statistics) command to
 list all open TCP sockets on port 8080. The command to list all open TCP sockets
 on port 8080 using `ss` is `sudo ss -tlnp 'sport = :8080'`
 ```
 
-`gpt-chat-cli` respects pipes and redirects:
+`gpt-chat-cli` respects pipes and redirects, so you can use it in combination with other command-line tools:
 
 ```text
 $ printf "What is smmsp in /etc/group?\n$(cat /etc/group | head)" | gpt-chat-cli
 [gpt-3.5-turbo-0301] `smmsp` is a system user and group used by the Sendmail mail transfer agent (MTA)
 for sending mail. The `smmsp` group is used to provide access to the Sendmail queue directory and
 other Sendmail-related files. Members of this group are allowed to read and write to the Sendmail
 queue directory and other Sendmail-related files.
@@ -97,15 +97,15 @@
     let average = sum / count as i32;
     println!("The average is {}", average);
 }
 
 This code creates a vector of numbers, calculates the sum of the numbers using the `iter()` method and the `sum()` method, counts the number of elements in the vector using the `len()` method, and then calculates the average by dividing the sum by the count. Finally, it prints the average to the console.
 ```
 
-List available models:
+To list all available models, use the following command:
 
 ```text
 $ gpt-chat-cli --list-models
 gpt-3.5-turbo
 gpt-3.5-turbo-0301
 gpt-4
 gpt-4-0314
@@ -161,31 +161,31 @@
 | Environmental Variable | Controls | Default Value |
 | --- | --- | --- |
 | `GPT_CLI_MODEL` | ID of the model to use | "gpt-3.5-turbo" |
 | `GPT_CLI_TEMPERATURE` | Sampling temperature to use, between 0 and 2 | 0.5 |
 | `GPT_CLI_FREQUENCY_PENALTY` | Number between -2.0 and 2.0. Positive values penalize new tokens based on their existing frequency in the text so far | 0 |
 | `GPT_CLI_PRESENCE_PENALTY` | Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the text so far | 0 |
 | `GPT_CLI_MAX_TOKENS` | The maximum number of tokens to generate in the chat completion | 2048 |
-| `GPT_CLI_TOP_P` | An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass | 1 |
+| `GPT_CLI_TOP_P` | An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with `top_p` probability mass | 1 |
 | `GPT_CLI_N_COMPLETIONS` | How many chat completion choices to generate for each input message | 1 |
 | `GPT_CLI_SYSTEM_MESSAGE` | Specify an alternative system message | [See this section](#system-message) |
 
 #### System Message
 
 The default [system message](https://platform.openai.com/docs/guides/chat/instructing-chat-models) is:
 
 ```text
 The current date and time is 2023-05-06 15:55:56.619232. When emitting code or producing markdown, ensure to label fenced code blocks with the language in use.'
 ```
 
-This can be overridden. GPT 3.5 seems to sometime forget to emit labels for fenced code blocks which prevents the syntax highlighting from taking effect. Thus, a reminder in the system message is recommended.
+This can be overridden. GPT 3.5 sometimes forgets to emit labels for fenced code blocks, which prevents the syntax highlighting from taking effect. Thus, a reminder in the system message is recommended.
 
 #### Tricks
 
-You can use heredoc in bash to create a prompt with includes a file:
+You can use heredoc in `bash` to create a prompt with includes a file:
 
 ```text
 $ gpt-chat-cli -i --prompt-from-fd 3 3<<EOF
 heredoc> Can you review this code:
 heredoc> $(cat quicksort.c)
 heredoc> EOF
 [#] Can you review this code:
@@ -204,17 +204,18 @@
 
 1. Naming: The function name `quicksort` is not very descriptive. It would be better to name it something like `quicksort_entries_by_access_time` to make it clear what it does.
 
 ...
 [#]
 ```
 
-#### Known issues
+#### Known Issues
 
 There are a couple known issues. PRs are accepted:
 
 1. `gpt-chat-cli` lacks shell completion
 2. `gpt-chat-cli` does not track token usage. Ideally, it should gracefully handle long messages and remove messages from the chat history if the number of tokens in the context is exceeded. If the tokens exceed the model's context, the following error will occur:
 
 ```text
 openai.error.InvalidRequestError: This model's maximum context length is 4097 tokens. However, your messages resulted in 9758 tokens. Please reduce the length of the messages.
 ```
+
```

### Comparing `gpt-chat-cli-0.1.0/pyproject.toml` & `gpt-chat-cli-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpt-chat-cli"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Flu0r1ne", email="flu0r1ne@flu0r1ne.net" },
 ]
 description = "A simple ChatGPT terminal CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `gpt-chat-cli-0.1.0/src/gpt_chat_cli/argparsing.py` & `gpt-chat-cli-0.1.1/src/gpt_chat_cli/argparsing.py`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.0/src/gpt_chat_cli/chat_colorizer.py` & `gpt-chat-cli-0.1.1/src/gpt_chat_cli/chat_colorizer.py`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.0/src/gpt_chat_cli/color.py` & `gpt-chat-cli-0.1.1/src/gpt_chat_cli/color.py`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.0/src/gpt_chat_cli/gcli.py` & `gpt-chat-cli-0.1.1/src/gpt_chat_cli/gcli.py`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.0/src/gpt_chat_cli/openai_wrappers.py` & `gpt-chat-cli-0.1.1/src/gpt_chat_cli/openai_wrappers.py`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.0/src/gpt_chat_cli/streaming_lexer.py` & `gpt-chat-cli-0.1.1/src/gpt_chat_cli/streaming_lexer.py`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/PKG-INFO` & `gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-chat-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple ChatGPT terminal CLI
 Author: Flu0r1ne
 Author-email: Flu0r1ne <flu0r1ne@flu0r1ne.net>
 Project-URL: Homepage, https://github.com/flu0r1ne/gpt-chat-cli
 Project-URL: Bug Tracker, https://github.com/flu0r1ne/gpt-chat-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,71 +12,71 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 gpt-chat-cli: a simple yet powerful ChatGPT CLI
 -----------------------------------------------
 
-## Intro
+## Introduction
 
-`gpt-chat-cli` is a simple, general purpose ChatGPT CLI. It brings the power of ChatGPT to the command line. It aims to be easy to use and configurable.
+`gpt-chat-cli` is a simple, general purpose ChatGPT CLI. It brings the power of ChatGPT to the command line. It aims to be easy to use and highly configurable.
 
 Some of the features include:
-- Streaming, real-time output
-- Interactive sessions with color and adornments
-- Support for any model which can be called through OpenAI's chat completions API.
+- Streaming, real-time output.
+- Interactive sessions with color and adornments.
+- Support for any model that can be called through OpenAI's chat completions API.
   [See model endpoint compatibility.](https://platform.openai.com/docs/models/model-endpoint-compatibility)
-- Modify model parameters including temperature, frequency penalty, presence penalty, top p, and the maximum number of tokens emitted
-- Dynamic code syntax highlighting
-- List available models
-- Respects unix norms. Input can be gathered from pipes, heredoc, files, and arbitrary file descriptors.
+- Ability to modify model parameters including temperature, frequency penalty, presence penalty, top p, and the maximum number of tokens emitted.
+- Dynamic code syntax highlighting.
+- List the available models.
+- Respects Unix norms. Input can be gathered from pipes, heredoc, files, and arbitrary file descriptors.
 
 ![gpt-chat-cli Completion Demo](./assets/images/gpt.gif)
 
 ### Installation
 
 ```bash
 pip install gpt-chat-cli
 ```
 
-The OpenAI API uses API keys for authentication. Visit your [API Keys page](https://platform.openai.com/account/api-keys) to retrieve the API key you'll use in your requests. 
+The OpenAI API uses API keys for authentication. Visit your [API Keys page](https://platform.openai.com/account/api-keys) to retrieve the API key you'll use in your requests:
 ```bash
 export OPENAI_API_KEY="INSERT_SECRET_KEY"
 ```
 
-Then, source the `OPENAI_API_KEY` environmental variable in your shell's configuration file. (That is, `~/.bashrc` or `~/.zshrc` for the Bash or Zsh shell, respectively.)
+Then, source the `OPENAI_API_KEY` environmental variable in your shell's configuration file. (That is, `~/.bashrc` or `~/.zshrc` for the Bash or Zsh shell, respectively):
 
 ```bash
 source ~/.bashrc
 ```
 
-### User guide
+### User Guide
 
 #### Basic Usage
 
 Without additional arguments, `gpt-chat-cli` will drop the user into an interactive shell:
 
 ```text
 $ gpt-chat-cli
 GPT Chat CLI version 0.1.0
 Press Control-D to exit
 [#] Hello!
 [gpt-3.5-turbo-0301] Hello! How can I assist you today?
 ```
 
-For a single completion, an initial message can be specified as the first positional:
+For a single completion, an initial message can be specified as the first positional argument:
 
 ```text
 $ gpt-chat-cli "In one sentence, who is Joseph Weizenbaum?"
 [gpt-3.5-turbo-0301] Joseph Weizenbaum was a German-American computer scientist
 and philosopher who is known for creating the ELIZA program, one of the first 
 natural language processing programs.
 ```
 
-Or, specify the inital message and drop into an interactive shell with `-i`:
+Alternatively, you can specify the initial message and drop into an interactive shell with `-i`:
 
 ```text
 $ gpt-chat-cli -i "What linux command prints a list of all open TCP sockets on port 8080?"
 GPT Chat CLI version 0.1.0
 Press Control-D to exit
 [#] What linux command prints a list of all open TCP sockets on port 8080?
 [gpt-3.5-turbo-0301] You can use the `lsof` (list open files) command to list all
@@ -86,15 +86,15 @@
 
 [#] Can do do this with ss?
 [gpt-3.5-turbo-0301] Yes, you can also use the `ss` (socket statistics) command to
 list all open TCP sockets on port 8080. The command to list all open TCP sockets
 on port 8080 using `ss` is `sudo ss -tlnp 'sport = :8080'`
 ```
 
-`gpt-chat-cli` respects pipes and redirects:
+`gpt-chat-cli` respects pipes and redirects, so you can use it in combination with other command-line tools:
 
 ```text
 $ printf "What is smmsp in /etc/group?\n$(cat /etc/group | head)" | gpt-chat-cli
 [gpt-3.5-turbo-0301] `smmsp` is a system user and group used by the Sendmail mail transfer agent (MTA)
 for sending mail. The `smmsp` group is used to provide access to the Sendmail queue directory and
 other Sendmail-related files. Members of this group are allowed to read and write to the Sendmail
 queue directory and other Sendmail-related files.
@@ -112,15 +112,15 @@
     let average = sum / count as i32;
     println!("The average is {}", average);
 }
 
 This code creates a vector of numbers, calculates the sum of the numbers using the `iter()` method and the `sum()` method, counts the number of elements in the vector using the `len()` method, and then calculates the average by dividing the sum by the count. Finally, it prints the average to the console.
 ```
 
-List available models:
+To list all available models, use the following command:
 
 ```text
 $ gpt-chat-cli --list-models
 gpt-3.5-turbo
 gpt-3.5-turbo-0301
 gpt-4
 gpt-4-0314
@@ -176,31 +176,31 @@
 | Environmental Variable | Controls | Default Value |
 | --- | --- | --- |
 | `GPT_CLI_MODEL` | ID of the model to use | "gpt-3.5-turbo" |
 | `GPT_CLI_TEMPERATURE` | Sampling temperature to use, between 0 and 2 | 0.5 |
 | `GPT_CLI_FREQUENCY_PENALTY` | Number between -2.0 and 2.0. Positive values penalize new tokens based on their existing frequency in the text so far | 0 |
 | `GPT_CLI_PRESENCE_PENALTY` | Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the text so far | 0 |
 | `GPT_CLI_MAX_TOKENS` | The maximum number of tokens to generate in the chat completion | 2048 |
-| `GPT_CLI_TOP_P` | An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass | 1 |
+| `GPT_CLI_TOP_P` | An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with `top_p` probability mass | 1 |
 | `GPT_CLI_N_COMPLETIONS` | How many chat completion choices to generate for each input message | 1 |
 | `GPT_CLI_SYSTEM_MESSAGE` | Specify an alternative system message | [See this section](#system-message) |
 
 #### System Message
 
 The default [system message](https://platform.openai.com/docs/guides/chat/instructing-chat-models) is:
 
 ```text
 The current date and time is 2023-05-06 15:55:56.619232. When emitting code or producing markdown, ensure to label fenced code blocks with the language in use.'
 ```
 
-This can be overridden. GPT 3.5 seems to sometime forget to emit labels for fenced code blocks which prevents the syntax highlighting from taking effect. Thus, a reminder in the system message is recommended.
+This can be overridden. GPT 3.5 sometimes forgets to emit labels for fenced code blocks, which prevents the syntax highlighting from taking effect. Thus, a reminder in the system message is recommended.
 
 #### Tricks
 
-You can use heredoc in bash to create a prompt with includes a file:
+You can use heredoc in `bash` to create a prompt with includes a file:
 
 ```text
 $ gpt-chat-cli -i --prompt-from-fd 3 3<<EOF
 heredoc> Can you review this code:
 heredoc> $(cat quicksort.c)
 heredoc> EOF
 [#] Can you review this code:
@@ -219,17 +219,18 @@
 
 1. Naming: The function name `quicksort` is not very descriptive. It would be better to name it something like `quicksort_entries_by_access_time` to make it clear what it does.
 
 ...
 [#]
 ```
 
-#### Known issues
+#### Known Issues
 
 There are a couple known issues. PRs are accepted:
 
 1. `gpt-chat-cli` lacks shell completion
 2. `gpt-chat-cli` does not track token usage. Ideally, it should gracefully handle long messages and remove messages from the chat history if the number of tokens in the context is exceeded. If the tokens exceed the model's context, the following error will occur:
 
 ```text
 openai.error.InvalidRequestError: This model's maximum context length is 4097 tokens. However, your messages resulted in 9758 tokens. Please reduce the length of the messages.
 ```
+
```

### Comparing `gpt-chat-cli-0.1.0/src/gpt_chat_cli.egg-info/SOURCES.txt` & `gpt-chat-cli-0.1.1/src/gpt_chat_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-chat-cli-0.1.0/tests/test_streaming_lexer.py` & `gpt-chat-cli-0.1.1/tests/test_streaming_lexer.py`

 * *Files identical despite different names*

