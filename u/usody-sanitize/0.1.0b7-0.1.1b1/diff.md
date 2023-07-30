# Comparing `tmp/usody_sanitize-0.1.0b7.tar.gz` & `tmp/usody_sanitize-0.1.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usody_sanitize-0.1.0b7.tar", max compression
+gzip compressed data, was "usody_sanitize-0.1.1b1.tar", max compression
```

## Comparing `usody_sanitize-0.1.0b7.tar` & `usody_sanitize-0.1.1b1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    18092 2023-02-19 02:19:59.304629 usody_sanitize-0.1.0b7/LICENSE
--rwxr-xr-x   0        0        0     4349 2023-04-19 05:21:38.796418 usody_sanitize-0.1.0b7/README.md
--rwxr-xr-x   0        0        0      744 2023-04-29 09:15:17.568121 usody_sanitize-0.1.0b7/pyproject.toml
--rwxr-xr-x   0        0        0       28 2023-04-29 09:15:17.571454 usody_sanitize-0.1.0b7/usody_sanitize/__init__.py
--rw-r--r--   0        0        0     2498 2023-05-02 07:52:43.370341 usody_sanitize-0.1.0b7/usody_sanitize/cmd_client.py
--rwxr-xr-x   0        0        0     4785 2023-04-19 05:21:37.169737 usody_sanitize-0.1.0b7/usody_sanitize/commands.py
--rwxr-xr-x   0        0        0    11955 2023-05-02 07:53:50.674347 usody_sanitize-0.1.0b7/usody_sanitize/erasure.py
--rwxr-xr-x   0        0        0     1120 2023-04-17 03:46:30.428865 usody_sanitize-0.1.0b7/usody_sanitize/main.py
--rw-r--r--   0        0        0     2975 2023-04-17 04:17:15.564592 usody_sanitize-0.1.0b7/usody_sanitize/methods.py
--rw-r--r--   0        0        0      206 2023-02-21 01:32:23.532667 usody_sanitize-0.1.0b7/usody_sanitize/schemas/__init__.py
--rw-r--r--   0        0        0      716 2023-02-21 01:33:13.740208 usody_sanitize-0.1.0b7/usody_sanitize/schemas/devices.py
--rw-r--r--   0        0        0     5368 2023-04-17 03:38:26.941252 usody_sanitize-0.1.0b7/usody_sanitize/schemas/erasure.py
--rw-r--r--   0        0        0     3635 2023-02-03 16:48:51.000000 usody_sanitize-0.1.0b7/usody_sanitize/schemas/export_data.py
--rwxr-xr-x   0        0        0     5412 2023-02-23 03:09:07.516501 usody_sanitize-0.1.0b7/usody_sanitize/steps.py
--rw-r--r--   0        0        0     1487 2023-02-22 05:49:02.035640 usody_sanitize-0.1.0b7/usody_sanitize/utils.py
--rw-r--r--   0        0        0     5327 1970-01-01 00:00:00.000000 usody_sanitize-0.1.0b7/setup.py
--rw-r--r--   0        0        0     5019 1970-01-01 00:00:00.000000 usody_sanitize-0.1.0b7/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-19 02:19:59.000000 usody_sanitize-0.1.1b1/LICENSE
+-rwxr-xr-x   0        0        0     1224 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/README.md
+-rwxr-xr-x   0        0        0      744 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/pyproject.toml
+-rwxr-xr-x   0        0        0       28 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/usody_sanitize/__init__.py
+-rw-r--r--   0        0        0     3108 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/usody_sanitize/cmd_client.py
+-rwxr-xr-x   0        0        0     4147 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/usody_sanitize/commands.py
+-rwxr-xr-x   0        0        0     2859 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/usody_sanitize/erasure.py
+-rw-r--r--   0        0        0     4049 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/usody_sanitize/methods.py
+-rw-r--r--   0        0        0     9898 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/usody_sanitize/sanitize.py
+-rw-r--r--   0        0        0      217 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/schemas/__init__.py
+-rw-r--r--   0        0        0     1880 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/schemas/definition.py
+-rw-r--r--   0        0        0      955 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/schemas/devices.py
+-rw-r--r--   0        0        0     3905 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/schemas/export_data.py
+-rw-r--r--   0        0        0     4186 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/schemas/sanitize.py
+-rwxr-xr-x   0        0        0     6891 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/steps.py
+-rw-r--r--   0        0        0     1522 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/utils.py
+-rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 usody_sanitize-0.1.1b1/PKG-INFO
```

### Comparing `usody_sanitize-0.1.0b7/LICENSE` & `usody_sanitize-0.1.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.0b7/pyproject.toml` & `usody_sanitize-0.1.1b1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usody-sanitize"
-version = "0.1.0-beta7"
+version = "0.1.1-beta1"
 
 description = "A tool to securely erase/wipe data on disks HDD and SSD with a proper sanitization process."
 repository = "https://github.com/usody/sanitize"
 authors = ["blkpws <me@blkpws.xyz>"]
 readme = "README.md"
 
 [tool.poetry_bumpversion.file."usody_sanitize/__init__.py"]
```

### Comparing `usody_sanitize-0.1.0b7/usody_sanitize/cmd_client.py` & `usody_sanitize-0.1.1b1/usody_sanitize/cmd_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,83 @@
-import sys
+import argparse
+import asyncio
+import datetime
 import json
 import logging
-import asyncio
-import argparse
+import pathlib
+import sys
 
 try:
     from usody_sanitize.erasure import DefaultMethods, auto_erase_disks
 except ModuleNotFoundError:
-    import pathlib
     sys.path.append(
         pathlib.Path(__file__).parent.parent.absolute().as_posix()
     )
     from usody_sanitize.erasure import DefaultMethods, auto_erase_disks
 
 from usody_sanitize import __version__ as app_version
 
-
 logging.getLogger("CMD")
 
 
+def parse_args():
+    parser = argparse.ArgumentParser(description='sanitize a disk')
+    parser.add_argument('-m', '--method', type=str, help='sanitize method',
+                        choices=['BASIC', 'BASELINE', 'ENHANCED'])
+
+    disk = parser.add_mutually_exclusive_group(required=True)
+    disk.add_argument('-d', '--device', type=str, action='append',
+                      help='path to the /dev/{disk} E.G.: /dev/sda')
+    disk.add_argument('-a', '--all', action='store_true',
+                      help='all disks unless the disk mounted as root')
+
+    parser.add_argument('--confirm', action='store_const', const=True,
+                        help='confirm to sanitize disks before proceed')
+
+    parser.add_argument('--version', action='version', version=app_version,
+                        help='show the version of usody_sanitize')
+
+    parser.add_argument('-l', '--log-level', dest='log_level', default='INFO',
+                        choices=['DEBUG', 'INFO', 'WARNING', 'ERROR',
+                                 'CRITICAL'],
+                        help='set the logging level (default: %(default)s)')
+
+    parser.add_argument('-o', '--output', default=".",
+                        help='set the output path to save the log file')
+
+    return parser.parse_args()
+
+
 def run_cmd():
     args = parse_args()
     configure_loggers(args.log_level)
 
     # Run erasures.
-    result = run_coroutine(auto_erase_disks(args.method, args.device))
-
-    # Todo: Add function to handle the result exports.
+    result = run_coroutine(
+        auto_erase_disks(args.method, args.device, confirm=args.confirm)
+    )
     logging.debug(json.dumps(result, indent=4))
-    with open('/tmp/erasure_output.json', 'w') as _fh:
-        json.dump(result, _fh, indent=4)
+
+    if not result:
+        return  # End here.
+
+    # Create export directory.
+    output_path = pathlib.Path(args.output)
+    if not output_path.exists():
+        output_path.mkdir(parents=True, exist_ok=True)
+        logging.debug(f"Creating directory `{output_path}`.")
+
+    # Export the output to a file.
+    for item in result:
+        item_serial_number = item.get('device_info', {}).get('serial_number')
+        current_date = datetime.datetime.now().date().isoformat()
+
+        file_name = f"{current_date}_{item_serial_number}.json"
+        with open(output_path / file_name, 'w') as _fh:
+            json.dump(item, _fh, indent=4)
 
 
 def configure_loggers(level="INFO"):
     logging.basicConfig(
         force=True,
         stream=sys.stdout,
         level=getattr(logging, level.upper()),
@@ -47,37 +91,9 @@
 
     try:
         return loop.run_until_complete(coro)
     finally:
         loop.close()
 
 
-def parse_args():
-    parser = argparse.ArgumentParser(description='sanitize a disk')
-    parser.add_argument('-m', '--method', type=str, help='sanitize method',
-                        choices=['BASIC', 'BASELINE', 'ENHANCED'])
-
-    # Select the
-    disk = parser.add_mutually_exclusive_group(required=True)
-    disk.add_argument('-d', '--device', type=str, action='append',
-                      help='path to the /dev/{disk} E.G.: /dev/sda')
-    disk.add_argument('-a', '--all', action='store_true',
-                      help='all disks unless the disk mounted as root')
-
-    parser.add_argument('--confirm', action='store_const', const=True,
-                        help='confirm to sanitize disks before proceed')
-
-    parser.add_argument('--version', action='version', version=app_version,
-                        help='show the version of usody_sanitize')
-
-    parser.add_argument('-l', '--log-level', dest='log_level', default='INFO',
-                        choices=['DEBUG', 'INFO', 'WARNING', 'ERROR',
-                                 'CRITICAL'],
-                        help='set the logging level (default: %(default)s)')
-
-    # Todo: Add output/export option.
-
-    return parser.parse_args()
-
-
 if __name__ == '__main__':
     run_cmd()
```

### Comparing `usody_sanitize-0.1.0b7/usody_sanitize/commands.py` & `usody_sanitize-0.1.1b1/usody_sanitize/commands.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,109 +1,53 @@
-import json
-import time
 import asyncio
+import json
 import logging
 import subprocess
-
+import time
+from pathlib import Path
 from typing import Optional, List, Any
+
 from usody_sanitize import schemas
 
 logger = logging.getLogger(__name__)
 
 
-async def list_blocks(
-        dev_path: Optional[str] = None,
-        children: bool = False,
-) -> List[schemas.Block]:
-    """Runs the command `lsblk` to get the information about devices.
-
-    Used maily to detect USB, live USB or disk attached.
-
-    :param Optional[str] dev_path:
-    :param bool children: Get partitions of each device.
-
-    :return:
-    """
-    command = ["lsblk", "-JOa" if children else "-JOad"]
-    logger.debug(f"Running command: `{command}`")
-    if dev_path:
-        command += [dev_path]
-    output_text = subprocess.check_output(command, text=True)
-
-    logger.debug(f"Processing `{command}` output.")
-    devices_json = json.loads(output_text.strip()).get("blockdevices", [])
-    return [schemas.Block.parse_obj(dev) for dev in devices_json]
-
-
-async def get_smart_info(dev_path: str) -> schemas.Smart:
-    """Gets the information of the device with the `smartctl` command.
-
-    Used to detect when a disk is SSD or HDD correctly, as lsblk don't
-    detect this value correctly.
-
-    :param str dev_path:
-    :return:
-    """
-    command = ["smartctl", "-aj", dev_path]
-    proc = await asyncio.create_subprocess_exec(
-        *command,
-        stdout=asyncio.subprocess.PIPE,
-        stderr=asyncio.subprocess.PIPE,
-    )
-    await proc.wait()
-    output = await proc.stdout.read()
-    smart_json = json.loads(output.decode('UTF-8').rstrip())
-    logger.debug(f"Smart for {dev_path} is: {smart_json}")
-    return schemas.Smart.parse_obj(smart_json)
-
-
-async def get_total_sectors(dev_path: str) -> int:
-    """Get the total
-    """
-    command = ["blockdev", "--getsz", dev_path]
-    proc = await asyncio.create_subprocess_exec(
-        *command,
-        stdout=asyncio.subprocess.PIPE,
-        stderr=asyncio.subprocess.PIPE,
-    )
-    await proc.wait()
-    if proc.returncode:
-        raise Exception(f"Can not get total disk sectors from {dev_path}")
-    return int(await proc.stdout.read())
+def get_disks():
+    """Simple way to get the disks that we support. """
+    return [p for p in Path('/dev').glob('sd?')] + \
+        [p for p in Path('/dev').glob('nvme?n?')]
 
 
 async def erasure_command(
         command: str,
         process_manager: Optional[Any] = None,
-) -> schemas.ErasureCommand:
-    """Runs the command given, but it returns a `schemas.ErasureCommand`
-    object with the processed data.
+) -> schemas.Exec:
+    """Runs the command given, but it returns a `schemas.Exec`
+    object with the command executed details.
 
     :param List[str] command: Command string to be executed like a shell
         on the system.
-    :param process_manager: Async function to allow to manipulate the
-        command process while still running.
+    :param process_manager: Async function to allow manipulating the
+        command process while it is still running.
 
     :return:
     """
     if isinstance(command, list):
         command = ' '.join(command)
 
-    cmd = schemas.ErasureCommand(command=command, start_time=time.time())
+    cmd = schemas.Exec(command=command)
     proc = await asyncio.create_subprocess_shell(
-        # "timeout 30 " +
         cmd.command,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
     )
 
     if process_manager:
         await process_manager(cmd, proc)
 
-    # await proc.communicate()
     await proc.wait()
     cmd.end_time = time.time()
 
     if cmd.stdout is None:
         stdout = await proc.stdout.read()
         cmd.stdout = stdout.decode('UTF-8').rstrip()
 
@@ -117,15 +61,15 @@
     return cmd
 
 
 async def read_from_sector(
         path_to_dev: str,
         sector: int,
         bs: int = 512,
-) -> schemas.ErasureCommand:
+) -> schemas.Exec:
     """Read the X bytes (bs) from a disk sector.
 
     :param str path_to_dev: Path to the device. Example: `/dev/sda`
     :param int sector: Sector to read on the disk.
     :param int bs: Sector sizes, by default 512 bytes.
 
     :return: schemas.ErasureCommand
@@ -133,26 +77,79 @@
     read_command = f"dd if={path_to_dev} bs={bs} count=1 skip={sector}" \
                    " | xxd -ps"
     logger.debug(f"{path_to_dev}: Read data on sector {sector}.")
     return await erasure_command(read_command)
 
 
 async def write_to_sector(
-        path_to_dev: str,
+        dev_path: str,
         sector: int,
         bs: int = 512,
         zeros: bool = False,
-) -> schemas.ErasureCommand:
+) -> schemas.Exec:
     """Write X bytes (bs size must be provided) to the disk sector.
 
-    :param str path_to_dev: Path to the device. Example: `/dev/sda`
+    :param str dev_path: Path to the device. Example: `/dev/sda`
     :param int sector: Sector to read.
     :param int bs: Sector sizes, by default 512 bytes.
     :param bool zeros: The pattern desired to use.
 
     :return: schemas.ErasureCommand
     """
-    write_command = f"dd if={'/dev/zero' if zeros else '/dev/random'}"\
+    write_command = f"dd if={'/dev/zero' if zeros else '/dev/random'}" \
                     f" of=/dev/sda bs={bs} count=1 seek={sector}"
     logger.debug(
-        f"Writing {'zeros' if zeros else 'random'} data into {path_to_dev}.")
+        f"{dev_path}: Writing {'zeros' if zeros else 'random'}"
+        f" data on sector {sector}.")
     return await erasure_command(write_command)
+
+
+def get_smart_info(dev_path):
+    """
+    Get SMART information for a device using smartctl.
+
+    Args:
+        dev_path (str): Path to device
+
+    Returns:
+        dict: JSON output from smartctl
+    """
+
+    # Build command
+    command = ["smartctl", "-aj", dev_path]
+
+    # Run command
+    proc = subprocess.run(command, stdout=subprocess.PIPE,
+                          stderr=subprocess.PIPE)
+
+    # Parse output
+    smart_json = json.loads(proc.stdout.decode('utf-8').rstrip())
+
+    # Print and return result
+    print(f"SMART for {dev_path} is: {smart_json}")
+    return smart_json
+
+
+def get_lsblk_info(dev_path):
+    """
+    Get device information using lsblk.
+
+    Args:
+        dev_path (str): Path to device
+
+    Returns:
+        dict: Device information from lsblk
+    """
+
+    # Build command
+    command = ["lsblk", "-JOad", dev_path]
+
+    # Run command
+    proc = subprocess.run(command, stdout=subprocess.PIPE,
+                          stderr=subprocess.PIPE)
+
+    # Parse output
+    device_info = json.loads(proc.stdout.strip()).get("blockdevices", [])[0]
+
+    # Print and return result
+    print(f"{dev_path}: `lsblk` is -> {device_info}")
+    return device_info
```

### Comparing `usody_sanitize-0.1.0b7/usody_sanitize/methods.py` & `usody_sanitize-0.1.1b1/usody_sanitize/methods.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,95 @@
 """Pre-defined sanitize methods to erase disks securely."""
 from usody_sanitize import schemas
 
 
-BASIC = schemas.ErasureMethod(
+BASIC = schemas.Method(
     name="Basic Erasure",
     # https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=917935
     standard="",
     description="A single-pass overwrite of the entire drive with"
                 " zeros. This method is relatively fast and simple,"
                 " but it may not be completely effective in destroying"
                 " all traces of the original data.",
     removal_process="Overwriting",
-    program="shred",
     verification_enabled=True,
     bad_sectors_enabled=False,
-    overwriting_steps=1,
+    overwriting_steps=[
+        schemas.Execution(tool="shred", pattern="random"),
+    ],
 )
 
-BASELINE = schemas.ErasureMethod(
+BASELINE = schemas.Method(
     name="Baseline Erasure",
     standard="NIST, Infosec HGM Baseline",
     description="Method for securely erasing data in compliance"
                 " with HMG Infosec Standard 5 guidelines includes"
                 " a single step of a random write process on the"
                 " full disk. This process overwrites all data with"
                 " a randomized pattern, ensuring that it cannot be"
                 " recovered. Built-in validation confirms that the"
                 " data has been written correctly, and a final"
                 " validation confirms that all data has been deleted.",
     removal_process="Overwriting",
-    program="badblocks",
     verification_enabled=False,
     bad_sectors_enabled=True,
-    overwriting_steps=1,
+    overwriting_steps=[
+        schemas.Execution(tool="badblocks", pattern="random"),
+    ],
 )
 
-CRYPTOGRAPHIC = schemas.ErasureMethod(
+CRYPTOGRAPHIC_ATA = schemas.Method(
     name="Baseline Cryptographic",
     standard="NIST, Infosec HGM Baseline",
     description="Method for securely erasing data in compliance"
                 " with HMG Infosec Standard 5 guidelines includes"
                 " a single step of a random write process on the"
                 " full disk. This process overwrites all data with"
                 " a randomized pattern, ensuring that it cannot be"
                 " recovered. Built-in validation confirms that the"
                 " data has been written correctly, and a final"
                 " validation confirms that all data has been deleted.",
     removal_process="Overwriting",
-    program="hdparm",
     verification_enabled=False,
+    overwriting_steps=[
+        schemas.Execution(tool="hdparm"),
+    ],
 )
 
-ENHANCED = schemas.ErasureMethod(
+CRYPTOGRAPHIC_NVME = schemas.Method(
+    name="Baseline Cryptographic",
+    standard="NIST, Infosec HGM Baseline",
+    description="Method for securely erasing data in compliance"
+                " with HMG Infosec Standard 5 guidelines includes"
+                " a single step of a random write process on the"
+                " full disk. This process overwrites all data with"
+                " a randomized pattern, ensuring that it cannot be"
+                " recovered. Built-in validation confirms that the"
+                " data has been written correctly, and a final"
+                " validation confirms that all data has been deleted.",
+    removal_process="Overwriting",
+    verification_enabled=False,
+    overwriting_steps=[
+        schemas.Execution(tool="nvme"),
+    ],
+)
+
+ENHANCED = schemas.Method(
     name="Enhanced Erasure",
     standard="HMG Infosec Standard 5",
     description="Method for securely erasing data in compliance"
                 " with HMG Infosec Standard 5 guidelines includes"
                 " a single step of a random write process on the"
                 " full disk. This process overwrites all data with"
                 " a randomized pattern, ensuring that it cannot be"
                 " recovered. Built-in validation confirms that the"
                 " data has been written correctly, and a final"
                 " validation confirms that all data has been deleted.",
     removal_process="Overwriting",
-    program="badblocks",
     verification_enabled=True,
     bad_sectors_enabled=True,
-    overwriting_steps=3,
+    overwriting_steps=[
+        schemas.Execution(tool="badblocks", pattern="random"),
+        schemas.Execution(tool="badblocks", pattern="random"),
+        schemas.Execution(tool="shred", pattern="zeros"),
+    ],
 )
```

### Comparing `usody_sanitize-0.1.0b7/usody_sanitize/schemas/erasure.py` & `usody_sanitize-0.1.1b1/usody_sanitize/schemas/sanitize.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+import time
 from typing import Optional, List
+
 from pydantic import BaseModel, Field
 
-from usody_sanitize.schemas.devices import Device
 from usody_sanitize import __version__ as app_version
+from usody_sanitize.schemas.definition import Method
+from usody_sanitize.schemas.devices import Device
 
 
-class ErasureCommand(BaseModel):
-    """Main and base class to define a collection of steps to proceed.
+class Exec(BaseModel):
+    """Define the data collected while executing each command, this is
+    used to prove the execution of all commands and steps to properly
+    sanitize the device.
     """
     description: Optional[str] = Field(
-        default=None, description="Step description")
-    command: str = Field(default=..., description="Command used on this step")
+        default=None, description="command description")
+    command: str = Field(default=..., description="command to be executed")
 
     stdout: Optional[str] = Field(
         default=None, description="normal output from the command executed")
     stderr: Optional[str] = Field(
         default=None, description="error output from the command executed")
 
     return_code: Optional[int] = Field(
@@ -25,103 +30,81 @@
                                    " correctly")
 
     start_time: float = Field(
         default=..., description="Exact time when the command started")
     end_time: Optional[float] = Field(
         default=None, description="Exact time when the command ended")
 
+    def __init__(self, *args, **kwargs):
+        if 'start_time' not in kwargs:
+            kwargs['start_time'] = time.time()
+        super().__init__(*args, **kwargs)
 
-class ErasureStep(BaseModel):
+
+class Step(BaseModel):
     """Main and base class to define a collection of steps to proceed.
     """
-    step: int = Field(default=..., description="Step number")
-    date_init: Optional[float] = Field(
-        default=None, description="Date at start of the step")
-    date_end: Optional[float] = Field(
-        default=None, description="Date at the end of the step")
+    step: Optional[int] = Field(default=None, description="Step number")
+    start_time: Optional[float] = Field(
+        default=None, description="start time of the step")
+    end_time: Optional[float] = Field(
+        default=None, description="end time of the step")
     duration: Optional[float] = Field(
-        default=None, description="Duration of the step")
-    commands: List[ErasureCommand] = Field(
-        default=[], description="")
-    success: bool = Field(default=False, description="Tells if the step has"
-                                                     "been executed correctly")
+        default=None, description="step duration time")
+    commands: List[Exec] = Field(
+        default=[], description="a list of commands executed for current step")
+    success: bool = Field(
+        default=False, description="Tells if the step has"
+                                   " been executed correctly")
 
+    def __init__(self, *args, **kwargs):
+        if 'start_time' not in kwargs:
+            kwargs['start_time'] = time.time()
+        super().__init__(*args, **kwargs)
 
-class ErasureValidation(BaseModel):
+    def end(self):
+        self.end_time = time.time()
+        # Todo: Remove this duration variable once the tool is more robust.
+        self.duration = self.end_time - self.start_time
+
+
+class SanitizeValidation(BaseModel):
     """Defines the validation process result.
     """
     result: Optional[bool] = Field(
         default=None, description="Defines if the validation is successful")
-    commands: List[ErasureCommand] = Field(
+    commands: List[Exec] = Field(
         default=[], description="A list of commands used to "
                                 "validate this process")
     data: dict = Field(
         default={}, description="Bytes read from each disk sector")
 
 
-class ErasureMethod(BaseModel):
-    name: str = Field(
-        default=..., description="Erasure method name (Basic,"
-                                 " Baseline Erasure, Baseline Cryptographic"
-                                 " or Enhanced)")
-    standard: str = Field(
-        default=..., description="Standard name (NIST SP-800-88 /  HMG"
-                                 " Infosec Standard 5 Baseline Standard /"
-                                 " HMG Infosec Standard 5 Baseline Enhanced")
-    description: Optional[str] = Field(
-        default=None, description="Description of the method")
-    removal_process: Optional[str] = Field(
-        default=None, description="Demagnetization / Destruction /"
-                                  " Overwriting / Cryptographic erase")
-    program: Optional[str] = Field(
-        default=None, description="None / shred / badblocks / hdparm")
-    verification_enabled: bool = Field(
-        default=False, description="Will check if the erasure has deleted"
-                                   " all the data on the disk by comparing"
-                                   " some data written on the disk before"
-                                   " the erasure with the data read after.")
-    bad_sectors_enabled: bool = Field(
-        default=False, description="If true, bad sectors will be checked"
-                                   "on the erasure process")
-    # sectors_total: Optional[int] = Field(
-    #     default=None, description="Total number of sectors")
-    # sectors_bad: Optional[int] = Field(
-    #     default=None, description="Total of bad sectors")
-    warnings: Optional[str] = Field(
-        default=None, description="Summary of the check (no / Bad sectors)")
-    overwriting_steps: Optional[int] = Field(
-        default=None, description="Number of overwriting steps")
-
-    class Config:
-        fields = {
-            "name": {"readonly": True},
-        }
-
-
-class ErasureCertificate(BaseModel):
-    erasure_steps: List[ErasureStep] = Field(
-        default=[], description="A list of erasure steps, each steps contain"
+class Sanitize(BaseModel):
+    """This contains all the data to create a certificate of the
+    complete sanitation process.
+    """
+    steps: List[Step] = Field(
+        default=[], description="a list of sanitize steps, each steps contain"
                                 " a list of commands and the result of each"
-                                " command.")
-    validation: Optional[ErasureValidation] = Field(
-        default=None, description="Information to certificate"
-                                  "the validation process.")
+                                " command")
+    validation: Optional[SanitizeValidation] = Field(
+        default=None, description="information to certificate"
+                                  "the validation process")
 
     # Storage Drive
     device_info: Device = Field(
         default=..., description="all info about the device")
 
     # Method
-    method: Optional[ErasureMethod] = Field(
-        default=None, description="Erasure method")
+    method: Optional[Method] = Field(
+        default=None, description="erasure method")
 
     result: bool = Field(
-        default=False, description="True means erasure has been pass"
+        default=False, description="true means erasure has been pass"
                                    " correctly, False means something"
                                    " failed and the data could not be"
-                                   " erased/wipe.")
+                                   " erased/wipe")
 
-    sanitize_version: str = Field(
+    version: str = Field(
         default=app_version,
-        description="Version of usody_sanitize python package.")
-
-
+        description="version of usody_sanitize python package")
```

### Comparing `usody_sanitize-0.1.0b7/usody_sanitize/schemas/export_data.py` & `usody_sanitize-0.1.1b1/usody_sanitize/schemas/export_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,18 @@
+"""
+Export Data Schema
+==================
+
+This module manages the data expected to be returned from the commands
+executed to export the device data, those commands are `smartmontools`
+and `lsblk`.
+"""
+
 from typing import Optional, List
+
 from pydantic import BaseModel, Field
 
 
 class Block(BaseModel):
     """Defines the schema of an output command as JSON format from
     the `lsblk` command.
     """
@@ -22,14 +32,15 @@
     model: Optional[str] = Field(default=None)
     vendor: Optional[str] = Field(default=None)
     uuid: Optional[str] = Field(default=None)
     type: Optional[str] = Field(default=None)
     hotplug: Optional[str] = Field(default=None)
     label: Optional[str] = Field(default=None)
     state: Optional[str] = Field(default=None)
+    phy_sec: Optional[int] = Field(default=None, alias='phy-sec')
 
     mountpoint: Optional[str] = Field(default=None)
 
     children: Optional[List["Block"]] = Field(default=None)
 
     class Config:
         extra = "allow"
```

### Comparing `usody_sanitize-0.1.0b7/usody_sanitize/steps.py` & `usody_sanitize-0.1.1b1/usody_sanitize/steps.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,43 @@
-import time
+"""
+Steps
+=====
+
+Here you will
+
+"""
+
 import logging
+from typing import Optional
 
 from usody_sanitize import schemas, commands, utils
 
 logger = logging.getLogger(__name__)
 
 
-async def erase_ssd_hdparm(dev_path: str) -> schemas.ErasureStep:
+async def erase_ssd_hdparm(
+        dev_path: str,
+        step: Optional[int] = None,
+) -> schemas.Step:
     """
-    Generates a erasure step for deleting SSD using hdparm.
+    Generates erasure step for deleting SSD using hdparm via ATA.
 
     :param str dev_path: Path to the device.
-    :return: schemas.ErasureStep
+    :param Optional[str] step: Path to the device.
+    :return: schemas.Step
 
     Example:
     >>> erase_ssd_hdparm("/dev/sda")
     """
-    step = schemas.ErasureStep(device=dev_path, step=1)
-    step.date_init = time.time()
+    step = schemas.Step(device=dev_path, step=step)
 
     # Start first command for this step.
     logger.debug(f"{dev_path}: Start command 1.")
     command1 = f"hdparm -I {dev_path}"
-    cmd1: schemas.ErasureCommand = await commands \
+    cmd1: schemas.Exec = await commands \
         .erasure_command(command1)
     cmd1.description = "Verify that the SSD disc is not frozen."
 
     if utils.find_text("(not[\t ]*frozen)", cmd1.stdout):
         cmd1.success = True
     else:
         cmd1.success = False
@@ -43,15 +54,14 @@
     cmd2.description = "Set a temporal password to lock the device."
 
     cmd2.success = cmd2.return_code == 0
 
     step.commands.append(cmd2)
     logger.debug(f"{dev_path}: Command 2 finished. \n{cmd2}")
     if cmd2.success is False:
-        logger.warning("")
         return step
 
     # Third command.
     logger.debug(f"{dev_path}: Start command 3.")
     command3 = f"hdparm --user-master --security-erase Usody {dev_path}"
     cmd3 = await commands.erasure_command(command3)
     cmd3.description = "Erase the SSD changing the encryption key."
@@ -63,97 +73,149 @@
         return step
 
     # Fourth command.
     logger.debug(f"{dev_path}: Start command 4.")
     command4 = f"hdparm -I {dev_path}"
     cmd4 = await commands.erasure_command(command4)
     cmd4.description = "Check the drive security is set to disabled"
-    # There is no problem if the drive is locked. A validation
-    # process of the data been erased is more important.
+
+    # Todo: Enable this pre-validation.
     # if utils.find_text(" *(not *enabled) *", cmd4.output):
     #     cmd4.success = True
     # else:
     #     cmd4.success = False
 
-    # @TODO: Validation step at the end.
-
     step.commands.append(cmd4)
     logger.debug(f"{dev_path}: Command 4 finished. {cmd4}")
 
     # Write final values on the step schema.
-    step.date_end = time.time()
-    step.duration = step.date_end - step.date_init
+    step.end()
     step.success = all(cmd.success for cmd in step.commands)
 
     logger.debug(f"{dev_path}: hdparm erasure step finished.")
     return step
 
 
-async def erase_hdd_shred(dev_path: str) -> schemas.ErasureStep:
+async def erase_nvme_nvmecli(
+        dev_path: str,
+        step: Optional[int] = None,
+) -> schemas.Step:
+    """Creates the erasure step schema with the delete nvme step. This
+    steps executes 1 command `nvme` from `nvme-cli` package.
+
+    :param str dev_path: Path to the device.
+    :param int step: Set the step number.
+    :return: schemas.Step
+
+    Example:
+    >>> erase_ssd_hdparm("/dev/sda")
+    """
+    step = schemas.Step(device=dev_path, step=step)
+
+    # Start first command for this step.
+    logger.debug(f"{dev_path}: Erasing disk.")
+    command1 = f"nvme format --ses=1 {dev_path}"
+    cmd1: schemas.Exec = await commands.erasure_command(command1)
+    cmd1.description = "Erase all contents from the disks with secure" \
+                       "erasure enabled (--ses=1)."
+    step.end()
+
+    logger.debug(f"{dev_path}: Command 1 finished. \n{cmd1}")
+    if cmd1.success is False:
+        return step
+
+    # Write final values on the step schema.
+    step.success = all(cmd.success for cmd in step.commands)
+    step.commands.append(cmd1)
+
+    logger.debug(f"{dev_path}: hdparm erasure step finished.")
+    return step
+
+
+async def erase_hdd_shred(
+        dev_path: str,
+        pattern: str = "random",
+        step: Optional[int] = None,
+
+) -> schemas.Step:
     """Runs erasure step for deleting HDD using shred.
 
     Shred is a command line utility for securely deleting files, it
     is the program used for the "Basic" erasure method.
 
     :param str dev_path: Path to the device.
-    :return: schemas.ErasureStep
+    :param str pattern: Pattern to apply on the erasure.
+    :param int step: Step number to be set on the step schema.
+    :return: schemas.Step
 
     Example:
     >>> erase_hdd_shred("/dev/sda")
     """
-    step = schemas.ErasureStep(device=dev_path, step=1)
-    step.date_init = time.time()
+    step = schemas.Step(device=dev_path, step=step)
 
     # Define the command to run, with zeros or random.
-    command = f"shred --force --verbose --zero --iterations=0 {dev_path}"
+    if pattern == "zeros":
+        command = f"shred --force --verbose --zero --iterations=0 {dev_path}"
+    else:
+        command = f"shred --force --verbose --iterations=1 {dev_path}"
+
     logger.debug(f"{dev_path} command: {command}")
 
     # Run the command.
-    cmd: schemas.ErasureCommand = await commands.erasure_command(
+    cmd: schemas.Exec = await commands.erasure_command(
         command=command, process_manager=utils.print_shred_progress)
     cmd.description = "Write zeros to the disk with `shred`."
+    step.end()
 
     # Write final values on the step schema.
-    step.commands.append(cmd)
-    step.date_end = time.time()
-    step.duration = step.date_end - step.date_init
     step.success = all(cmd.success for cmd in step.commands)
+    step.commands.append(cmd)
 
     logger.debug(f"{dev_path}: Badblocks erasure step finished.")
     return step
 
 
-async def erase_hdd_badblocks(dev_path: str) -> schemas.ErasureStep:
+async def erase_hdd_badblocks(
+        dev_path: str,
+        pattern: str = "random",
+        step: Optional[int] = None,
+) -> schemas.Step:
     """Runs erasure step for deleting HDD using `badblocks`.
 
     badblocks will delete the disk writting data into each sector.
 
     :param str dev_path: Path to the device.
+    :param str pattern: Pattern to apply on the erasure.
+    :param int step: Step number to be set on the step schema.
     :return: schemas.ErasureStep
 
     Example:
     >>> erase_hdd_badblocks("/dev/sda")
     """
-    step = schemas.ErasureStep(device=dev_path, step=1)
-    step.date_init = time.time()
+    step = schemas.Step(device=dev_path, step=step)
 
-    # Todo: Add -e argument to add a maximum of badblocks found.
+    # Todo: Add -e argument to add a maximum of `badblocks` found.
     # Define the command to run, with zeros or random.
     # Argument `-s` provides a progress info that cannot be received,
     #  causing a exception as no new lines are emitted.
-    command = f"badblocks -wv -p 1 -t random {dev_path}"
+
+    if pattern == "zeros":
+        command = f"badblocks -wv -p 1 -t 0 {dev_path}"
+    elif pattern == "random":
+        command = f"badblocks -wv -p 1 -t random {dev_path}"
+    else:
+        command = f"badblocks -wv -p 1 -t {pattern} {dev_path}"
+
     logger.debug(f"{dev_path} command: {command}")
 
     # Run the command.
-    cmd: schemas.ErasureCommand = await commands.erasure_command(
+    cmd: schemas.Exec = await commands.erasure_command(
         command=command, process_manager=utils.print_badblocks_progress)
     cmd.description = "Write random data into the disk with `badblocks`."
+    step.end()
 
     # Write final values on the step schema.
-    step.commands.append(cmd)
-    step.date_end = time.time()
-    step.duration = step.date_end - step.date_init
     step.success = all(cmd.success for cmd in step.commands)
+    step.commands.append(cmd)
 
     logger.debug(f"{dev_path}: Command badblocks erasure step finished.")
     return step
-
```

### Comparing `usody_sanitize-0.1.0b7/usody_sanitize/utils.py` & `usody_sanitize-0.1.1b1/usody_sanitize/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-import re
 import asyncio
 import logging
-
+import re
+from enum import Enum
 from typing import Optional
+
 from usody_sanitize import schemas
 
 logger = logging.getLogger(__name__)
 
 
+class PatternsModes(Enum):
+    ZEROS = 1
+    RANDOM = 2
+
+
 def get_spaced_numbers(max_num: int, items: int):
     """
     ```python
     step = (100000 - 0) / (6 - 1)
     numbers = [i * step for i in range(6)]
     ```
 
@@ -20,33 +26,31 @@
     :return:
     """
     step = (max_num - 1) / (items - 1)
     return [int(i * step) for i in range(items)]
 
 
 async def print_shred_progress(
-        cmd: schemas.ErasureCommand,
+        cmd: schemas.Exec,
         process: asyncio.subprocess.Process
 ):
     """Example how to process `shred` output."""
     async for line in process.stderr:
         logger.debug(f"{cmd.command}: {line}")
 
 
 async def print_badblocks_progress(
-        cmd: schemas.ErasureCommand,
+        cmd: schemas.Exec,
         process: asyncio.subprocess.Process
 ):
     """Example how to process `badblocks` output."""
     async for line in process.stderr:
         clean_line = line.decode('UTF-8').replace('\b', '').replace('\n', '')
         logger.debug(f"{cmd.command}: {clean_line}")
 
-    logger.debug("OUT")
-
 
 def find_text(re_expression: str, string: str) -> Optional[str]:
     """Searches for a regular expression in a string and returns the
     first match. Used to find text in the output of the commands.
 
     :param str re_expression:
     :param str string:
```

