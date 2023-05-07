# Comparing `tmp/xefab-0.1.8.tar.gz` & `tmp/xefab-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xefab-0.1.8.tar", max compression
+gzip compressed data, was "xefab-0.1.9.tar", max compression
```

## Comparing `xefab-0.1.8.tar` & `xefab-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    14289 2023-03-05 16:41:18.139472 xefab-0.1.8/README.rst
--rw-r--r--   0        0        0     1483 2023-03-05 16:41:18.139472 xefab-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       35 2023-03-05 16:41:18.139472 xefab-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0      999 2023-03-05 16:41:18.139472 xefab-0.1.8/tests/test_xefab.py
--rw-r--r--   0        0        0      131 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/__init__.py
--rw-r--r--   0        0        0     2321 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/collection.py
--rw-r--r--   0        0        0     6119 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/config.py
--rw-r--r--   0        0        0     1750 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/entrypoints.py
--rw-r--r--   0        0        0     3732 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/file_access.py
--rw-r--r--   0        0        0       53 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/hosts/__init__.py
--rw-r--r--   0        0        0      287 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/hosts/osg.py
--rw-r--r--   0        0        0        0 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/hosts/uchicago/__init__.py
--rw-r--r--   0        0        0      602 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/hosts/uchicago/dali.py
--rw-r--r--   0        0        0      699 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/hosts/uchicago/midway.py
--rw-r--r--   0        0        0    11931 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/main.py
--rw-r--r--   0        0        0     4823 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/pydantic_support.py
--rw-r--r--   0        0        0     1903 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/ssh_client.py
--rw-r--r--   0        0        0       34 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/tasks/__init__.py
--rw-r--r--   0        0        0     1093 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/tasks/admin.py
--rw-r--r--   0        0        0    12326 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/tasks/batchq.py
--rw-r--r--   0        0        0     1667 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/tasks/condorq.py
--rw-r--r--   0        0        0     6438 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/tasks/github.py
--rw-r--r--   0        0        0     5664 2023-03-05 16:41:18.139472 xefab-0.1.8/xefab/tasks/install.py
--rw-r--r--   0        0        0    16553 2023-03-05 16:41:18.143472 xefab-0.1.8/xefab/tasks/jupyter.py
--rw-r--r--   0        0        0     2107 2023-03-05 16:41:18.143472 xefab-0.1.8/xefab/tasks/main.py
--rw-r--r--   0        0        0     5748 2023-03-05 16:41:18.143472 xefab-0.1.8/xefab/tasks/mc_chain.py
--rw-r--r--   0        0        0     1620 2023-03-05 16:41:18.143472 xefab-0.1.8/xefab/tasks/secrets.py
--rw-r--r--   0        0        0     4239 2023-03-05 16:41:18.143472 xefab-0.1.8/xefab/tasks/shell.py
--rw-r--r--   0        0        0     1874 2023-03-05 16:41:18.143472 xefab-0.1.8/xefab/tasks/squeue.py
--rw-r--r--   0        0        0     6400 2023-03-05 16:41:18.143472 xefab-0.1.8/xefab/tasks/transfer.py
--rw-r--r--   0        0        0     2685 2023-03-05 16:41:18.143472 xefab-0.1.8/xefab/tasks/utils.py
--rw-r--r--   0        0        0     7191 2023-03-05 16:41:18.143472 xefab-0.1.8/xefab/utils.py
--rw-r--r--   0        0        0    15475 1970-01-01 00:00:00.000000 xefab-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    14289 2023-03-24 09:06:24.949983 xefab-0.1.9/README.rst
+-rw-r--r--   0        0        0     1483 2023-03-24 09:06:24.949983 xefab-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-03-24 09:06:24.949983 xefab-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      999 2023-03-24 09:06:24.949983 xefab-0.1.9/tests/test_xefab.py
+-rw-r--r--   0        0        0      131 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/__init__.py
+-rw-r--r--   0        0        0     2321 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/collection.py
+-rw-r--r--   0        0        0     6119 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/config.py
+-rw-r--r--   0        0        0     1750 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/entrypoints.py
+-rw-r--r--   0        0        0     3732 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/file_access.py
+-rw-r--r--   0        0        0       53 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/hosts/__init__.py
+-rw-r--r--   0        0        0      287 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/hosts/osg.py
+-rw-r--r--   0        0        0        0 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/hosts/uchicago/__init__.py
+-rw-r--r--   0        0        0      602 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/hosts/uchicago/dali.py
+-rw-r--r--   0        0        0      699 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/hosts/uchicago/midway.py
+-rw-r--r--   0        0        0    11931 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/main.py
+-rw-r--r--   0        0        0     4823 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/pydantic_support.py
+-rw-r--r--   0        0        0     1903 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/ssh_client.py
+-rw-r--r--   0        0        0       34 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/tasks/__init__.py
+-rw-r--r--   0        0        0     1093 2023-03-24 09:06:24.949983 xefab-0.1.9/xefab/tasks/admin.py
+-rw-r--r--   0        0        0    12326 2023-03-24 09:06:24.953983 xefab-0.1.9/xefab/tasks/batchq.py
+-rw-r--r--   0        0        0     1667 2023-03-24 09:06:24.953983 xefab-0.1.9/xefab/tasks/condorq.py
+-rw-r--r--   0        0        0     6438 2023-03-24 09:06:24.953983 xefab-0.1.9/xefab/tasks/github.py
+-rw-r--r--   0        0        0     5664 2023-03-24 09:06:24.953983 xefab-0.1.9/xefab/tasks/install.py
+-rw-r--r--   0        0        0    19354 2023-03-24 09:06:24.953983 xefab-0.1.9/xefab/tasks/jupyter.py
+-rw-r--r--   0        0        0     2107 2023-03-24 09:06:24.953983 xefab-0.1.9/xefab/tasks/main.py
+-rw-r--r--   0        0        0     5757 2023-03-24 09:06:24.953983 xefab-0.1.9/xefab/tasks/mc_chain.py
+-rw-r--r--   0        0        0     1620 2023-03-24 09:06:24.953983 xefab-0.1.9/xefab/tasks/secrets.py
+-rw-r--r--   0        0        0     4239 2023-03-24 09:06:24.953983 xefab-0.1.9/xefab/tasks/shell.py
+-rw-r--r--   0        0        0     1889 2023-03-24 09:06:24.953983 xefab-0.1.9/xefab/tasks/squeue.py
+-rw-r--r--   0        0        0     6400 2023-03-24 09:06:24.953983 xefab-0.1.9/xefab/tasks/transfer.py
+-rw-r--r--   0        0        0     2685 2023-03-24 09:06:24.953983 xefab-0.1.9/xefab/tasks/utils.py
+-rw-r--r--   0        0        0     7191 2023-03-24 09:06:24.953983 xefab-0.1.9/xefab/utils.py
+-rw-r--r--   0        0        0    15475 1970-01-01 00:00:00.000000 xefab-0.1.9/PKG-INFO
```

### Comparing `xefab-0.1.8/README.rst` & `xefab-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/pyproject.toml` & `xefab-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "xefab"
-version = "0.1.8"
+version = "0.1.9"
 homepage = "https://github.com/jmosbacher/xefab"
 description = "Top-level package for xefab."
 authors = ["Yossi Mosbacher <joe.mosbacher@gmail.com>"]
 readme = "README.rst"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
```

### Comparing `xefab-0.1.8/tests/test_xefab.py` & `xefab-0.1.9/tests/test_xefab.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/collection.py` & `xefab-0.1.9/xefab/collection.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/config.py` & `xefab-0.1.9/xefab/config.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/entrypoints.py` & `xefab-0.1.9/xefab/entrypoints.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/file_access.py` & `xefab-0.1.9/xefab/file_access.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/hosts/uchicago/dali.py` & `xefab-0.1.9/xefab/hosts/uchicago/dali.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/hosts/uchicago/midway.py` & `xefab-0.1.9/xefab/hosts/uchicago/midway.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/main.py` & `xefab-0.1.9/xefab/main.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/pydantic_support.py` & `xefab-0.1.9/xefab/pydantic_support.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/ssh_client.py` & `xefab-0.1.9/xefab/ssh_client.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/tasks/admin.py` & `xefab-0.1.9/xefab/tasks/admin.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/tasks/batchq.py` & `xefab-0.1.9/xefab/tasks/batchq.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/tasks/condorq.py` & `xefab-0.1.9/xefab/tasks/condorq.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/tasks/github.py` & `xefab-0.1.9/xefab/tasks/github.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/tasks/install.py` & `xefab-0.1.9/xefab/tasks/install.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/tasks/jupyter.py` & `xefab-0.1.9/xefab/tasks/jupyter.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 import time
 from io import BytesIO, StringIO
 from random import choices
 from string import ascii_lowercase
 
 from fabric.tasks import task
 from rich.progress import SpinnerColumn, TextColumn
+from rich.prompt import IntPrompt
+from xefab.tasks.shell import is_file
 
 from xefab.utils import ProgressContext, console, get_open_port
 
-from .squeue import parse_squeue_output
+from .squeue import parse_squeue_output, squeue
 from .utils import print_splash
 
 JOB_NAME = "xefab-jupyter"
 
 
 JOB_HEADER = """#!/bin/bash
 #SBATCH --job-name={job_name}
@@ -24,15 +26,15 @@
 #SBATCH --ntasks=1
 #SBATCH --cpus-per-task={n_cpu}
 #SBATCH --mem-per-cpu={mem_per_cpu}
 #SBATCH --time={max_hours}:00:00
 {extra_header}
 
 export NUMEXPR_MAX_THREADS={n_cpu}
-echo Starting jupyter job
+
 
 """
 
 GPU_HEADER = """\
 #SBATCH --partition=gpu2
 #SBATCH --gres=gpu:1
 
@@ -46,27 +48,36 @@
 """
 
 
 # This is only if the user is NOT starting the singularity container
 # (for singularity, starting jupyter is done in _xentenv_inner)
 START_JUPYTER = """
 echo $PYTHONPATH
+echo Starting jupyter job
+
 jupyter {jupyter} --no-browser --port={port} --ip=0.0.0.0 --notebook-dir {notebook_dir} 2>&1
 """
 
 
 START_JUPYTER_SINGULARITY = """
+SINGULARITY_CACHEDIR=$TMPDIR/singularity_cache
 
-SINGULARITY_CACHEDIR=/home/{user}/scratch/singularity_cache
+mkdir -p $SINGULARITY_CACHEDIR
+
+# SINGULARITY_CACHEDIR=/home/{user}/scratch/singularity_cache
+echo Loading singularity module
 
 module load singularity
 
-singularity exec {bind_str} {container} jupyter {jupyter} --no-browser --port={port} --ip=0.0.0.0 --notebook-dir {notebook_dir}
-"""
+echo Starting jupyter job
 
+singularity exec {bind_str} {container} jupyter {jupyter} --no-browser --port={port} --ip=0.0.0.0 
+
+"""
+# --notebook-dir {notebook_dir}
 
 @task(
     pre=[print_splash],
     help={
         "env": "Environment to run on",
         "partition": "Partition to run on (xenon1t or dali)",
         "bypass_reservation": "Dont attempt to use the xenon notebook reservation",
@@ -115,22 +126,14 @@
     debug: bool = False,
 ):
     """Start a jupyter analysis notebook on the remote \
 host and forward to local port via ssh-tunnel."""
 
     REMOTE_HOME = f"/home/{c.user}"
 
-    unique_id = "".join(choices(ascii_lowercase, k=4))
-    date = time.strftime("%Y%m%d")
-
-    job_name = f"jupyter_{unique_id}_{date}"
-    job_folder = f"{REMOTE_HOME}/xefab_jobs/{job_name}"
-
-    server_details_path = f"{job_folder}/server_details.json"
-
     if image_dir is None:
         image_dir = "/project2/lgrandi/xenonnt/singularity-images"
 
     if notebook_dir is None:
         notebook_dir = REMOTE_HOME
 
     if remote_port is None:
@@ -141,39 +144,91 @@
 
     # bind directories inside the container
     if binds is None:
         binds = f"/project2,/scratch/midway2/{c.user},/dali"
     if isinstance(binds, str):
         binds = [bind.strip() for bind in binds.split(",")]
     
-    if partition == "xenon1t" and '/dali' not in binds:
+    if partition == "xenon1t":
         binds.append("/project2/lgrandi/xenonnt/dali/lgrandi/xenonnt/software/cutax:/xenon/xenonnt/software/cutax")
 
     bind_str = " ".join([f"--bind {bind}" for bind in binds])
 
-    console.print(f"Using partition {partition}", style="info")
+    console.print(f"Using partition {partition}")
 
     local_port = get_open_port(start=local_port)
     env_vars = {}
 
     if local_cutax:
         console.print(
             "Container cutax being overwritten by user installed package.",
             style="warning",
         )
         env_vars["INSTALL_CUTAX"] = "0"
 
+    
+    if not force_new:
+        with ProgressContext() as progress:
+            existing_jobs = {}
+            with progress.enter_task("Checking for existing jobs") as task:
+                # Check for existing jobs
+                existing_jobs = get_existing_jobs(c)
+
+                if existing_jobs:
+                    progress.update(task, description="Found existing jobs.")
+                else:
+                    progress.update(task, description="No existing jobs found.")
+
+        if existing_jobs:
+            console.print("Found existing jobs, options:")
+            progress.console.print(f"(0): Start new job",)
+            jobnames = list(existing_jobs)
+            for i, job_name in enumerate(jobnames):
+                console.print(
+                    f"({i+1}): {job_name}", 
+                )
+            
+            selection = IntPrompt.ask(
+                "Select a job to connect to or start new job",
+                choices=list(map(str,range(0, len(jobnames) + 1))),
+                console=progress.console, default='0',
+            )
+    
+
+            if selection < len(jobnames) + 1:
+                job_name = jobnames[selection - 1]
+                server_details = existing_jobs[job_name]
+                job_folder = f"{REMOTE_HOME}/xefab_jobs/{job_name}"
+
+                with ProgressContext() as progress:
+                    attach_to_job(c, job_id=server_details['job_id'], local_port=local_port, 
+                                remote_host=server_details['remote_host'],
+                                remote_port=server_details['remote_port'], 
+                                token=server_details['token'], progress=progress,
+                                job_folder=job_folder, no_browser=no_browser, 
+                                detached=detached, debug=debug)
+                    return
+
     with ProgressContext() as progress:
+        unique_id = "".join(choices(ascii_lowercase, k=4))
+        date = time.strftime("%Y%m%d")
+
+        job_name = f"jupyter_{unique_id}_{date}" 
+        job_folder = f"{REMOTE_HOME}/xefab_jobs/{job_name}"
+
+        server_details_path = f"{job_folder}/server_details.json"
+
         with progress.enter_task("Checking connection and destination folder"):
             if not c.run(f"test -d {job_folder}", warn=True).ok:
                 progress.console.print(f"Creating {job_folder} on {c.host}")
                 c.run("mkdir -p " + job_folder)
 
         if env == "singularity":
-            s_container = f"{image_dir}/xenonnt-{tag}.simg"
+            s_container = f"/cvmfs/singularity.opensciencegrid.org/xenonnt/base-environment:{tag}"
+            # s_container = f"{image_dir}/xenonnt-{tag}.simg"
 
             # Add the singularity runner script to the batch job
             # batch_job = JOB_HEADER + f"{starter_path} "
             batch_job = JOB_HEADER + START_JUPYTER_SINGULARITY.format(
                 user=c.user,
                 bind_str=bind_str,
                 container=s_container,
@@ -353,18 +408,16 @@
                 )
 
             console.print("\nJupyter started succesfully.")
             console.print(f"Remote URL: \n{url}\n")
             remote_host, remote_port = url.split("/")[2].split(":")
             if "token" in url:
                 token = url.split("?")[1].split("=")[1]
-                local_url = f"http://localhost:{local_port}?token={token}"
             else:
                 token = ""
-                local_url = f"http://localhost:{local_port}"
 
         # Can never be too careful, make sure port numbers are integers
         local_port = int(local_port)
         remote_port = int(remote_port)
 
         server_details = {
             "job_id": job_id,
@@ -379,81 +432,105 @@
             "Writing server details to file",
             finished_description="Server details saved",
             warn=True,
         ):
             details_fd = StringIO(json.dumps(server_details, indent=4))
             c.put(details_fd, remote=server_details_path)
 
+        attach_to_job(c, job_id=job_id, local_port=local_port, remote_host=remote_host,
+            remote_port=remote_port, token=token, progress=progress, job_folder=job_folder,
+            no_browser=no_browser, detached=detached, debug=debug)
+
+def attach_to_job(c, *, job_id, local_port, remote_host, 
+            remote_port, token, progress, job_folder,
+            no_browser=False, detached=False, debug=False):
+    """Attach to a running job."""
+
         # Handle port forwarding
-        msg = f"Forwarding remote address {remote_host}:{remote_port} to local port {local_port}"
-        if not detached:
-            extra_msg = (
-                f"\nYou can access the notebook at \n{local_url}\n"
-                "   Press ENTER or CTRL-C to deactivate and cancel job."
-            )
-            with progress.enter_task(
-                msg + extra_msg,
-                exception_description="Exception raised while forwarding port",
-                warn=True,
-            ) as task:
-                with c.forward_local(
-                    local_port, remote_port=remote_port, remote_host=remote_host
-                ):
-                    time.sleep(3)
+    if token:
+        local_url = f"http://localhost:{local_port}?token={token}"
+    else:
+        local_url = f"http://localhost:{local_port}"
+    msg = f"Forwarding remote address {remote_host}:{remote_port} to local port {local_port}"
+    if not detached:
+        extra_msg = (
+            f"\nYou can access the notebook at \n{local_url}\n"
+            "   Press ENTER or CTRL-C to deactivate and cancel job."
+        )
+        with progress.enter_task(
+            msg + extra_msg,
+            exception_description="Exception raised while forwarding port",
+            warn=True,
+        ) as task:
+            with c.forward_local(
+                local_port, remote_port=remote_port, remote_host=remote_host
+            ):
+                time.sleep(3)
 
-                    if not no_browser:
-                        result = c.local(
-                            f"python -m webbrowser -t {local_url}", hide=True, warn=True
-                        )
-                    try:
-                        r = progress.console.input()
-                        progress.update(
-                            task, description="Deactivating port forwarding"
-                        )
-                        time.sleep(2)
-                    except KeyboardInterrupt:
-                        console.print("Keyboard interrupt received.")
-                    except Exception as e:
-                        if debug:
-                            console.print(f"Exception raised: {e}")
-                        else:
-                            console.print(f"Exception raised.")
+                if not no_browser:
+                    result = c.local(
+                        f"python -m webbrowser -t {local_url}", hide=True, warn=True
+                    )
+                try:
+                    r = progress.console.input()
+                    progress.update(
+                        task, description="Deactivating port forwarding"
+                    )
+                    time.sleep(2)
+                except KeyboardInterrupt:
+                    console.print("Keyboard interrupt received.")
+                except Exception as e:
+                    if debug:
+                        console.print(f"Exception raised: {e}")
+                    else:
+                        console.print(f"Exception raised.")
+
+        with progress.enter_task(
+            "Canceling job",
+            finished_description="Job canceled",
+            exception_description=f"Could not cancel job. Please cancel it manually. Job ID: {job_id}",
+            warn=True,
+        ):
+            c.run(f"scancel {job_id}", hide=True)
 
+        if not debug:
             with progress.enter_task(
-                "Canceling job",
-                finished_description="Job canceled",
-                exception_description=f"Could not cancel job. Please cancel it manually. Job ID: {job_id}",
-                warn=True,
+                "Cleaning up job files",
+                finished_description="Job folder removed",
+                exception_description=f"Could not remove job folder. Please remove it manually. Path: {job_folder}",
             ):
-                c.run(f"scancel {job_id}", hide=True)
-
-            if not debug:
-                with progress.enter_task(
-                    "Cleaning up job files",
-                    finished_description="Job folder removed",
-                    exception_description=f"Could not remove job folder. Please remove it manually. Path: {job_folder}",
-                ):
-                    for _ in range(3):
-                        time.sleep(2)
-                        result = c.run(f"rm -rf {job_folder}", hide=True, warn=True)
-                        if result.ok:
-                            break
-                    else:
-                        raise
+                for _ in range(3):
+                    time.sleep(2)
+                    result = c.run(f"rm -rf {job_folder}", hide=True, warn=True)
+                    if result.ok:
+                        break
+                else:
+                    raise
 
-        else:
-            # Detached mode - just forward the port and exit
-            with progress.enter_task(msg, warn=True) as task:
-                result = c.local(
-                    f"ssh -fN -L {local_port}:{remote_host}:{remote_port} {c.user}@{c.host} &",
-                    disown=True,
-                    hide=False,
-                    warn=True,
+    else:
+        # Detached mode - just forward the port and exit
+        with progress.enter_task(msg, warn=True) as task:
+            result = c.local(
+                f"ssh -fN -L {local_port}:{remote_host}:{remote_port} {c.user}@{c.host} &",
+                disown=True,
+                hide=False,
+                warn=True,
+            )
+            time.sleep(3)
+            console.print(f"You can access the notebook at \n{local_url}\n")
+            if result.ok and not no_browser:
+                c.local(
+                    f"python -m webbrowser -t {local_url}", hide=True, warn=True
                 )
-                time.sleep(3)
-                console.print(f"You can access the notebook at \n{local_url}\n")
-                if result.ok and not no_browser:
-                    c.local(
-                        f"python -m webbrowser -t {local_url}", hide=True, warn=True
-                    )
 
     console.print("Goodbye!")
+
+
+def get_existing_jobs(c):
+    """Find all running jupyter jobs on the remote host."""
+    df = squeue(c, hide=True)
+    running = {}
+    for job_name in df["NAME"]:
+        details_path = f"/home/{c.user}/xefab_jobs/{job_name}/server_details.json"
+        if job_name.startswith('jupyter') and is_file(c, details_path, hide=True):
+            running[job_name] = json.loads(c.run(f"cat {details_path}", hide=True).stdout)
+    return running
```

### Comparing `xefab-0.1.8/xefab/tasks/main.py` & `xefab-0.1.9/xefab/tasks/main.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/tasks/mc_chain.py` & `xefab-0.1.9/xefab/tasks/mc_chain.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from fabric.tasks import task
 from invoke.watchers import Responder
 from rich.console import Group
 from rich.live import Live
 from rich.panel import Panel
 from rich.text import Text
+from rich.prompt import Confirm
 
 from xefab.utils import ProgressContext, console
 
 from .github import clone
 from .shell import exists
 from .utils import print_splash
 
@@ -136,14 +137,14 @@
                             exit(0)
                     time.sleep(2)
         except KeyboardInterrupt:
             pass
 
         except Exception as e:
             console.print(e)
-    if remove_command is not None:
-        resp = console.input("Cancel workflow? \[y/N]: ")
-        if resp.lower() in ["y", "yes"]:
+    if remove_command is not None:        
+        cancel = Confirm.ask("Cancel workflow?")
+        if cancel:
             with c.cd(repo_dir):
                 with c.prefix("source setup_env.sh"):
                     c.run(f"{remove_command}")
     console.print("Goodbye!")
```

### Comparing `xefab-0.1.8/xefab/tasks/secrets.py` & `xefab-0.1.9/xefab/tasks/secrets.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/tasks/shell.py` & `xefab-0.1.9/xefab/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/tasks/squeue.py` & `xefab-0.1.9/xefab/tasks/squeue.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,16 @@
             row_data[name] = field
         squeue_data.append(row_data)
     return pd.DataFrame(squeue_data, columns=header_fields).dropna(how="all")
 
 
 @task(aliases=["job-queue"])
 def squeue(
-    c: Connection, user: str = "me", partition: str = None, out: str = ""
+    c: Connection, user: str = "me", partition: str = None, out: str = "", 
+    hide: bool = False, warn: bool = False,
 ) -> pd.DataFrame:
     """Get the job-queue status."""
 
     command = 'squeue --format="%.18i %.9P %.30j %.8u %.8T %.10M %.9l %.6D %R"'
 
     if user in ["*", "all"]:
         pass
@@ -37,29 +38,30 @@
         command += f" -u {c.user}"
     else:
         command += f" -u {user}"
 
     if partition:
         command += f" -p {partition}"
 
-    with console.status(f"Running {command} on {c.host}..."):
-        r = c.run(command, hide=True, warn=True)
-        squeue_output = r.stdout
-    if r.failed:
+    
+    r = c.run(command, hide=hide, warn=True)
+    squeue_output = r.stdout
+    if r.failed and not warn:
         console.print("Remote execution of squeue on {c.host} failed. stderr:")
         console.print(r.stderr)
         exit(r.return_code)
 
     df = parse_squeue_output(squeue_output)
 
     if out:
         with console.status(f"Saving squeue output to {out}..."):
             df.to_csv(out, index=False)
             time.sleep(0.5)
         console.print(f"Output written to {out}")
-    else:
+    if not hide:
         table = df_to_table(df)
         if len(df) > 10:
             with console.pager():
                 console.print(table)
         else:
             console.print(table)
+    return df
```

### Comparing `xefab-0.1.8/xefab/tasks/transfer.py` & `xefab-0.1.9/xefab/tasks/transfer.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/tasks/utils.py` & `xefab-0.1.9/xefab/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/xefab/utils.py` & `xefab-0.1.9/xefab/utils.py`

 * *Files identical despite different names*

### Comparing `xefab-0.1.8/PKG-INFO` & `xefab-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xefab
-Version: 0.1.8
+Version: 0.1.9
 Summary: Top-level package for xefab.
 Home-page: https://github.com/jmosbacher/xefab
 Author: Yossi Mosbacher
 Author-email: joe.mosbacher@gmail.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

