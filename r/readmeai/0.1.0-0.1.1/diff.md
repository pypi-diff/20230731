# Comparing `tmp/readmeai-0.1.0.tar.gz` & `tmp/readmeai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.1.0.tar", max compression
+gzip compressed data, was "readmeai-0.1.1.tar", max compression
```

## Comparing `readmeai-0.1.0.tar` & `readmeai-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-07-31 03:27:10.723147 readmeai-0.1.0/LICENSE
--rw-r--r--   0        0        0    17673 2023-07-31 03:27:10.723147 readmeai-0.1.0/README.md
--rw-r--r--   0        0        0     1927 2023-07-31 03:27:10.763148 readmeai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-31 03:27:10.763148 readmeai-0.1.0/readmeai/__init__.py
--rw-r--r--   0        0        0     7698 2023-07-31 03:27:10.763148 readmeai-0.1.0/readmeai/builder.py
--rw-r--r--   0        0        0     6342 2023-07-31 03:27:10.763148 readmeai-0.1.0/readmeai/conf.py
--rw-r--r--   0        0        0     4893 2023-07-31 03:27:10.763148 readmeai-0.1.0/readmeai/factory.py
--rw-r--r--   0        0        0     1722 2023-07-31 03:27:10.763148 readmeai-0.1.0/readmeai/logger.py
--rwxr-xr-x   0        0        0     3998 2023-07-31 03:27:10.763148 readmeai-0.1.0/readmeai/main.py
--rw-r--r--   0        0        0     7590 2023-07-31 03:27:10.767148 readmeai-0.1.0/readmeai/model.py
--rw-r--r--   0        0        0     7272 2023-07-31 03:27:10.767148 readmeai-0.1.0/readmeai/parse.py
--rw-r--r--   0        0        0     6536 2023-07-31 03:27:10.767148 readmeai-0.1.0/readmeai/preprocess.py
--rw-r--r--   0        0        0     3991 2023-07-31 03:27:10.767148 readmeai-0.1.0/readmeai/utils.py
--rw-r--r--   0        0        0    19190 1970-01-01 00:00:00.000000 readmeai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-31 10:58:03.775669 readmeai-0.1.1/LICENSE
+-rw-r--r--   0        0        0    17931 2023-07-31 10:58:03.775669 readmeai-0.1.1/README.md
+-rw-r--r--   0        0        0     2072 2023-07-31 10:58:03.823673 readmeai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/__init__.py
+-rw-r--r--   0        0        0     7736 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/builder.py
+-rw-r--r--   0        0        0     6342 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/conf.py
+-rw-r--r--   0        0        0     4955 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/factory.py
+-rw-r--r--   0        0        0     2113 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/logger.py
+-rwxr-xr-x   0        0        0     4044 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/main.py
+-rw-r--r--   0        0        0     7608 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/model.py
+-rw-r--r--   0        0        0     7272 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/parse.py
+-rw-r--r--   0        0        0     6419 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/preprocess.py
+-rw-r--r--   0        0        0     3991 2023-07-31 10:58:03.823673 readmeai-0.1.1/readmeai/utils.py
+-rw-r--r--   0        0        0    19409 1970-01-01 00:00:00.000000 readmeai-0.1.1/PKG-INFO
```

### Comparing `readmeai-0.1.0/LICENSE` & `readmeai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.0/README.md` & `readmeai-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,29 @@
     <h3>◦ Developed with OpenAI's GPT language model APIs.</h3>
     <br>
     <p align="center">
         <img src="https://img.shields.io/badge/Markdown-000000.svg?stylee&logo=Markdown&logoColor=white" alt="Markdown" />
         <img src="https://img.shields.io/badge/OpenAI-412991.svg?stylee&logo=OpenAI&logoColor=white" alt="OpenAI" />
         <img src="https://img.shields.io/badge/Python-3776AB.svg?stylee&logo=Python&logoColor=white" alt="Python" />
         <img src="https://img.shields.io/badge/Pytest-0A9EDC.svg?stylee&logo=Pytest&logoColor=white" alt="pytest" />
-        <img src="https://img.shields.io/badge/GNU%20Bash-4EAA25.svg?stylee&logo=GNU-Bash&logoColor=white" alt="Bash" />
-        <img src="https://img.shields.io/badge/Anaconda-44A833.svg?&logo=Anaconda&logoColor=white" alt="Anaconda" />
+        <img src="https://img.shields.io/badge/Docker-2496ED.svg?style&logo=Docker&logoColor=white" alt="Docker" />
+        <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style&logo=GitHub-Actions&logoColor=white" alt="actions" />
     </p>
-    <img src="https://img.shields.io/pypi/v/readmeai?color=5D6D7E&logo=python" alt="PyPI - License" />
-    <img src="https://img.shields.io/pypi/pyversions/readmeai?color=5D6D7E&logo=python" alt="PyPI - Python Version" />
+    <a href="https://pypi.org/project/readmeai/">
+        <img src="https://img.shields.io/pypi/v/readmeai?color=5D6D7E&logo=python" alt="PyPI - License" />
+    </a>
+    <a href="https://pypi.org/project/readmeai/">
+        <img src="https://img.shields.io/pypi/pyversions/readmeai?color=5D6D7E&logo=python" alt="PyPI - Python Version" />
+    </a>
+    <a href="https://pypi.org/project/readmeai/">
+        <img src="https://img.shields.io/pypi/dm/readmeai?color=5D6D7E" alt="PyPI - Downloads" />
+    </a>
     <img src="https://img.shields.io/github/license/eli64s/README-AI?color=5D6D7E" alt="GitHub license" />
-    <img src="https://img.shields.io/github/last-commit/eli64s/readme-ai?color=5D6D7E" alt="GitHub last commit" />
 </div>
 
-
 ---
 
 ## 📖 Table of Contents
 
 - [📖 Table of Contents](#-table-of-contents)
 - [📍 Overview](#-overview)
     - [🎯 *Motivation*](#-motivation)
@@ -45,15 +50,15 @@
 - [📄 License](#-license)
 - [👏 Acknowledgments](#-acknowledgments)
 
 ---
 
 ## 📍 Overview
 
-*README-AI* is a powerful, user-friendly command-line tool that generates extensive README markdown documents for your software and data projects. By providing a remote repository URL or directory path to your codebase, this tool will document your entire project, leveraging the capabilities of large language models and OpenAI's GPT APIs.
+*README-AI* is a powerful, user-friendly command-line tool that generates extensive README markdown documents for your software and data projects. By providing a remote repository URL or path to your codebase, this tool generates documentation for your entire project, leveraging the capabilities of large language models and OpenAI's GPT APIs.
 
 #### 🎯 *Motivation*
 
 Simplifies the process of writing and maintaining high-quality project documentation. My aim for this project is to provide all skill levels a tool that improves their technical workflow, in an efficient and user-friendly manner. Ultimately, the goal of *README-AI* is to improve the adoption and usability of open-source projects, enabling everyone to better understand and use open-source tools.
 #### ⚠️ *Disclaimer*
 
 *README-AI* is currently under development and has an opinionated configuration and setup. While this tool provides an excellent starting point for documentation, its important to review all text generated by the OpenAI API to ensure it accurately represents your codebase. Ensure all content in your repository is free of sensitive information before executing.
@@ -283,24 +288,24 @@
 
 - Python 3.9 or higher
 - Conda or Poetry package manager (recommended)
 - Access to the OpenAI API (see the setup guide below)
 
 #### 📂 Repository
 
-Most user's will run *README-AI* using the command-line, specifying their repository on run-time. However, if you would like to use the default configuration, you will need to update the [configuration file](./conf/conf.toml) with your repository's remote URL (GitHub, GitLab) or local directory path on your machine.
+Most user's will run *README-AI* using the command-line, specifying their repository on run-time. However, if you would like to use the default configuration, you will need to update the [configuration file](./conf/conf.toml) with your repository's remote URL or a local path to your codebase.
 
 ```toml
 [git]
 repository = "Insert your repository URL or local path here!"
 ```
 
 #### 🔐 OpenAI API
 
-To use the README-AI application, you will need to create an account with OpenAI to generate an API key. The steps below outline this setup process:
+To use the *README-AI* app, you must create an OpenAI API account and generate an API key. The steps below outline this process:
 
 <details closed><summary>OpenAI API User Guide</summary>
 
 1. Go to the [OpenAI website](https://platform.openai.com/).
 2. Click the "Sign up for free" button.
 3. Fill out the registration form with your information and agree to the terms of service.
 4. Once logged in, click on the "API" tab.
@@ -319,31 +324,36 @@
 > - The generation of the README.md file should typically complete in under 1 minute. If it takes longer than a few minutes, please terminate the process.
 >
 
 ---
 
 ### 📦 Installation
 
-1. Clone the *readme-ai* repository to your local machine.
+1. Clone the *readme-ai* repository to your machine.
 ```sh
 git clone https://github.com/eli64s/readme-ai
 ```
 
 2. Navigate to the *readme-ai* directory.
 ```sh
 cd readme-ai
 ```
 
-3. Use one of the following methods to install the required dependencies:
+3. Use any of the following methods to install project dependencies.
 
-> *Pip (PyPI Package)*
+> *Pip ([PyPI Package](https://pypi.org/project/readmeai/))*
 ```sh
 pip install readmeai
 ```
 
+> *Docker ([Docker Hub](https://hub.docker.com/repository/docker/zeroxeli/readme-ai/general))*
+```sh
+docker pull zeroxeli/readme-ai:latest
+```
+
 > *Bash*
 ```sh
 bash setup/setup.sh
 ```
 
 > *Conda*
 ```sh
@@ -353,68 +363,62 @@
 ```
 
 > *Poetry*
 ```sh
 poetry install
 ```
 
-> *Docker*
-```sh
-docker pull zeroxeli/readme-ai:0.0.6
-```
-
 ### 🎮 Using *README-AI*
 
 Use the command-line to provide the OpenAI API key (if not already set) and specify an output path for your README file, along with the path to your local repository or remote code repository. You can also provide the output path in the [configuration file](./conf/conf.toml)
 
 Command-Line Arguments:
 
 - `-k` or `--api-key`: Your OpenAI API key.
 - `-o` or `--output`: The output path for your README.md file.
 - `-r` or `--repository`: The URL or path to your code repository.
 - `-t` or `--template`: The README template format to use. (coming soon!)
 - `l` or `--language`: The language of text written in the README file (coming soon!)
 
-> *Pip (PyPI Package)*
+Use any of the following methods to run the *readme-ai* CLI application.
+
+> *Pip ([PyPI Package](https://pypi.org/project/readmeai/))*
 ```sh
 readmeai --api-key "YOUR_API_KEY" --output readme-ai.md --repository https://github.com/eli64s/readme-ai
 
 # Or export your OpenAI API key as an environment variable
 export OPENAI_API_KEY="YOUR_API_KEY"
 readmeai -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
-> *Conda*
+> *Docker ([Docker Hub](https://hub.docker.com/repository/docker/zeroxeli/readme-ai/general))*
 ```sh
-python readmeai/main.py --api-key "YOUR_API_KEY" --output readme-ai.md --repository https://github.com/eli64s/readme-ai
+docker run -it \
+-e OPENAI_API_KEY="YOUR_API_KEY" \
+-v "$(pwd)":/app zeroxeli/readme-ai:latest \
+readmeai -o readme-ai.md -r https://github.com/eli64s/readme-ai
+```
 
-# Or export your OpenAI API key as an environment variable
+> *Conda*
+```sh
 conda activate readmeai
 export OPENAI_API_KEY="YOUR_API_KEY"
 python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
 > *Poetry*
 ```sh
 poetry shell
 export OPENAI_API_KEY="YOUR_API_KEY"
 poetry run python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai
 ```
 
-> *Docker*
-```sh
-docker run -it \
--e OPENAI_API_KEY="YOUR_API_KEY" \
--v "$(pwd)":/app zeroxeli/readme-ai:0.0.6 \
-readmeai -o readme-ai.md -r https://github.com/eli64s/readme-ai
-```
-
 ### 🧪 Running Tests
 
-To run the unit-tests for README-AI, use the following command.
+Execute the following command to run the test suite.
 
 ```sh
 bash scripts/test.sh
 ```
 
 <p align="right">
   <a href="#top"><b>🔝 Return </b></a>
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
     ****** [https://img.icons8.com/?size=512&id=55494&format=png] [https://
              img.icons8.com/?size=512&id=kTuxVYRKeKEY&format=png]
                                README-AI ******
      **** â¦ Generate beautiful and informative README.md documents. ****
         **** â¦ Developed with OpenAI's GPT language model APIs. ****
 
-            [Markdown] [OpenAI] [Python] [pytest] [Bash] [Anaconda]
-[PyPI - License] [PyPI - Python Version] [GitHub license] [GitHub last commit]
+           [Markdown] [OpenAI] [Python] [pytest] [Docker] [actions]
+ [PyPI_-_License] [PyPI_-_Python_Version] [PyPI_-_Downloads] [GitHub license]
 --- ## ð Table of Contents - [ð Table of Contents](#-table-of-contents) -
 [ð Overview](#-overview) - [ð¯ *Motivation*](#-motivation) - [â ï¸
 *Disclaimer*](#ï¸-disclaimer) - [ð¾ Demo](#-demo) - [âï¸ Features](#ï¸-
 features) - [ð Getting Started](#-getting-started) - [âï¸ Dependencies]
 (#ï¸-dependencies) - [ð Repository](#-repository) - [ð OpenAI API](#-
 openai-api) - [ð¦ Installation](#-installation) - [ð® Using *README-AI*](#-
 using-readme-ai) - [ð§ª Running Tests](#-running-tests) - [ð  Future
 Development](#-future-development) - [ð Changelog](#-changelog) - [ð¤
 Contributing](#-contributing) - [ð License](#-license) - [ð
 Acknowledgments](#-acknowledgments) --- ## ð Overview *README-AI* is a
 powerful, user-friendly command-line tool that generates extensive README
 markdown documents for your software and data projects. By providing a remote
-repository URL or directory path to your codebase, this tool will document your
-entire project, leveraging the capabilities of large language models and
+repository URL or path to your codebase, this tool generates documentation for
+your entire project, leveraging the capabilities of large language models and
 OpenAI's GPT APIs. #### ð¯ *Motivation* Simplifies the process of writing and
 maintaining high-quality project documentation. My aim for this project is to
 provide all skill levels a tool that improves their technical workflow, in an
 efficient and user-friendly manner. Ultimately, the goal of *README-AI* is to
 improve the adoption and usability of open-source projects, enabling everyone
 to better understand and use open-source tools. #### â ï¸ *Disclaimer*
 *README-AI* is currently under development and has an opinionated configuration
@@ -115,67 +115,68 @@
                                                                     ð_Return
 --- ## ð Getting Started ### âï¸ Dependencies Before you begin, ensure
 that you have the following prerequisites installed: - Python 3.9 or higher -
 Conda or Poetry package manager (recommended) - Access to the OpenAI API (see
 the setup guide below) #### ð Repository Most user's will run *README-AI*
 using the command-line, specifying their repository on run-time. However, if
 you would like to use the default configuration, you will need to update the
-[configuration file](./conf/conf.toml) with your repository's remote URL
-(GitHub, GitLab) or local directory path on your machine. ```toml [git]
-repository = "Insert your repository URL or local path here!" ``` #### ð
-OpenAI API To use the README-AI application, you will need to create an account
-with OpenAI to generate an API key. The steps below outline this setup process:
-OpenAI API User Guide 1. Go to the [OpenAI website](https://
-platform.openai.com/). 2. Click the "Sign up for free" button. 3. Fill out the
-registration form with your information and agree to the terms of service. 4.
-Once logged in, click on the "API" tab. 5. Follow the instructions to create a
-new API key. 6. Copy the API key and keep it in a secure place.
+[configuration file](./conf/conf.toml) with your repository's remote URL or a
+local path to your codebase. ```toml [git] repository = "Insert your repository
+URL or local path here!" ``` #### ð OpenAI API To use the *README-AI* app,
+you must create an OpenAI API account and generate an API key. The steps below
+outline this process: OpenAI API User Guide 1. Go to the [OpenAI website]
+(https://platform.openai.com/). 2. Click the "Sign up for free" button. 3. Fill
+out the registration form with your information and agree to the terms of
+service. 4. Once logged in, click on the "API" tab. 5. Follow the instructions
+to create a new API key. 6. Copy the API key and keep it in a secure place.
 > **â ï¸ Note** > > - To maximize your experience with README-AI, it is
 recommended to set up a payment method on OpenAI's website. By doing so, you
 gain access to more powerful language models like gpt-3.5-turbo. Without a
 payment method, your usage will be restricted to the base gpt-3 models. This
 limitation might lead to less precise README files or potential errors during
 the generation process. > > - When using a payment method, make sure you have
 sufficient credits to run the README-AI application. Additionally, remember to
 regularly monitor your API usage and costs by visiting the [OpenAI API Usage
 Dashboard](https://platform.openai.com/account/usage). Please note that this
 API is not free and you will be charged for each request made, which can
 accumulate rapidly. > > - The generation of the README.md file should typically
 complete in under 1 minute. If it takes longer than a few minutes, please
 terminate the process. > --- ### ð¦ Installation 1. Clone the *readme-ai*
-repository to your local machine. ```sh git clone https://github.com/eli64s/
-readme-ai ``` 2. Navigate to the *readme-ai* directory. ```sh cd readme-ai ```
-3. Use one of the following methods to install the required dependencies: >
-*Pip (PyPI Package)* ```sh pip install readmeai ``` > *Bash* ```sh bash setup/
-setup.sh ``` > *Conda* ```sh conda create -n readmeai python=3.9 -y && \ conda
-activate readmeai && \ pip install -r requirements.txt ``` > *Poetry* ```sh
-poetry install ``` > *Docker* ```sh docker pull zeroxeli/readme-ai:0.0.6 ```
-### ð® Using *README-AI* Use the command-line to provide the OpenAI API key
-(if not already set) and specify an output path for your README file, along
-with the path to your local repository or remote code repository. You can also
-provide the output path in the [configuration file](./conf/conf.toml) Command-
-Line Arguments: - `-k` or `--api-key`: Your OpenAI API key. - `-o` or `--
-output`: The output path for your README.md file. - `-r` or `--repository`: The
-URL or path to your code repository. - `-t` or `--template`: The README
-template format to use. (coming soon!) - `l` or `--language`: The language of
-text written in the README file (coming soon!) > *Pip (PyPI Package)* ```sh
+repository to your machine. ```sh git clone https://github.com/eli64s/readme-ai
+``` 2. Navigate to the *readme-ai* directory. ```sh cd readme-ai ``` 3. Use any
+of the following methods to install project dependencies. > *Pip ([PyPI
+Package](https://pypi.org/project/readmeai/))* ```sh pip install readmeai ``` >
+*Docker ([Docker Hub](https://hub.docker.com/repository/docker/zeroxeli/readme-
+ai/general))* ```sh docker pull zeroxeli/readme-ai:latest ``` > *Bash* ```sh
+bash setup/setup.sh ``` > *Conda* ```sh conda create -n readmeai python=3.9 -
+y && \ conda activate readmeai && \ pip install -r requirements.txt ``` >
+*Poetry* ```sh poetry install ``` ### ð® Using *README-AI* Use the command-
+line to provide the OpenAI API key (if not already set) and specify an output
+path for your README file, along with the path to your local repository or
+remote code repository. You can also provide the output path in the
+[configuration file](./conf/conf.toml) Command-Line Arguments: - `-k` or `--
+api-key`: Your OpenAI API key. - `-o` or `--output`: The output path for your
+README.md file. - `-r` or `--repository`: The URL or path to your code
+repository. - `-t` or `--template`: The README template format to use. (coming
+soon!) - `l` or `--language`: The language of text written in the README file
+(coming soon!) Use any of the following methods to run the *readme-ai* CLI
+application. > *Pip ([PyPI Package](https://pypi.org/project/readmeai/))* ```sh
 readmeai --api-key "YOUR_API_KEY" --output readme-ai.md --repository https://
 github.com/eli64s/readme-ai # Or export your OpenAI API key as an environment
 variable export OPENAI_API_KEY="YOUR_API_KEY" readmeai -o readme-ai.md -
-r https://github.com/eli64s/readme-ai ``` > *Conda* ```sh python readmeai/
-main.py --api-key "YOUR_API_KEY" --output readme-ai.md --repository https://
-github.com/eli64s/readme-ai # Or export your OpenAI API key as an environment
-variable conda activate readmeai export OPENAI_API_KEY="YOUR_API_KEY" python
-readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai ``` >
-*Poetry* ```sh poetry shell export OPENAI_API_KEY="YOUR_API_KEY" poetry run
+r https://github.com/eli64s/readme-ai ``` > *Docker ([Docker Hub](https://
+hub.docker.com/repository/docker/zeroxeli/readme-ai/general))* ```sh docker run
+-it \ -e OPENAI_API_KEY="YOUR_API_KEY" \ -v "$(pwd)":/app zeroxeli/readme-ai:
+latest \ readmeai -o readme-ai.md -r https://github.com/eli64s/readme-ai ``` >
+*Conda* ```sh conda activate readmeai export OPENAI_API_KEY="YOUR_API_KEY"
 python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/readme-ai
-``` > *Docker* ```sh docker run -it \ -e OPENAI_API_KEY="YOUR_API_KEY" \ -v "$
-(pwd)":/app zeroxeli/readme-ai:0.0.6 \ readmeai -o readme-ai.md -r https://
-github.com/eli64s/readme-ai ``` ### ð§ª Running Tests To run the unit-tests
-for README-AI, use the following command. ```sh bash scripts/test.sh ```
+``` > *Poetry* ```sh poetry shell export OPENAI_API_KEY="YOUR_API_KEY" poetry
+run python readmeai/main.py -o readme-ai.md -r https://github.com/eli64s/
+readme-ai ``` ### ð§ª Running Tests Execute the following command to run the
+test suite. ```sh bash scripts/test.sh ```
                                                                     ð_Return
 --- ## ð  Future Development - [X] Add additional language support for
 populating the *installation*, *usage*, and *test* README sections. - [X]
 Upload the *readme-ai* CLI tool to PyPI under the module name [readmeai](https:
 //pypi.org/project/readmeai/). - [ ] Design and implement a variety of README
 template formats for different use-cases. - [ ] Add support for writing the
 README in any language (i.e. CN, ES, FR, JA, KO, RU). - [ ] Create UI with
```

### Comparing `readmeai-0.1.0/pyproject.toml` & `readmeai-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.1.0"
+version = "0.1.1"
 description = "🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
@@ -42,15 +42,14 @@
 pre-commit = "*"
 ruff = "*"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 colorlog = "^6.7.0"
 cachetools = "^5.3.1"
-dacite = "^1.8.1"
 gitpython = "^3.1.31"
 httpx = "^0.24.1"
 h2 = "^4.1.0"
 openai = "^0.27.8"
 pyyaml = "^6.0"
 responses = "^0.23.1"
 tabulate = "^0.9.0"
@@ -72,24 +71,30 @@
   "UP", # pyupgrade
   "RUF", # ruff
   "B", # flake8-bugbear
   "C4", # flake8-comprehensions
   "PTH", # flake8-use-pathlib
   "SIM", # flake8-simplify
   "TID", # flake8-tidy-imports
-
 ]
 
 [tool.ruff.isort]
 force-sort-within-sections = true
 split-on-trailing-comma = false
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
+[tool.isort]
+profile = "black"
+line_length = 88
+multi_line_output = 3
+include_trailing_comma = true
+virtual_env = ["venv", ".venv", "env", ".env", ".tox", ".nox"]
+
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 python_files = "test_*.py"
 addopts = "--strict-markers --disable-pytest-warnings"
 
 [tool.coverage.run]
 omit = ["tests/*", "*/__init__.py"]
```

### Comparing `readmeai-0.1.0/readmeai/builder.py` & `readmeai-0.1.1/readmeai/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,66 +7,66 @@
 
 from . import conf, factory, logger, utils
 
 LOGGER = logger.Logger(__name__)
 
 
 def build_markdown_file(
-    conf: conf.AppConfig,
+    config: conf.AppConfig,
     helper: conf.ConfigHelper,
     packages: list,
     summaries: tuple,
 ) -> None:
     """Builds the README Markdown file for your codebase."""
-    readme_sections = create_markdown_sections(conf, helper, packages, summaries)
+    readme_sections = create_markdown_sections(config, helper, packages, summaries)
     readme_file = "\n".join(readme_sections)
-    readme_path = Path.cwd() / conf.paths.readme
+    readme_path = Path.cwd() / config.paths.readme
     factory.FileHandler().write(readme_path, readme_file)
     LOGGER.info(f"README file generated at: {readme_path}")
 
 
 def create_markdown_sections(
-    conf: conf.AppConfig,
+    config: conf.AppConfig,
     helper: conf.ConfigHelper,
     packages: list,
     summaries: tuple,
 ) -> List[str]:
     """Creates each section of the README Markdown file."""
-    name = conf.git.name
-    repository = conf.git.repository
+    name = config.git.name
+    repository = config.git.repository
     user_repo = utils.get_user_repository_name(repository)
     cwd_path = Path.cwd()
-    badges_path = cwd_path / conf.paths.badges
+    badges_path = cwd_path / config.paths.badges
     badges_dict = factory.FileHandler().read(badges_path)
 
-    markdown_badges = conf.md.badges.format(
+    markdown_badges = config.md.badges.format(
         get_badges(badges_dict, packages), user_repo
     )
     markdown_badges = (
         utils.remove_substring(markdown_badges)
         if "invalid" in user_repo.lower()
         else markdown_badges
     )
     markdown_repository = create_directory_tree(repository)
     markdown_tables = create_tables(
-        create_markdown_tables(summaries), conf.md.dropdown, user_repo
+        create_markdown_tables(summaries), config.md.dropdown, user_repo
     )
-    markdown_setup_guide = create_setup_guide(conf, helper, summaries)
+    markdown_setup_guide = create_setup_guide(config, helper, summaries)
 
     markdown_sections = [
-        conf.md.header,
+        config.md.header,
         markdown_badges,
-        conf.md.toc,
-        conf.md.intro,
-        conf.md.tree,
+        config.md.toc,
+        config.md.intro,
+        config.md.tree,
         markdown_repository,
-        conf.md.modules,
+        config.md.modules,
         markdown_tables,
-        conf.md.setup.format(name, repository, *markdown_setup_guide),
-        conf.md.ending,
+        config.md.setup.format(name, repository, *markdown_setup_guide),
+        config.md.ending,
     ]
     return markdown_sections
 
 
 def get_badges(svg_icons: dict, dependencies: list) -> str:
     """Returns a list of badges for the project dependencies."""
     badges = [
@@ -109,21 +109,21 @@
     summary_list = []
     for module, summary in summaries:
         summary_list.append((module, summary))
     return summary_list
 
 
 def create_setup_guide(
-    conf: conf.AppConfig, helper: conf.ConfigHelper, summary_list: list
+    config: conf.AppConfig, helper: conf.ConfigHelper, summary_list: list
 ):
     """Creates the 'Getting Started' section of the README file."""
     try:
         default_install_command = (
             default_run_command
-        ) = default_test_command = conf.md.default
+        ) = default_test_command = config.md.default
 
         language_counts = {}
         for module, _ in summary_list:
             language = Path(module).suffix[1:]
             if language and language not in helper.ignore_files:
                 if language in language_counts:
                     language_counts[language] += 1
```

### Comparing `readmeai-0.1.0/readmeai/conf.py` & `readmeai-0.1.1/readmeai/conf.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.0/readmeai/factory.py` & `readmeai-0.1.1/readmeai/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,28 +32,28 @@
 
     def read(self, file_path: Union[str, Path]) -> Any:
         """Read the content of a file."""
         if file_path in self.cache:
             return self.cache[file_path]
 
         try:
-            file_extension = str(file_path).split(".")[-1]
+            file_extension = str(file_path).rsplit(".", maxsplit=1)[-1]
             reader = self.get_action(file_extension, "read")
             content = reader(file_path)
             self.cache[file_path] = content
             return content
         except Exception as excinfo:
             raise ReadFileException(
                 f"Exception: failed to read file {file_path}: {excinfo}"
             )
 
     def write(self, file_path: Union[str, Path], content: Any) -> None:
         """Write the content to a file."""
         try:
-            file_extension = str(file_path).split(".")[-1]
+            file_extension = str(file_path).rsplit(".", maxsplit=1)[-1]
             writer = self.get_action(file_extension, "write")
             writer(file_path, content)
         except Exception as excinfo:
             raise WriteFileException(
                 f"Exception: failed to write file {file_path}: {excinfo}"
             )
 
@@ -68,15 +68,15 @@
             raise ValueError(f"Unsupported action type: {action_type}")
 
         return action
 
     @staticmethod
     def read_json(file_path: Union[str, Path]) -> Dict[str, Any]:
         """Read the content of a JSON file."""
-        with open(file_path, "r") as file:
+        with open(file_path, "r", encoding="utf-8") as file:
             return json.load(file)
 
     @staticmethod
     def read_markdown(file_path: Union[str, Path]) -> str:
         """Read the content of a Markdown file."""
         with open(file_path, encoding="utf-8") as file:
             return file.read()
@@ -100,15 +100,15 @@
         """Read the content of a YAML file."""
         with open(file_path, "r", encoding="utf-8") as file:
             return yaml.safe_load(file)
 
     @staticmethod
     def write_json(file_path: Union[str, Path], content: Dict[str, Any]) -> None:
         """Write the content to a JSON file."""
-        with open(file_path, "w") as file:
+        with open(file_path, "w", encoding="utf-8") as file:
             json.dump(content, file, indent=4)
 
     @staticmethod
     def write_markdown(file_path: Union[str, Path], content: str) -> None:
         """Write the content to a Markdown file."""
         with open(file_path, "w", encoding="utf-8") as file:
             file.write(content)
```

### Comparing `readmeai-0.1.0/readmeai/logger.py` & `readmeai-0.1.1/readmeai/logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,53 +3,63 @@
 import logging
 import sys
 
 from colorlog import ColoredFormatter
 
 
 class Logger:
+    """Custom logger implementation."""
+
     _instance = None
 
     def __new__(cls, name, level="DEBUG"):
+        """Checks if an instance of the Logger class exists."""
         if cls._instance is None:
             cls._instance = super().__new__(cls)
-            cls._instance.name = name
-            cls._instance.level = level
+            cls._instance._name = name
+            cls._instance._level = level
             cls._instance._configure_logger()
         return cls._instance
 
     def _configure_logger(self):
+        """Configures the logger."""
         formatter = ColoredFormatter(
             "%(log_color)s%(levelname)-8s%(reset)s %(blue)s%(message)s",
             datefmt=None,
             reset=True,
             log_colors={
                 "DEBUG": "cyan",
                 "INFO": "green",
                 "WARNING": "yellow",
                 "ERROR": "red",
                 "CRITICAL": "red",
             },
         )
         handler = logging.StreamHandler(sys.stderr)
         handler.setFormatter(formatter)
-        logger = logging.getLogger(self.name)
+        logger = logging.getLogger(self._name)
         logger.addHandler(handler)
-        logger.setLevel(self.level)
+        logger.setLevel(self._level)
 
     def info(self, msg, *args, **kwargs):
-        logging.getLogger(self.name).info(msg, *args, **kwargs)
+        """Logs an info message."""
+        logging.getLogger(self._name).info(msg, *args, **kwargs)
 
     def debug(self, msg, *args, **kwargs):
-        logging.getLogger(self.name).debug(msg, *args, **kwargs)
+        """Logs a debug message."""
+        logging.getLogger(self._name).debug(msg, *args, **kwargs)
 
     def warning(self, msg, *args, **kwargs):
-        logging.getLogger(self.name).warning(msg, *args, **kwargs)
+        """Logs a warning message."""
+        logging.getLogger(self._name).warning(msg, *args, **kwargs)
 
     def error(self, msg, *args, **kwargs):
-        logging.getLogger(self.name).error(msg, *args, **kwargs)
+        """Logs an error message."""
+        logging.getLogger(self._name).error(msg, *args, **kwargs)
 
     def critical(self, msg, *args, **kwargs):
-        logging.getLogger(self.name).critical(msg, *args, **kwargs)
+        """Logs a critical message."""
+        logging.getLogger(self._name).critical(msg, *args, **kwargs)
 
     def log(self, level, msg, *args, **kwargs):
-        logging.getLogger(self.name).log(level, msg, *args, **kwargs)
+        """Logs a message at the specified level."""
+        logging.getLogger(self._name).log(level, msg, *args, **kwargs)
```

### Comparing `readmeai-0.1.0/readmeai/main.py` & `readmeai-0.1.1/readmeai/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #!/usr/bin/env python3
 
+"""Main entrypoint for README-AI application."""
+
 import asyncio
 import os
 from typing import Dict, List, Optional, Tuple
 
 import click
 
 from . import builder, conf, logger, model, preprocess
@@ -16,15 +18,15 @@
 
 async def main(api_key: str, output: str, repository: str) -> None:
     """Main entrypoint for README-AI application."""
     conf.ApiConfig.validate_api_key(api_key)
     conf.GitConfig.validate_repository(repository)
     config.git = conf.GitConfig(repository=repository)
     config.paths.readme = output
-    logger.info("Model: %s", dict(config.api, api_key=("*" * 16)))
+    logger.info("Model: %s", dict(config.api, api_key="*" * 16))
     logger.info("Repository: %s", config.git)
     llm = model.OpenAIHandler(config)
     await generate_readme(llm)
 
 
 async def generate_readme(llm: model.OpenAIHandler) -> None:
     """Orchestrates the README file generation process."""
@@ -123,12 +125,12 @@
     repository: str,
     template: Optional[int],
     language: Optional[str],
 ) -> None:
     """Cli entrypoint for readme-ai pypi package."""
     logger.info("README-AI is now executing.")
     asyncio.run(main(api_key, output, repository))
-    logger.info("README-AI execution complete.\n")
+    logger.info("README-AI execution complete.")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `readmeai-0.1.0/readmeai/model.py` & `readmeai-0.1.1/readmeai/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 
 
 class OpenAIHandler:
     """OpenAI API handler for generating text for the README.md file."""
 
     logger = logger.Logger(__name__)
 
-    def __init__(self, conf: conf.AppConfig):
+    def __init__(self, config: conf.AppConfig):
         """Initialize the OpenAI API handler.
 
         Parameters
         ----------
-        conf : conf.AppConfig
+        config : conf.AppConfig
             Configuration constant values.
         """
-        self.endpoint = conf.api.endpoint
-        self.engine = conf.api.engine
-        self.tokens = conf.api.tokens
-        self.tokens_max = conf.api.tokens_max
-        self.temperature = conf.api.temperature
-        self.rate_limit = conf.api.rate_limit
+        self.endpoint = config.api.endpoint
+        self.engine = config.api.engine
+        self.tokens = config.api.tokens
+        self.tokens_max = config.api.tokens_max
+        self.temperature = config.api.temperature
+        self.rate_limit = config.api.rate_limit
         self.cache = TTLCache(maxsize=500, ttl=600)
         self.http_client = httpx.AsyncClient(
             http2=True,
             timeout=30,
             limits=httpx.Limits(max_keepalive_connections=10, max_connections=100),
         )
         self.last_request_time = time.monotonic()
@@ -185,15 +185,15 @@
                 summary = data["choices"][0]["message"]["content"]
                 summary = utils.format_sentence(summary) if index != 3 else summary
 
                 self.logger.info(f"\nProcessing prompt: {index}\nResponse: {summary}")
                 self.cache[prompt] = summary
                 return index, summary
 
-        except openai.OpenAIException as excinfo:
+        except openai.error.OpenAIError as excinfo:
             self.logger.error(f"OpenAI Exception:\n{str(excinfo)}")
             return await self.null_summary(
                 index, f"OpenAI exception: {excinfo.response.status_code}"
             )
 
         except httpx.HTTPStatusError as excinfo:
             self.logger.error(f"HTTPStatus Exception:\n{str(excinfo)}")
```

### Comparing `readmeai-0.1.0/readmeai/parse.py` & `readmeai-0.1.1/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.0/readmeai/preprocess.py` & `readmeai-0.1.1/readmeai/preprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,53 +6,51 @@
 
 from . import conf, parse, utils
 
 
 class RepositoryParserWrapper:
     """Wrapper class for the RepositoryParser."""
 
-    def __init__(self, conf: conf.AppConfig, conf_helper: conf.ConfigHelper):
+    def __init__(self, config: conf.AppConfig, conf_helper: conf.ConfigHelper):
         self.parser = RepositoryParser(
-            conf, conf_helper.language_names, conf_helper.language_setup
+            config, conf_helper.language_names, conf_helper.language_setup
         )
 
     def get_unique_contents(self, contents: Dict, keys: List[str]) -> List[str]:
-        """Extracts the unqiue contents from the list of dicts."""
-        unique_contents = []
-        for key in keys:
-            unique_contents += list(set([data[key] for data in contents]))
-        return unique_contents
+        """Extracts the unique contents from the list of dicts."""
+        unique_contents = {data[key] for key in keys for data in contents}
+        return list(unique_contents)
 
     def get_file_contents(self, contents: Dict) -> Dict[str, str]:
         """Extracts the file contents from the list of dicts."""
         return {content["path"]: content["content"] for content in contents}
 
     def get_dependencies(
         self, repository: str, is_remote: bool = True
     ) -> Tuple[List[str], Dict[str, str]]:
-        """Extracts the dependencies and software used in the user's repository."""
+        """Extracts the dependencies of the user's repository."""
         contents = self.parser.analyze(repository, is_remote)
         dependencies = self.parser.get_dependency_file_contents(contents)
         attributes = ["extension", "language", "name"]
         dependencies.extend(self.get_unique_contents(contents, attributes))
         return list(set(dependencies)), self.get_file_contents(contents)
 
 
 class RepositoryParser:
     """Analyzes a local or remote git repository."""
 
     def __init__(
         self,
-        conf: conf.AppConfig,
+        config: conf.AppConfig,
         language_names: Dict[str, str],
         language_setup: Dict[str, str],
     ):
         self.language_names = language_names
         self.language_setup = language_setup
-        self.encoding_name = conf.api.encoding
+        self.encoding_name = config.api.encoding
 
     def analyze(self, root_path: str, is_remote: bool = False) -> List[Dict]:
         """Analyzes a local or remote git repository."""
         with tempfile.TemporaryDirectory() as temp_dir:
             if is_remote:
                 utils.clone_repository(root_path, temp_dir)
                 root_path = temp_dir
@@ -76,41 +74,40 @@
 
     def get_dependency_file_contents(self, contents: List[Dict]) -> List[str]:
         """Extracts dependency file contents from the list of dicts."""
         file_parsers = self._get_file_parsers()
         dependency_files = [
             content
             for content in contents
-            if any(file_name in content["name"] for file_name in file_parsers.keys())
+            if any(file_name in content["name"] for file_name in file_parsers)
         ]
 
         parsed_contents = []
         for content in dependency_files:
             parser = file_parsers[content["name"]]
             parsed_content = parser(content["content"])
             parsed_contents.append(parsed_content)
 
         return utils.flatten_list(parsed_contents)
 
     def generate_file_info(
         self, code_root: Path
     ) -> Generator[Tuple[str, Path, str], None, None]:
         """Generates a tuple of file information."""
-        for p in code_root.rglob("*"):
-            if p.is_file():
-                # Edge cases to handle, make more programmatic later
-                if str(p.relative_to(code_root)).startswith(".git/"):
+        for file_path in code_root.rglob("*"):
+            if file_path.is_file():
+                if str(file_path.relative_to(code_root)).startswith(".git/"):
                     continue
-                if ".github/workflows" in str(p.relative_to(code_root)):
-                    yield "github actions", p.relative_to(code_root), ""
+                if ".github/workflows" in str(file_path.relative_to(code_root)):
+                    yield "github actions", file_path.relative_to(code_root), ""
                 try:
-                    with p.open(encoding="utf-8") as file:
+                    with file_path.open(encoding="utf-8") as file:
                         content = file.read()
-                    relative_path = p.relative_to(code_root)
-                    yield p.name, relative_path, content
+                    relative_path = file_path.relative_to(code_root)
+                    yield file_path.name, relative_path, content
                 except UnicodeDecodeError:
                     continue
 
     def tokenize_content(self, contents: List[Dict]) -> List[Dict]:
         """Tokenizes the content of each file."""
         for content in contents:
             content["tokens"] = utils.get_token_count(
@@ -122,15 +119,15 @@
         """Maps file extensions to their programming languages."""
         for content in contents:
             content["language"] = self.language_names.get(
                 content["extension"], ""
             ).lower()
             setup = self.language_setup.get(content["language"], "")
             setup = setup if isinstance(setup, list) else [None, None]
-            while len(setup) < 3:  # Ensure there are three elements in the list
+            while len(setup) < 3:
                 setup.append(None)
             content["install"], content["run"], content["test"] = setup
         return contents
 
     @staticmethod
     def _get_file_parsers() -> Dict[str, callable]:
         """Returns a dictionary of callable file parser methods."""
```

### Comparing `readmeai-0.1.0/readmeai/utils.py` & `readmeai-0.1.1/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.1.0/PKG-INFO` & `readmeai-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7265 6164  : 2.1.Name: read
 00000020: 6d65 6169 0a56 6572 7369 6f6e 3a20 302e  meai.Version: 0.
-00000030: 312e 300a 5375 6d6d 6172 793a 20f0 9f9a  1.0.Summary: ...
+00000030: 312e 310a 5375 6d6d 6172 793a 20f0 9f9a  1.1.Summary: ...
 00000040: 8020 4765 6e65 7261 7465 2061 7765 736f  . Generate aweso
 00000050: 6d65 2052 4541 444d 452e 6d64 2066 696c  me README.md fil
 00000060: 6573 2066 726f 6d20 7468 6520 7465 726d  es from the term
 00000070: 696e 616c 2c20 706f 7765 7265 6420 6279  inal, powered by
 00000080: 204f 7065 6e41 4927 7320 4750 5420 6c61   OpenAI's GPT la
 00000090: 6e67 7561 6765 206d 6f64 656c 2041 5049  nguage model API
 000000a0: 7320 f09f 92ab 0a48 6f6d 652d 7061 6765  s .....Home-page
@@ -51,1150 +51,1164 @@
 00000320: 3a20 6361 6368 6574 6f6f 6c73 2028 3e3d  : cachetools (>=
 00000330: 352e 332e 312c 3c36 2e30 2e30 290a 5265  5.3.1,<6.0.0).Re
 00000340: 7175 6972 6573 2d44 6973 743a 2063 6c69  quires-Dist: cli
 00000350: 636b 2028 3e3d 382e 312e 362c 3c39 2e30  ck (>=8.1.6,<9.0
 00000360: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
 00000370: 743a 2063 6f6c 6f72 6c6f 6720 283e 3d36  t: colorlog (>=6
 00000380: 2e37 2e30 2c3c 372e 302e 3029 0a52 6571  .7.0,<7.0.0).Req
-00000390: 7569 7265 732d 4469 7374 3a20 6461 6369  uires-Dist: daci
-000003a0: 7465 2028 3e3d 312e 382e 312c 3c32 2e30  te (>=1.8.1,<2.0
-000003b0: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-000003c0: 743a 2067 6974 7079 7468 6f6e 2028 3e3d  t: gitpython (>=
-000003d0: 332e 312e 3331 2c3c 342e 302e 3029 0a52  3.1.31,<4.0.0).R
-000003e0: 6571 7569 7265 732d 4469 7374 3a20 6832  equires-Dist: h2
-000003f0: 2028 3e3d 342e 312e 302c 3c35 2e30 2e30   (>=4.1.0,<5.0.0
-00000400: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000410: 2068 7474 7078 2028 3e3d 302e 3234 2e31   httpx (>=0.24.1
-00000420: 2c3c 302e 3235 2e30 290a 5265 7175 6972  ,<0.25.0).Requir
-00000430: 6573 2d44 6973 743a 206f 7065 6e61 6920  es-Dist: openai 
-00000440: 283e 3d30 2e32 372e 382c 3c30 2e32 382e  (>=0.27.8,<0.28.
-00000450: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
-00000460: 3a20 7079 6461 6e74 6963 2028 3e3d 312e  : pydantic (>=1.
-00000470: 3130 2e39 2c3c 322e 302e 3029 0a52 6571  10.9,<2.0.0).Req
-00000480: 7569 7265 732d 4469 7374 3a20 7079 7961  uires-Dist: pyya
-00000490: 6d6c 2028 3e3d 362e 302c 3c37 2e30 290a  ml (>=6.0,<7.0).
-000004a0: 5265 7175 6972 6573 2d44 6973 743a 2072  Requires-Dist: r
-000004b0: 6573 706f 6e73 6573 2028 3e3d 302e 3233  esponses (>=0.23
-000004c0: 2e31 2c3c 302e 3234 2e30 290a 5265 7175  .1,<0.24.0).Requ
-000004d0: 6972 6573 2d44 6973 743a 2074 6162 756c  ires-Dist: tabul
-000004e0: 6174 6520 283e 3d30 2e39 2e30 2c3c 302e  ate (>=0.9.0,<0.
-000004f0: 3130 2e30 290a 5265 7175 6972 6573 2d44  10.0).Requires-D
-00000500: 6973 743a 2074 656e 6163 6974 7920 283e  ist: tenacity (>
-00000510: 3d38 2e32 2e32 2c3c 392e 302e 3029 0a52  =8.2.2,<9.0.0).R
-00000520: 6571 7569 7265 732d 4469 7374 3a20 7469  equires-Dist: ti
-00000530: 6b74 6f6b 656e 2028 3e3d 302e 342e 302c  ktoken (>=0.4.0,
-00000540: 3c30 2e35 2e30 290a 5265 7175 6972 6573  <0.5.0).Requires
-00000550: 2d44 6973 743a 2074 6f6d 6c20 283e 3d30  -Dist: toml (>=0
-00000560: 2e31 302e 322c 3c30 2e31 312e 3029 0a50  .10.2,<0.11.0).P
-00000570: 726f 6a65 6374 2d55 524c 3a20 446f 6375  roject-URL: Docu
-00000580: 6d65 6e74 6174 696f 6e2c 2068 7474 7073  mentation, https
-00000590: 3a2f 2f67 6974 6875 622e 636f 6d2f 656c  ://github.com/el
-000005a0: 6936 3473 2f72 6561 646d 652d 6169 2f62  i64s/readme-ai/b
-000005b0: 6c6f 622f 6d61 696e 2f52 4541 444d 452e  lob/main/README.
-000005c0: 6d64 0a44 6573 6372 6970 7469 6f6e 2d43  md.Description-C
-000005d0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-000005e0: 742f 6d61 726b 646f 776e 0a0a 3c64 6976  t/markdown..<div
-000005f0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00000600: 0a20 2020 203c 6831 2061 6c69 676e 3d22  .    <h1 align="
-00000610: 6365 6e74 6572 223e 0a20 2020 2020 2020  center">.       
-00000620: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000630: 3a2f 2f69 6d67 2e69 636f 6e73 382e 636f  ://img.icons8.co
-00000640: 6d2f 3f73 697a 653d 3531 3226 6964 3d35  m/?size=512&id=5
-00000650: 3534 3934 2666 6f72 6d61 743d 706e 6722  5494&format=png"
-00000660: 2077 6964 7468 3d22 3830 2220 2f3e 0a20   width="80" />. 
-00000670: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
-00000680: 2268 7474 7073 3a2f 2f69 6d67 2e69 636f  "https://img.ico
-00000690: 6e73 382e 636f 6d2f 3f73 697a 653d 3531  ns8.com/?size=51
-000006a0: 3226 6964 3d6b 5475 7856 5952 4b65 4b45  2&id=kTuxVYRKeKE
-000006b0: 5926 666f 726d 6174 3d70 6e67 2220 7769  Y&format=png" wi
-000006c0: 6474 683d 2238 3022 202f 3e0a 2020 2020  dth="80" />.    
-000006d0: 2020 2020 3c62 723e 5245 4144 4d45 2d41      <br>README-A
-000006e0: 490a 2020 2020 3c2f 6831 3e0a 2020 2020  I.    </h1>.    
-000006f0: 3c68 333e e297 a620 4765 6e65 7261 7465  <h3>... Generate
-00000700: 2062 6561 7574 6966 756c 2061 6e64 2069   beautiful and i
-00000710: 6e66 6f72 6d61 7469 7665 2052 4541 444d  nformative READM
-00000720: 452e 6d64 2064 6f63 756d 656e 7473 2e3c  E.md documents.<
-00000730: 2f68 333e 0a20 2020 203c 6833 3ee2 97a6  /h3>.    <h3>...
-00000740: 2044 6576 656c 6f70 6564 2077 6974 6820   Developed with 
-00000750: 4f70 656e 4149 2773 2047 5054 206c 616e  OpenAI's GPT lan
-00000760: 6775 6167 6520 6d6f 6465 6c20 4150 4973  guage model APIs
-00000770: 2e3c 2f68 333e 0a20 2020 203c 6272 3e0a  .</h3>.    <br>.
-00000780: 2020 2020 3c70 2061 6c69 676e 3d22 6365      <p align="ce
-00000790: 6e74 6572 223e 0a20 2020 2020 2020 203c  nter">.        <
-000007a0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000007b0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000007c0: 6261 6467 652f 4d61 726b 646f 776e 2d30  badge/Markdown-0
-000007d0: 3030 3030 302e 7376 673f 7374 796c 6565  00000.svg?stylee
-000007e0: 266c 6f67 6f3d 4d61 726b 646f 776e 266c  &logo=Markdown&l
-000007f0: 6f67 6f43 6f6c 6f72 3d77 6869 7465 2220  ogoColor=white" 
-00000800: 616c 743d 224d 6172 6b64 6f77 6e22 202f  alt="Markdown" /
-00000810: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
-00000820: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000830: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000840: 2f4f 7065 6e41 492d 3431 3239 3931 2e73  /OpenAI-412991.s
-00000850: 7667 3f73 7479 6c65 6526 6c6f 676f 3d4f  vg?stylee&logo=O
-00000860: 7065 6e41 4926 6c6f 676f 436f 6c6f 723d  penAI&logoColor=
-00000870: 7768 6974 6522 2061 6c74 3d22 4f70 656e  white" alt="Open
-00000880: 4149 2220 2f3e 0a20 2020 2020 2020 203c  AI" />.        <
-00000890: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000008a0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000008b0: 6261 6467 652f 5079 7468 6f6e 2d33 3737  badge/Python-377
-000008c0: 3641 422e 7376 673f 7374 796c 6565 266c  6AB.svg?stylee&l
-000008d0: 6f67 6f3d 5079 7468 6f6e 266c 6f67 6f43  ogo=Python&logoC
-000008e0: 6f6c 6f72 3d77 6869 7465 2220 616c 743d  olor=white" alt=
-000008f0: 2250 7974 686f 6e22 202f 3e0a 2020 2020  "Python" />.    
-00000900: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-00000910: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000920: 732e 696f 2f62 6164 6765 2f50 7974 6573  s.io/badge/Pytes
-00000930: 742d 3041 3945 4443 2e73 7667 3f73 7479  t-0A9EDC.svg?sty
-00000940: 6c65 6526 6c6f 676f 3d50 7974 6573 7426  lee&logo=Pytest&
-00000950: 6c6f 676f 436f 6c6f 723d 7768 6974 6522  logoColor=white"
-00000960: 2061 6c74 3d22 7079 7465 7374 2220 2f3e   alt="pytest" />
-00000970: 0a20 2020 2020 2020 203c 696d 6720 7372  .        <img sr
-00000980: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000990: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-000009a0: 474e 5525 3230 4261 7368 2d34 4541 4132  GNU%20Bash-4EAA2
-000009b0: 352e 7376 673f 7374 796c 6565 266c 6f67  5.svg?stylee&log
-000009c0: 6f3d 474e 552d 4261 7368 266c 6f67 6f43  o=GNU-Bash&logoC
-000009d0: 6f6c 6f72 3d77 6869 7465 2220 616c 743d  olor=white" alt=
-000009e0: 2242 6173 6822 202f 3e0a 2020 2020 2020  "Bash" />.      
-000009f0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000a00: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000a10: 696f 2f62 6164 6765 2f41 6e61 636f 6e64  io/badge/Anacond
-00000a20: 612d 3434 4138 3333 2e73 7667 3f26 6c6f  a-44A833.svg?&lo
-00000a30: 676f 3d41 6e61 636f 6e64 6126 6c6f 676f  go=Anaconda&logo
-00000a40: 436f 6c6f 723d 7768 6974 6522 2061 6c74  Color=white" alt
-00000a50: 3d22 416e 6163 6f6e 6461 2220 2f3e 0a20  ="Anaconda" />. 
-00000a60: 2020 203c 2f70 3e0a 2020 2020 3c69 6d67     </p>.    <img
-00000a70: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000a80: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000a90: 692f 762f 7265 6164 6d65 6169 3f63 6f6c  i/v/readmeai?col
-00000aa0: 6f72 3d35 4436 4437 4526 6c6f 676f 3d70  or=5D6D7E&logo=p
-00000ab0: 7974 686f 6e22 2061 6c74 3d22 5079 5049  ython" alt="PyPI
-00000ac0: 202d 204c 6963 656e 7365 2220 2f3e 0a20   - License" />. 
-00000ad0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00000ae0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000af0: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
-00000b00: 6f6e 732f 7265 6164 6d65 6169 3f63 6f6c  ons/readmeai?col
-00000b10: 6f72 3d35 4436 4437 4526 6c6f 676f 3d70  or=5D6D7E&logo=p
-00000b20: 7974 686f 6e22 2061 6c74 3d22 5079 5049  ython" alt="PyPI
-00000b30: 202d 2050 7974 686f 6e20 5665 7273 696f   - Python Versio
-00000b40: 6e22 202f 3e0a 2020 2020 3c69 6d67 2073  n" />.    <img s
-00000b50: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000b60: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00000b70: 622f 6c69 6365 6e73 652f 656c 6936 3473  b/license/eli64s
-00000b80: 2f52 4541 444d 452d 4149 3f63 6f6c 6f72  /README-AI?color
-00000b90: 3d35 4436 4437 4522 2061 6c74 3d22 4769  =5D6D7E" alt="Gi
-00000ba0: 7448 7562 206c 6963 656e 7365 2220 2f3e  tHub license" />
-00000bb0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-00000bc0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000bd0: 6473 2e69 6f2f 6769 7468 7562 2f6c 6173  ds.io/github/las
-00000be0: 742d 636f 6d6d 6974 2f65 6c69 3634 732f  t-commit/eli64s/
-00000bf0: 7265 6164 6d65 2d61 693f 636f 6c6f 723d  readme-ai?color=
-00000c00: 3544 3644 3745 2220 616c 743d 2247 6974  5D6D7E" alt="Git
-00000c10: 4875 6220 6c61 7374 2063 6f6d 6d69 7422  Hub last commit"
-00000c20: 202f 3e0a 3c2f 6469 763e 0a0a 0a2d 2d2d   />.</div>...---
-00000c30: 0a0a 2323 20f0 9f93 9620 5461 626c 6520  ..## .... Table 
-00000c40: 6f66 2043 6f6e 7465 6e74 730a 0a2d 205b  of Contents..- [
-00000c50: f09f 9396 2054 6162 6c65 206f 6620 436f  .... Table of Co
-00000c60: 6e74 656e 7473 5d28 232d 7461 626c 652d  ntents](#-table-
-00000c70: 6f66 2d63 6f6e 7465 6e74 7329 0a2d 205b  of-contents).- [
-00000c80: f09f 938d 204f 7665 7276 6965 775d 2823  .... Overview](#
-00000c90: 2d6f 7665 7276 6965 7729 0a20 2020 202d  -overview).    -
-00000ca0: 205b f09f 8eaf 202a 4d6f 7469 7661 7469   [.... *Motivati
-00000cb0: 6f6e 2a5d 2823 2d6d 6f74 6976 6174 696f  on*](#-motivatio
-00000cc0: 6e29 0a20 2020 202d 205b e29a a0ef b88f  n).    - [......
-00000cd0: 202a 4469 7363 6c61 696d 6572 2a5d 2823   *Disclaimer*](#
-00000ce0: efb8 8f2d 6469 7363 6c61 696d 6572 290a  ...-disclaimer).
-00000cf0: 2d20 5bf0 9f91 be20 4465 6d6f 5d28 232d  - [.... Demo](#-
-00000d00: 6465 6d6f 290a 2d20 5be2 9a99 efb8 8f20  demo).- [...... 
-00000d10: 4665 6174 7572 6573 5d28 23ef b88f 2d66  Features](#...-f
-00000d20: 6561 7475 7265 7329 0a2d 205b f09f 9a80  eatures).- [....
-00000d30: 2047 6574 7469 6e67 2053 7461 7274 6564   Getting Started
-00000d40: 5d28 232d 6765 7474 696e 672d 7374 6172  ](#-getting-star
-00000d50: 7465 6429 0a20 202d 205b e29c 94ef b88f  ted).  - [......
-00000d60: 2044 6570 656e 6465 6e63 6965 735d 2823   Dependencies](#
-00000d70: efb8 8f2d 6465 7065 6e64 656e 6369 6573  ...-dependencies
-00000d80: 290a 2020 2020 2d20 5bf0 9f93 8220 5265  ).    - [.... Re
-00000d90: 706f 7369 746f 7279 5d28 232d 7265 706f  pository](#-repo
-00000da0: 7369 746f 7279 290a 2020 2020 2d20 5bf0  sitory).    - [.
-00000db0: 9f94 9020 4f70 656e 4149 2041 5049 5d28  ... OpenAI API](
-00000dc0: 232d 6f70 656e 6169 2d61 7069 290a 2020  #-openai-api).  
-00000dd0: 2d20 5bf0 9f93 a620 496e 7374 616c 6c61  - [.... Installa
-00000de0: 7469 6f6e 5d28 232d 696e 7374 616c 6c61  tion](#-installa
-00000df0: 7469 6f6e 290a 2020 2d20 5bf0 9f8e ae20  tion).  - [.... 
-00000e00: 5573 696e 6720 2a52 4541 444d 452d 4149  Using *README-AI
-00000e10: 2a5d 2823 2d75 7369 6e67 2d72 6561 646d  *](#-using-readm
-00000e20: 652d 6169 290a 2020 2d20 5bf0 9fa7 aa20  e-ai).  - [.... 
-00000e30: 5275 6e6e 696e 6720 5465 7374 735d 2823  Running Tests](#
-00000e40: 2d72 756e 6e69 6e67 2d74 6573 7473 290a  -running-tests).
-00000e50: 2d20 5bf0 9f9b a020 4675 7475 7265 2044  - [.... Future D
-00000e60: 6576 656c 6f70 6d65 6e74 5d28 232d 6675  evelopment](#-fu
-00000e70: 7475 7265 2d64 6576 656c 6f70 6d65 6e74  ture-development
-00000e80: 290a 2d20 5bf0 9f93 9220 4368 616e 6765  ).- [.... Change
-00000e90: 6c6f 675d 2823 2d63 6861 6e67 656c 6f67  log](#-changelog
-00000ea0: 290a 2d20 5bf0 9fa4 9d20 436f 6e74 7269  ).- [.... Contri
-00000eb0: 6275 7469 6e67 5d28 232d 636f 6e74 7269  buting](#-contri
-00000ec0: 6275 7469 6e67 290a 2d20 5bf0 9f93 8420  buting).- [.... 
-00000ed0: 4c69 6365 6e73 655d 2823 2d6c 6963 656e  License](#-licen
-00000ee0: 7365 290a 2d20 5bf0 9f91 8f20 4163 6b6e  se).- [.... Ackn
-00000ef0: 6f77 6c65 6467 6d65 6e74 735d 2823 2d61  owledgments](#-a
-00000f00: 636b 6e6f 776c 6564 676d 656e 7473 290a  cknowledgments).
-00000f10: 0a2d 2d2d 0a0a 2323 20f0 9f93 8d20 4f76  .---..## .... Ov
-00000f20: 6572 7669 6577 0a0a 2a52 4541 444d 452d  erview..*README-
-00000f30: 4149 2a20 6973 2061 2070 6f77 6572 6675  AI* is a powerfu
-00000f40: 6c2c 2075 7365 722d 6672 6965 6e64 6c79  l, user-friendly
-00000f50: 2063 6f6d 6d61 6e64 2d6c 696e 6520 746f   command-line to
-00000f60: 6f6c 2074 6861 7420 6765 6e65 7261 7465  ol that generate
-00000f70: 7320 6578 7465 6e73 6976 6520 5245 4144  s extensive READ
-00000f80: 4d45 206d 6172 6b64 6f77 6e20 646f 6375  ME markdown docu
-00000f90: 6d65 6e74 7320 666f 7220 796f 7572 2073  ments for your s
-00000fa0: 6f66 7477 6172 6520 616e 6420 6461 7461  oftware and data
-00000fb0: 2070 726f 6a65 6374 732e 2042 7920 7072   projects. By pr
-00000fc0: 6f76 6964 696e 6720 6120 7265 6d6f 7465  oviding a remote
-00000fd0: 2072 6570 6f73 6974 6f72 7920 5552 4c20   repository URL 
-00000fe0: 6f72 2064 6972 6563 746f 7279 2070 6174  or directory pat
-00000ff0: 6820 746f 2079 6f75 7220 636f 6465 6261  h to your codeba
-00001000: 7365 2c20 7468 6973 2074 6f6f 6c20 7769  se, this tool wi
-00001010: 6c6c 2064 6f63 756d 656e 7420 796f 7572  ll document your
-00001020: 2065 6e74 6972 6520 7072 6f6a 6563 742c   entire project,
-00001030: 206c 6576 6572 6167 696e 6720 7468 6520   leveraging the 
-00001040: 6361 7061 6269 6c69 7469 6573 206f 6620  capabilities of 
-00001050: 6c61 7267 6520 6c61 6e67 7561 6765 206d  large language m
-00001060: 6f64 656c 7320 616e 6420 4f70 656e 4149  odels and OpenAI
-00001070: 2773 2047 5054 2041 5049 732e 0a0a 2323  's GPT APIs...##
-00001080: 2323 20f0 9f8e af20 2a4d 6f74 6976 6174  ## .... *Motivat
-00001090: 696f 6e2a 0a0a 5369 6d70 6c69 6669 6573  ion*..Simplifies
-000010a0: 2074 6865 2070 726f 6365 7373 206f 6620   the process of 
-000010b0: 7772 6974 696e 6720 616e 6420 6d61 696e  writing and main
-000010c0: 7461 696e 696e 6720 6869 6768 2d71 7561  taining high-qua
-000010d0: 6c69 7479 2070 726f 6a65 6374 2064 6f63  lity project doc
-000010e0: 756d 656e 7461 7469 6f6e 2e20 4d79 2061  umentation. My a
-000010f0: 696d 2066 6f72 2074 6869 7320 7072 6f6a  im for this proj
-00001100: 6563 7420 6973 2074 6f20 7072 6f76 6964  ect is to provid
-00001110: 6520 616c 6c20 736b 696c 6c20 6c65 7665  e all skill leve
-00001120: 6c73 2061 2074 6f6f 6c20 7468 6174 2069  ls a tool that i
-00001130: 6d70 726f 7665 7320 7468 6569 7220 7465  mproves their te
-00001140: 6368 6e69 6361 6c20 776f 726b 666c 6f77  chnical workflow
-00001150: 2c20 696e 2061 6e20 6566 6669 6369 656e  , in an efficien
-00001160: 7420 616e 6420 7573 6572 2d66 7269 656e  t and user-frien
-00001170: 646c 7920 6d61 6e6e 6572 2e20 556c 7469  dly manner. Ulti
-00001180: 6d61 7465 6c79 2c20 7468 6520 676f 616c  mately, the goal
-00001190: 206f 6620 2a52 4541 444d 452d 4149 2a20   of *README-AI* 
-000011a0: 6973 2074 6f20 696d 7072 6f76 6520 7468  is to improve th
-000011b0: 6520 6164 6f70 7469 6f6e 2061 6e64 2075  e adoption and u
-000011c0: 7361 6269 6c69 7479 206f 6620 6f70 656e  sability of open
-000011d0: 2d73 6f75 7263 6520 7072 6f6a 6563 7473  -source projects
-000011e0: 2c20 656e 6162 6c69 6e67 2065 7665 7279  , enabling every
-000011f0: 6f6e 6520 746f 2062 6574 7465 7220 756e  one to better un
-00001200: 6465 7273 7461 6e64 2061 6e64 2075 7365  derstand and use
-00001210: 206f 7065 6e2d 736f 7572 6365 2074 6f6f   open-source too
-00001220: 6c73 2e0a 2323 2323 20e2 9aa0 efb8 8f20  ls..#### ...... 
-00001230: 2a44 6973 636c 6169 6d65 722a 0a0a 2a52  *Disclaimer*..*R
-00001240: 4541 444d 452d 4149 2a20 6973 2063 7572  EADME-AI* is cur
-00001250: 7265 6e74 6c79 2075 6e64 6572 2064 6576  rently under dev
-00001260: 656c 6f70 6d65 6e74 2061 6e64 2068 6173  elopment and has
-00001270: 2061 6e20 6f70 696e 696f 6e61 7465 6420   an opinionated 
-00001280: 636f 6e66 6967 7572 6174 696f 6e20 616e  configuration an
-00001290: 6420 7365 7475 702e 2057 6869 6c65 2074  d setup. While t
-000012a0: 6869 7320 746f 6f6c 2070 726f 7669 6465  his tool provide
-000012b0: 7320 616e 2065 7863 656c 6c65 6e74 2073  s an excellent s
-000012c0: 7461 7274 696e 6720 706f 696e 7420 666f  tarting point fo
-000012d0: 7220 646f 6375 6d65 6e74 6174 696f 6e2c  r documentation,
-000012e0: 2069 7473 2069 6d70 6f72 7461 6e74 2074   its important t
-000012f0: 6f20 7265 7669 6577 2061 6c6c 2074 6578  o review all tex
-00001300: 7420 6765 6e65 7261 7465 6420 6279 2074  t generated by t
-00001310: 6865 204f 7065 6e41 4920 4150 4920 746f  he OpenAI API to
-00001320: 2065 6e73 7572 6520 6974 2061 6363 7572   ensure it accur
-00001330: 6174 656c 7920 7265 7072 6573 656e 7473  ately represents
-00001340: 2079 6f75 7220 636f 6465 6261 7365 2e20   your codebase. 
-00001350: 456e 7375 7265 2061 6c6c 2063 6f6e 7465  Ensure all conte
-00001360: 6e74 2069 6e20 796f 7572 2072 6570 6f73  nt in your repos
-00001370: 6974 6f72 7920 6973 2066 7265 6520 6f66  itory is free of
-00001380: 2073 656e 7369 7469 7665 2069 6e66 6f72   sensitive infor
-00001390: 6d61 7469 6f6e 2062 6566 6f72 6520 6578  mation before ex
-000013a0: 6563 7574 696e 672e 0a0a 4164 6469 7469  ecuting...Additi
-000013b0: 6f6e 616c 6c79 2c20 6672 6571 7565 6e74  onally, frequent
-000013c0: 6c79 206d 6f6e 6974 6f72 2079 6f75 7220  ly monitor your 
-000013d0: 4150 4920 7573 6167 6520 616e 6420 636f  API usage and co
-000013e0: 7374 7320 6279 2076 6973 6974 696e 6720  sts by visiting 
-000013f0: 7468 6520 5b4f 7065 6e41 4920 4150 4920  the [OpenAI API 
-00001400: 5573 6167 6520 4461 7368 626f 6172 645d  Usage Dashboard]
-00001410: 2868 7474 7073 3a2f 2f70 6c61 7466 6f72  (https://platfor
-00001420: 6d2e 6f70 656e 6169 2e63 6f6d 2f61 6363  m.openai.com/acc
-00001430: 6f75 6e74 2f75 7361 6765 292e 0a0a 2d2d  ount/usage)...--
-00001440: 2d0a 0a23 2320 f09f 91be 2044 656d 6f0a  -..## .... Demo.
-00001450: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00001460: 2f2f 796f 7574 752e 6265 2f70 6c2d 5663  //youtu.be/pl-Vc
-00001470: 5666 4762 626b 223e 0a20 2020 203c 696d  VfGbbk">.    <im
-00001480: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00001490: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-000014a0: 7465 6e74 2e63 6f6d 2f65 6c69 3634 732f  tent.com/eli64s/
-000014b0: 7265 6164 6d65 2d61 692f 6630 6335 6130  readme-ai/f0c5a0
-000014c0: 3338 6636 3361 6530 3462 3264 3434 3532  38f63ae04b2d4452
-000014d0: 3937 3436 3736 6139 3264 6234 3262 6538  974676a92db42be8
-000014e0: 6365 2f65 7861 6d70 6c65 732f 696d 6773  ce/examples/imgs
-000014f0: 2f64 656d 6f2e 706e 6722 2061 6c74 3d22  /demo.png" alt="
-00001500: 6465 6d6f 2076 6964 656f 223e 0a3c 2f61  demo video">.</a
-00001510: 3e0a 0a2d 2d2d 0a0a 2323 20e2 9a99 efb8  >..---..## .....
-00001520: 8f20 4665 6174 7572 6573 0a0a 3c68 3120  . Features..<h1 
-00001530: 616c 6967 6e3d 2263 656e 7465 7222 3e31  align="center">1
-00001540: 2e3c 6272 3ef0 9f91 873c 6272 3e3c 6272  .<br>....<br><br
-00001550: 3ef0 9f93 9120 436f 6465 6261 7365 2044  >.... Codebase D
-00001560: 6f63 756d 656e 7461 7469 6f6e 3c2f 6831  ocumentation</h1
-00001570: 3e0a 3c74 6162 6c65 3e0a 2020 2020 3c74  >.<table>.    <t
-00001580: 723e 0a20 2020 2020 2020 203c 7464 3e0a  r>.        <td>.
-00001590: 2020 2020 2020 2020 2020 2020 3c68 333e              <h3>
-000015a0: e297 a620 5265 706f 7369 746f 7279 2046  ... Repository F
-000015b0: 696c 6520 5375 6d6d 6172 6965 733c 2f68  ile Summaries</h
-000015c0: 333e 0a20 2020 2020 2020 2020 2020 203c  3>.            <
-000015d0: 756c 3e0a 2020 2020 2020 2020 2020 2020  ul>.            
-000015e0: 2020 2020 3c6c 693e 436f 6465 2073 756d      <li>Code sum
-000015f0: 6d61 7269 6573 2061 7265 2067 656e 6572  maries are gener
-00001600: 6174 6564 2066 6f72 2065 6163 6820 6669  ated for each fi
-00001610: 6c65 2076 6961 204f 7065 6e41 4927 7320  le via OpenAI's 
-00001620: 3c69 3e67 7074 2d33 2e35 2d74 7572 626f  <i>gpt-3.5-turbo
-00001630: 3c2f 693e 2065 6e67 696e 652e 3c2f 6c69  </i> engine.</li
-00001640: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001650: 2020 3c6c 693e 5468 6520 4669 6c65 2063    <li>The File c
-00001660: 6f6c 756d 6e20 696e 2074 6865 206d 6172  olumn in the mar
-00001670: 6b64 6f77 6e20 7461 626c 6520 636f 6e74  kdown table cont
-00001680: 6169 6e73 2061 206c 696e 6b20 746f 2074  ains a link to t
-00001690: 6865 2066 696c 6520 6f6e 2047 6974 4875  he file on GitHu
-000016a0: 622e 3c2f 6c69 3e0a 2020 2020 2020 2020  b.</li>.        
-000016b0: 2020 2020 3c2f 756c 3e0a 2020 2020 2020      </ul>.      
-000016c0: 2020 3c2f 7464 3e0a 2020 2020 3c2f 7472    </td>.    </tr
-000016d0: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-000016e0: 2020 203c 7464 3e0a 2020 2020 2020 2020     <td>.        
-000016f0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-00001700: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00001710: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00001720: 656c 6936 3473 2f72 6561 646d 652d 6169  eli64s/readme-ai
-00001730: 2f6d 6169 6e2f 6578 616d 706c 6573 2f69  /main/examples/i
-00001740: 6d67 732f 6d6f 6475 6c65 732e 706e 6722  mgs/modules.png"
-00001750: 2061 6c74 3d22 646f 6373 223e 0a20 2020   alt="docs">.   
-00001760: 2020 2020 203c 2f74 643e 0a20 2020 203c       </td>.    <
-00001770: 2f74 723e 0a3c 2f74 6162 6c65 3e0a 0a3c  /tr>.</table>..<
-00001780: 6831 2061 6c69 676e 3d22 6365 6e74 6572  h1 align="center
-00001790: 223e e292 893c 6272 3ef0 9f91 873c 6272  ">...<br>....<br
-000017a0: 3e3c 6272 3ef0 9f8e 9620 4261 6467 6573  ><br>.... Badges
-000017b0: 3c2f 6831 3e0a 3c74 6162 6c65 3e0a 2020  </h1>.<table>.  
-000017c0: 2020 3c74 723e 0a20 2020 2020 2020 203c    <tr>.        <
-000017d0: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
-000017e0: 3c68 333e e297 a620 496e 7472 6f64 7563  <h3>... Introduc
-000017f0: 7469 6f6e 2c20 4261 6467 6573 2c20 2620  tion, Badges, & 
-00001800: 5461 626c 6520 6f66 2043 6f6e 7465 6e74  Table of Content
-00001810: 733c 2f68 333e 0a20 2020 2020 2020 2020  s</h3>.         
-00001820: 2020 203c 756c 3e0a 2020 2020 2020 2020     <ul>.        
-00001830: 2020 2020 2020 2020 3c6c 693e 5468 6520          <li>The 
-00001840: 4f70 656e 4149 2041 5049 2069 7320 7072  OpenAI API is pr
-00001850: 6f6d 7074 6564 2074 6f20 6372 6561 7465  ompted to create
-00001860: 2061 2031 2d73 656e 7465 6e63 6520 7068   a 1-sentence ph
-00001870: 7261 7365 2064 6573 6372 6962 696e 6720  rase describing 
-00001880: 796f 7572 2070 726f 6a65 6374 2e3c 2f6c  your project.</l
-00001890: 693e 0a20 2020 2020 2020 2020 2020 2020  i>.             
-000018a0: 2020 203c 6c69 3e50 726f 6a65 6374 2064     <li>Project d
-000018b0: 6570 656e 6465 6e63 6965 7320 616e 6420  ependencies and 
-000018c0: 6d65 7461 6461 7461 2061 7265 2076 6973  metadata are vis
-000018d0: 7561 6c69 7a65 6420 7573 696e 6720 3c61  ualized using <a
-000018e0: 2068 7265 663d 2268 7474 7073 3a2f 2f73   href="https://s
-000018f0: 6869 656c 6473 2e69 6f2f 223e 5368 6965  hields.io/">Shie
-00001900: 6c64 732e 696f 3c2f 613e 2062 6164 6765  lds.io</a> badge
-00001910: 732e 3c2f 6c69 3e0a 2020 2020 2020 2020  s.</li>.        
-00001920: 2020 2020 2020 2020 3c6c 693e 4261 6467          <li>Badg
-00001930: 6573 2061 7265 2073 6f72 7465 6420 6279  es are sorted by
-00001940: 2068 6578 2063 6f64 652c 2064 6973 706c   hex code, displ
-00001950: 6179 6564 2066 726f 6d20 6c69 6768 7420  ayed from light 
-00001960: 746f 2064 6172 6b20 6875 6573 2e3c 2f6c  to dark hues.</l
-00001970: 693e 0a20 2020 2020 2020 2020 2020 203c  i>.            <
-00001980: 2f75 6c3e 0a20 2020 2020 2020 203c 2f74  /ul>.        </t
-00001990: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
-000019a0: 203c 7472 3e0a 2020 2020 2020 2020 3c74   <tr>.        <t
-000019b0: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
-000019c0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000019d0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-000019e0: 6f6e 7465 6e74 2e63 6f6d 2f65 6c69 3634  ontent.com/eli64
-000019f0: 732f 7265 6164 6d65 2d61 692f 6d61 696e  s/readme-ai/main
-00001a00: 2f65 7861 6d70 6c65 732f 696d 6773 2f68  /examples/imgs/h
-00001a10: 6561 6465 722e 706e 6722 2061 6c74 3d22  eader.png" alt="
-00001a20: 646f 6373 223e 0a20 2020 2020 2020 203c  docs">.        <
-00001a30: 2f74 643e 0a20 2020 203c 2f74 723e 0a3c  /td>.    </tr>.<
-00001a40: 2f74 6162 6c65 3e0a 0a3c 6831 2061 6c69  /table>..<h1 ali
-00001a50: 676e 3d22 6365 6e74 6572 223e e292 8a3c  gn="center">...<
-00001a60: 6272 3ef0 9f91 873c 6272 3e3c 6272 3ef0  br>....<br><br>.
-00001a70: 9fa7 9a20 5072 6f6d 7074 6564 2054 6578  ... Prompted Tex
-00001a80: 7420 4765 6e65 7261 7469 6f6e 3c2f 6831  t Generation</h1
-00001a90: 3e0a 3c74 6162 6c65 3e0a 2020 2020 3c74  >.<table>.    <t
-00001aa0: 723e 0a20 2020 2020 2020 203c 7464 3e0a  r>.        <td>.
-00001ab0: 2020 2020 2020 2020 2020 2020 3c68 333e              <h3>
-00001ac0: e297 a620 4665 6174 7572 6573 2054 6162  ... Features Tab
-00001ad0: 6c65 2026 204f 7665 7276 6965 773c 2f68  le & Overview</h
-00001ae0: 333e 0a20 2020 2020 2020 2020 2020 203c  3>.            <
-00001af0: 756c 3e0a 2020 2020 2020 2020 2020 2020  ul>.            
-00001b00: 2020 2020 3c6c 693e 4465 7461 696c 6564      <li>Detailed
-00001b10: 2070 726f 6d70 7473 2061 7265 2065 6d62   prompts are emb
-00001b20: 6564 6465 6420 7769 7468 2072 6570 6f73  edded with repos
-00001b30: 6974 6f72 7920 6d65 7461 6461 7461 2061  itory metadata a
-00001b40: 6e64 2070 6173 7365 6420 746f 2074 6865  nd passed to the
-00001b50: 204f 7065 6e41 4920 4150 492e 3c2f 6c69   OpenAI API.</li
-00001b60: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001b70: 2020 3c75 6c3e 0a20 2020 2020 2020 2020    <ul>.         
-00001b80: 2020 2020 2020 2020 2020 203c 6c69 3e3c             <li><
-00001b90: 656d 3e46 6561 7475 7265 733c 2f65 6d3e  em>Features</em>
-00001ba0: 2074 6162 6c65 2068 6967 686c 6967 6874   table highlight
-00001bb0: 7320 7661 7269 6f75 7320 7465 6368 6e69  s various techni
-00001bc0: 6361 6c20 6174 7472 6962 7574 6573 206f  cal attributes o
-00001bd0: 6620 796f 7572 2063 6f64 6562 6173 652e  f your codebase.
-00001be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001bf0: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
-00001c00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001c10: 6c69 3e3c 656d 3e4f 7665 7276 6965 773c  li><em>Overview<
-00001c20: 2f65 6d3e 2073 6563 7469 6f6e 2064 6573  /em> section des
-00001c30: 6372 6962 6573 2079 6f75 7220 7072 6f6a  cribes your proj
-00001c40: 6563 7427 7320 7573 6520 6361 7365 2061  ect's use case a
-00001c50: 6e64 2061 7070 6c69 6361 7469 6f6e 732e  nd applications.
-00001c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001c70: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
-00001c80: 2020 2020 2020 2020 2020 203c 2f75 6c3e             </ul>
-00001c90: 0a20 2020 2020 2020 2020 2020 203c 2f75  .            </u
-00001ca0: 6c3e 0a20 2020 2020 2020 203c 2f74 643e  l>.        </td>
-00001cb0: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
-00001cc0: 7472 3e0a 2020 2020 2020 2020 3c74 643e  tr>.        <td>
-00001cd0: 0a20 2020 2020 2020 2020 2020 203c 696d  .            <im
-00001ce0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00001cf0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00001d00: 7465 6e74 2e63 6f6d 2f65 6c69 3634 732f  tent.com/eli64s/
-00001d10: 7265 6164 6d65 2d61 692f 6d61 696e 2f65  readme-ai/main/e
-00001d20: 7861 6d70 6c65 732f 696d 6773 2f66 6561  xamples/imgs/fea
-00001d30: 7475 7265 732e 706e 6722 2061 6c74 3d22  tures.png" alt="
-00001d40: 6665 6174 7572 6573 223e 0a20 2020 2020  features">.     
-00001d50: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
-00001d60: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00001d70: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00001d80: 6f6d 2f65 6c69 3634 732f 7265 6164 6d65  om/eli64s/readme
-00001d90: 2d61 692f 6d61 696e 2f65 7861 6d70 6c65  -ai/main/example
-00001da0: 732f 696d 6773 2f6f 7665 7276 6965 772e  s/imgs/overview.
-00001db0: 706e 6722 2061 6c74 3d22 6f76 6572 7669  png" alt="overvi
-00001dc0: 6577 223e 0a20 2020 2020 2020 203c 2f74  ew">.        </t
-00001dd0: 643e 0a20 2020 203c 2f74 723e 0a3c 2f74  d>.    </tr>.</t
-00001de0: 6162 6c65 3e0a 0a3c 6831 2061 6c69 676e  able>..<h1 align
-00001df0: 3d22 6365 6e74 6572 223e e292 8b3c 6272  ="center">...<br
-00001e00: 3ef0 9f91 873c 6272 3e3c 6272 3ef0 9f8c  >....<br><br>...
-00001e10: b220 5265 706f 7369 746f 7279 2054 7265  . Repository Tre
-00001e20: 653c 2f68 313e 0a3c 7461 626c 653e 0a20  e</h1>.<table>. 
-00001e30: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
-00001e40: 3c74 643e 0a20 2020 2020 2020 2020 2020  <td>.           
-00001e50: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00001e60: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00001e70: 7263 6f6e 7465 6e74 2e63 6f6d 2f65 6c69  rcontent.com/eli
-00001e80: 3634 732f 7265 6164 6d65 2d61 692f 6d61  64s/readme-ai/ma
-00001e90: 696e 2f65 7861 6d70 6c65 732f 696d 6773  in/examples/imgs
-00001ea0: 2f74 7265 652e 706e 6722 2061 6c74 3d22  /tree.png" alt="
-00001eb0: 7472 6565 223e 0a20 2020 2020 2020 203c  tree">.        <
-00001ec0: 2f74 643e 0a20 2020 203c 2f74 723e 0a3c  /td>.    </tr>.<
-00001ed0: 2f74 6162 6c65 3e0a 0a3c 6831 2061 6c69  /table>..<h1 ali
-00001ee0: 676e 3d22 6365 6e74 6572 223e e292 8c3c  gn="center">...<
-00001ef0: 6272 3ef0 9f91 873c 6272 3e3c 6272 3ef0  br>....<br><br>.
-00001f00: 9f93 a620 4479 6e61 6d69 6320 5573 6572  ... Dynamic User
-00001f10: 2053 6574 7570 2047 7569 6465 733c 2f68   Setup Guides</h
-00001f20: 313e 0a3c 7461 626c 653e 0a20 2020 203c  1>.<table>.    <
-00001f30: 7472 3e0a 2020 2020 2020 2020 3c74 643e  tr>.        <td>
-00001f40: 0a20 2020 2020 2020 2020 2020 203c 6833  .            <h3
-00001f50: 3e3c 623e e297 a620 496e 7374 616c 6c61  ><b>... Installa
-00001f60: 7469 6f6e 2c20 5573 6167 652c 2026 2054  tion, Usage, & T
-00001f70: 6573 7469 6e67 3c2f 623e 3c2f 6833 3e0a  esting</b></h3>.
-00001f80: 2020 2020 2020 2020 2020 2020 3c75 6c3e              <ul>
-00001f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001fa0: 203c 6c69 3e47 656e 6572 6174 6573 2069   <li>Generates i
-00001fb0: 6e73 7472 7563 7469 6f6e 7320 666f 7220  nstructions for 
-00001fc0: 696e 7374 616c 6c69 6e67 2c20 7573 696e  installing, usin
-00001fd0: 672c 2061 6e64 2074 6573 7469 6e67 2079  g, and testing y
-00001fe0: 6f75 7220 636f 6465 6261 7365 2e3c 2f6c  our codebase.</l
-00001ff0: 693e 0a20 2020 2020 2020 2020 2020 2020  i>.             
-00002000: 2020 203c 6c69 3e52 4541 444d 452d 4149     <li>README-AI
-00002010: 2063 7572 7265 6e74 6c79 2073 7570 706f   currently suppo
-00002020: 7274 7320 7468 6973 2066 6561 7475 7265  rts this feature
-00002030: 2066 6f72 2063 6f64 6520 7772 6974 7465   for code writte
-00002040: 6e20 7769 7468 3a3c 2f6c 693e 0a20 2020  n with:</li>.   
-00002050: 2020 2020 2020 2020 2020 2020 203c 756c               <ul
-00002060: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002070: 2020 2020 2020 3c6c 693e 0a20 2020 2020        <li>.     
-00002080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002090: 2020 203c 693e 5079 7468 6f6e 2c20 5275     <i>Python, Ru
-000020a0: 7374 2c20 476f 2c20 432c 204b 6f74 6c69  st, Go, C, Kotli
-000020b0: 6e2c 204a 6176 612c 204a 6176 6153 6372  n, Java, JavaScr
-000020c0: 6970 742c 2054 7970 6553 6372 6970 742e  ipt, TypeScript.
-000020d0: 3c2f 693e 0a20 2020 2020 2020 2020 2020  </i>.           
-000020e0: 2020 2020 2020 2020 203c 2f6c 693e 0a20           </li>. 
-000020f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002100: 2f75 6c3e 0a20 2020 2020 2020 2020 2020  /ul>.           
-00002110: 203c 2f75 6c3e 0a20 2020 2020 2020 203c   </ul>.        <
-00002120: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
-00002130: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
-00002140: 3c74 643e 0a20 2020 2020 2020 2020 2020  <td>.           
-00002150: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00002160: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00002170: 7263 6f6e 7465 6e74 2e63 6f6d 2f65 6c69  rcontent.com/eli
-00002180: 3634 732f 7265 6164 6d65 2d61 692f 6d61  64s/readme-ai/ma
-00002190: 696e 2f65 7861 6d70 6c65 732f 696d 6773  in/examples/imgs
-000021a0: 2f67 6574 7469 6e67 5f73 7461 7274 6564  /getting_started
-000021b0: 2e70 6e67 2220 616c 743d 2267 6574 7469  .png" alt="getti
-000021c0: 6e67 5f73 7461 7274 6564 223e 0a20 2020  ng_started">.   
-000021d0: 2020 2020 203c 2f74 643e 0a20 2020 203c       </td>.    <
-000021e0: 2f74 723e 0a3c 2f74 6162 6c65 3e0a 0a3c  /tr>.</table>..<
-000021f0: 6831 2061 6c69 676e 3d22 6365 6e74 6572  h1 align="center
-00002200: 223e e292 8d3c 6272 3ef0 9f91 873c 6272  ">...<br>....<br
-00002210: 3e3c 6272 3ef0 9f91 a9e2 808d f09f 92bb  ><br>...........
-00002220: 436f 6e74 7269 6275 7469 6e67 2047 7569  Contributing Gui
-00002230: 6465 6c69 6e65 7320 2620 6d6f 7265 213c  delines & more!<
-00002240: 2f68 313e 0a0a 7c20 7c0a 7c2d 2d2d 2d2d  /h1>..| |.|-----
-00002250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002270: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 215b  ----------|.| ![
-00002280: 636f 6e74 7269 6275 7465 5d28 6874 7470  contribute](http
-00002290: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-000022a0: 6572 636f 6e74 656e 742e 636f 6d2f 656c  ercontent.com/el
-000022b0: 6936 3473 2f72 6561 646d 652d 6169 2f6d  i64s/readme-ai/m
-000022c0: 6169 6e2f 6578 616d 706c 6573 2f69 6d67  ain/examples/img
-000022d0: 732f 636c 6f73 696e 672e 706e 6729 207c  s/closing.png) |
-000022e0: 0a0a 3c68 3120 616c 6967 6e3d 2263 656e  ..<h1 align="cen
-000022f0: 7465 7222 3ee2 928e 3c62 723e f09f 9187  ter">...<br>....
-00002300: 3c62 723e 3c62 723e f09f 92a5 2045 7861  <br><br>.... Exa
-00002310: 6d70 6c65 2046 696c 6573 3c2f 6831 3e0a  mple Files</h1>.
-00002320: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00002330: 223e 4d61 726b 646f 776e 2065 7861 6d70  ">Markdown examp
-00002340: 6c65 2066 696c 6573 2067 656e 6572 6174  le files generat
-00002350: 6564 2062 7920 7468 6520 5245 4144 4d45  ed by the README
-00002360: 2d41 4920 6170 7021 3c2f 703e 0a3c 6469  -AI app!</p>.<di
-00002370: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
-00002380: 3e0a 2020 2020 3c74 6162 6c65 2061 6c69  >.    <table ali
-00002390: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
-000023a0: 2020 2020 203c 7472 3e0a 2020 2020 2020       <tr>.      
-000023b0: 2020 2020 2020 3c74 683e 3c2f 7468 3e0a        <th></th>.
-000023c0: 2020 2020 2020 2020 2020 2020 3c74 683e              <th>
-000023d0: 4578 616d 706c 6520 4669 6c65 3c2f 7468  Example File</th
-000023e0: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
-000023f0: 683e 5265 706f 7369 746f 7279 3c2f 7468  h>Repository</th
-00002400: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
-00002410: 683e 4c61 6e67 7561 6765 3c2f 7468 3e0a  h>Language</th>.
-00002420: 2020 2020 2020 2020 2020 2020 3c74 683e              <th>
-00002430: 4279 7465 733c 2f74 683e 0a20 2020 2020  Bytes</th>.     
-00002440: 2020 203c 2f74 723e 0a20 2020 2020 2020     </tr>.       
-00002450: 203c 7472 3e0a 2020 2020 2020 2020 2020   <tr>.          
-00002460: 2020 3c74 643e 31ef b88f e283 a33c 2f74    <td>1......</t
-00002470: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
-00002480: 7464 3e3c 6120 6872 6566 3d22 6874 7470  td><a href="http
-00002490: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
-000024a0: 6c69 3634 732f 7265 6164 6d65 2d61 692f  li64s/readme-ai/
-000024b0: 626c 6f62 2f6d 6169 6e2f 6578 616d 706c  blob/main/exampl
-000024c0: 6573 2f72 6561 646d 652d 7079 7468 6f6e  es/readme-python
-000024d0: 2e6d 6422 3e72 6561 646d 652d 7079 7468  .md">readme-pyth
-000024e0: 6f6e 2e6d 643c 2f61 3e3c 2f74 643e 0a20  on.md</a></td>. 
-000024f0: 2020 2020 2020 2020 2020 203c 7464 3e3c             <td><
-00002500: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00002510: 6769 7468 7562 2e63 6f6d 2f65 6c69 3634  github.com/eli64
-00002520: 732f 7265 6164 6d65 2d61 6922 3e72 6561  s/readme-ai">rea
-00002530: 646d 652d 6169 3c2f 613e 3c2f 7464 3e0a  dme-ai</a></td>.
-00002540: 2020 2020 2020 2020 2020 2020 3c74 643e              <td>
-00002550: 5079 7468 6f6e 3c2f 7464 3e0a 2020 2020  Python</td>.    
-00002560: 2020 2020 2020 2020 3c74 643e 0a20 2020          <td>.   
-00002570: 2020 2020 2020 2020 2020 2020 203c 703e               <p>
-00002580: 3139 2c38 3339 3c2f 703e 0a20 2020 2020  19,839</p>.     
-00002590: 2020 203c 2f74 723e 0a20 2020 2020 2020     </tr>.       
-000025a0: 203c 7464 3e32 efb8 8fe2 83a3 3c2f 7464   <td>2......</td
-000025b0: 3e0a 2020 2020 2020 2020 3c74 643e 3c61  >.        <td><a
-000025c0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-000025d0: 6974 6875 622e 636f 6d2f 656c 6936 3473  ithub.com/eli64s
-000025e0: 2f72 6561 646d 652d 6169 2f62 6c6f 622f  /readme-ai/blob/
-000025f0: 6d61 696e 2f65 7861 6d70 6c65 732f 7265  main/examples/re
-00002600: 6164 6d65 2d74 7970 6573 6372 6970 742e  adme-typescript.
-00002610: 6d64 223e 7265 6164 6d65 2d74 7970 6573  md">readme-types
-00002620: 6372 6970 742e 6d64 3c2f 613e 3c2f 7464  cript.md</a></td
-00002630: 3e0a 2020 2020 2020 2020 3c74 643e 3c61  >.        <td><a
-00002640: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00002650: 6974 6875 622e 636f 6d2f 5975 6265 726c  ithub.com/Yuberl
-00002660: 6579 2f43 6861 7447 5054 2d41 7070 2d52  ey/ChatGPT-App-R
-00002670: 6561 6374 2d4e 6174 6976 652d 5479 7065  eact-Native-Type
-00002680: 5363 7269 7074 223e 6368 6174 6770 742d  Script">chatgpt-
-00002690: 6170 702d 7265 6163 742d 7479 7065 7363  app-react-typesc
-000026a0: 7269 7074 3c2f 613e 3c2f 7464 3e0a 2020  ript</a></td>.  
-000026b0: 2020 2020 2020 3c74 643e 5479 7065 5363        <td>TypeSc
-000026c0: 7269 7074 2c20 5265 6163 743c 2f74 643e  ript, React</td>
-000026d0: 0a20 2020 2020 2020 203c 7464 3e0a 2020  .        <td>.  
-000026e0: 2020 2020 2020 2020 2020 3c70 3e39 3838            <p>988
-000026f0: 3c2f 703e 0a20 2020 2020 2020 2020 2020  </p>.           
-00002700: 203c 2f74 723e 0a20 2020 2020 2020 2020   </tr>.         
-00002710: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
-00002720: 2020 2020 2020 2020 3c74 643e 33ef b88f          <td>3...
-00002730: e283 a33c 2f74 643e 0a20 2020 2020 2020  ...</td>.       
-00002740: 2020 2020 2020 2020 203c 7464 3e3c 6120           <td><a 
-00002750: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00002760: 7468 7562 2e63 6f6d 2f65 6c69 3634 732f  thub.com/eli64s/
-00002770: 7265 6164 6d65 2d61 692f 626c 6f62 2f6d  readme-ai/blob/m
-00002780: 6169 6e2f 6578 616d 706c 6573 2f72 6561  ain/examples/rea
-00002790: 646d 652d 6a61 7661 7363 7269 7074 2e6d  dme-javascript.m
-000027a0: 6422 3e72 6561 646d 652d 6a61 7661 7363  d">readme-javasc
-000027b0: 7269 7074 2e6d 643c 2f61 3e3c 2f74 643e  ript.md</a></td>
-000027c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000027d0: 203c 7464 3e3c 6120 6872 6566 3d22 6874   <td><a href="ht
-000027e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000027f0: 2f69 646f 7361 6c2f 6173 7369 7374 616e  /idosal/assistan
-00002800: 742d 6368 6174 2d67 7074 223e 6173 7369  t-chat-gpt">assi
-00002810: 7374 616e 742d 6368 6174 2d67 7074 2d6a  stant-chat-gpt-j
-00002820: 6176 6173 6372 6970 743c 2f61 3e3c 2f74  avascript</a></t
-00002830: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
-00002840: 2020 203c 7464 3e4a 6176 6153 6372 6970     <td>JavaScrip
-00002850: 742c 2052 6561 6374 3c2f 7464 3e0a 2020  t, React</td>.  
-00002860: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
-00002870: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
-00002880: 2020 2020 2020 203c 703e 3231 323c 2f70         <p>212</p
-00002890: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
-000028a0: 7472 3e0a 2020 2020 2020 2020 2020 2020  tr>.            
-000028b0: 3c74 723e 0a20 2020 2020 2020 2020 2020  <tr>.           
-000028c0: 2020 2020 203c 7464 3e34 efb8 8fe2 83a3       <td>4......
-000028d0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
-000028e0: 2020 2020 2020 3c74 643e 3c61 2068 7265        <td><a hre
-000028f0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00002900: 622e 636f 6d2f 656c 6936 3473 2f72 6561  b.com/eli64s/rea
-00002910: 646d 652d 6169 2f62 6c6f 622f 6d61 696e  dme-ai/blob/main
-00002920: 2f65 7861 6d70 6c65 732f 7265 6164 6d65  /examples/readme
-00002930: 2d6b 6f74 6c69 6e2e 6d64 223e 7265 6164  -kotlin.md">read
-00002940: 6d65 2d6b 6f74 6c69 6e2e 6d64 3c2f 613e  me-kotlin.md</a>
-00002950: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
-00002960: 2020 2020 2020 3c74 643e 3c61 2068 7265        <td><a hre
-00002970: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00002980: 622e 636f 6d2f 7275 6d61 616e 2f66 696c  b.com/rumaan/fil
-00002990: 652e 696f 2d41 6e64 726f 6964 2d43 6c69  e.io-Android-Cli
-000029a0: 656e 7422 3e66 696c 652e 696f 2d61 6e64  ent">file.io-and
-000029b0: 726f 6964 2d63 6c69 656e 743c 2f61 3e3c  roid-client</a><
-000029c0: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
-000029d0: 2020 2020 203c 7464 3e4b 6f74 6c69 6e2c       <td>Kotlin,
-000029e0: 204a 6176 612c 2041 6e64 726f 6964 3c2f   Java, Android</
-000029f0: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
-00002a00: 2020 2020 3c74 643e 0a20 2020 2020 2020      <td>.       
-00002a10: 2020 2020 2020 2020 2020 2020 203c 703e               <p>
-00002a20: 3131 332c 3634 393c 2f70 3e0a 2020 2020  113,649</p>.    
-00002a30: 2020 2020 2020 2020 3c2f 7472 3e0a 2020          </tr>.  
-00002a40: 2020 2020 2020 2020 2020 3c74 723e 0a20            <tr>. 
-00002a50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002a60: 7464 3e35 efb8 8fe2 83a3 3c2f 7464 3e0a  td>5......</td>.
-00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a80: 3c74 643e 3c61 2068 7265 663d 2268 7474  <td><a href="htt
-00002a90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002aa0: 656c 6936 3473 2f72 6561 646d 652d 6169  eli64s/readme-ai
-00002ab0: 2f62 6c6f 622f 6d61 696e 2f65 7861 6d70  /blob/main/examp
-00002ac0: 6c65 732f 7265 6164 6d65 2d72 7573 742d  les/readme-rust-
-00002ad0: 632e 6d64 223e 7265 6164 6d65 2d72 7573  c.md">readme-rus
-00002ae0: 742d 632e 6d64 3c2f 613e 3c2f 7464 3e0a  t-c.md</a></td>.
-00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 3c74 643e 3c61 2068 7265 663d 2268 7474  <td><a href="htt
-00002b10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002b20: 446f 776e 5769 7468 5570 2f43 616c 6c4d  DownWithUp/CallM
-00002b30: 6f6e 223e 7275 7374 2d63 2d61 7070 3c2f  on">rust-c-app</
-00002b40: 613e 3c2f 7464 3e0a 2020 2020 2020 2020  a></td>.        
-00002b50: 2020 2020 2020 2020 3c74 643e 432c 2052          <td>C, R
-00002b60: 7573 743c 2f74 643e 0a20 2020 2020 2020  ust</td>.       
-00002b70: 2020 2020 2020 2020 203c 7464 3e0a 2020           <td>.  
-00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b90: 2020 3c70 3e37 323c 2f70 3e0a 2020 2020    <p>72</p>.    
-00002ba0: 2020 2020 2020 2020 3c2f 7472 3e0a 2020          </tr>.  
-00002bb0: 2020 2020 2020 2020 2020 3c74 723e 0a20            <tr>. 
-00002bc0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002bd0: 7464 3e36 efb8 8fe2 83a3 3c2f 7464 3e0a  td>6......</td>.
-00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bf0: 3c74 643e 3c61 2068 7265 663d 2268 7474  <td><a href="htt
-00002c00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002c10: 656c 6936 3473 2f72 6561 646d 652d 6169  eli64s/readme-ai
-00002c20: 2f62 6c6f 622f 6d61 696e 2f65 7861 6d70  /blob/main/examp
-00002c30: 6c65 732f 7265 6164 6d65 2d67 6f2e 6d64  les/readme-go.md
-00002c40: 223e 7265 6164 6d65 2d67 6f2e 6d64 3c2f  ">readme-go.md</
-00002c50: 613e 3c2f 7464 3e0a 2020 2020 2020 2020  a></td>.        
-00002c60: 2020 2020 2020 2020 3c74 643e 3c61 2068          <td><a h
-00002c70: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00002c80: 6875 622e 636f 6d2f 6f6c 6c69 6566 722f  hub.com/olliefr/
-00002c90: 646f 636b 6572 2d67 732d 7069 6e67 223e  docker-gs-ping">
-00002ca0: 676f 2d64 6f63 6b65 722d 6170 703c 2f61  go-docker-app</a
-00002cb0: 3e3c 2f74 643e 0a20 2020 2020 2020 2020  ></td>.         
-00002cc0: 2020 2020 2020 203c 7464 3e47 6f3c 2f74         <td>Go</t
-00002cd0: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
-00002ce0: 2020 203c 7464 3e0a 2020 2020 2020 2020     <td>.        
-00002cf0: 2020 2020 2020 2020 2020 2020 3c70 3e34              <p>4
-00002d00: 313c 2f70 3e0a 2020 2020 2020 2020 2020  1</p>.          
-00002d10: 2020 3c2f 7472 3e0a 2020 2020 2020 2020    </tr>.        
-00002d20: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
-00002d30: 2020 2020 2020 2020 203c 7464 3e37 efb8           <td>7..
-00002d40: 8fe2 83a3 3c2f 7464 3e0a 2020 2020 2020  ....</td>.      
-00002d50: 2020 2020 2020 2020 2020 3c74 643e 3c61            <td><a
-00002d60: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00002d70: 6974 6875 622e 636f 6d2f 656c 6936 3473  ithub.com/eli64s
-00002d80: 2f72 6561 646d 652d 6169 2f62 6c6f 622f  /readme-ai/blob/
-00002d90: 6d61 696e 2f65 7861 6d70 6c65 732f 7265  main/examples/re
-00002da0: 6164 6d65 2d6a 6176 612e 6d64 223e 7265  adme-java.md">re
-00002db0: 6164 6d65 2d6a 6176 612e 6d64 3c2f 613e  adme-java.md</a>
-00002dc0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
-00002dd0: 2020 2020 2020 3c74 643e 3c61 2068 7265        <td><a hre
-00002de0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00002df0: 622e 636f 6d2f 6176 6a69 6e64 6572 2f4d  b.com/avjinder/M
-00002e00: 696e 696d 616c 2d54 6f64 6f22 3e6a 6176  inimal-Todo">jav
-00002e10: 612d 6d69 6e69 6d61 6c2d 746f 646f 3c2f  a-minimal-todo</
-00002e20: 613e 3c2f 7464 3e0a 2020 2020 2020 2020  a></td>.        
-00002e30: 2020 2020 2020 2020 3c74 643e 4a61 7661          <td>Java
-00002e40: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
-00002e50: 2020 2020 2020 3c74 643e 0a20 2020 2020        <td>.     
-00002e60: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002e70: 703e 3137 2c37 3235 3c2f 703e 0a20 2020  p>17,725</p>.   
-00002e80: 2020 2020 2020 2020 203c 2f74 723e 0a20           </tr>. 
-00002e90: 2020 2020 2020 2020 2020 203c 7472 3e0a             <tr>.
-00002ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002eb0: 3c74 643e 38ef b88f e283 a33c 2f74 643e  <td>8......</td>
-00002ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ed0: 203c 7464 3e3c 6120 6872 6566 3d22 6874   <td><a href="ht
-00002ee0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002ef0: 2f65 6c69 3634 732f 7265 6164 6d65 2d61  /eli64s/readme-a
-00002f00: 692f 626c 6f62 2f6d 6169 6e2f 6578 616d  i/blob/main/exam
-00002f10: 706c 6573 2f72 6561 646d 652d 6661 7374  ples/readme-fast
-00002f20: 6170 692d 7265 6469 732e 6d64 223e 7265  api-redis.md">re
-00002f30: 6164 6d65 2d66 6173 7461 7069 2d72 6564  adme-fastapi-red
-00002f40: 6973 2e6d 643c 2f61 3e3c 2f74 643e 0a20  is.md</a></td>. 
-00002f50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002f60: 7464 3e3c 6120 6872 6566 3d22 6874 7470  td><a href="http
-00002f70: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f46  s://github.com/F
-00002f80: 6572 7261 7269 4447 2f61 7379 6e63 2d6d  errariDG/async-m
-00002f90: 6c2d 696e 6665 7265 6e63 6522 3e61 7379  l-inference">asy
-00002fa0: 6e63 2d6d 6c2d 696e 6665 7265 6e63 653c  nc-ml-inference<
-00002fb0: 2f61 3e3c 2f74 643e 0a20 2020 2020 2020  /a></td>.       
-00002fc0: 2020 2020 2020 2020 203c 7464 3e50 7974           <td>Pyt
-00002fd0: 686f 6e2c 2046 6173 7441 5049 2c20 5265  hon, FastAPI, Re
-00002fe0: 6469 733c 2f74 643e 0a20 2020 2020 2020  dis</td>.       
-00002ff0: 2020 2020 2020 2020 203c 7464 3e0a 2020           <td>.  
-00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003010: 2020 3c70 3e33 3535 3c2f 703e 0a20 2020    <p>355</p>.   
-00003020: 2020 2020 2020 2020 203c 2f74 723e 0a20           </tr>. 
-00003030: 2020 2020 2020 2020 2020 203c 7472 3e0a             <tr>.
-00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003050: 3c74 643e 39ef b88f e283 a33c 2f74 643e  <td>9......</td>
-00003060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003070: 203c 7464 3e3c 6120 6872 6566 3d22 6874   <td><a href="ht
-00003080: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003090: 2f65 6c69 3634 732f 7265 6164 6d65 2d61  /eli64s/readme-a
-000030a0: 692f 626c 6f62 2f6d 6169 6e2f 6578 616d  i/blob/main/exam
-000030b0: 706c 6573 2f72 6561 646d 652d 6d6c 6f70  ples/readme-mlop
-000030c0: 732e 6d64 223e 7265 6164 6d65 2d6d 6c6f  s.md">readme-mlo
-000030d0: 7073 2e6d 643c 2f61 3e3c 2f74 643e 0a20  ps.md</a></td>. 
-000030e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000030f0: 7464 3e3c 6120 6872 6566 3d22 6874 7470  td><a href="http
-00003100: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f47  s://github.com/G
-00003110: 6f6b 754d 6f68 616e 6461 732f 6d6c 6f70  okuMohandas/mlop
-00003120: 732d 636f 7572 7365 223e 6d6c 6f70 732d  s-course">mlops-
-00003130: 636f 7572 7365 3c2f 613e 3c2f 7464 3e0a  course</a></td>.
-00003140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003150: 3c74 643e 5079 7468 6f6e 2c20 4a75 7079  <td>Python, Jupy
-00003160: 7465 723c 2f74 643e 0a20 2020 2020 2020  ter</td>.       
-00003170: 2020 2020 2020 2020 203c 7464 3e0a 2020           <td>.  
-00003180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003190: 2020 3c70 3e38 2c35 3234 3c2f 703e 0a20    <p>8,524</p>. 
-000031a0: 2020 2020 2020 2020 2020 203c 2f74 723e             </tr>
-000031b0: 0a20 2020 2020 2020 2020 2020 203c 7472  .            <tr
-000031c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000031d0: 2020 3c74 643e f09f 949f 3c2f 7464 3e0a    <td>....</td>.
-000031e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031f0: 3c74 643e 3c61 2068 7265 663d 2268 7474  <td><a href="htt
-00003200: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003210: 656c 6936 3473 2f72 6561 646d 652d 6169  eli64s/readme-ai
-00003220: 2f62 6c6f 622f 6d61 696e 2f65 7861 6d70  /blob/main/examp
-00003230: 6c65 732f 7265 6164 6d65 2d70 7966 6c69  les/readme-pyfli
-00003240: 6e6b 2e6d 6422 3e72 6561 646d 652d 7079  nk.md">readme-py
-00003250: 666c 696e 6b2e 6d64 3c2f 613e 3c2f 7464  flink.md</a></td
-00003260: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00003270: 2020 3c74 643e 3c61 2068 7265 663d 2268    <td><a href="h
-00003280: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003290: 6d2f 656c 6936 3473 2f66 6c69 6e6b 2d66  m/eli64s/flink-f
-000032a0: 6c6f 7722 3e66 6c69 6e6b 2d66 6c6f 773c  low">flink-flow<
-000032b0: 2f61 3e3c 2f74 643e 0a20 2020 2020 2020  /a></td>.       
-000032c0: 2020 2020 2020 2020 203c 7464 3e50 7946           <td>PyF
-000032d0: 6c69 6e6b 3c2f 7464 3e0a 2020 2020 2020  link</td>.      
-000032e0: 2020 2020 2020 2020 2020 3c74 643e 0a20            <td>. 
-000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003300: 2020 203c 703e 3332 3c2f 703e 0a20 2020     <p>32</p>.   
-00003310: 2020 2020 2020 2020 203c 2f74 723e 0a20           </tr>. 
-00003320: 2020 203c 2f74 6162 6c65 3e0a 3c2f 6469     </table>.</di
-00003330: 763e 0a0a 0a3c 6831 2061 6c69 676e 3d22  v>...<h1 align="
-00003340: 6365 6e74 6572 223e e292 8f3c 6272 3ef0  center">...<br>.
-00003350: 9f91 873c 6272 3e3c 6272 3ef0 9f93 9c20  ...<br><br>.... 
-00003360: 4375 7374 6f6d 2052 4541 444d 4520 7465  Custom README te
-00003370: 6d70 6c61 7465 7320 636f 6d69 6e67 2073  mplates coming s
-00003380: 6f6f 6e21 3c2f 6831 3e0a 3c70 2061 6c69  oon!</h1>.<p ali
-00003390: 676e 3d22 6365 6e74 6572 223e 4465 7665  gn="center">Deve
-000033a0: 6c6f 7069 6e67 2061 2066 6561 7475 7265  loping a feature
-000033b0: 2074 6861 7420 616c 6c6f 7773 2075 7365   that allows use
-000033c0: 7273 2074 6f20 7365 6c65 6374 2066 726f  rs to select fro
-000033d0: 6d20 6120 7661 7269 6574 7920 6f66 2052  m a variety of R
-000033e0: 4541 444d 4520 666f 726d 6174 7320 616e  EADME formats an
-000033f0: 6420 7374 796c 6573 2e3c 2f70 3e0a 3c70  d styles.</p>.<p
-00003400: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00003410: 4375 7374 6f6d 2074 656d 706c 6174 6573  Custom templates
-00003420: 2077 696c 6c20 6265 2074 6169 6c6f 7265   will be tailore
-00003430: 6420 666f 7220 7573 652d 6361 7365 7320  d for use-cases 
-00003440: 7375 6368 2061 7320 6461 7461 2c20 6169  such as data, ai
-00003450: 2026 206d 6c2c 2072 6573 6561 7263 682c   & ml, research,
-00003460: 206d 696e 696d 616c 2c20 616e 6420 6d6f   minimal, and mo
-00003470: 7265 213c 2f70 3e0a 0a3c 7020 616c 6967  re!</p>..<p alig
-00003480: 6e3d 2272 6967 6874 223e 0a20 2020 203c  n="right">.    <
-00003490: 6120 6872 6566 3d22 2374 6f70 223e 3c62  a href="#top"><b
-000034a0: 3ef0 9f94 9d20 5265 7475 726e 203c 2f62  >.... Return </b
-000034b0: 3e3c 2f61 3e0a 3c2f 703e 0a0a 2d2d 2d0a  ></a>.</p>..---.
-000034c0: 0a23 2320 f09f 9a80 2047 6574 7469 6e67  .## .... Getting
-000034d0: 2053 7461 7274 6564 0a0a 2323 2320 e29c   Started..### ..
-000034e0: 94ef b88f 2044 6570 656e 6465 6e63 6965  .... Dependencie
-000034f0: 730a 0a42 6566 6f72 6520 796f 7520 6265  s..Before you be
-00003500: 6769 6e2c 2065 6e73 7572 6520 7468 6174  gin, ensure that
-00003510: 2079 6f75 2068 6176 6520 7468 6520 666f   you have the fo
-00003520: 6c6c 6f77 696e 6720 7072 6572 6571 7569  llowing prerequi
-00003530: 7369 7465 7320 696e 7374 616c 6c65 643a  sites installed:
-00003540: 0a0a 2d20 5079 7468 6f6e 2033 2e39 206f  ..- Python 3.9 o
-00003550: 7220 6869 6768 6572 0a2d 2043 6f6e 6461  r higher.- Conda
-00003560: 206f 7220 506f 6574 7279 2070 6163 6b61   or Poetry packa
-00003570: 6765 206d 616e 6167 6572 2028 7265 636f  ge manager (reco
-00003580: 6d6d 656e 6465 6429 0a2d 2041 6363 6573  mmended).- Acces
-00003590: 7320 746f 2074 6865 204f 7065 6e41 4920  s to the OpenAI 
-000035a0: 4150 4920 2873 6565 2074 6865 2073 6574  API (see the set
-000035b0: 7570 2067 7569 6465 2062 656c 6f77 290a  up guide below).
-000035c0: 0a23 2323 2320 f09f 9382 2052 6570 6f73  .#### .... Repos
-000035d0: 6974 6f72 790a 0a4d 6f73 7420 7573 6572  itory..Most user
-000035e0: 2773 2077 696c 6c20 7275 6e20 2a52 4541  's will run *REA
-000035f0: 444d 452d 4149 2a20 7573 696e 6720 7468  DME-AI* using th
-00003600: 6520 636f 6d6d 616e 642d 6c69 6e65 2c20  e command-line, 
-00003610: 7370 6563 6966 7969 6e67 2074 6865 6972  specifying their
-00003620: 2072 6570 6f73 6974 6f72 7920 6f6e 2072   repository on r
-00003630: 756e 2d74 696d 652e 2048 6f77 6576 6572  un-time. However
-00003640: 2c20 6966 2079 6f75 2077 6f75 6c64 206c  , if you would l
-00003650: 696b 6520 746f 2075 7365 2074 6865 2064  ike to use the d
-00003660: 6566 6175 6c74 2063 6f6e 6669 6775 7261  efault configura
-00003670: 7469 6f6e 2c20 796f 7520 7769 6c6c 206e  tion, you will n
-00003680: 6565 6420 746f 2075 7064 6174 6520 7468  eed to update th
-00003690: 6520 5b63 6f6e 6669 6775 7261 7469 6f6e  e [configuration
-000036a0: 2066 696c 655d 282e 2f63 6f6e 662f 636f   file](./conf/co
-000036b0: 6e66 2e74 6f6d 6c29 2077 6974 6820 796f  nf.toml) with yo
-000036c0: 7572 2072 6570 6f73 6974 6f72 7927 7320  ur repository's 
-000036d0: 7265 6d6f 7465 2055 524c 2028 4769 7448  remote URL (GitH
-000036e0: 7562 2c20 4769 744c 6162 2920 6f72 206c  ub, GitLab) or l
-000036f0: 6f63 616c 2064 6972 6563 746f 7279 2070  ocal directory p
-00003700: 6174 6820 6f6e 2079 6f75 7220 6d61 6368  ath on your mach
-00003710: 696e 652e 0a0a 6060 6074 6f6d 6c0a 5b67  ine...```toml.[g
-00003720: 6974 5d0a 7265 706f 7369 746f 7279 203d  it].repository =
-00003730: 2022 496e 7365 7274 2079 6f75 7220 7265   "Insert your re
-00003740: 706f 7369 746f 7279 2055 524c 206f 7220  pository URL or 
-00003750: 6c6f 6361 6c20 7061 7468 2068 6572 6521  local path here!
-00003760: 220a 6060 600a 0a23 2323 2320 f09f 9490  ".```..#### ....
-00003770: 204f 7065 6e41 4920 4150 490a 0a54 6f20   OpenAI API..To 
-00003780: 7573 6520 7468 6520 5245 4144 4d45 2d41  use the README-A
-00003790: 4920 6170 706c 6963 6174 696f 6e2c 2079  I application, y
-000037a0: 6f75 2077 696c 6c20 6e65 6564 2074 6f20  ou will need to 
-000037b0: 6372 6561 7465 2061 6e20 6163 636f 756e  create an accoun
-000037c0: 7420 7769 7468 204f 7065 6e41 4920 746f  t with OpenAI to
-000037d0: 2067 656e 6572 6174 6520 616e 2041 5049   generate an API
-000037e0: 206b 6579 2e20 5468 6520 7374 6570 7320   key. The steps 
-000037f0: 6265 6c6f 7720 6f75 746c 696e 6520 7468  below outline th
-00003800: 6973 2073 6574 7570 2070 726f 6365 7373  is setup process
-00003810: 3a0a 0a3c 6465 7461 696c 7320 636c 6f73  :..<details clos
-00003820: 6564 3e3c 7375 6d6d 6172 793e 4f70 656e  ed><summary>Open
-00003830: 4149 2041 5049 2055 7365 7220 4775 6964  AI API User Guid
-00003840: 653c 2f73 756d 6d61 7279 3e0a 0a31 2e20  e</summary>..1. 
-00003850: 476f 2074 6f20 7468 6520 5b4f 7065 6e41  Go to the [OpenA
-00003860: 4920 7765 6273 6974 655d 2868 7474 7073  I website](https
-00003870: 3a2f 2f70 6c61 7466 6f72 6d2e 6f70 656e  ://platform.open
-00003880: 6169 2e63 6f6d 2f29 2e0a 322e 2043 6c69  ai.com/)..2. Cli
-00003890: 636b 2074 6865 2022 5369 676e 2075 7020  ck the "Sign up 
-000038a0: 666f 7220 6672 6565 2220 6275 7474 6f6e  for free" button
-000038b0: 2e0a 332e 2046 696c 6c20 6f75 7420 7468  ..3. Fill out th
-000038c0: 6520 7265 6769 7374 7261 7469 6f6e 2066  e registration f
-000038d0: 6f72 6d20 7769 7468 2079 6f75 7220 696e  orm with your in
-000038e0: 666f 726d 6174 696f 6e20 616e 6420 6167  formation and ag
-000038f0: 7265 6520 746f 2074 6865 2074 6572 6d73  ree to the terms
-00003900: 206f 6620 7365 7276 6963 652e 0a34 2e20   of service..4. 
-00003910: 4f6e 6365 206c 6f67 6765 6420 696e 2c20  Once logged in, 
-00003920: 636c 6963 6b20 6f6e 2074 6865 2022 4150  click on the "AP
-00003930: 4922 2074 6162 2e0a 352e 2046 6f6c 6c6f  I" tab..5. Follo
-00003940: 7720 7468 6520 696e 7374 7275 6374 696f  w the instructio
-00003950: 6e73 2074 6f20 6372 6561 7465 2061 206e  ns to create a n
-00003960: 6577 2041 5049 206b 6579 2e0a 362e 2043  ew API key..6. C
-00003970: 6f70 7920 7468 6520 4150 4920 6b65 7920  opy the API key 
-00003980: 616e 6420 6b65 6570 2069 7420 696e 2061  and keep it in a
-00003990: 2073 6563 7572 6520 706c 6163 652e 0a0a   secure place...
-000039a0: 3c2f 6465 7461 696c 733e 0a3c 6272 3e0a  </details>.<br>.
-000039b0: 0a3e 202a 2ae2 9aa0 efb8 8f20 4e6f 7465  .> **...... Note
-000039c0: 2a2a 0a3e 0a3e 202d 2054 6f20 6d61 7869  **.>.> - To maxi
-000039d0: 6d69 7a65 2079 6f75 7220 6578 7065 7269  mize your experi
-000039e0: 656e 6365 2077 6974 6820 5245 4144 4d45  ence with README
-000039f0: 2d41 492c 2069 7420 6973 2072 6563 6f6d  -AI, it is recom
-00003a00: 6d65 6e64 6564 2074 6f20 7365 7420 7570  mended to set up
-00003a10: 2061 2070 6179 6d65 6e74 206d 6574 686f   a payment metho
-00003a20: 6420 6f6e 204f 7065 6e41 4927 7320 7765  d on OpenAI's we
-00003a30: 6273 6974 652e 2042 7920 646f 696e 6720  bsite. By doing 
-00003a40: 736f 2c20 796f 7520 6761 696e 2061 6363  so, you gain acc
-00003a50: 6573 7320 746f 206d 6f72 6520 706f 7765  ess to more powe
-00003a60: 7266 756c 206c 616e 6775 6167 6520 6d6f  rful language mo
-00003a70: 6465 6c73 206c 696b 6520 6770 742d 332e  dels like gpt-3.
-00003a80: 352d 7475 7262 6f2e 2057 6974 686f 7574  5-turbo. Without
-00003a90: 2061 2070 6179 6d65 6e74 206d 6574 686f   a payment metho
-00003aa0: 642c 2079 6f75 7220 7573 6167 6520 7769  d, your usage wi
-00003ab0: 6c6c 2062 6520 7265 7374 7269 6374 6564  ll be restricted
-00003ac0: 2074 6f20 7468 6520 6261 7365 2067 7074   to the base gpt
-00003ad0: 2d33 206d 6f64 656c 732e 2054 6869 7320  -3 models. This 
-00003ae0: 6c69 6d69 7461 7469 6f6e 206d 6967 6874  limitation might
-00003af0: 206c 6561 6420 746f 206c 6573 7320 7072   lead to less pr
-00003b00: 6563 6973 6520 5245 4144 4d45 2066 696c  ecise README fil
-00003b10: 6573 206f 7220 706f 7465 6e74 6961 6c20  es or potential 
-00003b20: 6572 726f 7273 2064 7572 696e 6720 7468  errors during th
-00003b30: 6520 6765 6e65 7261 7469 6f6e 2070 726f  e generation pro
-00003b40: 6365 7373 2e0a 3e0a 3e20 2d20 5768 656e  cess..>.> - When
-00003b50: 2075 7369 6e67 2061 2070 6179 6d65 6e74   using a payment
-00003b60: 206d 6574 686f 642c 206d 616b 6520 7375   method, make su
-00003b70: 7265 2079 6f75 2068 6176 6520 7375 6666  re you have suff
-00003b80: 6963 6965 6e74 2063 7265 6469 7473 2074  icient credits t
-00003b90: 6f20 7275 6e20 7468 6520 5245 4144 4d45  o run the README
-00003ba0: 2d41 4920 6170 706c 6963 6174 696f 6e2e  -AI application.
-00003bb0: 2041 6464 6974 696f 6e61 6c6c 792c 2072   Additionally, r
-00003bc0: 656d 656d 6265 7220 746f 2072 6567 756c  emember to regul
-00003bd0: 6172 6c79 206d 6f6e 6974 6f72 2079 6f75  arly monitor you
-00003be0: 7220 4150 4920 7573 6167 6520 616e 6420  r API usage and 
-00003bf0: 636f 7374 7320 6279 2076 6973 6974 696e  costs by visitin
-00003c00: 6720 7468 6520 5b4f 7065 6e41 4920 4150  g the [OpenAI AP
-00003c10: 4920 5573 6167 6520 4461 7368 626f 6172  I Usage Dashboar
-00003c20: 645d 2868 7474 7073 3a2f 2f70 6c61 7466  d](https://platf
-00003c30: 6f72 6d2e 6f70 656e 6169 2e63 6f6d 2f61  orm.openai.com/a
-00003c40: 6363 6f75 6e74 2f75 7361 6765 292e 2050  ccount/usage). P
-00003c50: 6c65 6173 6520 6e6f 7465 2074 6861 7420  lease note that 
-00003c60: 7468 6973 2041 5049 2069 7320 6e6f 7420  this API is not 
-00003c70: 6672 6565 2061 6e64 2079 6f75 2077 696c  free and you wil
-00003c80: 6c20 6265 2063 6861 7267 6564 2066 6f72  l be charged for
-00003c90: 2065 6163 6820 7265 7175 6573 7420 6d61   each request ma
-00003ca0: 6465 2c20 7768 6963 6820 6361 6e20 6163  de, which can ac
-00003cb0: 6375 6d75 6c61 7465 2072 6170 6964 6c79  cumulate rapidly
-00003cc0: 2e0a 3e0a 3e20 2d20 5468 6520 6765 6e65  ..>.> - The gene
-00003cd0: 7261 7469 6f6e 206f 6620 7468 6520 5245  ration of the RE
-00003ce0: 4144 4d45 2e6d 6420 6669 6c65 2073 686f  ADME.md file sho
-00003cf0: 756c 6420 7479 7069 6361 6c6c 7920 636f  uld typically co
-00003d00: 6d70 6c65 7465 2069 6e20 756e 6465 7220  mplete in under 
-00003d10: 3120 6d69 6e75 7465 2e20 4966 2069 7420  1 minute. If it 
-00003d20: 7461 6b65 7320 6c6f 6e67 6572 2074 6861  takes longer tha
-00003d30: 6e20 6120 6665 7720 6d69 6e75 7465 732c  n a few minutes,
-00003d40: 2070 6c65 6173 6520 7465 726d 696e 6174   please terminat
-00003d50: 6520 7468 6520 7072 6f63 6573 732e 0a3e  e the process..>
-00003d60: 0a0a 2d2d 2d0a 0a23 2323 20f0 9f93 a620  ..---..### .... 
-00003d70: 496e 7374 616c 6c61 7469 6f6e 0a0a 312e  Installation..1.
-00003d80: 2043 6c6f 6e65 2074 6865 202a 7265 6164   Clone the *read
-00003d90: 6d65 2d61 692a 2072 6570 6f73 6974 6f72  me-ai* repositor
-00003da0: 7920 746f 2079 6f75 7220 6c6f 6361 6c20  y to your local 
-00003db0: 6d61 6368 696e 652e 0a60 6060 7368 0a67  machine..```sh.g
-00003dc0: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
-00003dd0: 2f67 6974 6875 622e 636f 6d2f 656c 6936  /github.com/eli6
-00003de0: 3473 2f72 6561 646d 652d 6169 0a60 6060  4s/readme-ai.```
-00003df0: 0a0a 322e 204e 6176 6967 6174 6520 746f  ..2. Navigate to
-00003e00: 2074 6865 202a 7265 6164 6d65 2d61 692a   the *readme-ai*
-00003e10: 2064 6972 6563 746f 7279 2e0a 6060 6073   directory..```s
-00003e20: 680a 6364 2072 6561 646d 652d 6169 0a60  h.cd readme-ai.`
-00003e30: 6060 0a0a 332e 2055 7365 206f 6e65 206f  ``..3. Use one o
-00003e40: 6620 7468 6520 666f 6c6c 6f77 696e 6720  f the following 
-00003e50: 6d65 7468 6f64 7320 746f 2069 6e73 7461  methods to insta
-00003e60: 6c6c 2074 6865 2072 6571 7569 7265 6420  ll the required 
-00003e70: 6465 7065 6e64 656e 6369 6573 3a0a 0a3e  dependencies:..>
-00003e80: 202a 5069 7020 2850 7950 4920 5061 636b   *Pip (PyPI Pack
-00003e90: 6167 6529 2a0a 6060 6073 680a 7069 7020  age)*.```sh.pip 
-00003ea0: 696e 7374 616c 6c20 7265 6164 6d65 6169  install readmeai
-00003eb0: 0a60 6060 0a0a 3e20 2a42 6173 682a 0a60  .```..> *Bash*.`
-00003ec0: 6060 7368 0a62 6173 6820 7365 7475 702f  ``sh.bash setup/
-00003ed0: 7365 7475 702e 7368 0a60 6060 0a0a 3e20  setup.sh.```..> 
-00003ee0: 2a43 6f6e 6461 2a0a 6060 6073 680a 636f  *Conda*.```sh.co
-00003ef0: 6e64 6120 6372 6561 7465 202d 6e20 7265  nda create -n re
-00003f00: 6164 6d65 6169 2070 7974 686f 6e3d 332e  admeai python=3.
-00003f10: 3920 2d79 2026 2620 5c0a 636f 6e64 6120  9 -y && \.conda 
-00003f20: 6163 7469 7661 7465 2072 6561 646d 6561  activate readmea
-00003f30: 6920 2626 205c 0a70 6970 2069 6e73 7461  i && \.pip insta
-00003f40: 6c6c 202d 7220 7265 7175 6972 656d 656e  ll -r requiremen
-00003f50: 7473 2e74 7874 0a60 6060 0a0a 3e20 2a50  ts.txt.```..> *P
-00003f60: 6f65 7472 792a 0a60 6060 7368 0a70 6f65  oetry*.```sh.poe
-00003f70: 7472 7920 696e 7374 616c 6c0a 6060 600a  try install.```.
-00003f80: 0a3e 202a 446f 636b 6572 2a0a 6060 6073  .> *Docker*.```s
-00003f90: 680a 646f 636b 6572 2070 756c 6c20 7a65  h.docker pull ze
-00003fa0: 726f 7865 6c69 2f72 6561 646d 652d 6169  roxeli/readme-ai
-00003fb0: 3a30 2e30 2e36 0a60 6060 0a0a 2323 2320  :0.0.6.```..### 
-00003fc0: f09f 8eae 2055 7369 6e67 202a 5245 4144  .... Using *READ
-00003fd0: 4d45 2d41 492a 0a0a 5573 6520 7468 6520  ME-AI*..Use the 
-00003fe0: 636f 6d6d 616e 642d 6c69 6e65 2074 6f20  command-line to 
-00003ff0: 7072 6f76 6964 6520 7468 6520 4f70 656e  provide the Open
-00004000: 4149 2041 5049 206b 6579 2028 6966 206e  AI API key (if n
-00004010: 6f74 2061 6c72 6561 6479 2073 6574 2920  ot already set) 
-00004020: 616e 6420 7370 6563 6966 7920 616e 206f  and specify an o
-00004030: 7574 7075 7420 7061 7468 2066 6f72 2079  utput path for y
-00004040: 6f75 7220 5245 4144 4d45 2066 696c 652c  our README file,
-00004050: 2061 6c6f 6e67 2077 6974 6820 7468 6520   along with the 
-00004060: 7061 7468 2074 6f20 796f 7572 206c 6f63  path to your loc
-00004070: 616c 2072 6570 6f73 6974 6f72 7920 6f72  al repository or
-00004080: 2072 656d 6f74 6520 636f 6465 2072 6570   remote code rep
-00004090: 6f73 6974 6f72 792e 2059 6f75 2063 616e  ository. You can
-000040a0: 2061 6c73 6f20 7072 6f76 6964 6520 7468   also provide th
-000040b0: 6520 6f75 7470 7574 2070 6174 6820 696e  e output path in
-000040c0: 2074 6865 205b 636f 6e66 6967 7572 6174   the [configurat
-000040d0: 696f 6e20 6669 6c65 5d28 2e2f 636f 6e66  ion file](./conf
-000040e0: 2f63 6f6e 662e 746f 6d6c 290a 0a43 6f6d  /conf.toml)..Com
-000040f0: 6d61 6e64 2d4c 696e 6520 4172 6775 6d65  mand-Line Argume
-00004100: 6e74 733a 0a0a 2d20 602d 6b60 206f 7220  nts:..- `-k` or 
-00004110: 602d 2d61 7069 2d6b 6579 603a 2059 6f75  `--api-key`: You
-00004120: 7220 4f70 656e 4149 2041 5049 206b 6579  r OpenAI API key
-00004130: 2e0a 2d20 602d 6f60 206f 7220 602d 2d6f  ..- `-o` or `--o
-00004140: 7574 7075 7460 3a20 5468 6520 6f75 7470  utput`: The outp
-00004150: 7574 2070 6174 6820 666f 7220 796f 7572  ut path for your
-00004160: 2052 4541 444d 452e 6d64 2066 696c 652e   README.md file.
-00004170: 0a2d 2060 2d72 6020 6f72 2060 2d2d 7265  .- `-r` or `--re
-00004180: 706f 7369 746f 7279 603a 2054 6865 2055  pository`: The U
-00004190: 524c 206f 7220 7061 7468 2074 6f20 796f  RL or path to yo
-000041a0: 7572 2063 6f64 6520 7265 706f 7369 746f  ur code reposito
-000041b0: 7279 2e0a 2d20 602d 7460 206f 7220 602d  ry..- `-t` or `-
-000041c0: 2d74 656d 706c 6174 6560 3a20 5468 6520  -template`: The 
-000041d0: 5245 4144 4d45 2074 656d 706c 6174 6520  README template 
-000041e0: 666f 726d 6174 2074 6f20 7573 652e 2028  format to use. (
-000041f0: 636f 6d69 6e67 2073 6f6f 6e21 290a 2d20  coming soon!).- 
-00004200: 606c 6020 6f72 2060 2d2d 6c61 6e67 7561  `l` or `--langua
-00004210: 6765 603a 2054 6865 206c 616e 6775 6167  ge`: The languag
-00004220: 6520 6f66 2074 6578 7420 7772 6974 7465  e of text writte
-00004230: 6e20 696e 2074 6865 2052 4541 444d 4520  n in the README 
-00004240: 6669 6c65 2028 636f 6d69 6e67 2073 6f6f  file (coming soo
-00004250: 6e21 290a 0a3e 202a 5069 7020 2850 7950  n!)..> *Pip (PyP
-00004260: 4920 5061 636b 6167 6529 2a0a 6060 6073  I Package)*.```s
-00004270: 680a 7265 6164 6d65 6169 202d 2d61 7069  h.readmeai --api
-00004280: 2d6b 6579 2022 594f 5552 5f41 5049 5f4b  -key "YOUR_API_K
-00004290: 4559 2220 2d2d 6f75 7470 7574 2072 6561  EY" --output rea
-000042a0: 646d 652d 6169 2e6d 6420 2d2d 7265 706f  dme-ai.md --repo
-000042b0: 7369 746f 7279 2068 7474 7073 3a2f 2f67  sitory https://g
-000042c0: 6974 6875 622e 636f 6d2f 656c 6936 3473  ithub.com/eli64s
-000042d0: 2f72 6561 646d 652d 6169 0a0a 2320 4f72  /readme-ai..# Or
-000042e0: 2065 7870 6f72 7420 796f 7572 204f 7065   export your Ope
-000042f0: 6e41 4920 4150 4920 6b65 7920 6173 2061  nAI API key as a
-00004300: 6e20 656e 7669 726f 6e6d 656e 7420 7661  n environment va
-00004310: 7269 6162 6c65 0a65 7870 6f72 7420 4f50  riable.export OP
-00004320: 454e 4149 5f41 5049 5f4b 4559 3d22 594f  ENAI_API_KEY="YO
-00004330: 5552 5f41 5049 5f4b 4559 220a 7265 6164  UR_API_KEY".read
-00004340: 6d65 6169 202d 6f20 7265 6164 6d65 2d61  meai -o readme-a
-00004350: 692e 6d64 202d 7220 6874 7470 733a 2f2f  i.md -r https://
-00004360: 6769 7468 7562 2e63 6f6d 2f65 6c69 3634  github.com/eli64
-00004370: 732f 7265 6164 6d65 2d61 690a 6060 600a  s/readme-ai.```.
-00004380: 0a3e 202a 436f 6e64 612a 0a60 6060 7368  .> *Conda*.```sh
-00004390: 0a70 7974 686f 6e20 7265 6164 6d65 6169  .python readmeai
-000043a0: 2f6d 6169 6e2e 7079 202d 2d61 7069 2d6b  /main.py --api-k
-000043b0: 6579 2022 594f 5552 5f41 5049 5f4b 4559  ey "YOUR_API_KEY
-000043c0: 2220 2d2d 6f75 7470 7574 2072 6561 646d  " --output readm
-000043d0: 652d 6169 2e6d 6420 2d2d 7265 706f 7369  e-ai.md --reposi
-000043e0: 746f 7279 2068 7474 7073 3a2f 2f67 6974  tory https://git
-000043f0: 6875 622e 636f 6d2f 656c 6936 3473 2f72  hub.com/eli64s/r
-00004400: 6561 646d 652d 6169 0a0a 2320 4f72 2065  eadme-ai..# Or e
-00004410: 7870 6f72 7420 796f 7572 204f 7065 6e41  xport your OpenA
-00004420: 4920 4150 4920 6b65 7920 6173 2061 6e20  I API key as an 
-00004430: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-00004440: 6162 6c65 0a63 6f6e 6461 2061 6374 6976  able.conda activ
-00004450: 6174 6520 7265 6164 6d65 6169 0a65 7870  ate readmeai.exp
-00004460: 6f72 7420 4f50 454e 4149 5f41 5049 5f4b  ort OPENAI_API_K
-00004470: 4559 3d22 594f 5552 5f41 5049 5f4b 4559  EY="YOUR_API_KEY
-00004480: 220a 7079 7468 6f6e 2072 6561 646d 6561  ".python readmea
-00004490: 692f 6d61 696e 2e70 7920 2d6f 2072 6561  i/main.py -o rea
-000044a0: 646d 652d 6169 2e6d 6420 2d72 2068 7474  dme-ai.md -r htt
-000044b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000044c0: 656c 6936 3473 2f72 6561 646d 652d 6169  eli64s/readme-ai
-000044d0: 0a60 6060 0a0a 3e20 2a50 6f65 7472 792a  .```..> *Poetry*
-000044e0: 0a60 6060 7368 0a70 6f65 7472 7920 7368  .```sh.poetry sh
-000044f0: 656c 6c0a 6578 706f 7274 204f 5045 4e41  ell.export OPENA
-00004500: 495f 4150 495f 4b45 593d 2259 4f55 525f  I_API_KEY="YOUR_
-00004510: 4150 495f 4b45 5922 0a70 6f65 7472 7920  API_KEY".poetry 
-00004520: 7275 6e20 7079 7468 6f6e 2072 6561 646d  run python readm
-00004530: 6561 692f 6d61 696e 2e70 7920 2d6f 2072  eai/main.py -o r
-00004540: 6561 646d 652d 6169 2e6d 6420 2d72 2068  eadme-ai.md -r h
-00004550: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004560: 6d2f 656c 6936 3473 2f72 6561 646d 652d  m/eli64s/readme-
-00004570: 6169 0a60 6060 0a0a 3e20 2a44 6f63 6b65  ai.```..> *Docke
-00004580: 722a 0a60 6060 7368 0a64 6f63 6b65 7220  r*.```sh.docker 
-00004590: 7275 6e20 2d69 7420 5c0a 2d65 204f 5045  run -it \.-e OPE
-000045a0: 4e41 495f 4150 495f 4b45 593d 2259 4f55  NAI_API_KEY="YOU
-000045b0: 525f 4150 495f 4b45 5922 205c 0a2d 7620  R_API_KEY" \.-v 
-000045c0: 2224 2870 7764 2922 3a2f 6170 7020 7a65  "$(pwd)":/app ze
-000045d0: 726f 7865 6c69 2f72 6561 646d 652d 6169  roxeli/readme-ai
-000045e0: 3a30 2e30 2e36 205c 0a72 6561 646d 6561  :0.0.6 \.readmea
-000045f0: 6920 2d6f 2072 6561 646d 652d 6169 2e6d  i -o readme-ai.m
-00004600: 6420 2d72 2068 7474 7073 3a2f 2f67 6974  d -r https://git
-00004610: 6875 622e 636f 6d2f 656c 6936 3473 2f72  hub.com/eli64s/r
-00004620: 6561 646d 652d 6169 0a60 6060 0a0a 2323  eadme-ai.```..##
-00004630: 2320 f09f a7aa 2052 756e 6e69 6e67 2054  # .... Running T
-00004640: 6573 7473 0a0a 546f 2072 756e 2074 6865  ests..To run the
-00004650: 2075 6e69 742d 7465 7374 7320 666f 7220   unit-tests for 
-00004660: 5245 4144 4d45 2d41 492c 2075 7365 2074  README-AI, use t
-00004670: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-00004680: 6d61 6e64 2e0a 0a60 6060 7368 0a62 6173  mand...```sh.bas
-00004690: 6820 7363 7269 7074 732f 7465 7374 2e73  h scripts/test.s
-000046a0: 680a 6060 600a 0a3c 7020 616c 6967 6e3d  h.```..<p align=
-000046b0: 2272 6967 6874 223e 0a20 203c 6120 6872  "right">.  <a hr
-000046c0: 6566 3d22 2374 6f70 223e 3c62 3ef0 9f94  ef="#top"><b>...
-000046d0: 9d20 5265 7475 726e 203c 2f62 3e3c 2f61  . Return </b></a
-000046e0: 3e0a 3c2f 703e 0a0a 2d2d 2d0a 0a23 2320  >.</p>..---..## 
-000046f0: f09f 9ba0 2046 7574 7572 6520 4465 7665  .... Future Deve
-00004700: 6c6f 706d 656e 740a 0a2d 205b 585d 2041  lopment..- [X] A
-00004710: 6464 2061 6464 6974 696f 6e61 6c20 6c61  dd additional la
-00004720: 6e67 7561 6765 2073 7570 706f 7274 2066  nguage support f
-00004730: 6f72 2070 6f70 756c 6174 696e 6720 7468  or populating th
-00004740: 6520 2a69 6e73 7461 6c6c 6174 696f 6e2a  e *installation*
-00004750: 2c20 2a75 7361 6765 2a2c 2061 6e64 202a  , *usage*, and *
-00004760: 7465 7374 2a20 5245 4144 4d45 2073 6563  test* README sec
-00004770: 7469 6f6e 732e 0a2d 205b 585d 2055 706c  tions..- [X] Upl
-00004780: 6f61 6420 7468 6520 2a72 6561 646d 652d  oad the *readme-
-00004790: 6169 2a20 434c 4920 746f 6f6c 2074 6f20  ai* CLI tool to 
-000047a0: 5079 5049 2075 6e64 6572 2074 6865 206d  PyPI under the m
-000047b0: 6f64 756c 6520 6e61 6d65 205b 7265 6164  odule name [read
-000047c0: 6d65 6169 5d28 6874 7470 733a 2f2f 7079  meai](https://py
-000047d0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f72  pi.org/project/r
-000047e0: 6561 646d 6561 692f 292e 0a2d 205b 205d  eadmeai/)..- [ ]
-000047f0: 2044 6573 6967 6e20 616e 6420 696d 706c   Design and impl
-00004800: 656d 656e 7420 6120 7661 7269 6574 7920  ement a variety 
-00004810: 6f66 2052 4541 444d 4520 7465 6d70 6c61  of README templa
-00004820: 7465 2066 6f72 6d61 7473 2066 6f72 2064  te formats for d
-00004830: 6966 6665 7265 6e74 2075 7365 2d63 6173  ifferent use-cas
-00004840: 6573 2e0a 2d20 5b20 5d20 4164 6420 7375  es..- [ ] Add su
-00004850: 7070 6f72 7420 666f 7220 7772 6974 696e  pport for writin
-00004860: 6720 7468 6520 5245 4144 4d45 2069 6e20  g the README in 
-00004870: 616e 7920 6c61 6e67 7561 6765 2028 692e  any language (i.
-00004880: 652e 2043 4e2c 2045 532c 2046 522c 204a  e. CN, ES, FR, J
-00004890: 412c 204b 4f2c 2052 5529 2e0a 2d20 5b20  A, KO, RU)..- [ 
-000048a0: 5d20 4372 6561 7465 2055 4920 7769 7468  ] Create UI with
-000048b0: 205b 5465 7874 7561 6c5d 2868 7474 7073   [Textual](https
-000048c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5465  ://github.com/Te
-000048d0: 7874 7561 6c69 7a65 2f74 6578 7475 616c  xtualize/textual
-000048e0: 2920 6f72 2061 6e6f 7468 6572 2066 7261  ) or another fra
-000048f0: 6d65 776f 726b 2074 6f20 696d 7072 6f76  mework to improv
-00004900: 6520 7573 6572 2065 7870 6572 6965 6e63  e user experienc
-00004910: 652e 0a0a 2d2d 2d0a 0a23 2320 f09f 9392  e...---..## ....
-00004920: 2043 6861 6e67 656c 6f67 0a0a 5b43 6861   Changelog..[Cha
-00004930: 6e67 656c 6f67 5d28 2e2f 4348 414e 4745  ngelog](./CHANGE
-00004940: 4c4f 472e 6d64 290a 0a2d 2d2d 0a0a 2323  LOG.md)..---..##
-00004950: 20f0 9fa4 9d20 436f 6e74 7269 6275 7469   .... Contributi
-00004960: 6e67 0a0a 5b43 6f6e 7472 6962 7574 696e  ng..[Contributin
-00004970: 6720 4775 6964 656c 696e 6573 5d28 2e2f  g Guidelines](./
-00004980: 434f 4e54 5249 4255 5449 4e47 2e6d 6429  CONTRIBUTING.md)
-00004990: 0a0a 2d2d 2d0a 0a23 2320 f09f 9384 204c  ..---..## .... L
-000049a0: 6963 656e 7365 0a0a 5b4d 4954 5d28 2e2f  icense..[MIT](./
-000049b0: 4c49 4345 4e53 4529 0a0a 2d2d 2d0a 0a23  LICENSE)..---..#
-000049c0: 2320 f09f 918f 2041 636b 6e6f 776c 6564  # .... Acknowled
-000049d0: 676d 656e 7473 0a0a 2a42 6164 6765 732a  gments..*Badges*
-000049e0: 0a20 202d 205b 5368 6965 6c64 732e 696f  .  - [Shields.io
-000049f0: 5d28 6874 7470 733a 2f2f 7368 6965 6c64  ](https://shield
-00004a00: 732e 696f 2f29 0a20 202d 205b 4176 6565  s.io/).  - [Avee
-00004a10: 6b2d 5361 6861 2f47 6974 4875 622d 5072  k-Saha/GitHub-Pr
-00004a20: 6f66 696c 652d 4261 6467 6573 5d28 6874  ofile-Badges](ht
-00004a30: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00004a40: 2f41 7665 656b 2d53 6168 612f 4769 7448  /Aveek-Saha/GitH
-00004a50: 7562 2d50 726f 6669 6c65 2d42 6164 6765  ub-Profile-Badge
-00004a60: 7329 0a20 202d 205b 496c 6572 6961 796f  s).  - [Ileriayo
-00004a70: 2f4d 6172 6b64 6f77 6e2d 4261 6467 6573  /Markdown-Badges
-00004a80: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00004a90: 2e63 6f6d 2f49 6c65 7269 6179 6f2f 6d61  .com/Ileriayo/ma
-00004aa0: 726b 646f 776e 2d62 6164 6765 7329 0a0a  rkdown-badges)..
-00004ab0: 3c70 2061 6c69 676e 3d22 7269 6768 7422  <p align="right"
-00004ac0: 3e0a 2020 3c61 2068 7265 663d 2223 746f  >.  <a href="#to
-00004ad0: 7022 3e3c 623e f09f 949d 2052 6574 7572  p"><b>.... Retur
-00004ae0: 6e20 3c2f 623e 3c2f 613e 0a3c 2f70 3e0a  n </b></a>.</p>.
-00004af0: 0a2d 2d2d 0a0a                           .---..
+00000390: 7569 7265 732d 4469 7374 3a20 6769 7470  uires-Dist: gitp
+000003a0: 7974 686f 6e20 283e 3d33 2e31 2e33 312c  ython (>=3.1.31,
+000003b0: 3c34 2e30 2e30 290a 5265 7175 6972 6573  <4.0.0).Requires
+000003c0: 2d44 6973 743a 2068 3220 283e 3d34 2e31  -Dist: h2 (>=4.1
+000003d0: 2e30 2c3c 352e 302e 3029 0a52 6571 7569  .0,<5.0.0).Requi
+000003e0: 7265 732d 4469 7374 3a20 6874 7470 7820  res-Dist: httpx 
+000003f0: 283e 3d30 2e32 342e 312c 3c30 2e32 352e  (>=0.24.1,<0.25.
+00000400: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+00000410: 3a20 6f70 656e 6169 2028 3e3d 302e 3237  : openai (>=0.27
+00000420: 2e38 2c3c 302e 3238 2e30 290a 5265 7175  .8,<0.28.0).Requ
+00000430: 6972 6573 2d44 6973 743a 2070 7964 616e  ires-Dist: pydan
+00000440: 7469 6320 283e 3d31 2e31 302e 392c 3c32  tic (>=1.10.9,<2
+00000450: 2e30 2e30 290a 5265 7175 6972 6573 2d44  .0.0).Requires-D
+00000460: 6973 743a 2070 7979 616d 6c20 283e 3d36  ist: pyyaml (>=6
+00000470: 2e30 2c3c 372e 3029 0a52 6571 7569 7265  .0,<7.0).Require
+00000480: 732d 4469 7374 3a20 7265 7370 6f6e 7365  s-Dist: response
+00000490: 7320 283e 3d30 2e32 332e 312c 3c30 2e32  s (>=0.23.1,<0.2
+000004a0: 342e 3029 0a52 6571 7569 7265 732d 4469  4.0).Requires-Di
+000004b0: 7374 3a20 7461 6275 6c61 7465 2028 3e3d  st: tabulate (>=
+000004c0: 302e 392e 302c 3c30 2e31 302e 3029 0a52  0.9.0,<0.10.0).R
+000004d0: 6571 7569 7265 732d 4469 7374 3a20 7465  equires-Dist: te
+000004e0: 6e61 6369 7479 2028 3e3d 382e 322e 322c  nacity (>=8.2.2,
+000004f0: 3c39 2e30 2e30 290a 5265 7175 6972 6573  <9.0.0).Requires
+00000500: 2d44 6973 743a 2074 696b 746f 6b65 6e20  -Dist: tiktoken 
+00000510: 283e 3d30 2e34 2e30 2c3c 302e 352e 3029  (>=0.4.0,<0.5.0)
+00000520: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000530: 746f 6d6c 2028 3e3d 302e 3130 2e32 2c3c  toml (>=0.10.2,<
+00000540: 302e 3131 2e30 290a 5072 6f6a 6563 742d  0.11.0).Project-
+00000550: 5552 4c3a 2044 6f63 756d 656e 7461 7469  URL: Documentati
+00000560: 6f6e 2c20 6874 7470 733a 2f2f 6769 7468  on, https://gith
+00000570: 7562 2e63 6f6d 2f65 6c69 3634 732f 7265  ub.com/eli64s/re
+00000580: 6164 6d65 2d61 692f 626c 6f62 2f6d 6169  adme-ai/blob/mai
+00000590: 6e2f 5245 4144 4d45 2e6d 640a 4465 7363  n/README.md.Desc
+000005a0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+000005b0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+000005c0: 6f77 6e0a 0a3c 6469 7620 616c 6967 6e3d  own..<div align=
+000005d0: 2263 656e 7465 7222 3e0a 2020 2020 3c68  "center">.    <h
+000005e0: 3120 616c 6967 6e3d 2263 656e 7465 7222  1 align="center"
+000005f0: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
+00000600: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000610: 6963 6f6e 7338 2e63 6f6d 2f3f 7369 7a65  icons8.com/?size
+00000620: 3d35 3132 2669 643d 3535 3439 3426 666f  =512&id=55494&fo
+00000630: 726d 6174 3d70 6e67 2220 7769 6474 683d  rmat=png" width=
+00000640: 2238 3022 202f 3e0a 2020 2020 2020 2020  "80" />.        
+00000650: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000660: 2f2f 696d 672e 6963 6f6e 7338 2e63 6f6d  //img.icons8.com
+00000670: 2f3f 7369 7a65 3d35 3132 2669 643d 6b54  /?size=512&id=kT
+00000680: 7578 5659 524b 654b 4559 2666 6f72 6d61  uxVYRKeKEY&forma
+00000690: 743d 706e 6722 2077 6964 7468 3d22 3830  t=png" width="80
+000006a0: 2220 2f3e 0a20 2020 2020 2020 203c 6272  " />.        <br
+000006b0: 3e52 4541 444d 452d 4149 0a20 2020 203c  >README-AI.    <
+000006c0: 2f68 313e 0a20 2020 203c 6833 3ee2 97a6  /h1>.    <h3>...
+000006d0: 2047 656e 6572 6174 6520 6265 6175 7469   Generate beauti
+000006e0: 6675 6c20 616e 6420 696e 666f 726d 6174  ful and informat
+000006f0: 6976 6520 5245 4144 4d45 2e6d 6420 646f  ive README.md do
+00000700: 6375 6d65 6e74 732e 3c2f 6833 3e0a 2020  cuments.</h3>.  
+00000710: 2020 3c68 333e e297 a620 4465 7665 6c6f    <h3>... Develo
+00000720: 7065 6420 7769 7468 204f 7065 6e41 4927  ped with OpenAI'
+00000730: 7320 4750 5420 6c61 6e67 7561 6765 206d  s GPT language m
+00000740: 6f64 656c 2041 5049 732e 3c2f 6833 3e0a  odel APIs.</h3>.
+00000750: 2020 2020 3c62 723e 0a20 2020 203c 7020      <br>.    <p 
+00000760: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00000770: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000780: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000790: 6965 6c64 732e 696f 2f62 6164 6765 2f4d  ields.io/badge/M
+000007a0: 6172 6b64 6f77 6e2d 3030 3030 3030 2e73  arkdown-000000.s
+000007b0: 7667 3f73 7479 6c65 6526 6c6f 676f 3d4d  vg?stylee&logo=M
+000007c0: 6172 6b64 6f77 6e26 6c6f 676f 436f 6c6f  arkdown&logoColo
+000007d0: 723d 7768 6974 6522 2061 6c74 3d22 4d61  r=white" alt="Ma
+000007e0: 726b 646f 776e 2220 2f3e 0a20 2020 2020  rkdown" />.     
+000007f0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000800: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000810: 2e69 6f2f 6261 6467 652f 4f70 656e 4149  .io/badge/OpenAI
+00000820: 2d34 3132 3939 312e 7376 673f 7374 796c  -412991.svg?styl
+00000830: 6565 266c 6f67 6f3d 4f70 656e 4149 266c  ee&logo=OpenAI&l
+00000840: 6f67 6f43 6f6c 6f72 3d77 6869 7465 2220  ogoColor=white" 
+00000850: 616c 743d 224f 7065 6e41 4922 202f 3e0a  alt="OpenAI" />.
+00000860: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000870: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000880: 6965 6c64 732e 696f 2f62 6164 6765 2f50  ields.io/badge/P
+00000890: 7974 686f 6e2d 3337 3736 4142 2e73 7667  ython-3776AB.svg
+000008a0: 3f73 7479 6c65 6526 6c6f 676f 3d50 7974  ?stylee&logo=Pyt
+000008b0: 686f 6e26 6c6f 676f 436f 6c6f 723d 7768  hon&logoColor=wh
+000008c0: 6974 6522 2061 6c74 3d22 5079 7468 6f6e  ite" alt="Python
+000008d0: 2220 2f3e 0a20 2020 2020 2020 203c 696d  " />.        <im
+000008e0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+000008f0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000900: 6467 652f 5079 7465 7374 2d30 4139 4544  dge/Pytest-0A9ED
+00000910: 432e 7376 673f 7374 796c 6565 266c 6f67  C.svg?stylee&log
+00000920: 6f3d 5079 7465 7374 266c 6f67 6f43 6f6c  o=Pytest&logoCol
+00000930: 6f72 3d77 6869 7465 2220 616c 743d 2270  or=white" alt="p
+00000940: 7974 6573 7422 202f 3e0a 2020 2020 2020  ytest" />.      
+00000950: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000960: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000970: 696f 2f62 6164 6765 2f44 6f63 6b65 722d  io/badge/Docker-
+00000980: 3234 3936 4544 2e73 7667 3f73 7479 6c65  2496ED.svg?style
+00000990: 266c 6f67 6f3d 446f 636b 6572 266c 6f67  &logo=Docker&log
+000009a0: 6f43 6f6c 6f72 3d77 6869 7465 2220 616c  oColor=white" al
+000009b0: 743d 2244 6f63 6b65 7222 202f 3e0a 2020  t="Docker" />.  
+000009c0: 2020 2020 2020 3c69 6d67 2073 7263 3d22        <img src="
+000009d0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000009e0: 6c64 732e 696f 2f62 6164 6765 2f47 6974  lds.io/badge/Git
+000009f0: 4875 6225 3230 4163 7469 6f6e 732d 3230  Hub%20Actions-20
+00000a00: 3838 4646 2e73 7667 3f73 7479 6c65 266c  88FF.svg?style&l
+00000a10: 6f67 6f3d 4769 7448 7562 2d41 6374 696f  ogo=GitHub-Actio
+00000a20: 6e73 266c 6f67 6f43 6f6c 6f72 3d77 6869  ns&logoColor=whi
+00000a30: 7465 2220 616c 743d 2261 6374 696f 6e73  te" alt="actions
+00000a40: 2220 2f3e 0a20 2020 203c 2f70 3e0a 2020  " />.    </p>.  
+00000a50: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000a60: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000a70: 6563 742f 7265 6164 6d65 6169 2f22 3e0a  ect/readmeai/">.
+00000a80: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000a90: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000aa0: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000ab0: 7265 6164 6d65 6169 3f63 6f6c 6f72 3d35  readmeai?color=5
+00000ac0: 4436 4437 4526 6c6f 676f 3d70 7974 686f  D6D7E&logo=pytho
+00000ad0: 6e22 2061 6c74 3d22 5079 5049 202d 204c  n" alt="PyPI - L
+00000ae0: 6963 656e 7365 2220 2f3e 0a20 2020 203c  icense" />.    <
+00000af0: 2f61 3e0a 2020 2020 3c61 2068 7265 663d  /a>.    <a href=
+00000b00: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
+00000b10: 672f 7072 6f6a 6563 742f 7265 6164 6d65  g/project/readme
+00000b20: 6169 2f22 3e0a 2020 2020 2020 2020 3c69  ai/">.        <i
+00000b30: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000b40: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000b50: 7970 692f 7079 7665 7273 696f 6e73 2f72  ypi/pyversions/r
+00000b60: 6561 646d 6561 693f 636f 6c6f 723d 3544  eadmeai?color=5D
+00000b70: 3644 3745 266c 6f67 6f3d 7079 7468 6f6e  6D7E&logo=python
+00000b80: 2220 616c 743d 2250 7950 4920 2d20 5079  " alt="PyPI - Py
+00000b90: 7468 6f6e 2056 6572 7369 6f6e 2220 2f3e  thon Version" />
+00000ba0: 0a20 2020 203c 2f61 3e0a 2020 2020 3c61  .    </a>.    <a
+00000bb0: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+00000bc0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00000bd0: 7265 6164 6d65 6169 2f22 3e0a 2020 2020  readmeai/">.    
+00000be0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000bf0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000c00: 732e 696f 2f70 7970 692f 646d 2f72 6561  s.io/pypi/dm/rea
+00000c10: 646d 6561 693f 636f 6c6f 723d 3544 3644  dmeai?color=5D6D
+00000c20: 3745 2220 616c 743d 2250 7950 4920 2d20  7E" alt="PyPI - 
+00000c30: 446f 776e 6c6f 6164 7322 202f 3e0a 2020  Downloads" />.  
+00000c40: 2020 3c2f 613e 0a20 2020 203c 696d 6720    </a>.    <img 
+00000c50: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000c60: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000c70: 7562 2f6c 6963 656e 7365 2f65 6c69 3634  ub/license/eli64
+00000c80: 732f 5245 4144 4d45 2d41 493f 636f 6c6f  s/README-AI?colo
+00000c90: 723d 3544 3644 3745 2220 616c 743d 2247  r=5D6D7E" alt="G
+00000ca0: 6974 4875 6220 6c69 6365 6e73 6522 202f  itHub license" /
+00000cb0: 3e0a 3c2f 6469 763e 0a0a 2d2d 2d0a 0a23  >.</div>..---..#
+00000cc0: 2320 f09f 9396 2054 6162 6c65 206f 6620  # .... Table of 
+00000cd0: 436f 6e74 656e 7473 0a0a 2d20 5bf0 9f93  Contents..- [...
+00000ce0: 9620 5461 626c 6520 6f66 2043 6f6e 7465  . Table of Conte
+00000cf0: 6e74 735d 2823 2d74 6162 6c65 2d6f 662d  nts](#-table-of-
+00000d00: 636f 6e74 656e 7473 290a 2d20 5bf0 9f93  contents).- [...
+00000d10: 8d20 4f76 6572 7669 6577 5d28 232d 6f76  . Overview](#-ov
+00000d20: 6572 7669 6577 290a 2020 2020 2d20 5bf0  erview).    - [.
+00000d30: 9f8e af20 2a4d 6f74 6976 6174 696f 6e2a  ... *Motivation*
+00000d40: 5d28 232d 6d6f 7469 7661 7469 6f6e 290a  ](#-motivation).
+00000d50: 2020 2020 2d20 5be2 9aa0 efb8 8f20 2a44      - [...... *D
+00000d60: 6973 636c 6169 6d65 722a 5d28 23ef b88f  isclaimer*](#...
+00000d70: 2d64 6973 636c 6169 6d65 7229 0a2d 205b  -disclaimer).- [
+00000d80: f09f 91be 2044 656d 6f5d 2823 2d64 656d  .... Demo](#-dem
+00000d90: 6f29 0a2d 205b e29a 99ef b88f 2046 6561  o).- [...... Fea
+00000da0: 7475 7265 735d 2823 efb8 8f2d 6665 6174  tures](#...-feat
+00000db0: 7572 6573 290a 2d20 5bf0 9f9a 8020 4765  ures).- [.... Ge
+00000dc0: 7474 696e 6720 5374 6172 7465 645d 2823  tting Started](#
+00000dd0: 2d67 6574 7469 6e67 2d73 7461 7274 6564  -getting-started
+00000de0: 290a 2020 2d20 5be2 9c94 efb8 8f20 4465  ).  - [...... De
+00000df0: 7065 6e64 656e 6369 6573 5d28 23ef b88f  pendencies](#...
+00000e00: 2d64 6570 656e 6465 6e63 6965 7329 0a20  -dependencies). 
+00000e10: 2020 202d 205b f09f 9382 2052 6570 6f73     - [.... Repos
+00000e20: 6974 6f72 795d 2823 2d72 6570 6f73 6974  itory](#-reposit
+00000e30: 6f72 7929 0a20 2020 202d 205b f09f 9490  ory).    - [....
+00000e40: 204f 7065 6e41 4920 4150 495d 2823 2d6f   OpenAI API](#-o
+00000e50: 7065 6e61 692d 6170 6929 0a20 202d 205b  penai-api).  - [
+00000e60: f09f 93a6 2049 6e73 7461 6c6c 6174 696f  .... Installatio
+00000e70: 6e5d 2823 2d69 6e73 7461 6c6c 6174 696f  n](#-installatio
+00000e80: 6e29 0a20 202d 205b f09f 8eae 2055 7369  n).  - [.... Usi
+00000e90: 6e67 202a 5245 4144 4d45 2d41 492a 5d28  ng *README-AI*](
+00000ea0: 232d 7573 696e 672d 7265 6164 6d65 2d61  #-using-readme-a
+00000eb0: 6929 0a20 202d 205b f09f a7aa 2052 756e  i).  - [.... Run
+00000ec0: 6e69 6e67 2054 6573 7473 5d28 232d 7275  ning Tests](#-ru
+00000ed0: 6e6e 696e 672d 7465 7374 7329 0a2d 205b  nning-tests).- [
+00000ee0: f09f 9ba0 2046 7574 7572 6520 4465 7665  .... Future Deve
+00000ef0: 6c6f 706d 656e 745d 2823 2d66 7574 7572  lopment](#-futur
+00000f00: 652d 6465 7665 6c6f 706d 656e 7429 0a2d  e-development).-
+00000f10: 205b f09f 9392 2043 6861 6e67 656c 6f67   [.... Changelog
+00000f20: 5d28 232d 6368 616e 6765 6c6f 6729 0a2d  ](#-changelog).-
+00000f30: 205b f09f a49d 2043 6f6e 7472 6962 7574   [.... Contribut
+00000f40: 696e 675d 2823 2d63 6f6e 7472 6962 7574  ing](#-contribut
+00000f50: 696e 6729 0a2d 205b f09f 9384 204c 6963  ing).- [.... Lic
+00000f60: 656e 7365 5d28 232d 6c69 6365 6e73 6529  ense](#-license)
+00000f70: 0a2d 205b f09f 918f 2041 636b 6e6f 776c  .- [.... Acknowl
+00000f80: 6564 676d 656e 7473 5d28 232d 6163 6b6e  edgments](#-ackn
+00000f90: 6f77 6c65 6467 6d65 6e74 7329 0a0a 2d2d  owledgments)..--
+00000fa0: 2d0a 0a23 2320 f09f 938d 204f 7665 7276  -..## .... Overv
+00000fb0: 6965 770a 0a2a 5245 4144 4d45 2d41 492a  iew..*README-AI*
+00000fc0: 2069 7320 6120 706f 7765 7266 756c 2c20   is a powerful, 
+00000fd0: 7573 6572 2d66 7269 656e 646c 7920 636f  user-friendly co
+00000fe0: 6d6d 616e 642d 6c69 6e65 2074 6f6f 6c20  mmand-line tool 
+00000ff0: 7468 6174 2067 656e 6572 6174 6573 2065  that generates e
+00001000: 7874 656e 7369 7665 2052 4541 444d 4520  xtensive README 
+00001010: 6d61 726b 646f 776e 2064 6f63 756d 656e  markdown documen
+00001020: 7473 2066 6f72 2079 6f75 7220 736f 6674  ts for your soft
+00001030: 7761 7265 2061 6e64 2064 6174 6120 7072  ware and data pr
+00001040: 6f6a 6563 7473 2e20 4279 2070 726f 7669  ojects. By provi
+00001050: 6469 6e67 2061 2072 656d 6f74 6520 7265  ding a remote re
+00001060: 706f 7369 746f 7279 2055 524c 206f 7220  pository URL or 
+00001070: 7061 7468 2074 6f20 796f 7572 2063 6f64  path to your cod
+00001080: 6562 6173 652c 2074 6869 7320 746f 6f6c  ebase, this tool
+00001090: 2067 656e 6572 6174 6573 2064 6f63 756d   generates docum
+000010a0: 656e 7461 7469 6f6e 2066 6f72 2079 6f75  entation for you
+000010b0: 7220 656e 7469 7265 2070 726f 6a65 6374  r entire project
+000010c0: 2c20 6c65 7665 7261 6769 6e67 2074 6865  , leveraging the
+000010d0: 2063 6170 6162 696c 6974 6965 7320 6f66   capabilities of
+000010e0: 206c 6172 6765 206c 616e 6775 6167 6520   large language 
+000010f0: 6d6f 6465 6c73 2061 6e64 204f 7065 6e41  models and OpenA
+00001100: 4927 7320 4750 5420 4150 4973 2e0a 0a23  I's GPT APIs...#
+00001110: 2323 2320 f09f 8eaf 202a 4d6f 7469 7661  ### .... *Motiva
+00001120: 7469 6f6e 2a0a 0a53 696d 706c 6966 6965  tion*..Simplifie
+00001130: 7320 7468 6520 7072 6f63 6573 7320 6f66  s the process of
+00001140: 2077 7269 7469 6e67 2061 6e64 206d 6169   writing and mai
+00001150: 6e74 6169 6e69 6e67 2068 6967 682d 7175  ntaining high-qu
+00001160: 616c 6974 7920 7072 6f6a 6563 7420 646f  ality project do
+00001170: 6375 6d65 6e74 6174 696f 6e2e 204d 7920  cumentation. My 
+00001180: 6169 6d20 666f 7220 7468 6973 2070 726f  aim for this pro
+00001190: 6a65 6374 2069 7320 746f 2070 726f 7669  ject is to provi
+000011a0: 6465 2061 6c6c 2073 6b69 6c6c 206c 6576  de all skill lev
+000011b0: 656c 7320 6120 746f 6f6c 2074 6861 7420  els a tool that 
+000011c0: 696d 7072 6f76 6573 2074 6865 6972 2074  improves their t
+000011d0: 6563 686e 6963 616c 2077 6f72 6b66 6c6f  echnical workflo
+000011e0: 772c 2069 6e20 616e 2065 6666 6963 6965  w, in an efficie
+000011f0: 6e74 2061 6e64 2075 7365 722d 6672 6965  nt and user-frie
+00001200: 6e64 6c79 206d 616e 6e65 722e 2055 6c74  ndly manner. Ult
+00001210: 696d 6174 656c 792c 2074 6865 2067 6f61  imately, the goa
+00001220: 6c20 6f66 202a 5245 4144 4d45 2d41 492a  l of *README-AI*
+00001230: 2069 7320 746f 2069 6d70 726f 7665 2074   is to improve t
+00001240: 6865 2061 646f 7074 696f 6e20 616e 6420  he adoption and 
+00001250: 7573 6162 696c 6974 7920 6f66 206f 7065  usability of ope
+00001260: 6e2d 736f 7572 6365 2070 726f 6a65 6374  n-source project
+00001270: 732c 2065 6e61 626c 696e 6720 6576 6572  s, enabling ever
+00001280: 796f 6e65 2074 6f20 6265 7474 6572 2075  yone to better u
+00001290: 6e64 6572 7374 616e 6420 616e 6420 7573  nderstand and us
+000012a0: 6520 6f70 656e 2d73 6f75 7263 6520 746f  e open-source to
+000012b0: 6f6c 732e 0a23 2323 2320 e29a a0ef b88f  ols..#### ......
+000012c0: 202a 4469 7363 6c61 696d 6572 2a0a 0a2a   *Disclaimer*..*
+000012d0: 5245 4144 4d45 2d41 492a 2069 7320 6375  README-AI* is cu
+000012e0: 7272 656e 746c 7920 756e 6465 7220 6465  rrently under de
+000012f0: 7665 6c6f 706d 656e 7420 616e 6420 6861  velopment and ha
+00001300: 7320 616e 206f 7069 6e69 6f6e 6174 6564  s an opinionated
+00001310: 2063 6f6e 6669 6775 7261 7469 6f6e 2061   configuration a
+00001320: 6e64 2073 6574 7570 2e20 5768 696c 6520  nd setup. While 
+00001330: 7468 6973 2074 6f6f 6c20 7072 6f76 6964  this tool provid
+00001340: 6573 2061 6e20 6578 6365 6c6c 656e 7420  es an excellent 
+00001350: 7374 6172 7469 6e67 2070 6f69 6e74 2066  starting point f
+00001360: 6f72 2064 6f63 756d 656e 7461 7469 6f6e  or documentation
+00001370: 2c20 6974 7320 696d 706f 7274 616e 7420  , its important 
+00001380: 746f 2072 6576 6965 7720 616c 6c20 7465  to review all te
+00001390: 7874 2067 656e 6572 6174 6564 2062 7920  xt generated by 
+000013a0: 7468 6520 4f70 656e 4149 2041 5049 2074  the OpenAI API t
+000013b0: 6f20 656e 7375 7265 2069 7420 6163 6375  o ensure it accu
+000013c0: 7261 7465 6c79 2072 6570 7265 7365 6e74  rately represent
+000013d0: 7320 796f 7572 2063 6f64 6562 6173 652e  s your codebase.
+000013e0: 2045 6e73 7572 6520 616c 6c20 636f 6e74   Ensure all cont
+000013f0: 656e 7420 696e 2079 6f75 7220 7265 706f  ent in your repo
+00001400: 7369 746f 7279 2069 7320 6672 6565 206f  sitory is free o
+00001410: 6620 7365 6e73 6974 6976 6520 696e 666f  f sensitive info
+00001420: 726d 6174 696f 6e20 6265 666f 7265 2065  rmation before e
+00001430: 7865 6375 7469 6e67 2e0a 0a41 6464 6974  xecuting...Addit
+00001440: 696f 6e61 6c6c 792c 2066 7265 7175 656e  ionally, frequen
+00001450: 746c 7920 6d6f 6e69 746f 7220 796f 7572  tly monitor your
+00001460: 2041 5049 2075 7361 6765 2061 6e64 2063   API usage and c
+00001470: 6f73 7473 2062 7920 7669 7369 7469 6e67  osts by visiting
+00001480: 2074 6865 205b 4f70 656e 4149 2041 5049   the [OpenAI API
+00001490: 2055 7361 6765 2044 6173 6862 6f61 7264   Usage Dashboard
+000014a0: 5d28 6874 7470 733a 2f2f 706c 6174 666f  ](https://platfo
+000014b0: 726d 2e6f 7065 6e61 692e 636f 6d2f 6163  rm.openai.com/ac
+000014c0: 636f 756e 742f 7573 6167 6529 2e0a 0a2d  count/usage)...-
+000014d0: 2d2d 0a0a 2323 20f0 9f91 be20 4465 6d6f  --..## .... Demo
+000014e0: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+000014f0: 3a2f 2f79 6f75 7475 2e62 652f 706c 2d56  ://youtu.be/pl-V
+00001500: 6356 6647 6262 6b22 3e0a 2020 2020 3c69  cVfGbbk">.    <i
+00001510: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00001520: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00001530: 6e74 656e 742e 636f 6d2f 656c 6936 3473  ntent.com/eli64s
+00001540: 2f72 6561 646d 652d 6169 2f66 3063 3561  /readme-ai/f0c5a
+00001550: 3033 3866 3633 6165 3034 6232 6434 3435  038f63ae04b2d445
+00001560: 3239 3734 3637 3661 3932 6462 3432 6265  2974676a92db42be
+00001570: 3863 652f 6578 616d 706c 6573 2f69 6d67  8ce/examples/img
+00001580: 732f 6465 6d6f 2e70 6e67 2220 616c 743d  s/demo.png" alt=
+00001590: 2264 656d 6f20 7669 6465 6f22 3e0a 3c2f  "demo video">.</
+000015a0: 613e 0a0a 2d2d 2d0a 0a23 2320 e29a 99ef  a>..---..## ....
+000015b0: b88f 2046 6561 7475 7265 730a 0a3c 6831  .. Features..<h1
+000015c0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+000015d0: 312e 3c62 723e f09f 9187 3c62 723e 3c62  1.<br>....<br><b
+000015e0: 723e f09f 9391 2043 6f64 6562 6173 6520  r>.... Codebase 
+000015f0: 446f 6375 6d65 6e74 6174 696f 6e3c 2f68  Documentation</h
+00001600: 313e 0a3c 7461 626c 653e 0a20 2020 203c  1>.<table>.    <
+00001610: 7472 3e0a 2020 2020 2020 2020 3c74 643e  tr>.        <td>
+00001620: 0a20 2020 2020 2020 2020 2020 203c 6833  .            <h3
+00001630: 3ee2 97a6 2052 6570 6f73 6974 6f72 7920  >... Repository 
+00001640: 4669 6c65 2053 756d 6d61 7269 6573 3c2f  File Summaries</
+00001650: 6833 3e0a 2020 2020 2020 2020 2020 2020  h3>.            
+00001660: 3c75 6c3e 0a20 2020 2020 2020 2020 2020  <ul>.           
+00001670: 2020 2020 203c 6c69 3e43 6f64 6520 7375       <li>Code su
+00001680: 6d6d 6172 6965 7320 6172 6520 6765 6e65  mmaries are gene
+00001690: 7261 7465 6420 666f 7220 6561 6368 2066  rated for each f
+000016a0: 696c 6520 7669 6120 4f70 656e 4149 2773  ile via OpenAI's
+000016b0: 203c 693e 6770 742d 332e 352d 7475 7262   <i>gpt-3.5-turb
+000016c0: 6f3c 2f69 3e20 656e 6769 6e65 2e3c 2f6c  o</i> engine.</l
+000016d0: 693e 0a20 2020 2020 2020 2020 2020 2020  i>.             
+000016e0: 2020 203c 6c69 3e54 6865 2046 696c 6520     <li>The File 
+000016f0: 636f 6c75 6d6e 2069 6e20 7468 6520 6d61  column in the ma
+00001700: 726b 646f 776e 2074 6162 6c65 2063 6f6e  rkdown table con
+00001710: 7461 696e 7320 6120 6c69 6e6b 2074 6f20  tains a link to 
+00001720: 7468 6520 6669 6c65 206f 6e20 4769 7448  the file on GitH
+00001730: 7562 2e3c 2f6c 693e 0a20 2020 2020 2020  ub.</li>.       
+00001740: 2020 2020 203c 2f75 6c3e 0a20 2020 2020       </ul>.     
+00001750: 2020 203c 2f74 643e 0a20 2020 203c 2f74     </td>.    </t
+00001760: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
+00001770: 2020 2020 3c74 643e 0a20 2020 2020 2020      <td>.       
+00001780: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
+00001790: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+000017a0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+000017b0: 2f65 6c69 3634 732f 7265 6164 6d65 2d61  /eli64s/readme-a
+000017c0: 692f 6d61 696e 2f65 7861 6d70 6c65 732f  i/main/examples/
+000017d0: 696d 6773 2f6d 6f64 756c 6573 2e70 6e67  imgs/modules.png
+000017e0: 2220 616c 743d 2264 6f63 7322 3e0a 2020  " alt="docs">.  
+000017f0: 2020 2020 2020 3c2f 7464 3e0a 2020 2020        </td>.    
+00001800: 3c2f 7472 3e0a 3c2f 7461 626c 653e 0a0a  </tr>.</table>..
+00001810: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+00001820: 7222 3ee2 9289 3c62 723e f09f 9187 3c62  r">...<br>....<b
+00001830: 723e 3c62 723e f09f 8e96 2042 6164 6765  r><br>.... Badge
+00001840: 733c 2f68 313e 0a3c 7461 626c 653e 0a20  s</h1>.<table>. 
+00001850: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
+00001860: 3c74 643e 0a20 2020 2020 2020 2020 2020  <td>.           
+00001870: 203c 6833 3ee2 97a6 2049 6e74 726f 6475   <h3>... Introdu
+00001880: 6374 696f 6e2c 2042 6164 6765 732c 2026  ction, Badges, &
+00001890: 2054 6162 6c65 206f 6620 436f 6e74 656e   Table of Conten
+000018a0: 7473 3c2f 6833 3e0a 2020 2020 2020 2020  ts</h3>.        
+000018b0: 2020 2020 3c75 6c3e 0a20 2020 2020 2020      <ul>.       
+000018c0: 2020 2020 2020 2020 203c 6c69 3e54 6865           <li>The
+000018d0: 204f 7065 6e41 4920 4150 4920 6973 2070   OpenAI API is p
+000018e0: 726f 6d70 7465 6420 746f 2063 7265 6174  rompted to creat
+000018f0: 6520 6120 312d 7365 6e74 656e 6365 2070  e a 1-sentence p
+00001900: 6872 6173 6520 6465 7363 7269 6269 6e67  hrase describing
+00001910: 2079 6f75 7220 7072 6f6a 6563 742e 3c2f   your project.</
+00001920: 6c69 3e0a 2020 2020 2020 2020 2020 2020  li>.            
+00001930: 2020 2020 3c6c 693e 5072 6f6a 6563 7420      <li>Project 
+00001940: 6465 7065 6e64 656e 6369 6573 2061 6e64  dependencies and
+00001950: 206d 6574 6164 6174 6120 6172 6520 7669   metadata are vi
+00001960: 7375 616c 697a 6564 2075 7369 6e67 203c  sualized using <
+00001970: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001980: 7368 6965 6c64 732e 696f 2f22 3e53 6869  shields.io/">Shi
+00001990: 656c 6473 2e69 6f3c 2f61 3e20 6261 6467  elds.io</a> badg
+000019a0: 6573 2e3c 2f6c 693e 0a20 2020 2020 2020  es.</li>.       
+000019b0: 2020 2020 2020 2020 203c 6c69 3e42 6164           <li>Bad
+000019c0: 6765 7320 6172 6520 736f 7274 6564 2062  ges are sorted b
+000019d0: 7920 6865 7820 636f 6465 2c20 6469 7370  y hex code, disp
+000019e0: 6c61 7965 6420 6672 6f6d 206c 6967 6874  layed from light
+000019f0: 2074 6f20 6461 726b 2068 7565 732e 3c2f   to dark hues.</
+00001a00: 6c69 3e0a 2020 2020 2020 2020 2020 2020  li>.            
+00001a10: 3c2f 756c 3e0a 2020 2020 2020 2020 3c2f  </ul>.        </
+00001a20: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+00001a30: 2020 3c74 723e 0a20 2020 2020 2020 203c    <tr>.        <
+00001a40: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
+00001a50: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00001a60: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00001a70: 636f 6e74 656e 742e 636f 6d2f 656c 6936  content.com/eli6
+00001a80: 3473 2f72 6561 646d 652d 6169 2f6d 6169  4s/readme-ai/mai
+00001a90: 6e2f 6578 616d 706c 6573 2f69 6d67 732f  n/examples/imgs/
+00001aa0: 6865 6164 6572 2e70 6e67 2220 616c 743d  header.png" alt=
+00001ab0: 2264 6f63 7322 3e0a 2020 2020 2020 2020  "docs">.        
+00001ac0: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+00001ad0: 3c2f 7461 626c 653e 0a0a 3c68 3120 616c  </table>..<h1 al
+00001ae0: 6967 6e3d 2263 656e 7465 7222 3ee2 928a  ign="center">...
+00001af0: 3c62 723e f09f 9187 3c62 723e 3c62 723e  <br>....<br><br>
+00001b00: f09f a79a 2050 726f 6d70 7465 6420 5465  .... Prompted Te
+00001b10: 7874 2047 656e 6572 6174 696f 6e3c 2f68  xt Generation</h
+00001b20: 313e 0a3c 7461 626c 653e 0a20 2020 203c  1>.<table>.    <
+00001b30: 7472 3e0a 2020 2020 2020 2020 3c74 643e  tr>.        <td>
+00001b40: 0a20 2020 2020 2020 2020 2020 203c 6833  .            <h3
+00001b50: 3ee2 97a6 2046 6561 7475 7265 7320 5461  >... Features Ta
+00001b60: 626c 6520 2620 4f76 6572 7669 6577 3c2f  ble & Overview</
+00001b70: 6833 3e0a 2020 2020 2020 2020 2020 2020  h3>.            
+00001b80: 3c75 6c3e 0a20 2020 2020 2020 2020 2020  <ul>.           
+00001b90: 2020 2020 203c 6c69 3e44 6574 6169 6c65       <li>Detaile
+00001ba0: 6420 7072 6f6d 7074 7320 6172 6520 656d  d prompts are em
+00001bb0: 6265 6464 6564 2077 6974 6820 7265 706f  bedded with repo
+00001bc0: 7369 746f 7279 206d 6574 6164 6174 6120  sitory metadata 
+00001bd0: 616e 6420 7061 7373 6564 2074 6f20 7468  and passed to th
+00001be0: 6520 4f70 656e 4149 2041 5049 2e3c 2f6c  e OpenAI API.</l
+00001bf0: 693e 0a20 2020 2020 2020 2020 2020 2020  i>.             
+00001c00: 2020 203c 756c 3e0a 2020 2020 2020 2020     <ul>.        
+00001c10: 2020 2020 2020 2020 2020 2020 3c6c 693e              <li>
+00001c20: 3c65 6d3e 4665 6174 7572 6573 3c2f 656d  <em>Features</em
+00001c30: 3e20 7461 626c 6520 6869 6768 6c69 6768  > table highligh
+00001c40: 7473 2076 6172 696f 7573 2074 6563 686e  ts various techn
+00001c50: 6963 616c 2061 7474 7269 6275 7465 7320  ical attributes 
+00001c60: 6f66 2079 6f75 7220 636f 6465 6261 7365  of your codebase
+00001c70: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001c80: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
+00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ca0: 3c6c 693e 3c65 6d3e 4f76 6572 7669 6577  <li><em>Overview
+00001cb0: 3c2f 656d 3e20 7365 6374 696f 6e20 6465  </em> section de
+00001cc0: 7363 7269 6265 7320 796f 7572 2070 726f  scribes your pro
+00001cd0: 6a65 6374 2773 2075 7365 2063 6173 6520  ject's use case 
+00001ce0: 616e 6420 6170 706c 6963 6174 696f 6e73  and applications
+00001cf0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001d00: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
+00001d10: 2020 2020 2020 2020 2020 2020 3c2f 756c              </ul
+00001d20: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00001d30: 756c 3e0a 2020 2020 2020 2020 3c2f 7464  ul>.        </td
+00001d40: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
+00001d50: 3c74 723e 0a20 2020 2020 2020 203c 7464  <tr>.        <td
+00001d60: 3e0a 2020 2020 2020 2020 2020 2020 3c69  >.            <i
+00001d70: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00001d80: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00001d90: 6e74 656e 742e 636f 6d2f 656c 6936 3473  ntent.com/eli64s
+00001da0: 2f72 6561 646d 652d 6169 2f6d 6169 6e2f  /readme-ai/main/
+00001db0: 6578 616d 706c 6573 2f69 6d67 732f 6665  examples/imgs/fe
+00001dc0: 6174 7572 6573 2e70 6e67 2220 616c 743d  atures.png" alt=
+00001dd0: 2266 6561 7475 7265 7322 3e0a 2020 2020  "features">.    
+00001de0: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00001df0: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+00001e00: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00001e10: 636f 6d2f 656c 6936 3473 2f72 6561 646d  com/eli64s/readm
+00001e20: 652d 6169 2f6d 6169 6e2f 6578 616d 706c  e-ai/main/exampl
+00001e30: 6573 2f69 6d67 732f 6f76 6572 7669 6577  es/imgs/overview
+00001e40: 2e70 6e67 2220 616c 743d 226f 7665 7276  .png" alt="overv
+00001e50: 6965 7722 3e0a 2020 2020 2020 2020 3c2f  iew">.        </
+00001e60: 7464 3e0a 2020 2020 3c2f 7472 3e0a 3c2f  td>.    </tr>.</
+00001e70: 7461 626c 653e 0a0a 3c68 3120 616c 6967  table>..<h1 alig
+00001e80: 6e3d 2263 656e 7465 7222 3ee2 928b 3c62  n="center">...<b
+00001e90: 723e f09f 9187 3c62 723e 3c62 723e f09f  r>....<br><br>..
+00001ea0: 8cb2 2052 6570 6f73 6974 6f72 7920 5472  .. Repository Tr
+00001eb0: 6565 3c2f 6831 3e0a 3c74 6162 6c65 3e0a  ee</h1>.<table>.
+00001ec0: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+00001ed0: 203c 7464 3e0a 2020 2020 2020 2020 2020   <td>.          
+00001ee0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00001ef0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001f00: 6572 636f 6e74 656e 742e 636f 6d2f 656c  ercontent.com/el
+00001f10: 6936 3473 2f72 6561 646d 652d 6169 2f6d  i64s/readme-ai/m
+00001f20: 6169 6e2f 6578 616d 706c 6573 2f69 6d67  ain/examples/img
+00001f30: 732f 7472 6565 2e70 6e67 2220 616c 743d  s/tree.png" alt=
+00001f40: 2274 7265 6522 3e0a 2020 2020 2020 2020  "tree">.        
+00001f50: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+00001f60: 3c2f 7461 626c 653e 0a0a 3c68 3120 616c  </table>..<h1 al
+00001f70: 6967 6e3d 2263 656e 7465 7222 3ee2 928c  ign="center">...
+00001f80: 3c62 723e f09f 9187 3c62 723e 3c62 723e  <br>....<br><br>
+00001f90: f09f 93a6 2044 796e 616d 6963 2055 7365  .... Dynamic Use
+00001fa0: 7220 5365 7475 7020 4775 6964 6573 3c2f  r Setup Guides</
+00001fb0: 6831 3e0a 3c74 6162 6c65 3e0a 2020 2020  h1>.<table>.    
+00001fc0: 3c74 723e 0a20 2020 2020 2020 203c 7464  <tr>.        <td
+00001fd0: 3e0a 2020 2020 2020 2020 2020 2020 3c68  >.            <h
+00001fe0: 333e 3c62 3ee2 97a6 2049 6e73 7461 6c6c  3><b>... Install
+00001ff0: 6174 696f 6e2c 2055 7361 6765 2c20 2620  ation, Usage, & 
+00002000: 5465 7374 696e 673c 2f62 3e3c 2f68 333e  Testing</b></h3>
+00002010: 0a20 2020 2020 2020 2020 2020 203c 756c  .            <ul
+00002020: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002030: 2020 3c6c 693e 4765 6e65 7261 7465 7320    <li>Generates 
+00002040: 696e 7374 7275 6374 696f 6e73 2066 6f72  instructions for
+00002050: 2069 6e73 7461 6c6c 696e 672c 2075 7369   installing, usi
+00002060: 6e67 2c20 616e 6420 7465 7374 696e 6720  ng, and testing 
+00002070: 796f 7572 2063 6f64 6562 6173 652e 3c2f  your codebase.</
+00002080: 6c69 3e0a 2020 2020 2020 2020 2020 2020  li>.            
+00002090: 2020 2020 3c6c 693e 5245 4144 4d45 2d41      <li>README-A
+000020a0: 4920 6375 7272 656e 746c 7920 7375 7070  I currently supp
+000020b0: 6f72 7473 2074 6869 7320 6665 6174 7572  orts this featur
+000020c0: 6520 666f 7220 636f 6465 2077 7269 7474  e for code writt
+000020d0: 656e 2077 6974 683a 3c2f 6c69 3e0a 2020  en with:</li>.  
+000020e0: 2020 2020 2020 2020 2020 2020 2020 3c75                <u
+000020f0: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
+00002100: 2020 2020 2020 203c 6c69 3e0a 2020 2020         <li>.    
+00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002120: 2020 2020 3c69 3e50 7974 686f 6e2c 2052      <i>Python, R
+00002130: 7573 742c 2047 6f2c 2043 2c20 4b6f 746c  ust, Go, C, Kotl
+00002140: 696e 2c20 4a61 7661 2c20 4a61 7661 5363  in, Java, JavaSc
+00002150: 7269 7074 2c20 5479 7065 5363 7269 7074  ript, TypeScript
+00002160: 2e3c 2f69 3e0a 2020 2020 2020 2020 2020  .</i>.          
+00002170: 2020 2020 2020 2020 2020 3c2f 6c69 3e0a            </li>.
+00002180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002190: 3c2f 756c 3e0a 2020 2020 2020 2020 2020  </ul>.          
+000021a0: 2020 3c2f 756c 3e0a 2020 2020 2020 2020    </ul>.        
+000021b0: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+000021c0: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+000021d0: 203c 7464 3e0a 2020 2020 2020 2020 2020   <td>.          
+000021e0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+000021f0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00002200: 6572 636f 6e74 656e 742e 636f 6d2f 656c  ercontent.com/el
+00002210: 6936 3473 2f72 6561 646d 652d 6169 2f6d  i64s/readme-ai/m
+00002220: 6169 6e2f 6578 616d 706c 6573 2f69 6d67  ain/examples/img
+00002230: 732f 6765 7474 696e 675f 7374 6172 7465  s/getting_starte
+00002240: 642e 706e 6722 2061 6c74 3d22 6765 7474  d.png" alt="gett
+00002250: 696e 675f 7374 6172 7465 6422 3e0a 2020  ing_started">.  
+00002260: 2020 2020 2020 3c2f 7464 3e0a 2020 2020        </td>.    
+00002270: 3c2f 7472 3e0a 3c2f 7461 626c 653e 0a0a  </tr>.</table>..
+00002280: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+00002290: 7222 3ee2 928d 3c62 723e f09f 9187 3c62  r">...<br>....<b
+000022a0: 723e 3c62 723e f09f 91a9 e280 8df0 9f92  r><br>..........
+000022b0: bb43 6f6e 7472 6962 7574 696e 6720 4775  .Contributing Gu
+000022c0: 6964 656c 696e 6573 2026 206d 6f72 6521  idelines & more!
+000022d0: 3c2f 6831 3e0a 0a7c 207c 0a7c 2d2d 2d2d  </h1>..| |.|----
+000022e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000022f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2021  -----------|.| !
+00002310: 5b63 6f6e 7472 6962 7574 655d 2868 7474  [contribute](htt
+00002320: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00002330: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f65  sercontent.com/e
+00002340: 6c69 3634 732f 7265 6164 6d65 2d61 692f  li64s/readme-ai/
+00002350: 6d61 696e 2f65 7861 6d70 6c65 732f 696d  main/examples/im
+00002360: 6773 2f63 6c6f 7369 6e67 2e70 6e67 2920  gs/closing.png) 
+00002370: 7c0a 0a3c 6831 2061 6c69 676e 3d22 6365  |..<h1 align="ce
+00002380: 6e74 6572 223e e292 8e3c 6272 3ef0 9f91  nter">...<br>...
+00002390: 873c 6272 3e3c 6272 3ef0 9f92 a520 4578  .<br><br>.... Ex
+000023a0: 616d 706c 6520 4669 6c65 733c 2f68 313e  ample Files</h1>
+000023b0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+000023c0: 7222 3e4d 6172 6b64 6f77 6e20 6578 616d  r">Markdown exam
+000023d0: 706c 6520 6669 6c65 7320 6765 6e65 7261  ple files genera
+000023e0: 7465 6420 6279 2074 6865 2052 4541 444d  ted by the READM
+000023f0: 452d 4149 2061 7070 213c 2f70 3e0a 3c64  E-AI app!</p>.<d
+00002400: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
+00002410: 223e 0a20 2020 203c 7461 626c 6520 616c  ">.    <table al
+00002420: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00002430: 2020 2020 2020 3c74 723e 0a20 2020 2020        <tr>.     
+00002440: 2020 2020 2020 203c 7468 3e3c 2f74 683e         <th></th>
+00002450: 0a20 2020 2020 2020 2020 2020 203c 7468  .            <th
+00002460: 3e45 7861 6d70 6c65 2046 696c 653c 2f74  >Example File</t
+00002470: 683e 0a20 2020 2020 2020 2020 2020 203c  h>.            <
+00002480: 7468 3e52 6570 6f73 6974 6f72 793c 2f74  th>Repository</t
+00002490: 683e 0a20 2020 2020 2020 2020 2020 203c  h>.            <
+000024a0: 7468 3e4c 616e 6775 6167 653c 2f74 683e  th>Language</th>
+000024b0: 0a20 2020 2020 2020 2020 2020 203c 7468  .            <th
+000024c0: 3e42 7974 6573 3c2f 7468 3e0a 2020 2020  >Bytes</th>.    
+000024d0: 2020 2020 3c2f 7472 3e0a 2020 2020 2020      </tr>.      
+000024e0: 2020 3c74 723e 0a20 2020 2020 2020 2020    <tr>.         
+000024f0: 2020 203c 7464 3e31 efb8 8fe2 83a3 3c2f     <td>1......</
+00002500: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
+00002510: 3c74 643e 3c61 2068 7265 663d 2268 7474  <td><a href="htt
+00002520: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002530: 656c 6936 3473 2f72 6561 646d 652d 6169  eli64s/readme-ai
+00002540: 2f62 6c6f 622f 6d61 696e 2f65 7861 6d70  /blob/main/examp
+00002550: 6c65 732f 7265 6164 6d65 2d70 7974 686f  les/readme-pytho
+00002560: 6e2e 6d64 223e 7265 6164 6d65 2d70 7974  n.md">readme-pyt
+00002570: 686f 6e2e 6d64 3c2f 613e 3c2f 7464 3e0a  hon.md</a></td>.
+00002580: 2020 2020 2020 2020 2020 2020 3c74 643e              <td>
+00002590: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000025a0: 2f67 6974 6875 622e 636f 6d2f 656c 6936  /github.com/eli6
+000025b0: 3473 2f72 6561 646d 652d 6169 223e 7265  4s/readme-ai">re
+000025c0: 6164 6d65 2d61 693c 2f61 3e3c 2f74 643e  adme-ai</a></td>
+000025d0: 0a20 2020 2020 2020 2020 2020 203c 7464  .            <td
+000025e0: 3e50 7974 686f 6e3c 2f74 643e 0a20 2020  >Python</td>.   
+000025f0: 2020 2020 2020 2020 203c 7464 3e0a 2020           <td>.  
+00002600: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00002610: 3e31 392c 3833 393c 2f70 3e0a 2020 2020  >19,839</p>.    
+00002620: 2020 2020 3c2f 7472 3e0a 2020 2020 2020      </tr>.      
+00002630: 2020 3c74 643e 32ef b88f e283 a33c 2f74    <td>2......</t
+00002640: 643e 0a20 2020 2020 2020 203c 7464 3e3c  d>.        <td><
+00002650: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00002660: 6769 7468 7562 2e63 6f6d 2f65 6c69 3634  github.com/eli64
+00002670: 732f 7265 6164 6d65 2d61 692f 626c 6f62  s/readme-ai/blob
+00002680: 2f6d 6169 6e2f 6578 616d 706c 6573 2f72  /main/examples/r
+00002690: 6561 646d 652d 7479 7065 7363 7269 7074  eadme-typescript
+000026a0: 2e6d 6422 3e72 6561 646d 652d 7479 7065  .md">readme-type
+000026b0: 7363 7269 7074 2e6d 643c 2f61 3e3c 2f74  script.md</a></t
+000026c0: 643e 0a20 2020 2020 2020 203c 7464 3e3c  d>.        <td><
+000026d0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000026e0: 6769 7468 7562 2e63 6f6d 2f59 7562 6572  github.com/Yuber
+000026f0: 6c65 792f 4368 6174 4750 542d 4170 702d  ley/ChatGPT-App-
+00002700: 5265 6163 742d 4e61 7469 7665 2d54 7970  React-Native-Typ
+00002710: 6553 6372 6970 7422 3e63 6861 7467 7074  eScript">chatgpt
+00002720: 2d61 7070 2d72 6561 6374 2d74 7970 6573  -app-react-types
+00002730: 6372 6970 743c 2f61 3e3c 2f74 643e 0a20  cript</a></td>. 
+00002740: 2020 2020 2020 203c 7464 3e54 7970 6553         <td>TypeS
+00002750: 6372 6970 742c 2052 6561 6374 3c2f 7464  cript, React</td
+00002760: 3e0a 2020 2020 2020 2020 3c74 643e 0a20  >.        <td>. 
+00002770: 2020 2020 2020 2020 2020 203c 703e 3938             <p>98
+00002780: 383c 2f70 3e0a 2020 2020 2020 2020 2020  8</p>.          
+00002790: 2020 3c2f 7472 3e0a 2020 2020 2020 2020    </tr>.        
+000027a0: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+000027b0: 2020 2020 2020 2020 203c 7464 3e33 efb8           <td>3..
+000027c0: 8fe2 83a3 3c2f 7464 3e0a 2020 2020 2020  ....</td>.      
+000027d0: 2020 2020 2020 2020 2020 3c74 643e 3c61            <td><a
+000027e0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000027f0: 6974 6875 622e 636f 6d2f 656c 6936 3473  ithub.com/eli64s
+00002800: 2f72 6561 646d 652d 6169 2f62 6c6f 622f  /readme-ai/blob/
+00002810: 6d61 696e 2f65 7861 6d70 6c65 732f 7265  main/examples/re
+00002820: 6164 6d65 2d6a 6176 6173 6372 6970 742e  adme-javascript.
+00002830: 6d64 223e 7265 6164 6d65 2d6a 6176 6173  md">readme-javas
+00002840: 6372 6970 742e 6d64 3c2f 613e 3c2f 7464  cript.md</a></td
+00002850: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002860: 2020 3c74 643e 3c61 2068 7265 663d 2268    <td><a href="h
+00002870: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002880: 6d2f 6964 6f73 616c 2f61 7373 6973 7461  m/idosal/assista
+00002890: 6e74 2d63 6861 742d 6770 7422 3e61 7373  nt-chat-gpt">ass
+000028a0: 6973 7461 6e74 2d63 6861 742d 6770 742d  istant-chat-gpt-
+000028b0: 6a61 7661 7363 7269 7074 3c2f 613e 3c2f  javascript</a></
+000028c0: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
+000028d0: 2020 2020 3c74 643e 4a61 7661 5363 7269      <td>JavaScri
+000028e0: 7074 2c20 5265 6163 743c 2f74 643e 0a20  pt, React</td>. 
+000028f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002900: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
+00002910: 2020 2020 2020 2020 3c70 3e32 3132 3c2f          <p>212</
+00002920: 703e 0a20 2020 2020 2020 2020 2020 203c  p>.            <
+00002930: 2f74 723e 0a20 2020 2020 2020 2020 2020  /tr>.           
+00002940: 203c 7472 3e0a 2020 2020 2020 2020 2020   <tr>.          
+00002950: 2020 2020 2020 3c74 643e 34ef b88f e283        <td>4.....
+00002960: a33c 2f74 643e 0a20 2020 2020 2020 2020  .</td>.         
+00002970: 2020 2020 2020 203c 7464 3e3c 6120 6872         <td><a hr
+00002980: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00002990: 7562 2e63 6f6d 2f65 6c69 3634 732f 7265  ub.com/eli64s/re
+000029a0: 6164 6d65 2d61 692f 626c 6f62 2f6d 6169  adme-ai/blob/mai
+000029b0: 6e2f 6578 616d 706c 6573 2f72 6561 646d  n/examples/readm
+000029c0: 652d 6b6f 746c 696e 2e6d 6422 3e72 6561  e-kotlin.md">rea
+000029d0: 646d 652d 6b6f 746c 696e 2e6d 643c 2f61  dme-kotlin.md</a
+000029e0: 3e3c 2f74 643e 0a20 2020 2020 2020 2020  ></td>.         
+000029f0: 2020 2020 2020 203c 7464 3e3c 6120 6872         <td><a hr
+00002a00: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00002a10: 7562 2e63 6f6d 2f72 756d 6161 6e2f 6669  ub.com/rumaan/fi
+00002a20: 6c65 2e69 6f2d 416e 6472 6f69 642d 436c  le.io-Android-Cl
+00002a30: 6965 6e74 223e 6669 6c65 2e69 6f2d 616e  ient">file.io-an
+00002a40: 6472 6f69 642d 636c 6965 6e74 3c2f 613e  droid-client</a>
+00002a50: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
+00002a60: 2020 2020 2020 3c74 643e 4b6f 746c 696e        <td>Kotlin
+00002a70: 2c20 4a61 7661 2c20 416e 6472 6f69 643c  , Java, Android<
+00002a80: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
+00002a90: 2020 2020 203c 7464 3e0a 2020 2020 2020       <td>.      
+00002aa0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00002ab0: 3e31 3133 2c36 3439 3c2f 703e 0a20 2020  >113,649</p>.   
+00002ac0: 2020 2020 2020 2020 203c 2f74 723e 0a20           </tr>. 
+00002ad0: 2020 2020 2020 2020 2020 203c 7472 3e0a             <tr>.
+00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002af0: 3c74 643e 35ef b88f e283 a33c 2f74 643e  <td>5......</td>
+00002b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b10: 203c 7464 3e3c 6120 6872 6566 3d22 6874   <td><a href="ht
+00002b20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002b30: 2f65 6c69 3634 732f 7265 6164 6d65 2d61  /eli64s/readme-a
+00002b40: 692f 626c 6f62 2f6d 6169 6e2f 6578 616d  i/blob/main/exam
+00002b50: 706c 6573 2f72 6561 646d 652d 7275 7374  ples/readme-rust
+00002b60: 2d63 2e6d 6422 3e72 6561 646d 652d 7275  -c.md">readme-ru
+00002b70: 7374 2d63 2e6d 643c 2f61 3e3c 2f74 643e  st-c.md</a></td>
+00002b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b90: 203c 7464 3e3c 6120 6872 6566 3d22 6874   <td><a href="ht
+00002ba0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002bb0: 2f44 6f77 6e57 6974 6855 702f 4361 6c6c  /DownWithUp/Call
+00002bc0: 4d6f 6e22 3e72 7573 742d 632d 6170 703c  Mon">rust-c-app<
+00002bd0: 2f61 3e3c 2f74 643e 0a20 2020 2020 2020  /a></td>.       
+00002be0: 2020 2020 2020 2020 203c 7464 3e43 2c20           <td>C, 
+00002bf0: 5275 7374 3c2f 7464 3e0a 2020 2020 2020  Rust</td>.      
+00002c00: 2020 2020 2020 2020 2020 3c74 643e 0a20            <td>. 
+00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c20: 2020 203c 703e 3732 3c2f 703e 0a20 2020     <p>72</p>.   
+00002c30: 2020 2020 2020 2020 203c 2f74 723e 0a20           </tr>. 
+00002c40: 2020 2020 2020 2020 2020 203c 7472 3e0a             <tr>.
+00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c60: 3c74 643e 36ef b88f e283 a33c 2f74 643e  <td>6......</td>
+00002c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c80: 203c 7464 3e3c 6120 6872 6566 3d22 6874   <td><a href="ht
+00002c90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002ca0: 2f65 6c69 3634 732f 7265 6164 6d65 2d61  /eli64s/readme-a
+00002cb0: 692f 626c 6f62 2f6d 6169 6e2f 6578 616d  i/blob/main/exam
+00002cc0: 706c 6573 2f72 6561 646d 652d 676f 2e6d  ples/readme-go.m
+00002cd0: 6422 3e72 6561 646d 652d 676f 2e6d 643c  d">readme-go.md<
+00002ce0: 2f61 3e3c 2f74 643e 0a20 2020 2020 2020  /a></td>.       
+00002cf0: 2020 2020 2020 2020 203c 7464 3e3c 6120           <td><a 
+00002d00: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00002d10: 7468 7562 2e63 6f6d 2f6f 6c6c 6965 6672  thub.com/olliefr
+00002d20: 2f64 6f63 6b65 722d 6773 2d70 696e 6722  /docker-gs-ping"
+00002d30: 3e67 6f2d 646f 636b 6572 2d61 7070 3c2f  >go-docker-app</
+00002d40: 613e 3c2f 7464 3e0a 2020 2020 2020 2020  a></td>.        
+00002d50: 2020 2020 2020 2020 3c74 643e 476f 3c2f          <td>Go</
+00002d60: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
+00002d70: 2020 2020 3c74 643e 0a20 2020 2020 2020      <td>.       
+00002d80: 2020 2020 2020 2020 2020 2020 203c 703e               <p>
+00002d90: 3431 3c2f 703e 0a20 2020 2020 2020 2020  41</p>.         
+00002da0: 2020 203c 2f74 723e 0a20 2020 2020 2020     </tr>.       
+00002db0: 2020 2020 203c 7472 3e0a 2020 2020 2020       <tr>.      
+00002dc0: 2020 2020 2020 2020 2020 3c74 643e 37ef            <td>7.
+00002dd0: b88f e283 a33c 2f74 643e 0a20 2020 2020  .....</td>.     
+00002de0: 2020 2020 2020 2020 2020 203c 7464 3e3c             <td><
+00002df0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00002e00: 6769 7468 7562 2e63 6f6d 2f65 6c69 3634  github.com/eli64
+00002e10: 732f 7265 6164 6d65 2d61 692f 626c 6f62  s/readme-ai/blob
+00002e20: 2f6d 6169 6e2f 6578 616d 706c 6573 2f72  /main/examples/r
+00002e30: 6561 646d 652d 6a61 7661 2e6d 6422 3e72  eadme-java.md">r
+00002e40: 6561 646d 652d 6a61 7661 2e6d 643c 2f61  eadme-java.md</a
+00002e50: 3e3c 2f74 643e 0a20 2020 2020 2020 2020  ></td>.         
+00002e60: 2020 2020 2020 203c 7464 3e3c 6120 6872         <td><a hr
+00002e70: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00002e80: 7562 2e63 6f6d 2f61 766a 696e 6465 722f  ub.com/avjinder/
+00002e90: 4d69 6e69 6d61 6c2d 546f 646f 223e 6a61  Minimal-Todo">ja
+00002ea0: 7661 2d6d 696e 696d 616c 2d74 6f64 6f3c  va-minimal-todo<
+00002eb0: 2f61 3e3c 2f74 643e 0a20 2020 2020 2020  /a></td>.       
+00002ec0: 2020 2020 2020 2020 203c 7464 3e4a 6176           <td>Jav
+00002ed0: 613c 2f74 643e 0a20 2020 2020 2020 2020  a</td>.         
+00002ee0: 2020 2020 2020 203c 7464 3e0a 2020 2020         <td>.    
+00002ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f00: 3c70 3e31 372c 3732 353c 2f70 3e0a 2020  <p>17,725</p>.  
+00002f10: 2020 2020 2020 2020 2020 3c2f 7472 3e0a            </tr>.
+00002f20: 2020 2020 2020 2020 2020 2020 3c74 723e              <tr>
+00002f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002f40: 203c 7464 3e38 efb8 8fe2 83a3 3c2f 7464   <td>8......</td
+00002f50: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002f60: 2020 3c74 643e 3c61 2068 7265 663d 2268    <td><a href="h
+00002f70: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002f80: 6d2f 656c 6936 3473 2f72 6561 646d 652d  m/eli64s/readme-
+00002f90: 6169 2f62 6c6f 622f 6d61 696e 2f65 7861  ai/blob/main/exa
+00002fa0: 6d70 6c65 732f 7265 6164 6d65 2d66 6173  mples/readme-fas
+00002fb0: 7461 7069 2d72 6564 6973 2e6d 6422 3e72  tapi-redis.md">r
+00002fc0: 6561 646d 652d 6661 7374 6170 692d 7265  eadme-fastapi-re
+00002fd0: 6469 732e 6d64 3c2f 613e 3c2f 7464 3e0a  dis.md</a></td>.
+00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ff0: 3c74 643e 3c61 2068 7265 663d 2268 7474  <td><a href="htt
+00003000: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00003010: 4665 7272 6172 6944 472f 6173 796e 632d  FerrariDG/async-
+00003020: 6d6c 2d69 6e66 6572 656e 6365 223e 6173  ml-inference">as
+00003030: 796e 632d 6d6c 2d69 6e66 6572 656e 6365  ync-ml-inference
+00003040: 3c2f 613e 3c2f 7464 3e0a 2020 2020 2020  </a></td>.      
+00003050: 2020 2020 2020 2020 2020 3c74 643e 5079            <td>Py
+00003060: 7468 6f6e 2c20 4661 7374 4150 492c 2052  thon, FastAPI, R
+00003070: 6564 6973 3c2f 7464 3e0a 2020 2020 2020  edis</td>.      
+00003080: 2020 2020 2020 2020 2020 3c74 643e 0a20            <td>. 
+00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030a0: 2020 203c 703e 3335 353c 2f70 3e0a 2020     <p>355</p>.  
+000030b0: 2020 2020 2020 2020 2020 3c2f 7472 3e0a            </tr>.
+000030c0: 2020 2020 2020 2020 2020 2020 3c74 723e              <tr>
+000030d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000030e0: 203c 7464 3e39 efb8 8fe2 83a3 3c2f 7464   <td>9......</td
+000030f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00003100: 2020 3c74 643e 3c61 2068 7265 663d 2268    <td><a href="h
+00003110: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00003120: 6d2f 656c 6936 3473 2f72 6561 646d 652d  m/eli64s/readme-
+00003130: 6169 2f62 6c6f 622f 6d61 696e 2f65 7861  ai/blob/main/exa
+00003140: 6d70 6c65 732f 7265 6164 6d65 2d6d 6c6f  mples/readme-mlo
+00003150: 7073 2e6d 6422 3e72 6561 646d 652d 6d6c  ps.md">readme-ml
+00003160: 6f70 732e 6d64 3c2f 613e 3c2f 7464 3e0a  ops.md</a></td>.
+00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003180: 3c74 643e 3c61 2068 7265 663d 2268 7474  <td><a href="htt
+00003190: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000031a0: 476f 6b75 4d6f 6861 6e64 6173 2f6d 6c6f  GokuMohandas/mlo
+000031b0: 7073 2d63 6f75 7273 6522 3e6d 6c6f 7073  ps-course">mlops
+000031c0: 2d63 6f75 7273 653c 2f61 3e3c 2f74 643e  -course</a></td>
+000031d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000031e0: 203c 7464 3e50 7974 686f 6e2c 204a 7570   <td>Python, Jup
+000031f0: 7974 6572 3c2f 7464 3e0a 2020 2020 2020  yter</td>.      
+00003200: 2020 2020 2020 2020 2020 3c74 643e 0a20            <td>. 
+00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003220: 2020 203c 703e 382c 3532 343c 2f70 3e0a     <p>8,524</p>.
+00003230: 2020 2020 2020 2020 2020 2020 3c2f 7472              </tr
+00003240: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
+00003250: 723e 0a20 2020 2020 2020 2020 2020 2020  r>.             
+00003260: 2020 203c 7464 3ef0 9f94 9f3c 2f74 643e     <td>....</td>
+00003270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003280: 203c 7464 3e3c 6120 6872 6566 3d22 6874   <td><a href="ht
+00003290: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000032a0: 2f65 6c69 3634 732f 7265 6164 6d65 2d61  /eli64s/readme-a
+000032b0: 692f 626c 6f62 2f6d 6169 6e2f 6578 616d  i/blob/main/exam
+000032c0: 706c 6573 2f72 6561 646d 652d 7079 666c  ples/readme-pyfl
+000032d0: 696e 6b2e 6d64 223e 7265 6164 6d65 2d70  ink.md">readme-p
+000032e0: 7966 6c69 6e6b 2e6d 643c 2f61 3e3c 2f74  yflink.md</a></t
+000032f0: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
+00003300: 2020 203c 7464 3e3c 6120 6872 6566 3d22     <td><a href="
+00003310: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003320: 6f6d 2f65 6c69 3634 732f 666c 696e 6b2d  om/eli64s/flink-
+00003330: 666c 6f77 223e 666c 696e 6b2d 666c 6f77  flow">flink-flow
+00003340: 3c2f 613e 3c2f 7464 3e0a 2020 2020 2020  </a></td>.      
+00003350: 2020 2020 2020 2020 2020 3c74 643e 5079            <td>Py
+00003360: 466c 696e 6b3c 2f74 643e 0a20 2020 2020  Flink</td>.     
+00003370: 2020 2020 2020 2020 2020 203c 7464 3e0a             <td>.
+00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003390: 2020 2020 3c70 3e33 323c 2f70 3e0a 2020      <p>32</p>.  
+000033a0: 2020 2020 2020 2020 2020 3c2f 7472 3e0a            </tr>.
+000033b0: 2020 2020 3c2f 7461 626c 653e 0a3c 2f64      </table>.</d
+000033c0: 6976 3e0a 0a0a 3c68 3120 616c 6967 6e3d  iv>...<h1 align=
+000033d0: 2263 656e 7465 7222 3ee2 928f 3c62 723e  "center">...<br>
+000033e0: f09f 9187 3c62 723e 3c62 723e f09f 939c  ....<br><br>....
+000033f0: 2043 7573 746f 6d20 5245 4144 4d45 2074   Custom README t
+00003400: 656d 706c 6174 6573 2063 6f6d 696e 6720  emplates coming 
+00003410: 736f 6f6e 213c 2f68 313e 0a3c 7020 616c  soon!</h1>.<p al
+00003420: 6967 6e3d 2263 656e 7465 7222 3e44 6576  ign="center">Dev
+00003430: 656c 6f70 696e 6720 6120 6665 6174 7572  eloping a featur
+00003440: 6520 7468 6174 2061 6c6c 6f77 7320 7573  e that allows us
+00003450: 6572 7320 746f 2073 656c 6563 7420 6672  ers to select fr
+00003460: 6f6d 2061 2076 6172 6965 7479 206f 6620  om a variety of 
+00003470: 5245 4144 4d45 2066 6f72 6d61 7473 2061  README formats a
+00003480: 6e64 2073 7479 6c65 732e 3c2f 703e 0a3c  nd styles.</p>.<
+00003490: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+000034a0: 3e43 7573 746f 6d20 7465 6d70 6c61 7465  >Custom template
+000034b0: 7320 7769 6c6c 2062 6520 7461 696c 6f72  s will be tailor
+000034c0: 6564 2066 6f72 2075 7365 2d63 6173 6573  ed for use-cases
+000034d0: 2073 7563 6820 6173 2064 6174 612c 2061   such as data, a
+000034e0: 6920 2620 6d6c 2c20 7265 7365 6172 6368  i & ml, research
+000034f0: 2c20 6d69 6e69 6d61 6c2c 2061 6e64 206d  , minimal, and m
+00003500: 6f72 6521 3c2f 703e 0a0a 3c70 2061 6c69  ore!</p>..<p ali
+00003510: 676e 3d22 7269 6768 7422 3e0a 2020 2020  gn="right">.    
+00003520: 3c61 2068 7265 663d 2223 746f 7022 3e3c  <a href="#top"><
+00003530: 623e f09f 949d 2052 6574 7572 6e20 3c2f  b>.... Return </
+00003540: 623e 3c2f 613e 0a3c 2f70 3e0a 0a2d 2d2d  b></a>.</p>..---
+00003550: 0a0a 2323 20f0 9f9a 8020 4765 7474 696e  ..## .... Gettin
+00003560: 6720 5374 6172 7465 640a 0a23 2323 20e2  g Started..### .
+00003570: 9c94 efb8 8f20 4465 7065 6e64 656e 6369  ..... Dependenci
+00003580: 6573 0a0a 4265 666f 7265 2079 6f75 2062  es..Before you b
+00003590: 6567 696e 2c20 656e 7375 7265 2074 6861  egin, ensure tha
+000035a0: 7420 796f 7520 6861 7665 2074 6865 2066  t you have the f
+000035b0: 6f6c 6c6f 7769 6e67 2070 7265 7265 7175  ollowing prerequ
+000035c0: 6973 6974 6573 2069 6e73 7461 6c6c 6564  isites installed
+000035d0: 3a0a 0a2d 2050 7974 686f 6e20 332e 3920  :..- Python 3.9 
+000035e0: 6f72 2068 6967 6865 720a 2d20 436f 6e64  or higher.- Cond
+000035f0: 6120 6f72 2050 6f65 7472 7920 7061 636b  a or Poetry pack
+00003600: 6167 6520 6d61 6e61 6765 7220 2872 6563  age manager (rec
+00003610: 6f6d 6d65 6e64 6564 290a 2d20 4163 6365  ommended).- Acce
+00003620: 7373 2074 6f20 7468 6520 4f70 656e 4149  ss to the OpenAI
+00003630: 2041 5049 2028 7365 6520 7468 6520 7365   API (see the se
+00003640: 7475 7020 6775 6964 6520 6265 6c6f 7729  tup guide below)
+00003650: 0a0a 2323 2323 20f0 9f93 8220 5265 706f  ..#### .... Repo
+00003660: 7369 746f 7279 0a0a 4d6f 7374 2075 7365  sitory..Most use
+00003670: 7227 7320 7769 6c6c 2072 756e 202a 5245  r's will run *RE
+00003680: 4144 4d45 2d41 492a 2075 7369 6e67 2074  ADME-AI* using t
+00003690: 6865 2063 6f6d 6d61 6e64 2d6c 696e 652c  he command-line,
+000036a0: 2073 7065 6369 6679 696e 6720 7468 6569   specifying thei
+000036b0: 7220 7265 706f 7369 746f 7279 206f 6e20  r repository on 
+000036c0: 7275 6e2d 7469 6d65 2e20 486f 7765 7665  run-time. Howeve
+000036d0: 722c 2069 6620 796f 7520 776f 756c 6420  r, if you would 
+000036e0: 6c69 6b65 2074 6f20 7573 6520 7468 6520  like to use the 
+000036f0: 6465 6661 756c 7420 636f 6e66 6967 7572  default configur
+00003700: 6174 696f 6e2c 2079 6f75 2077 696c 6c20  ation, you will 
+00003710: 6e65 6564 2074 6f20 7570 6461 7465 2074  need to update t
+00003720: 6865 205b 636f 6e66 6967 7572 6174 696f  he [configuratio
+00003730: 6e20 6669 6c65 5d28 2e2f 636f 6e66 2f63  n file](./conf/c
+00003740: 6f6e 662e 746f 6d6c 2920 7769 7468 2079  onf.toml) with y
+00003750: 6f75 7220 7265 706f 7369 746f 7279 2773  our repository's
+00003760: 2072 656d 6f74 6520 5552 4c20 6f72 2061   remote URL or a
+00003770: 206c 6f63 616c 2070 6174 6820 746f 2079   local path to y
+00003780: 6f75 7220 636f 6465 6261 7365 2e0a 0a60  our codebase...`
+00003790: 6060 746f 6d6c 0a5b 6769 745d 0a72 6570  ``toml.[git].rep
+000037a0: 6f73 6974 6f72 7920 3d20 2249 6e73 6572  ository = "Inser
+000037b0: 7420 796f 7572 2072 6570 6f73 6974 6f72  t your repositor
+000037c0: 7920 5552 4c20 6f72 206c 6f63 616c 2070  y URL or local p
+000037d0: 6174 6820 6865 7265 2122 0a60 6060 0a0a  ath here!".```..
+000037e0: 2323 2323 20f0 9f94 9020 4f70 656e 4149  #### .... OpenAI
+000037f0: 2041 5049 0a0a 546f 2075 7365 2074 6865   API..To use the
+00003800: 202a 5245 4144 4d45 2d41 492a 2061 7070   *README-AI* app
+00003810: 2c20 796f 7520 6d75 7374 2063 7265 6174  , you must creat
+00003820: 6520 616e 204f 7065 6e41 4920 4150 4920  e an OpenAI API 
+00003830: 6163 636f 756e 7420 616e 6420 6765 6e65  account and gene
+00003840: 7261 7465 2061 6e20 4150 4920 6b65 792e  rate an API key.
+00003850: 2054 6865 2073 7465 7073 2062 656c 6f77   The steps below
+00003860: 206f 7574 6c69 6e65 2074 6869 7320 7072   outline this pr
+00003870: 6f63 6573 733a 0a0a 3c64 6574 6169 6c73  ocess:..<details
+00003880: 2063 6c6f 7365 643e 3c73 756d 6d61 7279   closed><summary
+00003890: 3e4f 7065 6e41 4920 4150 4920 5573 6572  >OpenAI API User
+000038a0: 2047 7569 6465 3c2f 7375 6d6d 6172 793e   Guide</summary>
+000038b0: 0a0a 312e 2047 6f20 746f 2074 6865 205b  ..1. Go to the [
+000038c0: 4f70 656e 4149 2077 6562 7369 7465 5d28  OpenAI website](
+000038d0: 6874 7470 733a 2f2f 706c 6174 666f 726d  https://platform
+000038e0: 2e6f 7065 6e61 692e 636f 6d2f 292e 0a32  .openai.com/)..2
+000038f0: 2e20 436c 6963 6b20 7468 6520 2253 6967  . Click the "Sig
+00003900: 6e20 7570 2066 6f72 2066 7265 6522 2062  n up for free" b
+00003910: 7574 746f 6e2e 0a33 2e20 4669 6c6c 206f  utton..3. Fill o
+00003920: 7574 2074 6865 2072 6567 6973 7472 6174  ut the registrat
+00003930: 696f 6e20 666f 726d 2077 6974 6820 796f  ion form with yo
+00003940: 7572 2069 6e66 6f72 6d61 7469 6f6e 2061  ur information a
+00003950: 6e64 2061 6772 6565 2074 6f20 7468 6520  nd agree to the 
+00003960: 7465 726d 7320 6f66 2073 6572 7669 6365  terms of service
+00003970: 2e0a 342e 204f 6e63 6520 6c6f 6767 6564  ..4. Once logged
+00003980: 2069 6e2c 2063 6c69 636b 206f 6e20 7468   in, click on th
+00003990: 6520 2241 5049 2220 7461 622e 0a35 2e20  e "API" tab..5. 
+000039a0: 466f 6c6c 6f77 2074 6865 2069 6e73 7472  Follow the instr
+000039b0: 7563 7469 6f6e 7320 746f 2063 7265 6174  uctions to creat
+000039c0: 6520 6120 6e65 7720 4150 4920 6b65 792e  e a new API key.
+000039d0: 0a36 2e20 436f 7079 2074 6865 2041 5049  .6. Copy the API
+000039e0: 206b 6579 2061 6e64 206b 6565 7020 6974   key and keep it
+000039f0: 2069 6e20 6120 7365 6375 7265 2070 6c61   in a secure pla
+00003a00: 6365 2e0a 0a3c 2f64 6574 6169 6c73 3e0a  ce...</details>.
+00003a10: 3c62 723e 0a0a 3e20 2a2a e29a a0ef b88f  <br>..> **......
+00003a20: 204e 6f74 652a 2a0a 3e0a 3e20 2d20 546f   Note**.>.> - To
+00003a30: 206d 6178 696d 697a 6520 796f 7572 2065   maximize your e
+00003a40: 7870 6572 6965 6e63 6520 7769 7468 2052  xperience with R
+00003a50: 4541 444d 452d 4149 2c20 6974 2069 7320  EADME-AI, it is 
+00003a60: 7265 636f 6d6d 656e 6465 6420 746f 2073  recommended to s
+00003a70: 6574 2075 7020 6120 7061 796d 656e 7420  et up a payment 
+00003a80: 6d65 7468 6f64 206f 6e20 4f70 656e 4149  method on OpenAI
+00003a90: 2773 2077 6562 7369 7465 2e20 4279 2064  's website. By d
+00003aa0: 6f69 6e67 2073 6f2c 2079 6f75 2067 6169  oing so, you gai
+00003ab0: 6e20 6163 6365 7373 2074 6f20 6d6f 7265  n access to more
+00003ac0: 2070 6f77 6572 6675 6c20 6c61 6e67 7561   powerful langua
+00003ad0: 6765 206d 6f64 656c 7320 6c69 6b65 2067  ge models like g
+00003ae0: 7074 2d33 2e35 2d74 7572 626f 2e20 5769  pt-3.5-turbo. Wi
+00003af0: 7468 6f75 7420 6120 7061 796d 656e 7420  thout a payment 
+00003b00: 6d65 7468 6f64 2c20 796f 7572 2075 7361  method, your usa
+00003b10: 6765 2077 696c 6c20 6265 2072 6573 7472  ge will be restr
+00003b20: 6963 7465 6420 746f 2074 6865 2062 6173  icted to the bas
+00003b30: 6520 6770 742d 3320 6d6f 6465 6c73 2e20  e gpt-3 models. 
+00003b40: 5468 6973 206c 696d 6974 6174 696f 6e20  This limitation 
+00003b50: 6d69 6768 7420 6c65 6164 2074 6f20 6c65  might lead to le
+00003b60: 7373 2070 7265 6369 7365 2052 4541 444d  ss precise READM
+00003b70: 4520 6669 6c65 7320 6f72 2070 6f74 656e  E files or poten
+00003b80: 7469 616c 2065 7272 6f72 7320 6475 7269  tial errors duri
+00003b90: 6e67 2074 6865 2067 656e 6572 6174 696f  ng the generatio
+00003ba0: 6e20 7072 6f63 6573 732e 0a3e 0a3e 202d  n process..>.> -
+00003bb0: 2057 6865 6e20 7573 696e 6720 6120 7061   When using a pa
+00003bc0: 796d 656e 7420 6d65 7468 6f64 2c20 6d61  yment method, ma
+00003bd0: 6b65 2073 7572 6520 796f 7520 6861 7665  ke sure you have
+00003be0: 2073 7566 6669 6369 656e 7420 6372 6564   sufficient cred
+00003bf0: 6974 7320 746f 2072 756e 2074 6865 2052  its to run the R
+00003c00: 4541 444d 452d 4149 2061 7070 6c69 6361  EADME-AI applica
+00003c10: 7469 6f6e 2e20 4164 6469 7469 6f6e 616c  tion. Additional
+00003c20: 6c79 2c20 7265 6d65 6d62 6572 2074 6f20  ly, remember to 
+00003c30: 7265 6775 6c61 726c 7920 6d6f 6e69 746f  regularly monito
+00003c40: 7220 796f 7572 2041 5049 2075 7361 6765  r your API usage
+00003c50: 2061 6e64 2063 6f73 7473 2062 7920 7669   and costs by vi
+00003c60: 7369 7469 6e67 2074 6865 205b 4f70 656e  siting the [Open
+00003c70: 4149 2041 5049 2055 7361 6765 2044 6173  AI API Usage Das
+00003c80: 6862 6f61 7264 5d28 6874 7470 733a 2f2f  hboard](https://
+00003c90: 706c 6174 666f 726d 2e6f 7065 6e61 692e  platform.openai.
+00003ca0: 636f 6d2f 6163 636f 756e 742f 7573 6167  com/account/usag
+00003cb0: 6529 2e20 506c 6561 7365 206e 6f74 6520  e). Please note 
+00003cc0: 7468 6174 2074 6869 7320 4150 4920 6973  that this API is
+00003cd0: 206e 6f74 2066 7265 6520 616e 6420 796f   not free and yo
+00003ce0: 7520 7769 6c6c 2062 6520 6368 6172 6765  u will be charge
+00003cf0: 6420 666f 7220 6561 6368 2072 6571 7565  d for each reque
+00003d00: 7374 206d 6164 652c 2077 6869 6368 2063  st made, which c
+00003d10: 616e 2061 6363 756d 756c 6174 6520 7261  an accumulate ra
+00003d20: 7069 646c 792e 0a3e 0a3e 202d 2054 6865  pidly..>.> - The
+00003d30: 2067 656e 6572 6174 696f 6e20 6f66 2074   generation of t
+00003d40: 6865 2052 4541 444d 452e 6d64 2066 696c  he README.md fil
+00003d50: 6520 7368 6f75 6c64 2074 7970 6963 616c  e should typical
+00003d60: 6c79 2063 6f6d 706c 6574 6520 696e 2075  ly complete in u
+00003d70: 6e64 6572 2031 206d 696e 7574 652e 2049  nder 1 minute. I
+00003d80: 6620 6974 2074 616b 6573 206c 6f6e 6765  f it takes longe
+00003d90: 7220 7468 616e 2061 2066 6577 206d 696e  r than a few min
+00003da0: 7574 6573 2c20 706c 6561 7365 2074 6572  utes, please ter
+00003db0: 6d69 6e61 7465 2074 6865 2070 726f 6365  minate the proce
+00003dc0: 7373 2e0a 3e0a 0a2d 2d2d 0a0a 2323 2320  ss..>..---..### 
+00003dd0: f09f 93a6 2049 6e73 7461 6c6c 6174 696f  .... Installatio
+00003de0: 6e0a 0a31 2e20 436c 6f6e 6520 7468 6520  n..1. Clone the 
+00003df0: 2a72 6561 646d 652d 6169 2a20 7265 706f  *readme-ai* repo
+00003e00: 7369 746f 7279 2074 6f20 796f 7572 206d  sitory to your m
+00003e10: 6163 6869 6e65 2e0a 6060 6073 680a 6769  achine..```sh.gi
+00003e20: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
+00003e30: 6769 7468 7562 2e63 6f6d 2f65 6c69 3634  github.com/eli64
+00003e40: 732f 7265 6164 6d65 2d61 690a 6060 600a  s/readme-ai.```.
+00003e50: 0a32 2e20 4e61 7669 6761 7465 2074 6f20  .2. Navigate to 
+00003e60: 7468 6520 2a72 6561 646d 652d 6169 2a20  the *readme-ai* 
+00003e70: 6469 7265 6374 6f72 792e 0a60 6060 7368  directory..```sh
+00003e80: 0a63 6420 7265 6164 6d65 2d61 690a 6060  .cd readme-ai.``
+00003e90: 600a 0a33 2e20 5573 6520 616e 7920 6f66  `..3. Use any of
+00003ea0: 2074 6865 2066 6f6c 6c6f 7769 6e67 206d   the following m
+00003eb0: 6574 686f 6473 2074 6f20 696e 7374 616c  ethods to instal
+00003ec0: 6c20 7072 6f6a 6563 7420 6465 7065 6e64  l project depend
+00003ed0: 656e 6369 6573 2e0a 0a3e 202a 5069 7020  encies...> *Pip 
+00003ee0: 285b 5079 5049 2050 6163 6b61 6765 5d28  ([PyPI Package](
+00003ef0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00003f00: 2f70 726f 6a65 6374 2f72 6561 646d 6561  /project/readmea
+00003f10: 692f 2929 2a0a 6060 6073 680a 7069 7020  i/))*.```sh.pip 
+00003f20: 696e 7374 616c 6c20 7265 6164 6d65 6169  install readmeai
+00003f30: 0a60 6060 0a0a 3e20 2a44 6f63 6b65 7220  .```..> *Docker 
+00003f40: 285b 446f 636b 6572 2048 7562 5d28 6874  ([Docker Hub](ht
+00003f50: 7470 733a 2f2f 6875 622e 646f 636b 6572  tps://hub.docker
+00003f60: 2e63 6f6d 2f72 6570 6f73 6974 6f72 792f  .com/repository/
+00003f70: 646f 636b 6572 2f7a 6572 6f78 656c 692f  docker/zeroxeli/
+00003f80: 7265 6164 6d65 2d61 692f 6765 6e65 7261  readme-ai/genera
+00003f90: 6c29 292a 0a60 6060 7368 0a64 6f63 6b65  l))*.```sh.docke
+00003fa0: 7220 7075 6c6c 207a 6572 6f78 656c 692f  r pull zeroxeli/
+00003fb0: 7265 6164 6d65 2d61 693a 6c61 7465 7374  readme-ai:latest
+00003fc0: 0a60 6060 0a0a 3e20 2a42 6173 682a 0a60  .```..> *Bash*.`
+00003fd0: 6060 7368 0a62 6173 6820 7365 7475 702f  ``sh.bash setup/
+00003fe0: 7365 7475 702e 7368 0a60 6060 0a0a 3e20  setup.sh.```..> 
+00003ff0: 2a43 6f6e 6461 2a0a 6060 6073 680a 636f  *Conda*.```sh.co
+00004000: 6e64 6120 6372 6561 7465 202d 6e20 7265  nda create -n re
+00004010: 6164 6d65 6169 2070 7974 686f 6e3d 332e  admeai python=3.
+00004020: 3920 2d79 2026 2620 5c0a 636f 6e64 6120  9 -y && \.conda 
+00004030: 6163 7469 7661 7465 2072 6561 646d 6561  activate readmea
+00004040: 6920 2626 205c 0a70 6970 2069 6e73 7461  i && \.pip insta
+00004050: 6c6c 202d 7220 7265 7175 6972 656d 656e  ll -r requiremen
+00004060: 7473 2e74 7874 0a60 6060 0a0a 3e20 2a50  ts.txt.```..> *P
+00004070: 6f65 7472 792a 0a60 6060 7368 0a70 6f65  oetry*.```sh.poe
+00004080: 7472 7920 696e 7374 616c 6c0a 6060 600a  try install.```.
+00004090: 0a23 2323 20f0 9f8e ae20 5573 696e 6720  .### .... Using 
+000040a0: 2a52 4541 444d 452d 4149 2a0a 0a55 7365  *README-AI*..Use
+000040b0: 2074 6865 2063 6f6d 6d61 6e64 2d6c 696e   the command-lin
+000040c0: 6520 746f 2070 726f 7669 6465 2074 6865  e to provide the
+000040d0: 204f 7065 6e41 4920 4150 4920 6b65 7920   OpenAI API key 
+000040e0: 2869 6620 6e6f 7420 616c 7265 6164 7920  (if not already 
+000040f0: 7365 7429 2061 6e64 2073 7065 6369 6679  set) and specify
+00004100: 2061 6e20 6f75 7470 7574 2070 6174 6820   an output path 
+00004110: 666f 7220 796f 7572 2052 4541 444d 4520  for your README 
+00004120: 6669 6c65 2c20 616c 6f6e 6720 7769 7468  file, along with
+00004130: 2074 6865 2070 6174 6820 746f 2079 6f75   the path to you
+00004140: 7220 6c6f 6361 6c20 7265 706f 7369 746f  r local reposito
+00004150: 7279 206f 7220 7265 6d6f 7465 2063 6f64  ry or remote cod
+00004160: 6520 7265 706f 7369 746f 7279 2e20 596f  e repository. Yo
+00004170: 7520 6361 6e20 616c 736f 2070 726f 7669  u can also provi
+00004180: 6465 2074 6865 206f 7574 7075 7420 7061  de the output pa
+00004190: 7468 2069 6e20 7468 6520 5b63 6f6e 6669  th in the [confi
+000041a0: 6775 7261 7469 6f6e 2066 696c 655d 282e  guration file](.
+000041b0: 2f63 6f6e 662f 636f 6e66 2e74 6f6d 6c29  /conf/conf.toml)
+000041c0: 0a0a 436f 6d6d 616e 642d 4c69 6e65 2041  ..Command-Line A
+000041d0: 7267 756d 656e 7473 3a0a 0a2d 2060 2d6b  rguments:..- `-k
+000041e0: 6020 6f72 2060 2d2d 6170 692d 6b65 7960  ` or `--api-key`
+000041f0: 3a20 596f 7572 204f 7065 6e41 4920 4150  : Your OpenAI AP
+00004200: 4920 6b65 792e 0a2d 2060 2d6f 6020 6f72  I key..- `-o` or
+00004210: 2060 2d2d 6f75 7470 7574 603a 2054 6865   `--output`: The
+00004220: 206f 7574 7075 7420 7061 7468 2066 6f72   output path for
+00004230: 2079 6f75 7220 5245 4144 4d45 2e6d 6420   your README.md 
+00004240: 6669 6c65 2e0a 2d20 602d 7260 206f 7220  file..- `-r` or 
+00004250: 602d 2d72 6570 6f73 6974 6f72 7960 3a20  `--repository`: 
+00004260: 5468 6520 5552 4c20 6f72 2070 6174 6820  The URL or path 
+00004270: 746f 2079 6f75 7220 636f 6465 2072 6570  to your code rep
+00004280: 6f73 6974 6f72 792e 0a2d 2060 2d74 6020  ository..- `-t` 
+00004290: 6f72 2060 2d2d 7465 6d70 6c61 7465 603a  or `--template`:
+000042a0: 2054 6865 2052 4541 444d 4520 7465 6d70   The README temp
+000042b0: 6c61 7465 2066 6f72 6d61 7420 746f 2075  late format to u
+000042c0: 7365 2e20 2863 6f6d 696e 6720 736f 6f6e  se. (coming soon
+000042d0: 2129 0a2d 2060 6c60 206f 7220 602d 2d6c  !).- `l` or `--l
+000042e0: 616e 6775 6167 6560 3a20 5468 6520 6c61  anguage`: The la
+000042f0: 6e67 7561 6765 206f 6620 7465 7874 2077  nguage of text w
+00004300: 7269 7474 656e 2069 6e20 7468 6520 5245  ritten in the RE
+00004310: 4144 4d45 2066 696c 6520 2863 6f6d 696e  ADME file (comin
+00004320: 6720 736f 6f6e 2129 0a0a 5573 6520 616e  g soon!)..Use an
+00004330: 7920 6f66 2074 6865 2066 6f6c 6c6f 7769  y of the followi
+00004340: 6e67 206d 6574 686f 6473 2074 6f20 7275  ng methods to ru
+00004350: 6e20 7468 6520 2a72 6561 646d 652d 6169  n the *readme-ai
+00004360: 2a20 434c 4920 6170 706c 6963 6174 696f  * CLI applicatio
+00004370: 6e2e 0a0a 3e20 2a50 6970 2028 5b50 7950  n...> *Pip ([PyP
+00004380: 4920 5061 636b 6167 655d 2868 7474 7073  I Package](https
+00004390: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000043a0: 6563 742f 7265 6164 6d65 6169 2f29 292a  ect/readmeai/))*
+000043b0: 0a60 6060 7368 0a72 6561 646d 6561 6920  .```sh.readmeai 
+000043c0: 2d2d 6170 692d 6b65 7920 2259 4f55 525f  --api-key "YOUR_
+000043d0: 4150 495f 4b45 5922 202d 2d6f 7574 7075  API_KEY" --outpu
+000043e0: 7420 7265 6164 6d65 2d61 692e 6d64 202d  t readme-ai.md -
+000043f0: 2d72 6570 6f73 6974 6f72 7920 6874 7470  -repository http
+00004400: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00004410: 6c69 3634 732f 7265 6164 6d65 2d61 690a  li64s/readme-ai.
+00004420: 0a23 204f 7220 6578 706f 7274 2079 6f75  .# Or export you
+00004430: 7220 4f70 656e 4149 2041 5049 206b 6579  r OpenAI API key
+00004440: 2061 7320 616e 2065 6e76 6972 6f6e 6d65   as an environme
+00004450: 6e74 2076 6172 6961 626c 650a 6578 706f  nt variable.expo
+00004460: 7274 204f 5045 4e41 495f 4150 495f 4b45  rt OPENAI_API_KE
+00004470: 593d 2259 4f55 525f 4150 495f 4b45 5922  Y="YOUR_API_KEY"
+00004480: 0a72 6561 646d 6561 6920 2d6f 2072 6561  .readmeai -o rea
+00004490: 646d 652d 6169 2e6d 6420 2d72 2068 7474  dme-ai.md -r htt
+000044a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000044b0: 656c 6936 3473 2f72 6561 646d 652d 6169  eli64s/readme-ai
+000044c0: 0a60 6060 0a0a 3e20 2a44 6f63 6b65 7220  .```..> *Docker 
+000044d0: 285b 446f 636b 6572 2048 7562 5d28 6874  ([Docker Hub](ht
+000044e0: 7470 733a 2f2f 6875 622e 646f 636b 6572  tps://hub.docker
+000044f0: 2e63 6f6d 2f72 6570 6f73 6974 6f72 792f  .com/repository/
+00004500: 646f 636b 6572 2f7a 6572 6f78 656c 692f  docker/zeroxeli/
+00004510: 7265 6164 6d65 2d61 692f 6765 6e65 7261  readme-ai/genera
+00004520: 6c29 292a 0a60 6060 7368 0a64 6f63 6b65  l))*.```sh.docke
+00004530: 7220 7275 6e20 2d69 7420 5c0a 2d65 204f  r run -it \.-e O
+00004540: 5045 4e41 495f 4150 495f 4b45 593d 2259  PENAI_API_KEY="Y
+00004550: 4f55 525f 4150 495f 4b45 5922 205c 0a2d  OUR_API_KEY" \.-
+00004560: 7620 2224 2870 7764 2922 3a2f 6170 7020  v "$(pwd)":/app 
+00004570: 7a65 726f 7865 6c69 2f72 6561 646d 652d  zeroxeli/readme-
+00004580: 6169 3a6c 6174 6573 7420 5c0a 7265 6164  ai:latest \.read
+00004590: 6d65 6169 202d 6f20 7265 6164 6d65 2d61  meai -o readme-a
+000045a0: 692e 6d64 202d 7220 6874 7470 733a 2f2f  i.md -r https://
+000045b0: 6769 7468 7562 2e63 6f6d 2f65 6c69 3634  github.com/eli64
+000045c0: 732f 7265 6164 6d65 2d61 690a 6060 600a  s/readme-ai.```.
+000045d0: 0a3e 202a 436f 6e64 612a 0a60 6060 7368  .> *Conda*.```sh
+000045e0: 0a63 6f6e 6461 2061 6374 6976 6174 6520  .conda activate 
+000045f0: 7265 6164 6d65 6169 0a65 7870 6f72 7420  readmeai.export 
+00004600: 4f50 454e 4149 5f41 5049 5f4b 4559 3d22  OPENAI_API_KEY="
+00004610: 594f 5552 5f41 5049 5f4b 4559 220a 7079  YOUR_API_KEY".py
+00004620: 7468 6f6e 2072 6561 646d 6561 692f 6d61  thon readmeai/ma
+00004630: 696e 2e70 7920 2d6f 2072 6561 646d 652d  in.py -o readme-
+00004640: 6169 2e6d 6420 2d72 2068 7474 7073 3a2f  ai.md -r https:/
+00004650: 2f67 6974 6875 622e 636f 6d2f 656c 6936  /github.com/eli6
+00004660: 3473 2f72 6561 646d 652d 6169 0a60 6060  4s/readme-ai.```
+00004670: 0a0a 3e20 2a50 6f65 7472 792a 0a60 6060  ..> *Poetry*.```
+00004680: 7368 0a70 6f65 7472 7920 7368 656c 6c0a  sh.poetry shell.
+00004690: 6578 706f 7274 204f 5045 4e41 495f 4150  export OPENAI_AP
+000046a0: 495f 4b45 593d 2259 4f55 525f 4150 495f  I_KEY="YOUR_API_
+000046b0: 4b45 5922 0a70 6f65 7472 7920 7275 6e20  KEY".poetry run 
+000046c0: 7079 7468 6f6e 2072 6561 646d 6561 692f  python readmeai/
+000046d0: 6d61 696e 2e70 7920 2d6f 2072 6561 646d  main.py -o readm
+000046e0: 652d 6169 2e6d 6420 2d72 2068 7474 7073  e-ai.md -r https
+000046f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 656c  ://github.com/el
+00004700: 6936 3473 2f72 6561 646d 652d 6169 0a60  i64s/readme-ai.`
+00004710: 6060 0a0a 2323 2320 f09f a7aa 2052 756e  ``..### .... Run
+00004720: 6e69 6e67 2054 6573 7473 0a0a 4578 6563  ning Tests..Exec
+00004730: 7574 6520 7468 6520 666f 6c6c 6f77 696e  ute the followin
+00004740: 6720 636f 6d6d 616e 6420 746f 2072 756e  g command to run
+00004750: 2074 6865 2074 6573 7420 7375 6974 652e   the test suite.
+00004760: 0a0a 6060 6073 680a 6261 7368 2073 6372  ..```sh.bash scr
+00004770: 6970 7473 2f74 6573 742e 7368 0a60 6060  ipts/test.sh.```
+00004780: 0a0a 3c70 2061 6c69 676e 3d22 7269 6768  ..<p align="righ
+00004790: 7422 3e0a 2020 3c61 2068 7265 663d 2223  t">.  <a href="#
+000047a0: 746f 7022 3e3c 623e f09f 949d 2052 6574  top"><b>.... Ret
+000047b0: 7572 6e20 3c2f 623e 3c2f 613e 0a3c 2f70  urn </b></a>.</p
+000047c0: 3e0a 0a2d 2d2d 0a0a 2323 20f0 9f9b a020  >..---..## .... 
+000047d0: 4675 7475 7265 2044 6576 656c 6f70 6d65  Future Developme
+000047e0: 6e74 0a0a 2d20 5b58 5d20 4164 6420 6164  nt..- [X] Add ad
+000047f0: 6469 7469 6f6e 616c 206c 616e 6775 6167  ditional languag
+00004800: 6520 7375 7070 6f72 7420 666f 7220 706f  e support for po
+00004810: 7075 6c61 7469 6e67 2074 6865 202a 696e  pulating the *in
+00004820: 7374 616c 6c61 7469 6f6e 2a2c 202a 7573  stallation*, *us
+00004830: 6167 652a 2c20 616e 6420 2a74 6573 742a  age*, and *test*
+00004840: 2052 4541 444d 4520 7365 6374 696f 6e73   README sections
+00004850: 2e0a 2d20 5b58 5d20 5570 6c6f 6164 2074  ..- [X] Upload t
+00004860: 6865 202a 7265 6164 6d65 2d61 692a 2043  he *readme-ai* C
+00004870: 4c49 2074 6f6f 6c20 746f 2050 7950 4920  LI tool to PyPI 
+00004880: 756e 6465 7220 7468 6520 6d6f 6475 6c65  under the module
+00004890: 206e 616d 6520 5b72 6561 646d 6561 695d   name [readmeai]
+000048a0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+000048b0: 672f 7072 6f6a 6563 742f 7265 6164 6d65  g/project/readme
+000048c0: 6169 2f29 2e0a 2d20 5b20 5d20 4465 7369  ai/)..- [ ] Desi
+000048d0: 676e 2061 6e64 2069 6d70 6c65 6d65 6e74  gn and implement
+000048e0: 2061 2076 6172 6965 7479 206f 6620 5245   a variety of RE
+000048f0: 4144 4d45 2074 656d 706c 6174 6520 666f  ADME template fo
+00004900: 726d 6174 7320 666f 7220 6469 6666 6572  rmats for differ
+00004910: 656e 7420 7573 652d 6361 7365 732e 0a2d  ent use-cases..-
+00004920: 205b 205d 2041 6464 2073 7570 706f 7274   [ ] Add support
+00004930: 2066 6f72 2077 7269 7469 6e67 2074 6865   for writing the
+00004940: 2052 4541 444d 4520 696e 2061 6e79 206c   README in any l
+00004950: 616e 6775 6167 6520 2869 2e65 2e20 434e  anguage (i.e. CN
+00004960: 2c20 4553 2c20 4652 2c20 4a41 2c20 4b4f  , ES, FR, JA, KO
+00004970: 2c20 5255 292e 0a2d 205b 205d 2043 7265  , RU)..- [ ] Cre
+00004980: 6174 6520 5549 2077 6974 6820 5b54 6578  ate UI with [Tex
+00004990: 7475 616c 5d28 6874 7470 733a 2f2f 6769  tual](https://gi
+000049a0: 7468 7562 2e63 6f6d 2f54 6578 7475 616c  thub.com/Textual
+000049b0: 697a 652f 7465 7874 7561 6c29 206f 7220  ize/textual) or 
+000049c0: 616e 6f74 6865 7220 6672 616d 6577 6f72  another framewor
+000049d0: 6b20 746f 2069 6d70 726f 7665 2075 7365  k to improve use
+000049e0: 7220 6578 7065 7269 656e 6365 2e0a 0a2d  r experience...-
+000049f0: 2d2d 0a0a 2323 20f0 9f93 9220 4368 616e  --..## .... Chan
+00004a00: 6765 6c6f 670a 0a5b 4368 616e 6765 6c6f  gelog..[Changelo
+00004a10: 675d 282e 2f43 4841 4e47 454c 4f47 2e6d  g](./CHANGELOG.m
+00004a20: 6429 0a0a 2d2d 2d0a 0a23 2320 f09f a49d  d)..---..## ....
+00004a30: 2043 6f6e 7472 6962 7574 696e 670a 0a5b   Contributing..[
+00004a40: 436f 6e74 7269 6275 7469 6e67 2047 7569  Contributing Gui
+00004a50: 6465 6c69 6e65 735d 282e 2f43 4f4e 5452  delines](./CONTR
+00004a60: 4942 5554 494e 472e 6d64 290a 0a2d 2d2d  IBUTING.md)..---
+00004a70: 0a0a 2323 20f0 9f93 8420 4c69 6365 6e73  ..## .... Licens
+00004a80: 650a 0a5b 4d49 545d 282e 2f4c 4943 454e  e..[MIT](./LICEN
+00004a90: 5345 290a 0a2d 2d2d 0a0a 2323 20f0 9f91  SE)..---..## ...
+00004aa0: 8f20 4163 6b6e 6f77 6c65 6467 6d65 6e74  . Acknowledgment
+00004ab0: 730a 0a2a 4261 6467 6573 2a0a 2020 2d20  s..*Badges*.  - 
+00004ac0: 5b53 6869 656c 6473 2e69 6f5d 2868 7474  [Shields.io](htt
+00004ad0: 7073 3a2f 2f73 6869 656c 6473 2e69 6f2f  ps://shields.io/
+00004ae0: 290a 2020 2d20 5b41 7665 656b 2d53 6168  ).  - [Aveek-Sah
+00004af0: 612f 4769 7448 7562 2d50 726f 6669 6c65  a/GitHub-Profile
+00004b00: 2d42 6164 6765 735d 2868 7474 7073 3a2f  -Badges](https:/
+00004b10: 2f67 6974 6875 622e 636f 6d2f 4176 6565  /github.com/Avee
+00004b20: 6b2d 5361 6861 2f47 6974 4875 622d 5072  k-Saha/GitHub-Pr
+00004b30: 6f66 696c 652d 4261 6467 6573 290a 2020  ofile-Badges).  
+00004b40: 2d20 5b49 6c65 7269 6179 6f2f 4d61 726b  - [Ileriayo/Mark
+00004b50: 646f 776e 2d42 6164 6765 735d 2868 7474  down-Badges](htt
+00004b60: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004b70: 496c 6572 6961 796f 2f6d 6172 6b64 6f77  Ileriayo/markdow
+00004b80: 6e2d 6261 6467 6573 290a 0a3c 7020 616c  n-badges)..<p al
+00004b90: 6967 6e3d 2272 6967 6874 223e 0a20 203c  ign="right">.  <
+00004ba0: 6120 6872 6566 3d22 2374 6f70 223e 3c62  a href="#top"><b
+00004bb0: 3ef0 9f94 9d20 5265 7475 726e 203c 2f62  >.... Return </b
+00004bc0: 3e3c 2f61 3e0a 3c2f 703e 0a0a 2d2d 2d0a  ></a>.</p>..---.
+00004bd0: 0a                                       .
```

