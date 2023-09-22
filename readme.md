
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>test1
</h1>
<h3>◦ Test1: Celebrating Innovation One Commit at a Time!</h3>
<h3>◦ Developed with the software and tools listed below.</h3>

<p align="center">
<img src="https://img.shields.io/badge/Python-3776AB.svg?style&logo=Python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/Markdown-000000.svg?style&logo=Markdown&logoColor=white" alt="Markdown" />
<img src="https://img.shields.io/badge/JSON-000000.svg?style&logo=JSON&logoColor=white" alt="JSON" />
</p>
<img src="https://img.shields.io/github/languages/top/turium23/test1?style&color=5D6D7E" alt="GitHub top language" />
<img src="https://img.shields.io/github/languages/code-size/turium23/test1?style&color=5D6D7E" alt="GitHub code size in bytes" />
<img src="https://img.shields.io/github/commit-activity/m/turium23/test1?style&color=5D6D7E" alt="GitHub commit activity" />
<img src="https://img.shields.io/github/license/turium23/test1?style&color=5D6D7E" alt="GitHub license" />
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

The project leverages GPT-3 chatbot capabilities to automatically generate comments for code, providing an English-language understanding of the program's functionality. It comprises a console application that accepts any python file and feeds it to OpenAI’s ChatGPT API to generate intelligible commentary embedded with the original lines of code. This Auto-Documentation enhances the readability of the code, thereby aiding both novice learners and experienced developers in comprehension. Thus, this application offers a valuable proposition for controlled, understandable coding documentation, reducing manual efforts while fostering transparency in programming.

---

## ⚙️ Features

HTTPStatus Exception: 429

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                                                                                           | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ---                                                                                            | ---                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [json_my.json](https://github.com/turium23/test1/blob/main/json_my.json)                       | The provided code snippet represents metadata for various AI models denoted as "t5-vicuna-3b", "camel-5b", and "mpt-7b". Details consist of model attributes (like name, VGA utilization, hub resources), custom generation configurations, and brief descriptions. There's information about performance metrics, thumbnail image URLs. It also showcases example use-cases where details of the individual dialogue pairs are enlisted. |
| [t5_vicuna_3b.py](https://github.com/turium23/test1/blob/main/t5_vicuna_3b.py)                 | This code defines a dictionary for the specification of a machine learning model: "T5 Vicuna". Key parameters include model parameters, VRAM usage for different formats, source repository details, and model thumbnail URLs. Other information includes a general description, the default configuration, and working example. The model is hosted on LMSYS and based on Google's Flan-T5-XL model.                                     |
| [main.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\main.py)                 | This script initiates an AutoDoc console application that employs chatbots to generate documentation for Python files. User-entered configurations are fetched from "config.ini". Users supply a file through a command-line argument. If the file exists, the content and language info are used alongside authenticated tokens to produce documentation. The altered'commented' code file is then outputted.                            |
| [autodoc.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\autodoc.py)   | The script initializes a'ChatGPT' chatbot to auto-generate comments for provided code. It reads the input code and divides it for commenting. The chatbot produces a comment for each piece, getting appended to the original code. Errors are highlighted using color-coded messages. It currently supports multiple languages listed in ‘Settings’.                                                                                     |
| [divider.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\divider.py)   | HTTPStatus Exception: 429                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [file.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\file.py)         | The provided code defines a File class representing a file. This class has methods to open, read content from the file and retrieve the coding language based on its extension. Upon initialization, it normalizes, absolute forms the input path, and separates directory and file information. It can also create a new "commented" version of the file in the same directory.                                                          |
| [prompt.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\prompt.py)     | HTTPStatus Exception: 429                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [result.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\result.py)     | HTTPStatus Exception: 429                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [settings.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\settings.py) | HTTPStatus Exception: 429                                                                                                                                                                                                                                                                                                                                                                                                                 |

</details>

---

## 🚀 Getting Started

### ✔️ Prerequisites

Before you begin, ensure that you have the following prerequisites installed:
> - `ℹ️ Requirement 1`
> - `ℹ️ Requirement 2`
> - `ℹ️ ...`

### 📦 Installation

1. Clone the test1 repository:
```sh
git clone https://github.com/turium23/test1
```

2. Change to the project directory:
```sh
cd test1
```

3. Install the dependencies:
```sh
pip install -r requirements.txt
```

### 🎮 Using test1

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
