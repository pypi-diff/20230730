# Comparing `tmp/mdgpt-0.3.0.tar.gz` & `tmp/mdgpt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdgpt-0.3.0.tar", max compression
+gzip compressed data, was "mdgpt-0.3.1.tar", max compression
```

## Comparing `mdgpt-0.3.0.tar` & `mdgpt-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-18 20:46:07.614765 mdgpt-0.3.0/LICENSE
--rw-r--r--   0        0        0     5552 2023-07-27 21:10:00.673003 mdgpt-0.3.0/README.md
--rw-r--r--   0        0        0     7746 2023-07-29 21:09:50.848726 mdgpt-0.3.0/mdgpt/__init__.py
--rw-r--r--   0        0        0     4322 2023-07-29 21:00:05.927261 mdgpt-0.3.0/mdgpt/build.py
--rw-r--r--   0        0        0     1301 2023-07-29 20:35:09.844197 mdgpt-0.3.0/mdgpt/image.py
--rw-r--r--   0        0        0      448 2023-07-24 21:53:42.866848 mdgpt-0.3.0/mdgpt/misc.py
--rw-r--r--   0        0        0     2715 2023-07-29 20:36:43.111687 mdgpt-0.3.0/mdgpt/models.py
--rw-r--r--   0        0        0    11060 2023-07-29 20:45:20.754845 mdgpt-0.3.0/mdgpt/translate.py
--rw-r--r--   0        0        0     5726 2023-07-29 14:25:42.495475 mdgpt-0.3.0/mdgpt/utils.py
--rw-r--r--   0        0        0      940 2023-07-29 20:58:09.903291 mdgpt-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6817 2023-07-29 21:12:23.429977 mdgpt-0.3.0/setup.py
--rw-r--r--   0        0        0     6531 2023-07-29 21:12:23.430647 mdgpt-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-18 20:46:07.614765 mdgpt-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5552 2023-07-27 21:10:00.673003 mdgpt-0.3.1/README.md
+-rw-r--r--   0        0        0     8009 2023-07-30 00:39:42.717647 mdgpt-0.3.1/mdgpt/__init__.py
+-rw-r--r--   0        0        0     4322 2023-07-29 21:00:05.927261 mdgpt-0.3.1/mdgpt/build.py
+-rw-r--r--   0        0        0     1301 2023-07-29 20:35:09.844197 mdgpt-0.3.1/mdgpt/image.py
+-rw-r--r--   0        0        0      448 2023-07-24 21:53:42.866848 mdgpt-0.3.1/mdgpt/misc.py
+-rw-r--r--   0        0        0     2715 2023-07-29 20:36:43.111687 mdgpt-0.3.1/mdgpt/models.py
+-rw-r--r--   0        0        0    10989 2023-07-30 00:37:31.021435 mdgpt-0.3.1/mdgpt/translate.py
+-rw-r--r--   0        0        0     5726 2023-07-29 14:25:42.495475 mdgpt-0.3.1/mdgpt/utils.py
+-rw-r--r--   0        0        0      940 2023-07-30 00:44:32.624266 mdgpt-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6817 2023-07-30 00:45:53.837730 mdgpt-0.3.1/setup.py
+-rw-r--r--   0        0        0     6531 2023-07-30 00:45:53.838303 mdgpt-0.3.1/PKG-INFO
```

### Comparing `mdgpt-0.3.0/LICENSE` & `mdgpt-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdgpt-0.3.0/README.md` & `mdgpt-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mdgpt-0.3.0/mdgpt/__init__.py` & `mdgpt-0.3.1/mdgpt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,42 +17,40 @@
 from mdgpt.utils import get_lang_dict
 from mdgpt.utils import get_markdown_files
 from mdgpt.translate import save_json_translated
 from mdgpt.translate import translate_missing_json
 from mdgpt.translate import get_translation_tasks
 from mdgpt.translate import translate_markdown_file
 from mdgpt.translate import get_target_file
+from mdgpt.image import create_image
 
 
 load_dotenv()
 
 
 def cli():
 
     args = parse_args()
     cfg = get_prompt_config(args.prompt, **vars(args))
 
     source_lang = get_lang_dict(cfg.LANGUAGE)
     source_lang['dir'] = cfg.SOURCE_DIR if cfg.SOURCE_DIR else cfg.LANGUAGE
 
-    if args.action == 'build':
-        _build(cfg, source_lang)
-
-    elif args.action == 'translate':
-        _translate(cfg, source_lang)
-
-    elif args.action == 'image':
-        from mdgpt.image import create_image
-        create_image(cfg)
-
-    elif args.action == 'debug':
-        _debug(cfg)
-
+    funcs = {
+        'build': _build,
+        'translate': _translate,
+        'debug': _debug,
+        'image': _image,
+    }
+
+    func = funcs.get(args.action)
+    if func is not None:
+        func(cfg)
     else:
-        print('Unknown action')
+        print('[red]Unknown action')
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Build and translate markdown files from a prompt configuration file')
     parser.add_argument('action', type=str, help='Action to perform')
     parser.add_argument('prompt', type=str, help='Path to prompt configuration file without extension')
     parser.add_argument('-d', '--dir', dest='dir', type=str, required=False, help='Root directory for language subdirectories and files')
@@ -60,28 +58,27 @@
     parser.add_argument('-l', '--lang', dest='lang', type=str, required=False, help='Source language in ISO 639-1 two-letter code')
     parser.add_argument('-s', '--source-dir', dest='source_dir', type=str, help='Optional Source directory. Defaults to lang')
     parser.add_argument('-t', '--target', dest='target', type=str, required=False, help='Target language in ISO 639-1 two-letter code')
 
     return parser.parse_args()
 
 
-def _build(cfg: PromptConfig, source_lang):
+def _build(cfg: PromptConfig):
     print(f'Building {cfg.ROOT_DIR} ...')
 
     prompt_tokens = completion_tokens = 0
     skips = oks = errors = 0
 
     wcfg = cfg.WEBSITE_BUILDER
     if wcfg is None:
         print('[red]No website builder config found.')
         exit(1)
 
     tasks = get_build_tasks(wcfg)
     total_tasks = len(tasks)
-    print('Tasks:', len(tasks))
 
     for i in track(range(total_tasks), description="Building ..."):
         step = tasks[i]
 
         print_details = f'({i+1}/{total_tasks}) Writing {step.destination} ...'
         print(print_details, end='', flush=True)
 
@@ -106,15 +103,15 @@
     print(f'completion_tokens: {completion_tokens}')
 
     print(f'[yellow]skips: {skips}')
     print(f'[green]oks: {oks}')
     print(f'[red]errors: {errors}')
 
 
-def _translate(cfg: PromptConfig, source_lang):
+def _translate(cfg: PromptConfig):
     tasks = get_translation_tasks(cfg)
     total_tasks = len(tasks)
 
     prompt_tokens = completion_tokens = 0
     errors = skips = oks = 0
 
     # Build url maps for each target language
@@ -129,72 +126,33 @@
 
     # Execute translation tasks
     try:
         for i in track(range(total_tasks), description="Translating ..."):
             task = tasks[i]
             action, target, file = task.split(':')[:3]
 
+            target_lang = lang_matrix[target]
+
             if action == 'js':
+                result, usage = _translate_js(cfg, i, target, total_tasks, url_matrix[target], missing_matrix[target], lang_matrix[target],)
+            elif action == 'md':
+                result, usage = _translate_md(cfg, i, total_tasks, file, target, target_lang, url_matrix[target])
 
-                url_map = url_matrix[target]
-                missing = missing_matrix[target]
-                target_lang = lang_matrix[target]
-
-                print_details = f'{i+1}/{total_tasks} Translating file urls {cfg.LANGUAGE} -> {target} ...'
-                print(print_details, end='', flush=True)   # end='\r',
-
-                if len(missing) == 0:
-                    print(f'[yellow]{print_details} Skip!')
-                    skips += 1
-
-                if len(missing) > 0:
-                    missing_translations = translate_missing_json(cfg, missing, source_lang, target_lang)
-
-                    # Backfill missing translations
-                    for key, value in missing_translations.items():
-                        if value is not None and len(value) > 0:
-                            url_map[key] = value
-
-                    # Save url_map ...
-                    save_json_translated(cfg, url_map, target)
-                    print(f'[green]{print_details} ok ;)')
-                    oks += 1
+            if usage:
+                prompt_tokens += usage['prompt_tokens']
+                completion_tokens += usage['completion_tokens']
+                # log_usage(f'translate_{action}', target, file, usage['prompt_tokens'], usage['completion_tokens'])
 
-            elif action == 'md':
+            if result == 'ok':
+                oks += 1
+            elif result == 'skip':
+                skips += 1
+            elif result == 'error':
+                errors += 1
 
-                # Check if file exists
-                root = Path(cfg.ROOT_DIR)
-                target_path = get_target_file(file, root, target, url_matrix[target])
-
-                print_details = f'{i+1}/{total_tasks} Translating {target_path} ...'
-
-                print(print_details, end='', flush=True)   # end='\r',
-                if target_path.exists():
-                    skip = True
-                    if cfg.FILE:
-                        if cfg.FILE == file:
-                            skip = False
-
-                    if skip:
-                        skips += 1
-                        print(f'[yellow]{print_details} Skip!')
-                        continue
-
-                if usage := translate_markdown_file(cfg, file, source_lang, target_lang, url_matrix[target]):
-                    prompt_tokens += usage['prompt_tokens']
-                    completion_tokens += usage['completion_tokens']
-                    log_usage('translate_md', target, file, usage['prompt_tokens'], usage['completion_tokens'])
-
-                    oks += 1
-
-                    print(f'[green]{print_details} ok!')
-
-                else:
-                    errors += 1
-                    print(f'[red]{print_details} error!')
     except KeyboardInterrupt:
         print('Interrupted!')
     except Exception as e:
         print('An error occurred:', e)
 
     print('---')
     print('prompt_tokens:', prompt_tokens)
@@ -202,14 +160,67 @@
     print('---')
     print(f'[bold]Tasks: {total_tasks}')
     print(f'[yellow]skips: {skips}')
     print(f'[green]oks: {oks}')
     print(f'[red]errors: {errors}')
 
 
+def _translate_js(cfg: PromptConfig, i, target, total_tasks, url_map, missing, target_lang):
+    print_details = f'{i+1}/{total_tasks} Translating file urls {cfg.LANGUAGE} -> {target} ...'
+    print(print_details, end='', flush=True)   # end='\r',
+
+    if len(missing) == 0:
+        print(f'[yellow]{print_details} Skip!')
+        return 'skip', None
+
+    if len(missing) > 0:
+        missing_translations, usage = translate_missing_json(cfg, missing, target_lang)
+
+        # Backfill missing translations
+        for key, value in missing_translations.items():
+            if value is not None and len(value) > 0:
+                url_map[key] = value
+
+        # Save url_map ...
+        save_json_translated(cfg, url_map, target)
+        print(f'[green]{print_details} ok ;)')
+        return 'ok', usage
+
+
+def _translate_md(cfg: PromptConfig, i, total_tasks, file, target, target_lang, url_map):
+    # Check if file exists
+    root = Path(cfg.ROOT_DIR)
+    target_path = get_target_file(file, root, target, url_map)
+
+    print_details = f'{i+1}/{total_tasks} Translating {target_path} ...'
+
+    print(print_details, end='', flush=True)   # end='\r',
+    if target_path.exists():
+        skip = True
+        if cfg.FILE:
+            if cfg.FILE == file:
+                skip = False
+
+        if skip:
+            print(f'[yellow]{print_details} Skip!')
+            return 'skip', None
+
+    if usage := translate_markdown_file(cfg, file, target_lang, url_map):
+        # prompt_tokens += usage['prompt_tokens']
+        # completion_tokens += usage['completion_tokens']
+        log_usage('translate_md', target, file, usage['prompt_tokens'], usage['completion_tokens'])
+
+        print(f'[green]{print_details} ok!')
+        return 'ok', usage
+
+    else:
+        print(f'[red]{print_details} error!')
+        return 'error', None
+
+
 def _debug(cfg: PromptConfig):
     print(f'cfg:', cfg)
 
     unique_matters = []
     matters = []
     root_path = Path(cfg.ROOT_DIR, cfg.SOURCE_DIR or cfg.LANGUAGE)
     files = get_markdown_files(root_path)
@@ -217,7 +228,11 @@
         content = Path(root_path, file).read_text()
         matter = frontmatter.loads(content)
         for k, v in matter.metadata.items():
             if k not in unique_matters:
                 unique_matters.append(k)
 
     print('unique_matters:', sorted(unique_matters))
+
+
+def _image(cfg: PromptConfig):
+    create_image(cfg)
```

### Comparing `mdgpt-0.3.0/mdgpt/build.py` & `mdgpt-0.3.1/mdgpt/build.py`

 * *Files identical despite different names*

### Comparing `mdgpt-0.3.0/mdgpt/image.py` & `mdgpt-0.3.1/mdgpt/image.py`

 * *Files identical despite different names*

### Comparing `mdgpt-0.3.0/mdgpt/models.py` & `mdgpt-0.3.1/mdgpt/models.py`

 * *Files identical despite different names*

### Comparing `mdgpt-0.3.0/mdgpt/translate.py` & `mdgpt-0.3.1/mdgpt/translate.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,17 +132,17 @@
 def generate_md_promt(prompt_messages, post, lang, target_lang, field_keys, field_keys_delete=None):
     frontmatter = generate_frontmatter(post, field_keys, field_keys_delete)
 
     return [
         {
             'role': msg.role,
             'content': msg.prompt.format(
-                lang=lang,
-                lang_name=lang['name'],
-                lang_code=lang['code'],
+                # lang=lang,
+                lang_name=lang.name,
+                lang_code=lang.code,
                 target_lang=target_lang,
                 target_lang_name=target_lang['name'],
                 target_lang_code=target_lang['code'],
                 frontmatter=frontmatter,
                 content=post.content
             )
         } for msg in prompt_messages
@@ -193,25 +193,24 @@
         if target_file.exists():
             continue
 
         filtered_files.append(file)
     return filtered_files
 
 
-def translate_markdown_file(prompt_cfg: PromptConfig, file, src, target, url_map, ignore_existing=True):
+def translate_markdown_file(prompt_cfg: PromptConfig, file, target, url_map, ignore_existing=True):
     root = Path(prompt_cfg.ROOT_DIR)
 
-    src_code, src_name, src_dir = src['code'], src['name'], src['dir']
-    trg_code, trg_name, trg_dir = target['code'], target['name'], target['dir']
+    trg_dir = target['dir']
 
-    with open(root / src_dir / file) as f:
+    with open(root / prompt_cfg.LANG.directory / file) as f:
         post = frontmatter.load(f)
 
     target_path = get_target_file(file, root, trg_dir, url_map)
-    messages = generate_md_promt(prompt_cfg.MARKDOWN_PROMPT, post, src, target, prompt_cfg.FIELD_KEYS, prompt_cfg.FIELD_KEYS_DELETE)
+    messages = generate_md_promt(prompt_cfg.MARKDOWN_PROMPT, post, prompt_cfg.LANG, target, prompt_cfg.FIELD_KEYS, prompt_cfg.FIELD_KEYS_DELETE)
     options = get_gpt_options(prompt_cfg.MODEL)
 
     try:
         response, usage = get_chat_response(messages, **options)
     except Exception as e:
         # raise Exception(f'Could not get response for {file}: {e}')
         print(f'Could not get response for {file}: {e}')
@@ -251,36 +250,36 @@
     filename = f'{prompt_cfg.LANGUAGE}_{target}.json'
     src_file = Path(f'{prompt_cfg.ROOT_DIR}/.mdgpt-urls/{filename}')
 
     src_file.parent.mkdir(parents=True, exist_ok=True)
     src_file.write_text(json.dumps(json_dict, indent=2))
 
 
-def translate_missing_json(prompt_cfg: PromptConfig, json_dict, src, target):
+def translate_missing_json(prompt_cfg: PromptConfig, json_dict, target):
     messages = [
         {
             'role': msg.role,
             'content': msg.prompt.format(
-                lang=src,
-                lang_name=src['name'],
-                lang_code=src['code'],
+                # lang=src,
+                lang_name=prompt_cfg.LANG.name,
+                lang_code=prompt_cfg.LANG.code,
                 target_lang=target,
                 target_lang_name=target['name'],
                 target_lang_code=target['code'],
                 content=json.dumps(json_dict, indent=2))
         }
         for msg in prompt_cfg.URL_PROMPT
     ]
     options = get_gpt_options(prompt_cfg.MODEL)
     response, usage = get_chat_response(messages, **options)
-    log_usage('translate_json', target['code'], f'{src["code"]}_{target["code"]}', usage['prompt_tokens'], usage['completion_tokens'])
+    log_usage('translate_json', target['code'], f'{prompt_cfg.LANG.code}_{target["code"]}', usage['prompt_tokens'], usage['completion_tokens'])
 
     response_json = json.loads(response)
 
-    return response_json
+    return response_json, usage
 
 def translate_json(prompt_cfg: PromptConfig, json_dict, src, target, ignore_existing=True):
 
     filename = f'{src["code"]}_{target["code"]}.json'
     src_file = Path(f'{prompt_cfg.ROOT_DIR}/.mdgpt-urls/{filename}')
 
     if src_file.exists():
```

### Comparing `mdgpt-0.3.0/mdgpt/utils.py` & `mdgpt-0.3.1/mdgpt/utils.py`

 * *Files identical despite different names*

### Comparing `mdgpt-0.3.0/pyproject.toml` & `mdgpt-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   | dist
   | venv
 )/
 '''
 
 [tool.poetry]
 name = "mdgpt"
-version = "0.3.0"
+version = "0.3.1"
 description = "Translate markdown files using OpenAI ChatGPT, and generate localized copies of each file."
 authors = ["Jeppe Bårris <jeppe@barris.dk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Djarnis/mdGPT"
 repository = "https://github.com/Djarnis/mdGPT"
 keywords = ["markdown", "translation", "openai", "chatgpt", "gpt"]
```

### Comparing `mdgpt-0.3.0/setup.py` & `mdgpt-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'rich>=13.4.2,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['mdgpt = mdgpt:cli']}
 
 setup_kwargs = {
     'name': 'mdgpt',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Translate markdown files using OpenAI ChatGPT, and generate localized copies of each file.',
     'long_description': '# mdGPT - Mark Down General Purpose Transformer\n\nTranslate markdown files using OpenAI ChatGPT, and generate localized copies of each file.\n\n## Installation\n\n### Using pip\n\n```bash\npip install mdgpt\n```\n\nSet environment variable `OPENAI_API_KEY` or create it in a `.env` file\n\n```bash\nexport OPENAI_API_KEY=YOUR_API_KEY\n```\n\nDownload example prompts:\n\n```bash\ncurl -o example.yaml https://raw.githubusercontent.com/Djarnis/mdGPT/main/prompts.yaml\n```\n\nUse the example `WEBSITE_BUILDER` option from the prompts to build some example files;\n\n```bash\nmdgpt build example\n```\n\nTranslate these markdown files into Finish (fi) versions:\n\n```bash\nmdgpt translate example --target fi\n```\n\nor Danish (da):\n\n```bash\nmdgpt translate example --target da\n```\n\nor German (de):\n\n```bash\nmdgpt translate example --target de\n```\n\nOr whatever. Just make sure it is an ISO 639-1 two-letter language code, and all should be fine.\n\nAdjust the `example.yaml` prompts to suit your needs.\n\n#### MODEL\n\nYou can change the `MODEL` to any engine supported by OpenAI, change the default temperature, and adjust max tokens.\n\nDefault values are:\n\n```yaml\nMODEL:\n    temperature: 0.2\n    engine: gpt-3.5-turbo\n    max_tokens: 2048\n```\n\n#### WEBSITE_BUILDER\n\nThis option is used for building mark down documents, given the example instructions below:\n\n```yaml\nWEBSITE_BUILDER:\n    title: The AI Markdown Translator\n    description: Translate markdown files for websites\n    system_prompt: |\n        Only reply in valid markdown with frontmatter.\n        No explanations. No notes.\n        Language: {lang[name]}\n        Markdown Document:\n        ---\n        # Frontmatter attributes:\n        title: Title of webpage\n        description: Short meta description\n        ---\n        <!-- markdown content -->\n    user_suffix: |\n        Respond in valid markdown format including all provided frontmatter attributes.\n\n    steps:\n        - prompt: |\n              Write the homepage content for the fictive product "The AI Markdown Translator" in {lang[name]} ({lang[code]}).\n          destination: index.md\n        - prompt: |\n              Write the "About Us" page content for a fictive team behind the fictive product "The AI Markdown Translator" in {lang[name]} ({lang[code]}).\n          destination: about.md\n        - prompt: |\n              Write the history for the fictive product "The AI Markdown Translator" in {lang[name]} ({lang[code]}), starting in 2019 with 5 major milestones.\n          destination: history.md\n```\n\n#### URL_PROMPT\n\nThis prompt is used when translating file paths.\n\n#### MARKDOWN_PROMPT\n\nThis prompt is used when translating markdown files.\n\n#### ONLY_INDEXES\n\nOptional boolean value, if you only want `index.md` files translated.\n\n```yaml\nONLY_INDEXES: True\n```\n\n#### FIELD_KEYS\n\nOptional list of frontmatter keys you want to translate.\n\nPer default, all keys will be translated, but you can define selected ones here.\n\n```yaml\nFIELD_KEYS:\n    - title\n    - description\n    - keywords\n    - heading\n    - teaser\n```\n\n---\n\n### Using repo source and Poetry:\n\n#### Step 1: Install Poetry\n\nPoetry is a tool for dependency management and packaging in Python. It allows you to declare the libraries your project depends on and it will manage (install/update) them for you.\n\nOn Unix-based systems like Linux and MacOS, you can install Poetry by using the following command in your terminal:\n\n```bash\ncurl -sSL https://install.python-poetry.org | python -\n```\n\nOn Windows, you can use PowerShell to install Poetry with the following command:\n\n```powershell\n(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | python -\n```\n\nYou can check if Poetry was installed correctly by running:\n\n```bash\npoetry --version\n```\n\n#### Step 2: Rename .env.tpl to .env\n\nIn your project directory, you have a file named .env.tpl which serves as a template for environment variables. To use this file, you should rename it to .env.\n\nOn Unix-based systems, use the following command:\n\n```bash\nmv .env.tpl .env\n```\n\nOn Windows, use the following command:\n\n```powershell\nrename .env.tpl .env\n```\n\n#### Step 3: Add OPENAI_API_KEY value to .env\n\nOpen your .env file in a text editor. You should see a line that looks something like this:\n\n```bash\nOPENAI_API_KEY=\n```\n\nAfter the equal sign, add your OpenAI API key in quotes. It should look something like this:\n\n```bash\nOPENAI_API_KEY="your-api-key-goes-here"\n```\n\nSave the .env file and close it.\n\n_Please note:_\n\n-   Make sure to replace "your-api-key-goes-here" with your actual OpenAI API key.\n-   Do not share your .env file or post it online, as it contains sensitive information.\n\n#### Step 4: Install mdGPT\n\nFrom the project directory, install mdGPT and its dependencies:\n\n```bash\npoetry install\n```\n\nThis installs mdGPT and all its dependencies, and you can now follow the example below.\n\n## Example\n\n### Build Markdown files\n\nThe example website ([./example/en](example/en)) was created using the `WEBSITE_BUILDER` option included in the [prompts.yaml](prompts.yaml) file.\n\n```bash\npoetry run mdgpt build example\n```\n\nWhich will create these files in the ./example/en directory:\n\n-   index.md\n-   about.md\n-   contact.md\n-   history.md\n\n## Translate website\n\nTo translate the markdown files into Finish (fi) versions, run this command:\n\n```bash\npoetry run mdgot translate example --target fi\n```\n\nAnd you should get a `/fi` subdirectory ./example/fi/ containing these files, translated from their original English (en) source:\n\n-   index.md\n-   tietoja.md\n-   yhteystiedot.md\n-   historia.md\n',
     'author': 'Jeppe Bårris',
     'author_email': 'jeppe@barris.dk',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Djarnis/mdGPT',
```

### Comparing `mdgpt-0.3.0/PKG-INFO` & `mdgpt-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdgpt
-Version: 0.3.0
+Version: 0.3.1
 Summary: Translate markdown files using OpenAI ChatGPT, and generate localized copies of each file.
 Home-page: https://github.com/Djarnis/mdGPT
 License: MIT
 Keywords: markdown,translation,openai,chatgpt,gpt
 Author: Jeppe Bårris
 Author-email: jeppe@barris.dk
 Requires-Python: >=3.10,<4.0
```

