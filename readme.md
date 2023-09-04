
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>test1
</h1>
<h3>◦ test1: Unlocking your coding potential.</h3>
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

The project is primarily focused on generating code documentation using the ChatGPT language model. It accepts a code file as input and creates a commented version of the file with generated documentation for better understanding and maintainability. This functionality adds value by automating the otherwise time-consuming and manual task of documenting code and can improve collaboration and code readability for developers.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The system follows a modular architecture with components organized into separate modules. The architecture promotes code reuse and makes the system extensible. |
| **📖 Documentation**   | Documentation is fairly comprehensive, covering the main functionalities and usage of each component. More details could be provided on configurations and development setup. |
| **🔗 Dependencies**    | The system relies on external libraries such as colorama for syntax highlighting and regular expressions for pattern matching. |
| **🧩 Modularity**      | The system exhibits a good level of modularity with separate modules for code division, file operations, prompt generation, and result processing. Allows for easy maintenance and future enhancements. |
| **✔️ Testing**          | No explicit information on testing strategies or tools. It is recommended to have proper unit tests and possibly integration tests for critical components. |
| **⚡️ Performance**      | Performance is dependent on the underlying hardware and resources. No specific performance optimizations are mentioned in the codebase or documentation. Code efficiency could be further reviewed for potential optimization opportunities. |
| **🔐 Security**        | The codebase does not explicitly mention security measures. The system may benefit from input validation and sanitization to prevent code injection or malicious actions. Access controls and authentication for external services should also be considered. |
| **🔀 Version Control** | Git is used for version control, allowing easy collaboration, branching, and merging. Proper branching and version tagging methodologies could be adopted for more efficient collaboration and release management. |
| **🔌 Integrations**    | The system does not have explicit integrations with external systems or services. However, it could be extended to integrate with additional code analysis tools or external code repositories. |
| **📶 Scalability**     | The system's scalability would depend on factors such as resource availability and code optimization. No specific information is mentioned regarding the scalability of the codebase. Proper architecture and design considerations should be taken into account for handling potential growth. |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                                                                                           | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ---                                                                                            | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| [json_my.json](https://github.com/turium23/test1/blob/main/json_my.json)                       | HTTPStatus Exception: 400                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| [t5_vicuna_3b.py](https://github.com/turium23/test1/blob/main/t5_vicuna_3b.py)                 | The code snippet provides information about the T5 Vicuna model, including its category, display name, thumbnails, parameters, VRAM usage, hub details, default generator configuration, description, and an example prompt and response. The model is fine-tuned based on a Google Flan-T5-XL model and is trained on the ShareGPT dataset in the Vicuna style.                                                                                             |
| [main.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\main.py)                 | This code snippet provides a console application for generating code documentation using ChatGPT. It takes a code file as input and creates a commented file with the generated documentation. The authentication credentials and code file path are provided through command-line arguments.                                                                                                                                                                |
| [autodoc.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\autodoc.py)   | This code snippet initializes an AutoDoc class that generates comments for code snippets. It divides the code into smaller parts, connects to a ChatGPT chatbot, generates comments for each part, and merges the comments with the original code. The result is the commented code.                                                                                                                                                                         |
| [divider.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\divider.py)   | The code defines a class called "Divider" that can divide text into smaller chunks based on language-specific patterns. The "divide" method uses regular expressions to find the start and end points of each chunk. The resulting chunks are stored in the "__splitted_content" list and returned as the output.                                                                                                                                            |
| [file.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\file.py)         | The code snippet defines a File class that represents a file on the system. It provides methods to retrieve the file's content, language, and create a new file with commented content. The class utilizes the os module to manipulate file paths and access file operations such as reading and writing.                                                                                                                                                    |
| [prompt.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\prompt.py)     | The code defines a Prompt class that takes a language and text. It has a create method that reads a model file related to the language, replaces "CODE" with the given text, and returns the modified content.                                                                                                                                                                                                                                               |
| [result.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\result.py)     | This code snippet defines a Result class with an init method to initialize attributes.The get method checks the language and calls the corresponding private method (__py or __ts) to process the code.The __py method uses regex to find specific text patterns in the comments and modify the code accordingly.The __ts method also uses regex to extract comments and adds comment blocks to the code.The modified code is then returned by both methods. |
| [settings.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\settings.py) | This code snippet provides settings for syntax highlighting in various supported programming languages (Python, TypeScript, JavaScript) using colorama. It defines regular expressions to identify the starting and ending points of code segments (e.g., classes, functions) in each language. It also assigns color and style codes for different text elements.                                                                                           |

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
