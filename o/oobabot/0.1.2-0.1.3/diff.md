# Comparing `tmp/oobabot-0.1.2.tar.gz` & `tmp/oobabot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oobabot-0.1.2.tar", max compression
+gzip compressed data, was "oobabot-0.1.3.tar", max compression
```

## Comparing `oobabot-0.1.2.tar` & `oobabot-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-05-04 00:39:46.200078 oobabot-0.1.2/LICENSE
--rw-r--r--   0        0        0     7464 2023-05-04 05:25:50.455313 oobabot-0.1.2/README.md
--rw-r--r--   0        0        0      609 2023-05-04 06:11:36.022566 oobabot-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       45 2023-05-04 06:11:56.742561 oobabot-0.1.2/src/oobabot/__init__.py
--rw-r--r--   0        0        0       69 2023-05-04 00:39:46.200078 oobabot-0.1.2/src/oobabot/__main__.py
--rw-r--r--   0        0        0     9425 2023-05-04 05:57:27.632802 oobabot-0.1.2/src/oobabot/discord_bot.py
--rw-r--r--   0        0        0     1560 2023-05-04 00:39:46.200078 oobabot-0.1.2/src/oobabot/fancy_logging.py
--rw-r--r--   0        0        0     2939 2023-05-04 00:39:46.200078 oobabot-0.1.2/src/oobabot/ooba_client.py
--rwxr-xr-x   0        0        0     2159 2023-05-04 04:15:27.736485 oobabot-0.1.2/src/oobabot/oobabot.py
--rw-r--r--   0        0        0     6658 2023-05-04 00:39:46.200078 oobabot-0.1.2/src/oobabot/response_stats.py
--rw-r--r--   0        0        0     2729 2023-05-04 00:39:46.200078 oobabot-0.1.2/src/oobabot/sentence_splitter.py
--rw-r--r--   0        0        0     3899 2023-05-04 06:00:50.732746 oobabot-0.1.2/src/oobabot/settings.py
--rw-r--r--   0        0        0     8297 1970-01-01 00:00:00.000000 oobabot-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-03 00:11:59.534663 oobabot-0.1.3/LICENSE
+-rw-r--r--   0        0        0     8513 2023-05-07 08:27:31.575186 oobabot-0.1.3/README.md
+-rw-r--r--   0        0        0      967 2023-05-07 08:29:52.158852 oobabot-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-05-07 08:29:39.308544 oobabot-0.1.3/src/oobabot/__init__.py
+-rw-r--r--   0        0        0       69 2023-05-05 00:57:20.206747 oobabot-0.1.3/src/oobabot/__main__.py
+-rw-r--r--   0        0        0    13698 2023-05-07 08:22:57.238237 oobabot-0.1.3/src/oobabot/discord_bot.py
+-rw-r--r--   0        0        0     1572 2023-05-05 00:57:22.929461 oobabot-0.1.3/src/oobabot/fancy_logging.py
+-rw-r--r--   0        0        0     3296 2023-05-05 00:57:24.331138 oobabot-0.1.3/src/oobabot/ooba_client.py
+-rwxr-xr-x   0        0        0     2157 2023-05-05 00:57:25.553393 oobabot-0.1.3/src/oobabot/oobabot.py
+-rw-r--r--   0        0        0     6586 2023-05-05 00:57:26.704654 oobabot-0.1.3/src/oobabot/response_stats.py
+-rw-r--r--   0        0        0     2695 2023-05-05 00:57:27.771786 oobabot-0.1.3/src/oobabot/sentence_splitter.py
+-rw-r--r--   0        0        0     3981 2023-05-05 00:57:28.849070 oobabot-0.1.3/src/oobabot/settings.py
+-rw-r--r--   0        0        0     9346 1970-01-01 00:00:00.000000 oobabot-0.1.3/PKG-INFO
```

### Comparing `oobabot-0.1.2/LICENSE` & `oobabot-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.2/README.md` & `oobabot-0.1.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,38 @@
 # `oobabot`
 
 **`oobabot`** is a Discord bot which talks to a Large Language Model AIs (like LLaMA, llama.cpp, etc...), running on [oobabooga's text-generation-webui](https://github.com/oobabooga/text-generation-webui).
 
 [![python lint and test with poetry](https://github.com/chrisrude/oobabot/actions/workflows/python-package.yml/badge.svg)](https://github.com/chrisrude/oobabot/actions/workflows/python-package.yml)
 
+## Installation
+
+```bash
+  pip install oobabot
+```
+
+requires python 3.8+
+
+## Usage
+
+```bash
+$ oobabot --wakewords rosie cat --ai-name Rosie --persona "you are a cat named Rosie"
+
+2023-05-04 00:24:10,968 DEBUG Oobabooga base URL: ws://localhost:5005
+2023-05-04 00:24:11,133 INFO Connected to Oobabooga!
+2023-05-04 00:24:11,133 DEBUG Connecting to Discord...
+2023-05-04 00:24:13,807 INFO Connected to discord as RosieAI#0000 (ID: 1100100011101010101)
+2023-05-04 00:24:13,807 DEBUG monitoring DMs, plus 24 channels across 1 server(s)
+2023-05-04 00:24:13,807 DEBUG AI name: Rosie
+2023-05-04 00:24:13,807 DEBUG AI persona: you are a cat named Rosie
+2023-05-04 00:24:13,807 DEBUG wakewords: rosie, cat
+```
+
+See below for more details on the command line options.
+
 ## Motivation
 
 ![oobabot in action!](./docs/oobabot.png "discord action shot")
 
 Text-generative UIs are cool to run at home, and Discord is fun to mess with your friends.  Why not combine the two and have something awesome!
 
 Real motivation: I wanted a chatbot in my discord that would act like my cat.  A "catbot" if you will.
@@ -39,15 +64,15 @@
 ~: pip install oobabot
 
 ~: export DISCORD_TOKEN = __your_bots_discord_token__
 
 ~: oobabot --base-url ws://oobabooga-hostname:5005/ --ai-name YourBotsName --persona "You are a cat named YourBotsName"
 ```
 
-You should now be able to run oobabot from whenever pip installed it.
+You should now be able to run oobabot from wherever pip installed it.
 
 ```none
 usage: oobabot [-h] [--base-url BASE_URL] [--ai-name AI_NAME] [--wakewords [WAKEWORDS ...]]
                [--persona PERSONA] [--local-repl] [--log-all-the-things LOG_ALL_THE_THINGS]
 
 Discord bot for oobabooga's text-generation-webui
 
@@ -156,12 +181,17 @@
 
 By default, **`oobabot`** will listen for three types of messages in the servers it's connected to:
 
  1. any message in which **`oobabot`**'s account is @-mentioned
  1. any direct message
  1. any message containing a provided wakeword (see Optional Settings)
 
+Also, the bot has a random chance of sending follow-up messages within the
+same channel if others reply within 120 seconds of its last post.  The exact
+parameters for this are in flux, but is meant to simulate a natural conversation
+flow, without forcing others to always post a wakeword.
+
 ## Known Issues
 
-- ooba's text generation can errs with OOM when more than one request comes in at once.
+- ooba's text generation can error with OOM when more than one request comes in at once.
 - sometimes the bot wants to continue conversations on behalf of other members of the chatroom.  I have some hacks in place to notice and truncate this behavior, but it can lead to terse responses on occasion.
 - found one not listed here?  [Create an issue](https://github.com/chrisrude/oobabot/issues) on github!
```

### Comparing `oobabot-0.1.2/src/oobabot/fancy_logging.py` & `oobabot-0.1.3/src/oobabot/fancy_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-
 import logging
 
 FOREGROUND_COLORS = {
     "black": 30,
     "red": 31,
     "green": 32,
     "yellow": 33,
     "blue": 34,
     "magenta": 35,
     "cyan": 36,
     "white": 37,
 }
 
 
-def apply_color(color, text: str = '%(message)s') -> str:
+def apply_color(color, text: str = "%(message)s") -> str:
     return f"\033[{FOREGROUND_COLORS[color]}m{text}\033[0m"
 
 
 PREFIX = f'{apply_color("yellow", "%(asctime)s")} %(levelname)s '
 
 FORMATS = {
-    logging.DEBUG: PREFIX + apply_color('cyan'),
-    logging.INFO: PREFIX + apply_color('white'),
-    logging.WARNING: PREFIX + apply_color('yellow'),
-    logging.ERROR: PREFIX + apply_color('red'),
-    logging.CRITICAL: PREFIX + apply_color('red'),
+    logging.DEBUG: PREFIX + apply_color("cyan"),
+    logging.INFO: PREFIX + apply_color("white"),
+    logging.WARNING: PREFIX + apply_color("yellow"),
+    logging.ERROR: PREFIX + apply_color("red"),
+    logging.CRITICAL: PREFIX + apply_color("red"),
 }
 
 
 class ColorfulLoggingFormatter(logging.Formatter):
     def __init__(self) -> None:
         super().__init__()
         self.formatters = {}
         for logging_level in FORMATS.keys():
             self.formatters[logging_level] = logging.Formatter(
-                FORMATS.get(logging_level))
+                FORMATS.get(logging_level)
+            )
 
     def format(self, record: logging.LogRecord) -> str:
         formatter = self.formatters.get(record.levelno)
         if formatter:
             return formatter.format(record)
         else:
             return record.getMessage()
```

### Comparing `oobabot-0.1.2/src/oobabot/ooba_client.py` & `oobabot-0.1.3/src/oobabot/ooba_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,97 +1,111 @@
 # Purpose: Streaming client for the Ooba API.
 # Can provide the response by token or by sentence.
 #
 
+from asyncio.exceptions import TimeoutError
 import json
+from socket import gaierror
 import typing
+from urllib.parse import urljoin
+
 import websockets as ws  # weird, but needed to avoid long lines later
+from websockets.exceptions import WebSocketException
 
 from oobabot.sentence_splitter import SentenceSplitter
-from urllib.parse import urljoin
+
+
+class OobaClientError(Exception):
+    pass
 
 
 class OobaClient:
     # Purpose: Streaming client for the Ooba API.
     # Can provide the response by token or by sentence.
 
-    END_OF_INPUT = ''
+    END_OF_INPUT = ""
 
     def __init__(self, base_url: str):
         self.api_url = urljoin(base_url, self.STREAMING_URI_PATH)
         self.total_response_tokens = 0
 
     DEFAULT_REQUEST_PARAMS = {
-        'max_new_tokens': 250,
-        'do_sample': True,
-        'temperature': 1.3,
-        'top_p': 0.1,
-        'typical_p': 1,
-        'repetition_penalty': 1.18,
-        'top_k': 40,
-        'min_length': 0,
-        'no_repeat_ngram_size': 0,
-        'num_beams': 1,
-        'penalty_alpha': 0,
-        'length_penalty': 1,
-        'early_stopping': False,
-        'seed': -1,
-        'add_bos_token': True,
-        'truncation_length': 2048,
-        'ban_eos_token': False,
-        'skip_special_tokens': True,
-        'stopping_strings': [],
+        "max_new_tokens": 250,
+        "do_sample": True,
+        "temperature": 1.3,
+        "top_p": 0.1,
+        "typical_p": 1,
+        "repetition_penalty": 1.18,
+        "top_k": 40,
+        "min_length": 0,
+        "no_repeat_ngram_size": 0,
+        "num_beams": 1,
+        "penalty_alpha": 0,
+        "length_penalty": 1,
+        "early_stopping": False,
+        "seed": -1,
+        "add_bos_token": True,
+        "truncation_length": 2048,
+        "ban_eos_token": False,
+        "skip_special_tokens": True,
+        "stopping_strings": [],
     }
 
-    STREAMING_URI_PATH = './api/v1/stream'
+    STREAMING_URI_PATH = "./api/v1/stream"
 
-    async def try_connect(self) -> str:
-        '''
+    async def try_connect(self):
+        """
         Attempt to connect to the oobabooga server.
 
         Returns:
-            str, error message if unsuccessful, empty string on success
-        '''
+            nothing, if the connection test was successful
+
+        Raises:
+            OobaClientError, if the connection fails
+        """
         try:
-            async with ws.connect(self.api_url) as _:  # type: ignore
-                return ''
-        except Exception as e:
-            return str(e)
-
-    async def request_by_sentence(self, prompt: str) \
-            -> typing.AsyncIterator[str]:
-        '''
+            async with ws.connect(self.api_url):  # type: ignore
+                return
+        except (
+            ConnectionRefusedError,
+            gaierror,
+            TimeoutError,
+            WebSocketException,
+        ) as e:
+            raise OobaClientError(f"Failed to connect to {self.api_url}: {e}", e)
+
+    async def request_by_sentence(self, prompt: str) -> typing.AsyncIterator[str]:
+        """
         Yields each complete sentence of the response as it arrives.
-        '''
+        """
 
         splitter = SentenceSplitter()
         async for new_token in self.request_by_token(prompt):
             for sentence in splitter.by_sentence(new_token):
                 yield sentence
 
-    async def request_by_token(self, prompt: str) \
-            -> typing.AsyncIterator[str]:
-        '''
+    async def request_by_token(self, prompt: str) -> typing.AsyncIterator[str]:
+        """
         Yields each token of the response as it arrives.
-        '''
+        """
 
         request = {
-            'prompt': prompt,
+            "prompt": prompt,
         }
         request.update(self.DEFAULT_REQUEST_PARAMS)
 
         async with ws.connect(self.api_url) as websocket:  # type: ignore
             await websocket.send(json.dumps(request))
 
             while True:
                 incoming_data = await websocket.recv()
                 incoming_data = json.loads(incoming_data)
 
-                if 'text_stream' == incoming_data['event']:
-                    if (incoming_data['text']):
+                if "text_stream" == incoming_data["event"]:
+                    if incoming_data["text"]:
                         self.total_response_tokens += 1
-                        yield incoming_data['text']
+                        yield incoming_data["text"]
 
-                elif 'stream_end' == incoming_data['event']:
+                elif "stream_end" == incoming_data["event"]:
                     # Make sure any unprinted text is flushed.
                     yield self.END_OF_INPUT
                     return
```

### Comparing `oobabot-0.1.2/src/oobabot/response_stats.py` & `oobabot-0.1.3/src/oobabot/response_stats.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,197 +1,194 @@
 import time
 
-from oobabot.ooba_client import OobaClient
 from oobabot.fancy_logging import get_logger
+from oobabot.ooba_client import OobaClient
 
 
 class ResponseStats:
-    '''
+    """
     Purpose: collects timing and rate statistics for a single response
-    '''
+    """
 
     def __init__(self, ooba_client: OobaClient, prompt: str):
         self.ooba_client = ooba_client
         self.start_time = time.time()
         self.start_tokens = ooba_client.total_response_tokens
         self.duration = 0
         self.latency = 0
         self.tokens = 0
         self.prompt_len = len(prompt)
 
     def log_response_part(self) -> None:
-        '''
+        """
         Call this each time the response is updated by the AI.
-        '''
+        """
 
         now = time.time()
         if not self.latency:
             self.latency = now - self.start_time
         self.duration = now - self.start_time
-        self.tokens = self.ooba_client.total_response_tokens - \
-            self.start_tokens
+        self.tokens = self.ooba_client.total_response_tokens - self.start_tokens
 
     def tokens_per_second(self) -> float:
-        '''
+        """
         Returns the rate at which tokens were generated, in tokens per second.
-        '''
+        """
         if not self.duration:
             return 0
         return self.tokens / self.duration
 
     def write_to_log(self, log_prefix: str) -> None:
-        '''
+        """
         This writes the statistics for this specific
         request to the log.
-        '''
+        """
         get_logger().debug(
-            log_prefix +
-            f"tokens: {self.tokens}, " +
-            f"time: {self.duration:.2f}s, " +
-            f"latency: {self.latency:.2f}s, " +
-            f"rate: {self.tokens_per_second():.2f} tok/s")
+            log_prefix
+            + f"tokens: {self.tokens}, "
+            + f"time: {self.duration:.2f}s, "
+            + f"latency: {self.latency:.2f}s, "
+            + f"rate: {self.tokens_per_second():.2f} tok/s"
+        )
 
 
 class AggregateResponseStats:
-    '''
+    """
     Purpose: collects timing and rate statistics for all AggregateResponseStats
-    '''
+    """
 
     def __init__(self, ooba_client: OobaClient):
         self.ooba_client = ooba_client
         self.total_requests_received = 0
         self.total_successful_responses = 0
         self.total_failed_responses = 0
         self.total_response_time_seconds = 0
         self.total_response_latency_seconds = 0
         self.prompt_max_chars = 0
         self.prompt_min_chars = 0
         self.prompt_total_chars = 0
 
     def log_request_arrived(self, prompt) -> ResponseStats:
-        '''
+        """
         Call this when a request has arrived.
         This must be followed by zero or more calls
         to log_response_part(), and then exactly one call to
         either log_response_failure() or log_response_success().
-        '''
+        """
         result = ResponseStats(self.ooba_client, prompt)
 
         self.total_requests_received += 1
         # update the prompt stats now
         if self.prompt_max_chars < result.prompt_len:
             self.prompt_max_chars = result.prompt_len
         if self.prompt_min_chars > result.prompt_len:
             self.prompt_min_chars = result.prompt_len
         self.prompt_total_chars += result.prompt_len
 
         return result
 
     def log_response_failure(self) -> None:
-        '''
+        """
         Track the statistics for a failed response.
-        '''
+        """
         self.total_failed_responses += 1
 
     def log_response_success(self, response: ResponseStats) -> None:
-        '''
+        """
         Track the statistics for a successful response, and
         averages them into the overall statistics.
 
         Parameters:
          - response: the Response object returned
               by log_request_arrived()
-        '''
+        """
         self.total_successful_responses += 1
         self.total_response_time_seconds += response.duration
         self.total_response_latency_seconds += response.latency
 
     def error_rate(self) -> float:
-        '''
+        """
         Returns the percentage of requests that failed.
-        '''
+        """
         if 0 == self.total_requests_received:
             return 0.0
         return 100 * self.total_failed_responses / self.total_requests_received
 
     def average_response_time(self) -> float:
-        '''
+        """
         Returns the average response time in seconds.
-        '''
+        """
         if 0 == self.total_successful_responses:
             return 0.0
-        return self.total_response_time_seconds / \
-            self.total_successful_responses
+        return self.total_response_time_seconds / self.total_successful_responses
 
     def average_response_latency(self) -> float:
-        '''
+        """
         Returns the average response latency in seconds.
-        '''
+        """
         if 0 == self.total_successful_responses:
             return 0.0
-        return self.total_response_latency_seconds / \
-            self.total_successful_responses
+        return self.total_response_latency_seconds / self.total_successful_responses
 
     def average_tokens_per_second(self) -> float:
-        '''
+        """
         Returns the average rate at which tokens were generated,
         in tokens per second.
-        '''
+        """
         if 0 == self.total_successful_responses:
             return 0.0
-        return self.ooba_client.total_response_tokens / \
-            self.total_response_time_seconds
+        return self.ooba_client.total_response_tokens / self.total_response_time_seconds
 
     def average_prompt_length(self) -> float:
-        '''
+        """
         Returns the average prompt length in characters.
-        '''
+        """
         if 0 == self.total_requests_received:
             return 0.0
         return self.prompt_total_chars / self.total_requests_received
 
     def write_stat_summary_to_log(self) -> None:
-        '''
+        """
         This writes a summary of the statistics to the log.
         Call this after all AggregateResponseStats have been handled.
-        '''
+        """
         if 0 == self.total_requests_received:
-            get_logger().info('No requests handled')
+            get_logger().info("No requests handled")
             return
 
         get_logger().info(
-            f'Recevied {self.total_requests_received} request(s), ' +
-            f'sent {self.total_successful_responses} successful responses ' +
-            f'and failed to send one {self.total_failed_responses} times(s)')
+            f"Recevied {self.total_requests_received} request(s), "
+            + f"sent {self.total_successful_responses} successful responses "
+            + f"and failed to send one {self.total_failed_responses} times(s)"
+        )
 
-        if (self.total_failed_responses > 0):
+        if self.total_failed_responses > 0:
             get_logger().error(
-                'Error rate:                  ' +
-                f'{self.error_rate()}%'
+                "Error rate:                  " + f"{self.error_rate()}%"
             )
 
-        if (self.total_successful_responses > 0):
+        if self.total_successful_responses > 0:
             get_logger().debug(
-                'Average response time:       ' +
-                f'{self.average_response_time():6.2f}s'
+                "Average response time:       "
+                + f"{self.average_response_time():6.2f}s"
             )
             get_logger().debug(
-                'Average response latency:    ' +
-                f'{self.average_response_latency():6.2f}s'
+                "Average response latency:    "
+                + f"{self.average_response_latency():6.2f}s"
             )
             get_logger().debug(
-                'Average tokens per response: ' +
-                f'{self.average_tokens_per_second():6.2f}'
+                "Average tokens per response: "
+                + f"{self.average_tokens_per_second():6.2f}"
             )
 
         if self.total_response_time_seconds > 0:
             get_logger().debug(
-                'Average tokens per second:   ' +
-                f'{self.average_tokens_per_second():6.2f}'
+                "Average tokens per second:   "
+                + f"{self.average_tokens_per_second():6.2f}"
             )
 
         get_logger().debug(
-            'Prompt length:               ' +
-            f'max: {self.prompt_max_chars}, ' +
-            f'min: {self.prompt_min_chars}, ' +
-            f'avg: {self.average_prompt_length():.2f}'
+            "Prompt length: "
+            + f"max: {self.prompt_max_chars}, "
+            + f"min: {self.prompt_min_chars}, "
+            + f"avg: {self.average_prompt_length():.2f}"
         )
```

### Comparing `oobabot-0.1.2/src/oobabot/sentence_splitter.py` & `oobabot-0.1.3/src/oobabot/sentence_splitter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,75 @@
 # Purpose: Split a string into sentences, based on a set of terminators.
 #          This is a helper class for ooba_client.py.
-import pysbd
 import typing
 
+import pysbd
+
 
 class SentenceSplitter:
-    '''
+    """
     Purpose: Split an English string into sentences.
-    '''
+    """
 
     # anything that can't be in a real response
-    END_OF_INPUT = ''
+    END_OF_INPUT = ""
 
     def __init__(self):
         self.printed_idx = 0
-        self.full_response = ''
-        self.segmenter = pysbd.Segmenter(
-            language="en", clean=False, char_span=True)
-
-    def by_sentence(self, new_token: str) \
-            -> typing.Generator[str, None, None]:
-        '''
+        self.full_response = ""
+        self.segmenter = pysbd.Segmenter(language="en", clean=False, char_span=True)
+
+    def by_sentence(self, new_token: str) -> typing.Generator[str, None, None]:
+        """
         Collects tokens into a single string, looks for ends of english
         sentences, then yields each sentence as soon as it's found.
 
         Parameters:
             new_token: str, the next token to add to the string
 
         Returns:
             Generator[str, None, None], yields each sentence
 
         Note:
         When there is no longer any input, the caller must pass
         SentenceSplitter.END_OF_INPUT to this function.  This
         function will then yield any remaining text, even if it
         doesn't look like a full sentence.
-        '''
+        """
 
         self.full_response += new_token
-        unseen = self.full_response[self.printed_idx:]
+        unseen = self.full_response[self.printed_idx :]
 
         # if we've reached the end of input, yield it all,
         # even if we don't think it's a full sentence.
-        if (self.END_OF_INPUT == new_token):
+        if self.END_OF_INPUT == new_token:
             to_print = unseen.strip()
-            if (to_print):
+            if to_print:
                 yield unseen
             self.printed_idx += len(unseen)
             return
 
         segments = self.segmenter.segment(unseen)
 
         # any remaining non-sentence things will be in the last element
         # of the list.  Don't print that yet.  At the very worst, we'll
         # print it when the END_OF_INPUT signal is reached.
         for sentence_w_char_spans in segments[:-1]:
-
             # sentence_w_char_spans is a class with the following fields:
             #  - sent: str, sentence text
             #  - start: start idx of 'sent', relative to original string
             #  - end: end idx of 'sent', relative to original string
             #
             # we want to remove the last '\n' if there is one.
             # we do want to include any other whitespace, though.
 
             to_print = sentence_w_char_spans.sent  # type: ignore
-            if (to_print.endswith('\n')):
+            if to_print.endswith("\n"):
                 to_print = to_print[:-1]
 
             yield to_print
 
         # since we've printed all the previous segments,
         # the start of the last segment becomes the starting
         # point for the next roud.
-        if (len(segments) > 0):
+        if len(segments) > 0:
             self.printed_idx += segments[-1].start  # type: ignore
```

### Comparing `oobabot-0.1.2/src/oobabot/settings.py` & `oobabot-0.1.3/src/oobabot/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,105 @@
-
 import argparse
 import os
 
 
 class Settings(argparse.ArgumentParser):
     # Purpose: reads settings from environment variables and command line
     #          arguments
 
-    DISCORD_TOKEN_ENV_VAR = 'DISCORD_TOKEN'
-    DISCORD_TOKEN = os.environ.get(DISCORD_TOKEN_ENV_VAR, '')
+    DISCORD_TOKEN_ENV_VAR = "DISCORD_TOKEN"
+    DISCORD_TOKEN = os.environ.get(DISCORD_TOKEN_ENV_VAR, "")
 
-    OOBABOT_PERSONA_ENV_VAR = 'OOBABOT_PERSONA'
-    OOBABOT_PERSONA = os.environ.get(OOBABOT_PERSONA_ENV_VAR, '')
+    OOBABOT_PERSONA_ENV_VAR = "OOBABOT_PERSONA"
+    OOBABOT_PERSONA = os.environ.get(OOBABOT_PERSONA_ENV_VAR, "")
 
-    DEFAULT_WAKEWORDS = ['oobabot']
-    DEFAULT_URL = 'ws://localhost:5005'
+    DEFAULT_WAKEWORDS = ["oobabot"]
+    DEFAULT_URL = "ws://localhost:5005"
 
     def __init__(self):
         self._settings = None
         self.wakewords = []
 
         super().__init__(
             description="Discord bot for oobabooga's text-generation-webui",
-            epilog='Also, to authenticate to Discord, you must set the ' +
-            'environment variable:\n'
-            f"\t{self.DISCORD_TOKEN_ENV_VAR} = <your bot's discord token>"
+            epilog="Also, to authenticate to Discord, you must set the "
+            + "environment variable:\n"
+            f"\t{self.DISCORD_TOKEN_ENV_VAR} = <your bot's discord token>",
         )
         self.add_argument(
-            '--base-url',
+            "--base-url",
             type=str,
             default=self.DEFAULT_URL,
-            help='Base URL for the oobabooga instance.  ' +
-            'This should be ws://hostname[:port] for plain websocket ' +
-            'connections, or wss://hostname[:port] for websocket ' +
-            'connections over TLS.'
+            help="Base URL for the oobabooga instance.  "
+            + "This should be ws://hostname[:port] for plain websocket "
+            + "connections, or wss://hostname[:port] for websocket "
+            + "connections over TLS.",
         )
         self.add_argument(
-            '--ai-name',
+            "--ai-name",
             type=str,
-            default='oobabot',
-            help='Name of the AI to use for requests.  ' +
-            'This can be whatever you want, but might make sense ' +
-            'to be the name of the bot in Discord.'
+            default="oobabot",
+            help="Name of the AI to use for requests.  "
+            + "This can be whatever you want, but might make sense "
+            + "to be the name of the bot in Discord.",
         )
         self.add_argument(
-            '--wakewords',
+            "--wakewords",
             type=str,
-            nargs='*',
+            nargs="*",
             default=self.DEFAULT_WAKEWORDS,
-            help='One or more words that the bot will listen for.\n ' +
-            'The bot will listen in all discord channels can ' +
-            'access for one of these words to be mentioned, then reply ' +
-            'to any messages it sees with a matching word.  ' +
-            'The bot will always reply to @-mentions and ' +
-            'direct messages, even if no wakewords are supplied.')
+            help="One or more words that the bot will listen for.\n "
+            + "The bot will listen in all discord channels can "
+            + "access for one of these words to be mentioned, then reply "
+            + "to any messages it sees with a matching word.  "
+            + "The bot will always reply to @-mentions and "
+            + "direct messages, even if no wakewords are supplied.",
+        )
         self.add_argument(
-            '--persona',
+            "--persona",
             type=str,
             default=self.OOBABOT_PERSONA,
-            help='This prefix will be added in front of every user-supplied ' +
-            "request.  This is useful for setting up a 'character' for the " +
-            'bot to play.  Alternatively, this can be set with the ' +
-            f'{self.OOBABOT_PERSONA_ENV_VAR} environment variable.'
+            help="This prefix will be added in front of every user-supplied "
+            + "request.  This is useful for setting up a 'character' for the "
+            + "bot to play.  Alternatively, this can be set with the "
+            + f"{self.OOBABOT_PERSONA_ENV_VAR} environment variable.",
         )
         self.add_argument(
-            '--local-repl',
+            "--local-repl",
             default=False,
-            help='start a local REPL, instead of connecting to Discord',
-            action='store_true'
+            help="start a local REPL, instead of connecting to Discord",
+            action="store_true",
         )
         self.add_argument(
-            '--log-all-the-things',
+            "--log-all-the-things",
             default=False,
-            help='prints all oobabooga requests and responses in their ' +
-            'entirety to STDOUT',
-            action='store_true'
+            help="prints all oobabooga requests and responses in their "
+            + "entirety to STDOUT",
+            action="store_true",
         )
 
     def settings(self) -> dict[str, str]:
         if self._settings is None:
             self._settings = self.parse_args().__dict__
 
-            # this is a bit of a hack, but it's the only setting
-            # that's not a string, so with this we can be more
-            # strict with the type hints later
-            self.wakewords = self._settings.pop('wakewords')
+            # this is a bit of a hack, but by doing this with
+            # non-str settings, we can add stronger type hints
+            self.wakewords = self._settings.pop("wakewords")
+            self.log_all_the_things = self._settings.pop("log_all_the_things")
 
             # either we're using a local REPL, or we're connecting to Discord.
             # assume the user wants to connect to Discord
             if not (self.local_repl or self.DISCORD_TOKEN):
-                msg = f"Please set the '{Settings.DISCORD_TOKEN_ENV_VAR}' " + \
-                    "environment variable to your bot's discord token."
+                msg = (
+                    f"Please set the '{Settings.DISCORD_TOKEN_ENV_VAR}' "
+                    + "environment variable to your bot's discord token."
+                )
                 # will exit() after printing
                 self.error(msg)
 
         return self._settings
 
     def __getattr__(self, name) -> str:
-        return self.settings().get(name, '')
+        return self.settings().get(name, "")
 
     def __repr__(self) -> str:
         return super().__repr__()
```

### Comparing `oobabot-0.1.2/PKG-INFO` & `oobabot-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oobabot
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui
 Home-page: https://github.com/chrisrude/oobabot
 License: MIT
 Author: Christopher Rude
 Author-email: chris@rudesoftware.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,39 @@
 
 # `oobabot`
 
 **`oobabot`** is a Discord bot which talks to a Large Language Model AIs (like LLaMA, llama.cpp, etc...), running on [oobabooga's text-generation-webui](https://github.com/oobabooga/text-generation-webui).
 
 [![python lint and test with poetry](https://github.com/chrisrude/oobabot/actions/workflows/python-package.yml/badge.svg)](https://github.com/chrisrude/oobabot/actions/workflows/python-package.yml)
 
+## Installation
+
+```bash
+  pip install oobabot
+```
+
+requires python 3.8+
+
+## Usage
+
+```bash
+$ oobabot --wakewords rosie cat --ai-name Rosie --persona "you are a cat named Rosie"
+
+2023-05-04 00:24:10,968 DEBUG Oobabooga base URL: ws://localhost:5005
+2023-05-04 00:24:11,133 INFO Connected to Oobabooga!
+2023-05-04 00:24:11,133 DEBUG Connecting to Discord...
+2023-05-04 00:24:13,807 INFO Connected to discord as RosieAI#0000 (ID: 1100100011101010101)
+2023-05-04 00:24:13,807 DEBUG monitoring DMs, plus 24 channels across 1 server(s)
+2023-05-04 00:24:13,807 DEBUG AI name: Rosie
+2023-05-04 00:24:13,807 DEBUG AI persona: you are a cat named Rosie
+2023-05-04 00:24:13,807 DEBUG wakewords: rosie, cat
+```
+
+See below for more details on the command line options.
+
 ## Motivation
 
 ![oobabot in action!](./docs/oobabot.png "discord action shot")
 
 Text-generative UIs are cool to run at home, and Discord is fun to mess with your friends.  Why not combine the two and have something awesome!
 
 Real motivation: I wanted a chatbot in my discord that would act like my cat.  A "catbot" if you will.
@@ -60,15 +85,15 @@
 ~: pip install oobabot
 
 ~: export DISCORD_TOKEN = __your_bots_discord_token__
 
 ~: oobabot --base-url ws://oobabooga-hostname:5005/ --ai-name YourBotsName --persona "You are a cat named YourBotsName"
 ```
 
-You should now be able to run oobabot from whenever pip installed it.
+You should now be able to run oobabot from wherever pip installed it.
 
 ```none
 usage: oobabot [-h] [--base-url BASE_URL] [--ai-name AI_NAME] [--wakewords [WAKEWORDS ...]]
                [--persona PERSONA] [--local-repl] [--log-all-the-things LOG_ALL_THE_THINGS]
 
 Discord bot for oobabooga's text-generation-webui
 
@@ -177,13 +202,18 @@
 
 By default, **`oobabot`** will listen for three types of messages in the servers it's connected to:
 
  1. any message in which **`oobabot`**'s account is @-mentioned
  1. any direct message
  1. any message containing a provided wakeword (see Optional Settings)
 
+Also, the bot has a random chance of sending follow-up messages within the
+same channel if others reply within 120 seconds of its last post.  The exact
+parameters for this are in flux, but is meant to simulate a natural conversation
+flow, without forcing others to always post a wakeword.
+
 ## Known Issues
 
-- ooba's text generation can errs with OOM when more than one request comes in at once.
+- ooba's text generation can error with OOM when more than one request comes in at once.
 - sometimes the bot wants to continue conversations on behalf of other members of the chatroom.  I have some hacks in place to notice and truncate this behavior, but it can lead to terse responses on occasion.
 - found one not listed here?  [Create an issue](https://github.com/chrisrude/oobabot/issues) on github!
```

