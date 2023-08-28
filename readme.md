
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>readme-ai
</h1>
<h3>◦ Readme-ai: Elevating Code Understanding!</h3>
<h3>◦ Developed with the software and tools listed below.</h3>

<p align="center">
<img src="https://img.shields.io/badge/GNU%20Bash-4EAA25.svg?style&logo=GNU-Bash&logoColor=white" alt="GNU%20Bash" />
<img src="https://img.shields.io/badge/precommit-FAB040.svg?style&logo=pre-commit&logoColor=black" alt="precommit" />
<img src="https://img.shields.io/badge/OpenAI-412991.svg?style&logo=OpenAI&logoColor=white" alt="OpenAI" />
<img src="https://img.shields.io/badge/Python-3776AB.svg?style&logo=Python&logoColor=white" alt="Python" />

<img src="https://img.shields.io/badge/Docker-2496ED.svg?style&logo=Docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/Pytest-0A9EDC.svg?style&logo=Pytest&logoColor=white" alt="Pytest" />
<img src="https://img.shields.io/badge/Markdown-000000.svg?style&logo=Markdown&logoColor=white" alt="Markdown" />
<img src="https://img.shields.io/badge/JSON-000000.svg?style&logo=JSON&logoColor=white" alt="JSON" />
</p>
<img src="https://img.shields.io/github/languages/top/eli64s/readme-ai?style&color=5D6D7E" alt="GitHub top language" />
<img src="https://img.shields.io/github/languages/code-size/eli64s/readme-ai?style&color=5D6D7E" alt="GitHub code size in bytes" />
<img src="https://img.shields.io/github/commit-activity/m/eli64s/readme-ai?style&color=5D6D7E" alt="GitHub commit activity" />
<img src="https://img.shields.io/github/license/eli64s/readme-ai?style&color=5D6D7E" alt="GitHub license" />
</div>

---

## 📒 Table of Contents
- [📒 Table of Contents](#-table-of-contents)
- [📍 Overview](#-overview)
- [⚙️ Features](#-features)
- [📂 Project Structure](#project-structure)
- [🧩 Modules](#modules)
- [🚀 Getting Started](#-getting-started)
- [🗺 Roadmap](#-roadmap)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [👏 Acknowledgments](#-acknowledgments)

---


## 📍 Overview

The project "readme-ai" is designed to automate the process of generating high-quality README Markdown files for codebases. It leverages OpenAI's GPT-3 model to generate intelligent code summaries, slogans, overviews, and features. By parsing various file formats like YAML, TOML, and JSON, it extracts and analyzes dependencies related to different development tools. With its robust capabilities, this project aims to save developers time and effort in manually creating README files, enhancing the overall documentation quality and user experience of software projects.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular architecture with separate components for handling file I/O, preprocessing, model usage, logging, and CLI. It uses factory classes for multiple file formats, and Pydantic models for configuration constants. The application follows a command-line interface (CLI) design pattern to orchestrate the README file generation process. |
| **📖 Documentation**   | The codebase has comprehensive documentation. Each file has a clear description of its purpose and functionality. The README.md file provides an overview of the project and explains the installation and usage instructions. The code also contains comments and docstrings to explain important concepts and functions. |
| **🔗 Dependencies**    | The project relies on various external dependencies, including Python libraries like Pydantic and OpenAI's GPT package. It also uses third-party software like Docker and Conda. The project relies on Git and GitHub for version control and code collaboration. |
| **🧩 Modularity**      | The codebase is designed with modularity in mind, separating functionality into different modules. Each file has a specific role, such as handling file I/O, preprocessing, model usage, or configuration. The codebase follows the SOLID principles, allowing for easy extensibility and maintainability. |
| **✔️ Testing**          | The codebase includes a test script that uses pytest to generate and analyze code coverage reports. The tests cover various aspects of the project, including the file I/O, preprocessing, model usage, and data extraction components. The tests verify the correct behavior of different functionalities, improving overall code quality. |
| **⚡️ Performance**      | The project's performance is primarily dependent on the efficiency of the OpenAI API for generating text. The caching mechanism implemented in the codebase helps improve performance by reducing API calls. The implementation is efficient, and the codebase optimizes resource usage, ensuring smooth execution. |
| **🔐 Security**        | The system ensures data security and functionality by handling API requests, rate limiting, and error handling properly. The codebase uses secure communication channels with the OpenAI API. However, further security measures, such as input validation and protection against potential vulnerabilities, could be considered for more comprehensive security. |
| **🔀 Version Control** | The codebase is stored in a Git repository and follows best practices for version control. It includes a Makefile with commands for managing the project, such as cleaning files and fixing untracked files. The use of git commit and git push enables team collaboration and revision control. |
| **🔌 Integrations**    | The project integrates with external services and tools such as Docker, Conda, and Git/GitHub. It utilizes Docker for containerization and provides scripts to build and run Docker images. It also supports creating and activating Conda environments for running the project. The codebase fetches content from GitHub repositories and works well with the Git version control system. |
| **📶 Scalability**     | The codebase appears to scale well. It follows modular practices, allowing individual components to be extended or replaced as needed. The use of external APIs ensures that the project can leverage other

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                                                                                                    | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ---                                                                                                     | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| [Dockerfile](https://github.com/eli64s/readme-ai/blob/main/Dockerfile)                                  | This code snippet sets up a Docker image with Python 3.9 installed. It installs system dependencies, creates and switches to a non-root user, sets the PATH for user scripts, and installs the "readmeai" package from PyPI. Finally, it sets the command to run the CLI.                                                                                                                                                                                                |
| [Makefile](https://github.com/eli64s/readme-ai/blob/main/Makefile)                                      | The provided code snippet includes a Makefile with various commands for project management:-`clean`: Cleans unnecessary files and performs style formatting-`style`: Executes style formatting using various tools-`conda`: Creates a conda environment and installs dependencies-`venv`: Creates a virtual environment and installs dependencies-`git-fix`: Fixes git's untracked project files                                                                         |
| [badges_compressed.json](https://github.com/eli64s/readme-ai/blob/main/conf\svg\badges_compressed.json) | Prompt exceeds max token limit: 12709.                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| [builder.py](https://github.com/eli64s/readme-ai/blob/main/readmeai\builder.py)                         | This code snippet builds a README Markdown file for a codebase. It creates various sections such as badges, table of contents, intro, directory tree, modules, setup guide, etc. It fetches and formats data from configuration files and generates Markdown tables for code summaries. The snippet also includes functions to get and format badges, create a directory tree, and execute a file tree command.                                                          |
| [conf.py](https://github.com/eli64s/readme-ai/blob/main/readmeai\conf.py)                               | The code snippet provides Pydantic models for configuration constants. It includes configuration models for API, Git repository, Markdown, file paths, prompts, and the overall application. It also provides a helper class for loading and handling configuration files.                                                                                                                                                                                               |
| [factory.py](https://github.com/eli64s/readme-ai/blob/main/readmeai\factory.py)                         | This code snippet provides a Factory Class named "FileHandler" to handle different file I/O operations. It supports reading and writing files of various formats such as JSON, Markdown, TOML, Text, and YAML. It handles exceptions for file read and write operations, and also implements caching for read operations to improve efficiency. The class uses different methods for each file format to perform the read and write operations.                          |
| [logger.py](https://github.com/eli64s/readme-ai/blob/main/readmeai\logger.py)                           | The code snippet provides a custom logger class that allows logging messages at different levels (info, debug, warning, error, critical) with configurable formatting. This class ensures that only one instance of the logger exists.                                                                                                                                                                                                                                   |
| [main.py](https://github.com/eli64s/readme-ai/blob/main/readmeai\main.py)                               | This code is the main entry point for a README-AI application. It sets up the necessary configurations, parses command line options, and orchestrates the README file generation process. It uses an OpenAI model for generating code summaries, slogans, overviews, and features for a given repository. The generated content is then formatted and built into a Markdown file. The code also includes a CLI entry point for running the application.                  |
| [model.py](https://github.com/eli64s/readme-ai/blob/main/readmeai\model.py)                             | This code snippet defines an OpenAI API handler that generates text for a README file. It provides functions to convert code to natural language text and to generate text using prompts and OpenAI's GPT-3. It handles API requests, rate limiting, caching, and error handling.                                                                                                                                                                                        |
| [parse.py](https://github.com/eli64s/readme-ai/blob/main/readmeai\parse.py)                             | The code snippet provides methods for parsing various file formats (such as YAML, TOML, JSON, and more) and extracting dependencies related to different software development tools and languages (e.g., Docker, Conda, Pipenv, Pyproject, Requirements, Cargo, NPM, Yarn, Maven, and more). It relies on regular expressions and library-specific parsing techniques to extract the dependencies.                                                                       |
| [preprocess.py](https://github.com/eli64s/readme-ai/blob/main/readmeai\preprocess.py)                   | The code snippet provides a class for preprocessing a codebase. It incorporates functions to extract unique content and file contents, analyze a local or remote git repository, and generate file information and dependency file contents. It also includes methods to tokenize content and map file extensions to programming languages. The snippet ensures smooth preprocessing of the input codebase.                                                              |
| [utils.py](https://github.com/eli64s/readme-ai/blob/main/readmeai\utils.py)                             | This code snippet provides utility methods for the readme-ai application. It includes functionalities for cloning a repository, extracting information from a GitHub URL, adjusting the maximum number of tokens based on a prompt, counting tokens in a text string, truncating a text string based on the maximum number of tokens, checking the validity of a file and URL, flattening a nested list, formatting generated text, and removing text between HTML tags. |
| [build_image.sh](https://github.com/eli64s/readme-ai/blob/main/scripts\build_image.sh)                  | The provided code snippet builds a Docker image called "readme-ai" and tags it with the version "latest". It then uses Docker Buildx to build the image in both amd64 and arm64 platforms and pushes it to the Docker registry. The final output confirms the successful push of the new image.                                                                                                                                                                          |
| [clean.sh](https://github.com/eli64s/readme-ai/blob/main/scripts\clean.sh)                              | This bash script removes backup files, cache files and directories, VS Code settings, build artifacts, pytest cache, benchmarks, and specific files from the current directory.                                                                                                                                                                                                                                                                                          |
| [run.sh](https://github.com/eli64s/readme-ai/blob/main/scripts\run.sh)                                  | The code snippet activates a Conda environment named "readmeai" and executes a Python script called "main.py" from the "readmeai" package. It also sets the shell option to exit on error, and enables the option to fail fast when a pipeline command fails.                                                                                                                                                                                                            |
| [run_batch.sh](https://github.com/eli64s/readme-ai/blob/main/scripts\run_batch.sh)                      | The code snippet fetches different GitHub repositories, extracts their README content, and saves it into separate markdown files.                                                                                                                                                                                                                                                                                                                                        |
| [test.sh](https://github.com/eli64s/readme-ai/blob/main/scripts\test.sh)                                | This Bash script activates a conda environment, generates a coverage report using pytest, and sets various directories and files to include/exclude. It also removes unwanted files and folders.                                                                                                                                                                                                                                                                         |
| [setup.sh](https://github.com/eli64s/readme-ai/blob/main/setup\setup.sh)                                | This script checks for the existence of a conda environment, installs the "tree" command if not already installed, checks for the presence of Git and Python 3.8+, creates a new conda environment named "readmeai" with the required packages, activates the environment, adds the Python path to PATH, installs the required packages using pip, and finally deactivates the environment. The script also provides informative messages throughout the setup process.  |

</details>

---

## 🚀 Getting Started

### ✔️ Prerequisites

Before you begin, ensure that you have the following prerequisites installed:
> - `ℹ️ Requirement 1`
> - `ℹ️ Requirement 2`
> - `ℹ️ ...`

### 📦 Installation

1. Clone the readme-ai repository:
```sh
git clone https://github.com/eli64s/readme-ai
```

2. Change to the project directory:
```sh
cd readme-ai
```

3. Install the dependencies:
```sh
pip install -r requirements.txt
```

### 🎮 Using readme-ai

```sh
python main.py
```

### 🧪 Running Tests
```sh
pytest
```

---


## 🗺 Roadmap

> - [X] `ℹ️  Task 1: Implement X`
> - [ ] `ℹ️  Task 2: Refactor Y`
> - [ ] `ℹ️ ...`


---

## 🤝 Contributing

Contributions are always welcome! Please follow these steps:
1. Fork the project repository. This creates a copy of the project on your account that you can modify without affecting the original project.
2. Clone the forked repository to your local machine using a Git client like Git or GitHub Desktop.
3. Create a new branch with a descriptive name (e.g., `new-feature-branch` or `bugfix-issue-123`).
```sh
git checkout -b new-feature-branch
```
4. Make changes to the project's codebase.
5. Commit your changes to your local branch with a clear commit message that explains the changes you've made.
```sh
git commit -m 'Implemented new feature.'
```
6. Push your changes to your forked repository on GitHub using the following command
```sh
git push origin new-feature-branch
```
7. Create a new pull request to the original project repository. In the pull request, describe the changes you've made and why they're necessary.
The project maintainers will review your changes and provide feedback or merge them into the main branch.

---

## 📄 License

This project is licensed under the `ℹ️  INSERT-LICENSE-TYPE` License. See the [LICENSE](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository) file for additional info.

---

## 👏 Acknowledgments

> - `ℹ️  List any resources, contributors, inspiration, etc.`

---
