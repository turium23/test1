
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>test1
</h1>
<h3>◦ Transform code testing with test1: Simplify, accelerate, excellence.</h3>
<h3>◦ Developed with the software and tools listed below.</h3>

<p align="center">
<img src="https://img.shields.io/badge/Python-3776AB.svg?style&logo=Python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/JSON-000000.svg?style&logo=JSON&logoColor=white" alt="JSON" />
<img src="https://img.shields.io/badge/Markdown-000000.svg?style&logo=Markdown&logoColor=white" alt="Markdown" />
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

The project contains code for two main functionalities-a T5 model called "T5 Vicuna" for generating engaging blog posts about travel destinations in a specific style, and an AutoDoc console application for generating code documentation using ChatGPT. The T5 Vicuna model is based on Google's Flan-T5-XL and provides the ability to generate responses in the Vicuna style using parameters and fine-tuning on a ShareGPT dataset. The AutoDoc application automates code documentation by splitting the provided code into parts, connecting to a ChatGPT model, and generating comments for each part, resulting in a new file with the generated documentation comments. These functionalities add value by simplifying the process of generating content for travel blogs and automating the code documentation process for developers.

---

## ⚙️ Features

| Feature                | Description                                                           |
|------------------------|-----------------------------------------------------------------------|
| **⚙️ Architecture**     | The system follows a modular architecture with clear separation of concerns using different modules for code generation, text division, file operations, and prompt handling. The architecture promotes code reusability and maintainability.                                          |
| **📖 Documentation**   | The repository lacks comprehensive documentation. The existing file summaries provide some insight, but additional documentation, such as README files or inline comments, would improve the ease of understanding the codebase.                                            |
| **🔗 Dependencies**    | The codebase relies on external libraries `colorama` for text color and style formatting in settings, and `beautifulsoup4` for parsing and manipulating HTML in some additional files which are dependent on `prompt.py`.                                                |
| **🧩 Modularity**      | The system is well-organized into smaller modules, each handling a specific part of the code generation process. This modularity facilitates code reuse, testability, and debuggability.                                                               |
| **✔️ Testing**          | The system does not have any explicit testing strategy or tools mentioned. The implementation would benefit from having test suites to ensure code correctness and prevent regressions.                                                                    |
| **⚡️ Performance**      | The performance of the system depends on the underlying machine's capabilities, such as available memory, processing power, and network connection. No specific optimizations have been implemented in the code regarding performance.          |
| **🔐 Security**        | The codebase does not have explicit security measures implemented. Handling secure data or ensuring application security should be considered as an additional implementation aspect.                                                           |
| **🔀 Version Control** | Git is used as the version control system. It allows collaborative development, tracks changes in the codebase, and enables versioning and rollback if needed. The repo provides access control with user permission management.             |
| **🔌 Integrations**    | The system does not have any direct integrations mentioned. However, it can be extended and integrated with other systems through the code generation and file processing capabilities provided.                                    |
| **📶 Scalability**     | The codebase does not explicitly address scalability concerns. The system's scalability will largely depend on the resources available to handle increased traffic, input size, and demand. Scalability improvements can be added based on specific requirements.    |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                                                                                           | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ---                                                                                            | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| [json_my.json](https://github.com/turium23/test1/blob/main/json_my.json)                       | HTTPStatus Exception: 400                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [t5_vicuna_3b.py](https://github.com/turium23/test1/blob/main/t5_vicuna_3b.py)                 | The provided code snippet describes a T5 model called "T5 Vicuna," categorized as "<10B." It includes parameters, VRAM values, and Hub information. The model is based on Flan-T5-XL from Google and fine-tuned on ShareGPT dataset curated by LMSYS. Its purpose is to generate responses in the Vicuna style. An example travel blog post about Hawaii is provided as an illustration. The model's core functionalities involve generating engaging blog posts and responses in the specified style. |
| [main.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\main.py)                 | This code snippet is a console application called AutoDoc, designed to generate code documentation using ChatGPT. It reads a configuration file, authenticates with ChatGPT using provided credentials, takes a code file as input, checks if it exists, creates an AutoDoc instance with the file's content and language, executes the documentation generation process, and finally creates a new file with the generated documentation comments.                                                    |
| [autodoc.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\autodoc.py)   | This code snippet sets up an AutoDoc class that generates comments for code. It divides the code into parts, connects to a ChatGPT model, and generates comments for each part. Finally, it merges the comments with the code to produce commented code.                                                                                                                                                                                                                                               |
| [divider.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\divider.py)   | The provided code snippet is a class called `Divider` that is used to split a given text based on the start and end patterns defined in a settings file. The `divide()` method searches for these patterns using regular expressions and divides the text accordingly. The split sections are stored in the `__splitted_content` list and returned as the result.                                                                                                                                      |
| [file.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\file.py)         | The code snippet defines a File class that represents a file on the system. It provides methods to retrieve the file's content, determine its language, and create a new commented version of the file. The class uses the os module to perform operations on the file system like getting file paths and reading/writing file content.                                                                                                                                                                |
| [prompt.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\prompt.py)     | This code defines a class that represents a prompt. It takes in a language and text as input and provides a create method that replaces the placeholder "CODE" in a file associated with the given language with the provided text, returning the updated content as a string.                                                                                                                                                                                                                         |
| [result.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\result.py)     | The provided code snippet defines a class `Result` with three private attributes: `code`, `text_comment`, and `language`. The `get` method returns modified code based on the language. In the `__py` method, the code is processed to add comments extracted from the text_comment using specific formatting for Python. In the `__ts` method, comments are added to the code using a different formatting approach for TypeScript and JavaScript.                                                    |
| [settings.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\settings.py) | The code snippet defines various text colors and styles using the colorama library. It also defines a Settings class with supported languages and regex patterns to identify code sections based on language.                                                                                                                                                                                                                                                                                          |

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
