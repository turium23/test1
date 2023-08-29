
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>test1
</h1>
<h3>◦ Building blocks of success – Test1 on GitHub.</h3>
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

The project is an Auto Documenting tool that generates code documentation using ChatGPT. The core functionalities include dividing the code into sections, generating comments for each section with ChatGPT, and merging the comments with the original code. The purpose of the tool is to automate the code documentation process, saving developers time and effort. Its value proposition lies in creating well-commented code files, enhancing code understanding and maintainability.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The system follows a modular architecture with separate modules for different functionalities such as code division, generation of comments, and file handling. The AutoDoc class coordinates the overall execution, interacting with ChatGPT to generate comments. The resulting comments are then merged with the original code. This design promotes code reusability and maintainability.    |
| **📖 Documentation**   | The project has decent documentation, with each file providing a summary of its functionality. However, more detailed documentation explaining the modules, classes, and their methods would improve understanding and ease of use for new developers. Adding docstrings and usage examples will enhance comprehensiveness.    |
| **🔗 Dependencies**    | The system relies on external libraries like ChatGPT for generating code comments and colorama for text coloring. It is essential to mention all the required dependencies explicitly for easy setup and maintenance. The project uses black and flake8 for code formatting and linting, respectively.    |
| **🧩 Modularity**      | The system is well-organized into smaller, interchangeable modules, specifically catering to code division, documentation generation, file handling, and result processing. Each module focuses on a specific aspect and promotes code reuse and readability. Additional features could be added as separate modules to further enhance modularity.    |
| **✔️ Testing**          | The codebase lacks a dedicated testing framework and test cases to validate the behavior of the implemented functionality. The addition of unit tests and integration tests would ensure that the system works as expected and minimize the chance of introducing bugs and regressions. Adoption of popular testing frameworks like pytest or unittest is recommended.    |
| **⚡️ Performance**      | The system's performance can be enhanced by optimizing the code generation process using ChatGPT. By utilizing efficient algorithms and caching, the overall execution time can be reduced. Additionally, performance profiling and monitoring can identify and address any bottlenecks to ensure optimal resource usage.    |
| **🔐 Security**        | The project does not introduce any specific security measures apart from standard file access control. It is crucial to ensure that the system handles user data securely, by implementing proper input validation and optimizing any potential security vulnerabilities.    |
| **🔀 Version Control** | The project is version-controlled using Git, with the codebase hosted on GitHub. Setting up and following best practices for branching, pull requests, and code reviews ensures safe collaboration and easier maintenance. Periodic tagging and release management contribute to better versioning.    |
| **🔌 Integrations**    | The system currently does not have any direct integrations with external services or systems. However, it can be extended to integrate with code collaboration platforms or CI/CD pipelines for efficient documentation generation during the software development process.    |
| **📶 Scalability**     | The system's scalability is limited by the usage of ChatGPT for code comments generation. The performance and scalability of this aspect depend on ChatGPT's capabilities. The addition of distributed processing techniques and scalability improvements in ChatGPT can enhance the system's ability to handle increasing workloads.    |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                                                                                           | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ---                                                                                            | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| [json_my.json](https://github.com/turium23/test1/blob/main/json_my.json)                       | HTTPStatus Exception: 400                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| [main.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\main.py)                 | This code snippet implements an AutoDoc application that generates code documentation using ChatGPT. It reads a config file for authentication details and accepts a code file as input. It checks if the file exists, then creates an AutoDoc instance with authentication and code file details. The AutoDoc generates documentation using ChatGPT and the resulting documentation is saved as comments in the code file.                                                         |
| [autodoc.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\autodoc.py)   | The provided code snippet is a part of an Auto Documenting tool.-It initializes a class AutoDoc with config, code, and language parameters.-Inside the class, it interacts with ChatGPT to generate comments for each part of the divided code.-Then, it merges the comments with the original code to create a commented version.-The start() method handles the overall execution of the tool.                                                                                    |
| [divider.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\divider.py)   | The code defines a class called Divider that splits a given text into sections based on specific start and end patterns defined in the Settings module. The divided sections are stored in a list and returned as the final result.                                                                                                                                                                                                                                                 |
| [file.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\file.py)         | This code snippet defines a File class that represents a file on the system. It can retrieve the content of the file, determine its language, and create a new commented file with the specified content. The file path is normalized and stored as private attributes.                                                                                                                                                                                                             |
| [prompt.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\prompt.py)     | The code snippet defines a Prompt class that takes in a language and a text parameter. It has a create method that reads a file based on the language parameter and replaces "CODE" in the file with the text parameter. The method returns the modified file content as a string.                                                                                                                                                                                                  |
| [result.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\result.py)     | The provided code snippet defines a Result class that processes code comments in Python (py) and TypeScript/JavaScript (ts, js) languages. It extracts comments containing special format and inserts them as code comments within the code. The code uses regular expressions to find comments, extract the necessary information, and modify the code accordingly.                                                                                                                |
| [settings.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\settings.py) | This code snippet defines attributes and regex patterns for different programming languages in the `Settings` class. It imports and sets colorama styles for text coloring. The `supported_languages` attribute stores a list of supported languages. The `divide_start` dictionary defines regex patterns for identifying the start of a code block in each language. The `divide_end` dictionary defines regex patterns for identifying the end of a code block in each language. |

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
