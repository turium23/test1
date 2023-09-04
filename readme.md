<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>test1
</h1>
<h3>◦ Breaking barriers, testing limits with test1!</h3>
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

The project consists of code and utilities for generating code documentation using an AI model called ChatGPT. It offers tools for dividing code into parts, connecting to the ChatGPT model to generate comments, and merging the comments with the code. The project aims to automate and streamline the process of adding code comments, saving developers time and effort in documenting their code. Its value proposition lies in its ability to quickly generate meaningful and informative comments that enhance code readability and maintainability.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular architecture, with separate modules for different functionalities like T5 Vicuna configuration, code generation using ChatGPT, code commenting, and file manipulation. It is organized into small, interchangeable components.   |
| **📖 Documentation**   | The codebase is well-documented, providing detailed descriptions of each file's purpose and functionality. Comments are included within the code files for better understanding. The README file provides an overview of the project and its usage.   |
| **🔗 Dependencies**    | The project relies on external libraries like TensorFlow, Flax, and transformers for T5 Vicuna model configuration and fine-tuning. It also uses ChatGPT as an external service for code documentation generation.   |
| **🧩 Modularity**      | The codebase is highly modular, separating different functionalities into separate modules. These modules are designed to be interchangeable and reusable, providing flexibility and maintainability.   |
| **✔️ Testing**          | The codebase does not include explicit information on testing strategies or tools. It is recommended to implement automated testing to ensure software quality and stability.   |
| **⚡️ Performance**      | Performance cannot be analyzed based solely on the codebase. However, using pre-trained models like T5 Vicuna and ChatGPT may result in high computational and memory requirements. Optimization techniques like model quantization could be considered.   |
| **🔐 Security**        | The codebase does not explicitly address security measures. However, it is essential to ensure user data confidentiality and prevent unauthorized access, especially when interacting with external services like ChatGPT.   |
| **🔀 Version Control** | The codebase is hosted on GitHub, utilizing Git as the version control system. This enables collaboration, change tracking, and easy code sharing. Branches and pull requests can be used for efficient code review and integration.   |
| **🔌 Integrations**    | The codebase integrates with ChatGPT as an external service for code documentation generation. It demonstrates a smooth integration between the AutoDoc tool and ChatGPT model.   |
| **📶 Scalability**     | Scalability depends on the infrastructure used to deploy and serve the codebase. T5 Vicuna and ChatGPT models can handle increased workload by using distributed computing and load balancing techniques. However, the codebase itself does not include specific scalability measures.   |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                                                                                           | Summary                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ---                                                                                            | ---                                                                                                                                                                                                                                                                                                                                                                                                                            |
| [t5_vicuna_3b.py](https://github.com/turium23/test1/blob/main/t5_vicuna_3b.py)                 | The code provides information and configuration details for the T5 Vicuna model, including its category, display name, thumbnails, parameters, VRAM usage, base and checkpoint hubs, default configuration file, and description. It also includes an example of generating an engaging travel blog post using the model. This code supports fine-tuning based on Google's Flan-T5-XL and is curated by LMSYS in Vicuna style. |
| [main.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\main.py)                 | This code is a console application that generates code documentation using ChatGPT. It takes a code file as input and generates comments based on the code's functionality. The comments are then added to the code file itself.                                                                                                                                                                                               |
| [autodoc.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\autodoc.py)   | This code is an AutoDoc tool that generates comments for code snippets. It divides the code into parts, connects to a ChatGPT model for generating comments, and then merges the comments with the code. The tool supports multiple programming languages and requires authentication with session token or login details. It provides a simple command-line interface for the user.                                           |
| [divider.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\divider.py)   | This code defines a class called "Divider" which is used to split a given text into smaller parts based on specific patterns defined in the Settings module. It uses regular expressions to find the start and end positions of the dividing patterns in the text. The split parts are stored in a list and returned as the output.                                                                                            |
| [file.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\file.py)         | The code defines a File class with functionalities to get file content, extract language, and create a commented duplicate file with modified content.                                                                                                                                                                                                                                                                         |
| [prompt.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\prompt.py)     | The code defines a Prompt class with an initializer that takes a language and text. The create method reads a file based on the language, replaces "CODE" with the text, and returns the updated content as a string.                                                                                                                                                                                                          |
| [result.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\result.py)     | This code defines a class called "Result" that takes code, text comment, and language as input. The "get" method returns modified code based on the language. For Python, it extracts names and comments from the text comment and inserts them as docstrings. For TS/JS, it appends comments above the corresponding code blocks.                                                                                             |
| [settings.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\settings.py) | The code imports necessary modules and declares variables with color templates. It also contains a Settings class with supported languages and divide patterns for extraction.                                                                                                                                                                                                                                                 |

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
