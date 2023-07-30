# Comparing `tmp/readmeai-0.0.453.tar.gz` & `tmp/readmeai-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.0.453.tar", max compression
+gzip compressed data, was "readmeai-0.0.50.tar", max compression
```

## Comparing `readmeai-0.0.453.tar` & `readmeai-0.0.50.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.453/LICENSE
--rw-r--r--   0        0        0    17515 2023-07-30 09:02:26.210378 readmeai-0.0.453/README.md
--rw-r--r--   0        0        0     2470 2023-07-30 09:01:42.392715 readmeai-0.0.453/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.453/readmeai/__init__.py
--rw-r--r--   0        0        0     7699 2023-07-30 08:47:06.328508 readmeai-0.0.453/readmeai/builder.py
--rw-r--r--   0        0        0     6343 2023-07-30 08:44:10.050885 readmeai-0.0.453/readmeai/conf.py
--rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.453/readmeai/factory.py
--rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.453/readmeai/logger.py
--rwxr-xr-x   0        0        0     3997 2023-07-30 08:48:59.042518 readmeai-0.0.453/readmeai/main.py
--rw-r--r--   0        0        0     7590 2023-07-30 08:47:03.763889 readmeai-0.0.453/readmeai/model.py
--rw-r--r--   0        0        0     7273 2023-07-30 08:34:53.114073 readmeai-0.0.453/readmeai/parse.py
--rw-r--r--   0        0        0     6536 2023-07-30 08:41:41.081277 readmeai-0.0.453/readmeai/preprocess.py
--rw-r--r--   0        0        0     3991 2023-07-30 08:41:30.482622 readmeai-0.0.453/readmeai/utils.py
--rw-r--r--   0        0        0    19048 1970-01-01 00:00:00.000000 readmeai-0.0.453/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.50/LICENSE
+-rw-r--r--   0        0        0    17599 2023-07-30 09:44:18.539250 readmeai-0.0.50/README.md
+-rw-r--r--   0        0        0     2469 2023-07-30 09:49:16.030425 readmeai-0.0.50/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.50/readmeai/__init__.py
+-rw-r--r--   0        0        0     7699 2023-07-30 08:47:06.328508 readmeai-0.0.50/readmeai/builder.py
+-rw-r--r--   0        0        0     6343 2023-07-30 08:44:10.050885 readmeai-0.0.50/readmeai/conf.py
+-rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.50/readmeai/factory.py
+-rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.50/readmeai/logger.py
+-rwxr-xr-x   0        0        0     3997 2023-07-30 08:48:59.042518 readmeai-0.0.50/readmeai/main.py
+-rw-r--r--   0        0        0     7590 2023-07-30 08:47:03.763889 readmeai-0.0.50/readmeai/model.py
+-rw-r--r--   0        0        0     7273 2023-07-30 08:34:53.114073 readmeai-0.0.50/readmeai/parse.py
+-rw-r--r--   0        0        0     6536 2023-07-30 08:41:41.081277 readmeai-0.0.50/readmeai/preprocess.py
+-rw-r--r--   0        0        0     3991 2023-07-30 08:41:30.482622 readmeai-0.0.50/readmeai/utils.py
+-rw-r--r--   0        0        0    19131 1970-01-01 00:00:00.000000 readmeai-0.0.50/PKG-INFO
```

### Comparing `readmeai-0.0.453/LICENSE` & `readmeai-0.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.453/README.md` & `readmeai-0.0.50/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
         <img src="https://img.shields.io/badge/Markdown-000000.svg?stylee&logo=Markdown&logoColor=white" alt="Markdown" />
         <img src="https://img.shields.io/badge/OpenAI-412991.svg?stylee&logo=OpenAI&logoColor=white" alt="OpenAI" />
         <img src="https://img.shields.io/badge/Python-3776AB.svg?stylee&logo=Python&logoColor=white" alt="Python" />
         <img src="https://img.shields.io/badge/Pytest-0A9EDC.svg?stylee&logo=Pytest&logoColor=white" alt="pytest" />
         <img src="https://img.shields.io/badge/GNU%20Bash-4EAA25.svg?stylee&logo=GNU-Bash&logoColor=white" alt="Bash" />
         <img src="https://img.shields.io/badge/Anaconda-44A833.svg?&logo=Anaconda&logoColor=white" alt="Anaconda" />
     </p>
-    <img src="https://img.shields.io/github/languages/top/eli64s/README-AI?color=5D6D7E" alt="GitHub top language" />
-    <img src="https://img.shields.io/github/commit-activity/m/eli64s/README-AI?color=5D6D7E" alt="GitHub commit activity" />
-    <img src="https://img.shields.io/github/last-commit/eli64s/readme-ai?color=5D6D7E" alt="GitHub last commit" />
+    <img src="https://img.shields.io/pypi/v/readmeai?color=5D6D7E&logo=python" alt="PyPI - License" />
+    <img src="https://img.shields.io/pypi/pyversions/readmeai?color=5D6D7E&logo=python" alt="PyPI - Python Version" />
     <img src="https://img.shields.io/github/license/eli64s/README-AI?color=5D6D7E" alt="GitHub license" />
+    <img src="https://img.shields.io/github/last-commit/eli64s/readme-ai?color=5D6D7E" alt="GitHub last commit" />
 </div>
 
 
 ---
 
 ## 📖 Table of Contents
 
@@ -54,15 +54,15 @@
 #### 🎯 *Motivation*
 
 Simplifies the process of writing and maintaining high-quality project documentation. My aim for this project is to provide all skill levels a tool that improves their technical workflow, in an efficient and user-friendly manner. Ultimately, the goal of *README-AI* is to improve the adoption and usability of open-source projects, enabling everyone to better understand and use open-source tools.
 #### ⚠️ *Disclaimer*
 
 *README-AI* is currently under development and has an opinionated configuration and setup. While this tool provides an excellent starting point for documentation, its important to review all text generated by the OpenAI API to ensure it accurately represents your codebase. Ensure all content in your repository is free of sensitive information before executing.
 
-Additionally, regularly monitor your API usage and costs by visiting the [OpenAI API Usage](https://platform.openai.com/account/usage).
+Additionally, frequently monitor your API usage and costs by visiting the [OpenAI API Usage Dashboard](https://platform.openai.com/account/usage).
 
 ---
 
 ## 👾 Demo
 
 <a href="https://youtu.be/pl-VcVfGbbk">
     <img src="examples/imgs/demo.png" alt="readme-ai demo video">
@@ -332,54 +332,54 @@
 2. Navigate to the *readme-ai* directory.
 ```sh
 cd readme-ai
 ```
 
 3. Use one of the following methods to install the required dependencies:
 
+> Pip (PyPi Package)
 ```sh
-# With Pip
 pip install readmeai
 ```
 
+> Bash
 ```sh
-# With Bash
 bash setup/setup.sh
 ```
 
+> Conda
 ```sh
-# With Conda
 conda create -n readmeai python=3.9 -y && \
 conda activate readmeai && \
 poetry install
 ```
 
+> Poetry
 ```sh
-# With Poetry
 poetry install
 ```
 
+> Docker
 ```sh
-# With Docker
-docker pull zeroxeli/readme-ai:0.0.4
+docker pull zeroxeli/readme-ai:0.0.5
 ```
 
 ### 🎮 Using *README-AI*
 
 Use the command-line to provide the OpenAI API key (if not already set) and specify an output path for your README file, along with the path to your local repository or remote code repository. You can also provide the output path in the [configuration file](./conf/conf.toml)
 
 Command-Line Arguments:
 
 - `-k` or `--api-key`: Your OpenAI API key.
 - `-o` or `--output`: The output path for your README.md file.
 - `-r` or `--repository`: The URL or path to your code repository.
 - `-t` or `--template`: The README template format to use. (coming soon!)
 - `l` or `--language`: The language of text written in the README file (coming soon!)
 
-> Pip
+> Pip (PyPi Package)
 ```sh
 readmeai --api-key "YOUR_API_KEY" --output readme-ai.md --repository https://github.com/eli64s/readme-ai
 
 # Or export your OpenAI API key as an environment variable
 export OPENAI_API_KEY="YOUR_API_KEY"
 readmeai -k $OPENAI_API_KEY -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
@@ -401,36 +401,36 @@
 poetry run python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
 > Docker
 ```sh
 docker run -it \
 -e OPENAI_API_KEY="YOUR_API_KEY" \
--v "$(pwd)":/app \
--w /app zeroxeli/readme-ai:0.0.4 \
-python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai
+-v "$(pwd)":/app zeroxeli/readme-ai:0.0.5 \
+readmeai -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
 ### 🧪 Running Tests
 
 To run the unit-tests for README-AI, use the following command.
 
-```bash
+```sh
 bash scripts/test.sh
 ```
 
 <p align="right">
   <a href="#top"><b>🔝 Return </b></a>
 </p>
 
 ---
 
 ## 🛠 Future Development
 
 - [X] Add additional language support for populating the *installation*, *usage*, and *test* README sections.
+- [X] Upload the *readme-ai* cli tool to PyPi under the module name [readmeai](https://pypi.org/project/readmeai/).
 - [ ] Design and implement a variety of README template formats for different use-cases.
 - [ ] Add support for writing the README in any language (i.e. CN, ES, FR, JA, KO, RU).
 - [ ] Create UI with [Textual](https://github.com/Textualize/textual) or another framework to improve user experience.
 
 ---
 
 ## 📒 Changelog
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
     ****** [https://img.icons8.com/?size=512&id=55494&format=png] [https://
              img.icons8.com/?size=512&id=kTuxVYRKeKEY&format=png]
                                README-AI ******
      **** â¦ Generate beautiful and informative README.md documents. ****
         **** â¦ Developed with OpenAI's GPT language model APIs. ****
 
             [Markdown] [OpenAI] [Python] [pytest] [Bash] [Anaconda]
-  [GitHub top language] [GitHub commit activity] [GitHub last commit] [GitHub
-                                   license]
+[PyPI - License] [PyPI - Python Version] [GitHub license] [GitHub last commit]
 --- ## ð Table of Contents - [ð Table of Contents](#-table-of-contents) -
 [ð Overview](#-overview) - [ð¯ *Motivation*](#-motivation) - [â ï¸
 *Disclaimer*](#ï¸-disclaimer) - [ð¾ Demo](#-demo) - [âï¸ Features](#ï¸-
 features) - [ð Getting Started](#-getting-started) - [âï¸ Dependencies]
 (#ï¸-dependencies) - [ð Repository](#-repository) - [ð OpenAI API](#-
 openai-api) - [ð¦ Installation](#-installation) - [ð® Using *README-AI*](#-
 using-readme-ai) - [ð§ª Running Tests](#-running-tests) - [ð  Future
@@ -28,17 +27,17 @@
 improve the adoption and usability of open-source projects, enabling everyone
 to better understand and use open-source tools. #### â ï¸ *Disclaimer*
 *README-AI* is currently under development and has an opinionated configuration
 and setup. While this tool provides an excellent starting point for
 documentation, its important to review all text generated by the OpenAI API to
 ensure it accurately represents your codebase. Ensure all content in your
 repository is free of sensitive information before executing. Additionally,
-regularly monitor your API usage and costs by visiting the [OpenAI API Usage]
-(https://platform.openai.com/account/usage). --- ## ð¾ Demo [readme-ai_demo
-video] --- ## âï¸ Features
+frequently monitor your API usage and costs by visiting the [OpenAI API Usage
+Dashboard](https://platform.openai.com/account/usage). --- ## ð¾ Demo
+[readme-ai_demo_video] --- ## âï¸ Features
                                    ****** 1.
                                      ð
 
                       ð Codebase Documentation ******
 **** â¦ Repository File Summaries ****
     * Code summaries are generated for each file via OpenAI's gpt-3.5-turbo
       engine.
@@ -141,49 +140,51 @@
 Dashboard](https://platform.openai.com/account/usage). Please note that this
 API is not free and you will be charged for each request made, which can
 accumulate rapidly. > > - The generation of the README.md file should typically
 complete in under 1 minute. If it takes longer than a few minutes, please
 terminate the process. > --- ### ð¦ Installation 1. Clone the *readme-ai*
 repository to your local machine. ```sh git clone https://github.com/eli64s/
 readme-ai ``` 2. Navigate to the *readme-ai* directory. ```sh cd readme-ai ```
-3. Use one of the following methods to install the required dependencies: ```sh
-# With Pip pip install readmeai ``` ```sh # With Bash bash setup/setup.sh ```
-```sh # With Conda conda create -n readmeai python=3.9 -y && \ conda activate
-readmeai && \ poetry install ``` ```sh # With Poetry poetry install ``` ```sh #
-With Docker docker pull zeroxeli/readme-ai:0.0.4 ``` ### ð® Using *README-AI*
-Use the command-line to provide the OpenAI API key (if not already set) and
-specify an output path for your README file, along with the path to your local
+3. Use one of the following methods to install the required dependencies: > Pip
+(PyPi Package) ```sh pip install readmeai ``` > Bash ```sh bash setup/setup.sh
+``` > Conda ```sh conda create -n readmeai python=3.9 -y && \ conda activate
+readmeai && \ poetry install ``` > Poetry ```sh poetry install ``` > Docker
+```sh docker pull zeroxeli/readme-ai:0.0.5 ``` ### ð® Using *README-AI* Use
+the command-line to provide the OpenAI API key (if not already set) and specify
+an output path for your README file, along with the path to your local
 repository or remote code repository. You can also provide the output path in
 the [configuration file](./conf/conf.toml) Command-Line Arguments: - `-k` or `-
 -api-key`: Your OpenAI API key. - `-o` or `--output`: The output path for your
 README.md file. - `-r` or `--repository`: The URL or path to your code
 repository. - `-t` or `--template`: The README template format to use. (coming
 soon!) - `l` or `--language`: The language of text written in the README file
-(coming soon!) > Pip ```sh readmeai --api-key "YOUR_API_KEY" --output readme-
-ai.md --repository https://github.com/eli64s/readme-ai # Or export your OpenAI
-API key as an environment variable export OPENAI_API_KEY="YOUR_API_KEY"
-readmeai -k $OPENAI_API_KEY -o readme-ai.md -r https://github.com/eli64s/
-readme-ai ``` > Conda ```sh python readmeai/main.py --api-key "YOUR_API_KEY" --
+(coming soon!) > Pip (PyPi Package) ```sh readmeai --api-key "YOUR_API_KEY" --
 output readme-ai.md --repository https://github.com/eli64s/readme-ai # Or
-export your OpenAI API key as an environment variable conda activate readmeai
-export OPENAI_API_KEY="YOUR_API_KEY" python readmeai/main.py -o readme-ai.md -
-r https://github.com/eli64s/readme-ai ``` > Poetry ```sh poetry shell export
-OPENAI_API_KEY="YOUR_API_KEY" poetry run python readmeai/main.py -o readme-
-ai.md -r https://github.com/eli64s/readme-ai ``` > Docker ```sh docker run -it
-\ -e OPENAI_API_KEY="YOUR_API_KEY" \ -v "$(pwd)":/app \ -w /app zeroxeli/
-readme-ai:0.0.4 \ python readmeai/main.py -o readme-ai.md -r https://
-github.com/eli64s/readme-ai ``` ### ð§ª Running Tests To run the unit-tests
-for README-AI, use the following command. ```bash bash scripts/test.sh ```
+export your OpenAI API key as an environment variable export
+OPENAI_API_KEY="YOUR_API_KEY" readmeai -k $OPENAI_API_KEY -o readme-ai.md -
+r https://github.com/eli64s/readme-ai ``` > Conda ```sh python readmeai/main.py
+--api-key "YOUR_API_KEY" --output readme-ai.md --repository https://github.com/
+eli64s/readme-ai # Or export your OpenAI API key as an environment variable
+conda activate readmeai export OPENAI_API_KEY="YOUR_API_KEY" python readmeai/
+main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai ``` > Poetry
+```sh poetry shell export OPENAI_API_KEY="YOUR_API_KEY" poetry run python
+readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai ``` >
+Docker ```sh docker run -it \ -e OPENAI_API_KEY="YOUR_API_KEY" \ -v "$(pwd)":/
+app zeroxeli/readme-ai:0.0.5 \ readmeai -o readme-ai.md -r https://github.com/
+eli64s/readme-ai ``` ### ð§ª Running Tests To run the unit-tests for README-
+AI, use the following command. ```sh bash scripts/test.sh ```
                                                                     ð_Return
 --- ## ð  Future Development - [X] Add additional language support for
-populating the *installation*, *usage*, and *test* README sections. - [ ]
-Design and implement a variety of README template formats for different use-
-cases. - [ ] Add support for writing the README in any language (i.e. CN, ES,
-FR, JA, KO, RU). - [ ] Create UI with [Textual](https://github.com/Textualize/
-textual) or another framework to improve user experience. --- ## ð Changelog
-[Changelog](./CHANGELOG.md) --- ## ð¤ Contributing [Contributing Guidelines]
-(./CONTRIBUTING.md) --- ## ð License [MIT](./LICENSE) --- ## ð
-Acknowledgments *Badges* - [Shields.io](https://shields.io/) - [Aveek-Saha/
-GitHub-Profile-Badges](https://github.com/Aveek-Saha/GitHub-Profile-Badges) -
-[Ileriayo/Markdown-Badges](https://github.com/Ileriayo/markdown-badges)
+populating the *installation*, *usage*, and *test* README sections. - [X]
+Upload the *readme-ai* cli tool to PyPi under the module name [readmeai](https:
+//pypi.org/project/readmeai/). - [ ] Design and implement a variety of README
+template formats for different use-cases. - [ ] Add support for writing the
+README in any language (i.e. CN, ES, FR, JA, KO, RU). - [ ] Create UI with
+[Textual](https://github.com/Textualize/textual) or another framework to
+improve user experience. --- ## ð Changelog [Changelog](./CHANGELOG.md) --
+- ## ð¤ Contributing [Contributing Guidelines](./CONTRIBUTING.md) --- ## ð
+License [MIT](./LICENSE) --- ## ð Acknowledgments *Badges* - [Shields.io]
+(https://shields.io/) - [Aveek-Saha/GitHub-Profile-Badges](https://github.com/
+Aveek-Saha/GitHub-Profile-Badges) - [Ileriayo/Markdown-Badges](https://
+github.com/Ileriayo/markdown-badges)
                                                                     ð_Return
 ---
```

### Comparing `readmeai-0.0.453/pyproject.toml` & `readmeai-0.0.50/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.0.453"
+version = "0.0.50"
 description = "🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
```

### Comparing `readmeai-0.0.453/readmeai/builder.py` & `readmeai-0.0.50/readmeai/builder.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.453/readmeai/conf.py` & `readmeai-0.0.50/readmeai/conf.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.453/readmeai/factory.py` & `readmeai-0.0.50/readmeai/factory.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.453/readmeai/logger.py` & `readmeai-0.0.50/readmeai/logger.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.453/readmeai/main.py` & `readmeai-0.0.50/readmeai/main.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.453/readmeai/model.py` & `readmeai-0.0.50/readmeai/model.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.453/readmeai/parse.py` & `readmeai-0.0.50/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.453/readmeai/preprocess.py` & `readmeai-0.0.50/readmeai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.453/readmeai/utils.py` & `readmeai-0.0.50/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.453/PKG-INFO` & `readmeai-0.0.50/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmeai
-Version: 0.0.453
+Version: 0.0.50
 Summary: 🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/readme-ai
 License: MIT
 Keywords: markdown,readme,readme-template,shieldsio,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,awesome-chatgpt,openai-python,chatgpt-python,openai-chatbot,gpt-35-turbo,gpt-4-api,llm-agent
 Author: Eli
 Author-email: 0x.eli.64s@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -44,18 +44,18 @@
         <img src="https://img.shields.io/badge/Markdown-000000.svg?stylee&logo=Markdown&logoColor=white" alt="Markdown" />
         <img src="https://img.shields.io/badge/OpenAI-412991.svg?stylee&logo=OpenAI&logoColor=white" alt="OpenAI" />
         <img src="https://img.shields.io/badge/Python-3776AB.svg?stylee&logo=Python&logoColor=white" alt="Python" />
         <img src="https://img.shields.io/badge/Pytest-0A9EDC.svg?stylee&logo=Pytest&logoColor=white" alt="pytest" />
         <img src="https://img.shields.io/badge/GNU%20Bash-4EAA25.svg?stylee&logo=GNU-Bash&logoColor=white" alt="Bash" />
         <img src="https://img.shields.io/badge/Anaconda-44A833.svg?&logo=Anaconda&logoColor=white" alt="Anaconda" />
     </p>
-    <img src="https://img.shields.io/github/languages/top/eli64s/README-AI?color=5D6D7E" alt="GitHub top language" />
-    <img src="https://img.shields.io/github/commit-activity/m/eli64s/README-AI?color=5D6D7E" alt="GitHub commit activity" />
-    <img src="https://img.shields.io/github/last-commit/eli64s/readme-ai?color=5D6D7E" alt="GitHub last commit" />
+    <img src="https://img.shields.io/pypi/v/readmeai?color=5D6D7E&logo=python" alt="PyPI - License" />
+    <img src="https://img.shields.io/pypi/pyversions/readmeai?color=5D6D7E&logo=python" alt="PyPI - Python Version" />
     <img src="https://img.shields.io/github/license/eli64s/README-AI?color=5D6D7E" alt="GitHub license" />
+    <img src="https://img.shields.io/github/last-commit/eli64s/readme-ai?color=5D6D7E" alt="GitHub last commit" />
 </div>
 
 
 ---
 
 ## 📖 Table of Contents
 
@@ -87,15 +87,15 @@
 #### 🎯 *Motivation*
 
 Simplifies the process of writing and maintaining high-quality project documentation. My aim for this project is to provide all skill levels a tool that improves their technical workflow, in an efficient and user-friendly manner. Ultimately, the goal of *README-AI* is to improve the adoption and usability of open-source projects, enabling everyone to better understand and use open-source tools.
 #### ⚠️ *Disclaimer*
 
 *README-AI* is currently under development and has an opinionated configuration and setup. While this tool provides an excellent starting point for documentation, its important to review all text generated by the OpenAI API to ensure it accurately represents your codebase. Ensure all content in your repository is free of sensitive information before executing.
 
-Additionally, regularly monitor your API usage and costs by visiting the [OpenAI API Usage](https://platform.openai.com/account/usage).
+Additionally, frequently monitor your API usage and costs by visiting the [OpenAI API Usage Dashboard](https://platform.openai.com/account/usage).
 
 ---
 
 ## 👾 Demo
 
 <a href="https://youtu.be/pl-VcVfGbbk">
     <img src="examples/imgs/demo.png" alt="readme-ai demo video">
@@ -365,54 +365,54 @@
 2. Navigate to the *readme-ai* directory.
 ```sh
 cd readme-ai
 ```
 
 3. Use one of the following methods to install the required dependencies:
 
+> Pip (PyPi Package)
 ```sh
-# With Pip
 pip install readmeai
 ```
 
+> Bash
 ```sh
-# With Bash
 bash setup/setup.sh
 ```
 
+> Conda
 ```sh
-# With Conda
 conda create -n readmeai python=3.9 -y && \
 conda activate readmeai && \
 poetry install
 ```
 
+> Poetry
 ```sh
-# With Poetry
 poetry install
 ```
 
+> Docker
 ```sh
-# With Docker
-docker pull zeroxeli/readme-ai:0.0.4
+docker pull zeroxeli/readme-ai:0.0.5
 ```
 
 ### 🎮 Using *README-AI*
 
 Use the command-line to provide the OpenAI API key (if not already set) and specify an output path for your README file, along with the path to your local repository or remote code repository. You can also provide the output path in the [configuration file](./conf/conf.toml)
 
 Command-Line Arguments:
 
 - `-k` or `--api-key`: Your OpenAI API key.
 - `-o` or `--output`: The output path for your README.md file.
 - `-r` or `--repository`: The URL or path to your code repository.
 - `-t` or `--template`: The README template format to use. (coming soon!)
 - `l` or `--language`: The language of text written in the README file (coming soon!)
 
-> Pip
+> Pip (PyPi Package)
 ```sh
 readmeai --api-key "YOUR_API_KEY" --output readme-ai.md --repository https://github.com/eli64s/readme-ai
 
 # Or export your OpenAI API key as an environment variable
 export OPENAI_API_KEY="YOUR_API_KEY"
 readmeai -k $OPENAI_API_KEY -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
@@ -434,36 +434,36 @@
 poetry run python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
 > Docker
 ```sh
 docker run -it \
 -e OPENAI_API_KEY="YOUR_API_KEY" \
--v "$(pwd)":/app \
--w /app zeroxeli/readme-ai:0.0.4 \
-python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai
+-v "$(pwd)":/app zeroxeli/readme-ai:0.0.5 \
+readmeai -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
 ### 🧪 Running Tests
 
 To run the unit-tests for README-AI, use the following command.
 
-```bash
+```sh
 bash scripts/test.sh
 ```
 
 <p align="right">
   <a href="#top"><b>🔝 Return </b></a>
 </p>
 
 ---
 
 ## 🛠 Future Development
 
 - [X] Add additional language support for populating the *installation*, *usage*, and *test* README sections.
+- [X] Upload the *readme-ai* cli tool to PyPi under the module name [readmeai](https://pypi.org/project/readmeai/).
 - [ ] Design and implement a variety of README template formats for different use-cases.
 - [ ] Add support for writing the README in any language (i.e. CN, ES, FR, JA, KO, RU).
 - [ ] Create UI with [Textual](https://github.com/Textualize/textual) or another framework to improve user experience.
 
 ---
 
 ## 📒 Changelog
```

