# Comparing `tmp/code_aimpetus-0.1.2-py3-none-any.whl.zip` & `tmp/code_aimpetus-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,22 @@
-Zip file size: 5881 bytes, number of entries: 15
+Zip file size: 8499 bytes, number of entries: 20
 -rw-r--r--  2.0 fat      118 b- defN 20-Feb-02 00:00 code_aimpetus/__init__.py
--rw-r--r--  2.0 fat      527 b- defN 20-Feb-02 00:00 code_aimpetus/__main__.py
--rw-r--r--  2.0 fat      350 b- defN 20-Feb-02 00:00 code_aimpetus/celery.py
+-rw-r--r--  2.0 fat      529 b- defN 20-Feb-02 00:00 code_aimpetus/__main__.py
+-rw-r--r--  2.0 fat      260 b- defN 20-Feb-02 00:00 code_aimpetus/celery.py
+-rw-r--r--  2.0 fat      569 b- defN 20-Feb-02 00:00 code_aimpetus/common_options.py
+-rw-r--r--  2.0 fat      294 b- defN 20-Feb-02 00:00 code_aimpetus/settings.py
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 code_aimpetus/gh/__init__.py
--rw-r--r--  2.0 fat      856 b- defN 20-Feb-02 00:00 code_aimpetus/gh/repo.py
+-rw-r--r--  2.0 fat     1187 b- defN 20-Feb-02 00:00 code_aimpetus/gh/repo.py
+-rw-r--r--  2.0 fat      462 b- defN 20-Feb-02 00:00 code_aimpetus/gh/utility.py
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 code_aimpetus/gh/issues/__init__.py
--rw-r--r--  2.0 fat      709 b- defN 20-Feb-02 00:00 code_aimpetus/gh/issues/close.py
--rw-r--r--  2.0 fat      643 b- defN 20-Feb-02 00:00 code_aimpetus/gh/issues/list.py
+-rw-r--r--  2.0 fat     1272 b- defN 20-Feb-02 00:00 code_aimpetus/gh/issues/check_templates.py
+-rw-r--r--  2.0 fat     1026 b- defN 20-Feb-02 00:00 code_aimpetus/gh/issues/close.py
+-rw-r--r--  2.0 fat      724 b- defN 20-Feb-02 00:00 code_aimpetus/gh/issues/get.py
+-rw-r--r--  2.0 fat      903 b- defN 20-Feb-02 00:00 code_aimpetus/gh/issues/list.py
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 code_aimpetus/gh/pull_requests/__init__.py
--rw-r--r--  2.0 fat      635 b- defN 20-Feb-02 00:00 code_aimpetus/gh/pull_requests/list.py
-?rw-r--r--  2.0 fat      986 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.2.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 fat       54 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 fat     1092 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat     1284 b- defN 20-Feb-02 00:00 code_aimpetus-0.1.2.dist-info/RECORD
-15 files, 7341 bytes uncompressed, 3711 bytes compressed:  49.4%
+-rw-r--r--  2.0 fat      896 b- defN 20-Feb-02 00:00 code_aimpetus/gh/pull_requests/list.py
+?rw-r--r--  2.0 fat      986 b- defN 20-Feb-02 00:00 code_aimpetus-0.2.0.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 code_aimpetus-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 fat       54 b- defN 20-Feb-02 00:00 code_aimpetus-0.2.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 fat     1092 b- defN 20-Feb-02 00:00 code_aimpetus-0.2.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat     1722 b- defN 20-Feb-02 00:00 code_aimpetus-0.2.0.dist-info/RECORD
+20 files, 12181 bytes uncompressed, 5639 bytes compressed:  53.7%
```

## zipnote {}

```diff
@@ -3,44 +3,59 @@
 
 Filename: code_aimpetus/__main__.py
 Comment: 
 
 Filename: code_aimpetus/celery.py
 Comment: 
 
+Filename: code_aimpetus/common_options.py
+Comment: 
+
+Filename: code_aimpetus/settings.py
+Comment: 
+
 Filename: code_aimpetus/gh/__init__.py
 Comment: 
 
 Filename: code_aimpetus/gh/repo.py
 Comment: 
 
+Filename: code_aimpetus/gh/utility.py
+Comment: 
+
 Filename: code_aimpetus/gh/issues/__init__.py
 Comment: 
 
+Filename: code_aimpetus/gh/issues/check_templates.py
+Comment: 
+
 Filename: code_aimpetus/gh/issues/close.py
 Comment: 
 
+Filename: code_aimpetus/gh/issues/get.py
+Comment: 
+
 Filename: code_aimpetus/gh/issues/list.py
 Comment: 
 
 Filename: code_aimpetus/gh/pull_requests/__init__.py
 Comment: 
 
 Filename: code_aimpetus/gh/pull_requests/list.py
 Comment: 
 
-Filename: code_aimpetus-0.1.2.dist-info/METADATA
+Filename: code_aimpetus-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: code_aimpetus-0.1.2.dist-info/WHEEL
+Filename: code_aimpetus-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: code_aimpetus-0.1.2.dist-info/entry_points.txt
+Filename: code_aimpetus-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: code_aimpetus-0.1.2.dist-info/licenses/LICENSE
+Filename: code_aimpetus-0.2.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: code_aimpetus-0.1.2.dist-info/RECORD
+Filename: code_aimpetus-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## code_aimpetus/__main__.py

```diff
@@ -1,15 +1,16 @@
 import click
-from .celery import start_app
 
 from code_aimpetus.gh.issues.close import close_issue
 from code_aimpetus.gh.issues.list import list_issues
 from code_aimpetus.gh.pull_requests.list import list_pull_requests
 from code_aimpetus.gh.repo import create_github_repo
 
+from .celery import start_app
+
 
 @click.group()
 def cli():
     pass
 
 
 cli.add_command(list_pull_requests)
```

## code_aimpetus/celery.py

```diff
@@ -1,17 +1,13 @@
-import os
-
 import click
 from celery import Celery
-from dotenv import load_dotenv
 
-load_dotenv()
+from code_aimpetus.settings import BROKER_URL
 
 # Initialize Celery with Redis as the broker
-broker_url = os.getenv("CELERY_BROKER_URL", "redis://:codeai@redis:6379/0")
 
-app = Celery("codeai", broker=broker_url, backend=broker_url)
+app = Celery("codeai", broker=BROKER_URL, backend=BROKER_URL)
 
 
 @click.command()
 def start_app():
     app.start()
```

## code_aimpetus/gh/repo.py

```diff
@@ -1,25 +1,32 @@
-import os
-
 import click
+from common_options import apply_github_token
 from github import Github
+from loguru import logger
 
 
 @click.command()
-@click.option(
-    "--token",
-    help="Your GitHub access token",
-    default=os.environ.get("GITHUB_TOKEN", ""),
-)
+@apply_github_token
 @click.option("--repo_name", help="The name of the new repository", required=True)
 @click.option("--description", help="The description of the new repository", default="")
 @click.option("--private", help="Set the repository to private", is_flag=True)
 def create_github_repo(token, repo_name, description=None, private=False):
+    """
+    Create a new GitHub repository
+
+    Args:
+        token (str): GitHub access token
+        repo_name (str): The name of the new repository
+        description (str): The description of the new repository
+        private (bool): Set the repository to private
+
+    Returns:
+        github.Repository.Repository: A GitHub repository object."""
     g = Github(token)
     user = g.get_user()
     try:
         repo = user.create_repo(repo_name, description=description, private=private)
-        print(f"Successfully created repository: {repo_name}")
+        logger.info(f"Successfully created repository: {repo}")
         return repo
     except Exception as e:
-        print(f"Error creating repository: {e}")
+        logger.info(f"Error creating repository: {e}")
         return None
```

## code_aimpetus/gh/issues/close.py

```diff
@@ -1,25 +1,42 @@
-import os
-
 import click
+from common_options import apply_github_options
+from gh.issues.get import get_issue
 from github import Github
+from loguru import logger
 
 
 @click.command()
-@click.option(
-    "--token",
-    help="Your GitHub access token",
-    default=os.environ.get("GITHUB_TOKEN", ""),
-)
-@click.option(
-    "--owner", help="Repository owner", default=os.environ.get("GITHUB_OWNER", "")
-)
-@click.option(
-    "--repo", help="Repository name", default=os.environ.get("GITHUB_REPO", "")
-)
+@apply_github_options
 @click.option("--issue_number", type=int, help="Issue number to close")
-def close_issue(token, owner, repo, issue_number):
+def close_issue(token, owner, repo, issue_number) -> None:
+    """
+    Close an issue for a given repository
+
+    Args:
+        token (str): GitHub access token.
+        owner (str): Repository owner.
+        repo (str): Repository name.
+        issue_number (int): Issue number to close.
+
+    Returns:
+        None
+    """
     g = Github(token)
     repo = g.get_repo(f"{owner}/{repo}")
-    issue = repo.get_issue(issue_number)
+    issue = get_issue(issue_number)
+    close_gh_issue(issue)
+
+
+def close_gh_issue(issue) -> None:
+    """
+    Close an issue for a given repository
+
+    Args:
+        issue (github.Issue.Issue): A GitHub issue object.
+
+    Returns:
+        None
+    """
+
     issue.edit(state="closed")
-    print(f"Closed issue #{issue_number}")
+    logger.info(f"Closed issue #{issue.number}")
```

## code_aimpetus/gh/issues/list.py

```diff
@@ -1,25 +1,30 @@
-import os
-
 import click
-from github import Github
+from common_options import apply_github_options
+from github.Issue import Issue
+from github.PaginatedList import PaginatedList
+from github.Repository import Repository
+from loguru import logger
+
+from code_aimpetus.gh.utility import get_repo
 
 
 @click.command()
-@click.option(
-    "--token",
-    help="Your GitHub access token",
-    default=os.environ.get("GITHUB_TOKEN", ""),
-)
-@click.option(
-    "--owner", help="Repository owner", default=os.environ.get("GITHUB_OWNER", "")
-)
-@click.option(
-    "--repo", help="Repository name", default=os.environ.get("GITHUB_REPO", "")
-)
-def list_issues(token, owner, repo):
-    g = Github(token)
-    repo = g.get_repo(f"{owner}/{repo}")
+@apply_github_options
+def list_issues(token: str, owner: str, repo: str) -> PaginatedList[Issue]:
+    """
+    List all issues for a given repository
+
+    Args:
+        token (str): GitHub access token.
+        owner (str): Repository owner.
+        repo (str): Repository name.
+
+    Returns:
+        github.PaginatedList.PaginatedList[github.Issue.Issue]:
+            A list of GitHub issue objects.
+    """
+    repo: Repository = get_repo(token, owner, repo)
     issues = repo.get_issues(state="open")
     for issue in issues:
-        print(f"#{issue.number}: {issue.title}")
+        logger.info(f"#{issue.number}: {issue.title}")
     return issues
```

## code_aimpetus/gh/pull_requests/list.py

```diff
@@ -1,24 +1,29 @@
-import os
-
 import click
-from github import Github
+from gh.utility import get_repo
+from github.PaginatedList import PaginatedList
+from github.PullRequest import PullRequest
+from loguru import logger
+
+from code_aimpetus.common_options import apply_github_options
 
 
 @click.command()
-@click.option(
-    "--token",
-    help="Your GitHub access token",
-    default=os.environ.get("GITHUB_TOKEN", ""),
-)
-@click.option(
-    "--owner", help="Repository owner", default=os.environ.get("GITHUB_OWNER", "")
-)
-@click.option(
-    "--repo", help="Repository name", default=os.environ.get("GITHUB_REPO", "")
-)
-def list_pull_requests(token, owner, repo):
-    g = Github(token)
-    repo = g.get_repo(f"{owner}/{repo}")
+@apply_github_options
+def list_pull_requests(token, owner, repo) -> PaginatedList[PullRequest]:
+    """
+    List all pull requests for a given repository
+
+    Args:
+        token (str): GitHub access token.
+        owner (str): Repository owner.
+        repo (str): Repository name.
+
+    Returns:
+        github.PaginatedList.PaginatedList[github.PullRequest.PullRequest]:
+            A list of GitHub pull request objects.
+    """
+    repo = get_repo(token, owner, repo)
     pull_requests = repo.get_pulls(state="open")
     for pr in pull_requests:
-        print(f"#{pr.number}: {pr.title}")
+        logger.info(f"#{pr.number}: {pr.title}")
+    return pull_requests
```

## Comparing `code_aimpetus-0.1.2.dist-info/METADATA` & `code_aimpetus-0.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-aimpetus
-Version: 0.1.2
+Version: 0.2.0
 Summary: Code.
 Project-URL: Homepage, https://github.com/BillSchumacher/CodeAImpteus
 Project-URL: Bug Tracker, https://github.com/BillSchumacher/CodeAImpteus
 Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `code_aimpetus-0.1.2.dist-info/licenses/LICENSE` & `code_aimpetus-0.2.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `code_aimpetus-0.1.2.dist-info/RECORD` & `code_aimpetus-0.2.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 code_aimpetus/__init__.py,sha256=yHZr4lXRn-CwKqk6nIa2fdyamKlaSeAX513DYAy9ZZA,118
-code_aimpetus/__main__.py,sha256=7bFBprt_V914K4ntGYpJCNxnBA4uCkObnQbFipkp1Bc,527
-code_aimpetus/celery.py,sha256=dEY_n5znKoOniDs2Gb3Es-eN-HkZ60LhDtauPRtY7Oc,350
+code_aimpetus/__main__.py,sha256=BwryVn7AiYYEvkISA-PdrUsTpGEjfjbO3Wa_R1bBFwI,529
+code_aimpetus/celery.py,sha256=L-wjIeBKFLcFSGotDRxKw76lpimuhQu7SoDkbo7zkHo,260
+code_aimpetus/common_options.py,sha256=QJ_P-G-9PWPrYqJ284O2CRvRCSLULeUZAn0kuqqgEd0,569
+code_aimpetus/settings.py,sha256=xoPFtWqfjglSA0zeBTjCQ7AW8opwI7m5TlBFZZSp6K8,294
 code_aimpetus/gh/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-code_aimpetus/gh/repo.py,sha256=G7FdBkZXl_cC-T9iFBQK_U9Wi0h8peglOmspIUwH7nU,856
+code_aimpetus/gh/repo.py,sha256=HnioQ-587i4rbBNFK_gWlSVcXpqxNpaFehm844WLtlE,1187
+code_aimpetus/gh/utility.py,sha256=zJE2QbIm7uEvOKUyygBO-fNqvr6_wLQCkZ3HPnB_04Q,462
 code_aimpetus/gh/issues/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-code_aimpetus/gh/issues/close.py,sha256=N4IvjBJYgC971gyBdAOCZGGvtymPgGHSKXz29tcMw40,709
-code_aimpetus/gh/issues/list.py,sha256=Y7tsdT3OCy-cCMjO7WVpS10pEOwouImtg2WiXi7DUGg,643
+code_aimpetus/gh/issues/check_templates.py,sha256=7jsrbOlbrxuC0MzBNjnE64YWPgmlmkwvMaNmqZmSk3Q,1272
+code_aimpetus/gh/issues/close.py,sha256=N_4NB5_XGiDfjHgNBU_0LekMTHls1y6MpUMYAx4ImE4,1026
+code_aimpetus/gh/issues/get.py,sha256=jabubEAGj3XGMrCeOSJZrLXc67wiq_0Opj4WgGcZpvg,724
+code_aimpetus/gh/issues/list.py,sha256=3vqHthE8lebfgnw7R9dGKisaVZPDoCPtztPdYYSRt2Q,903
 code_aimpetus/gh/pull_requests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-code_aimpetus/gh/pull_requests/list.py,sha256=RKJq1LqlB880bf46pPWGp3ECHpr2kkXSmoI4sGY0iAQ,635
-code_aimpetus-0.1.2.dist-info/METADATA,sha256=QIm384fdWsclKfCVOO7GnSFu1MwOi3lbE68XBdIuaSk,986
-code_aimpetus-0.1.2.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
-code_aimpetus-0.1.2.dist-info/entry_points.txt,sha256=sAV4Xu1Nm6EBUKvDngEFjyi59m4jV0H4poDUecPP3XM,54
-code_aimpetus-0.1.2.dist-info/licenses/LICENSE,sha256=UNCyTrL3doVY4uukQXlEkFM8XJd1GM9QGSh3ElWaO0Y,1092
-code_aimpetus-0.1.2.dist-info/RECORD,,
+code_aimpetus/gh/pull_requests/list.py,sha256=T1XLAJbt3y9kM5OtJGWguEumWvZJ8i-akD7GTWiTPJ8,896
+code_aimpetus-0.2.0.dist-info/METADATA,sha256=2eamtPlexw5BqvYQkljgIgEZA--HlwNMelRMM7nfERA,986
+code_aimpetus-0.2.0.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+code_aimpetus-0.2.0.dist-info/entry_points.txt,sha256=sAV4Xu1Nm6EBUKvDngEFjyi59m4jV0H4poDUecPP3XM,54
+code_aimpetus-0.2.0.dist-info/licenses/LICENSE,sha256=UNCyTrL3doVY4uukQXlEkFM8XJd1GM9QGSh3ElWaO0Y,1092
+code_aimpetus-0.2.0.dist-info/RECORD,,
```

