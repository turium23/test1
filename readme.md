<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>test1
</h1>
<h3>◦ Test1: Unleash the power of seamless collaboration.</h3>
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

The project consists of two main functionalities. The first one is a codebase for a "T5 Vicuna" model, which includes parameters, VRAM usage, model hubs, default configuration, and an example for generating a travel blog post. The second functionality is a console application that uses AI to automatically generate documentation from code files. It extracts documentation using the AutoDoc module and adds the resulting documentation as comments in the code file. This project provides a convenient way to generate documentation using AI, saving time and effort for developers.

---

## ⚙️ Features

| Feature                | Description                                                                                                                                                                                                                       |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **⚙️ Architecture**     | The codebase adopts a modular design, with separate modules for different functionalities such as T5 Vicuna model, AutoDoc module, Divider class, File class, Prompt class, Result class, and Settings class.                            |
| **📖 Documentation**   | The documentation of the codebase is informative and comprehensive. Each file contains a summary of its purpose and functionality. However, the codebase does not have extensive inline comments or detailed explanations within the code. |
| **🔗 Dependencies**    | The codebase relies on various external libraries including Transformers, PyTorch, Tokenizers, ChatGPTAPI, Regex, and Colorama. These libraries provide necessary functionalities for training models, file operations, and text processing. |
| **🧩 Modularity**      | The codebase is well-organized into separate modules, allowing easy interchangeability and reusability of components. Each module has a clear purpose and encapsulates specific functionality.                                        |
| **✔️ Testing**          | The codebase does not mention specific testing strategies or tools. to ensure the system's reliability and robustness. Additional testing documentation, such as unit tests, would be beneficial to ensure quality assurance.               |
| **⚡️ Performance**      | The performance of the system depends on external dependencies, such as Transformers and PyTorch, which are highly optimized for efficient computation and resource usage. The provided code does not have specific optimizations at the code level.    |
| **🔐 Security**        | The codebase does not implement specific security measures. However, as the system mainly deals with code documentation generation and model training, strict security measures might not be the primary concern.                              |
| **🔀 Version Control** | The codebase adopts Git as the version control system, utilizing features like commit history, branching, and merging. This allows for effective collaboration among developers and easy tracking of code changes and improvements.                     |
| **🔌 Integrations**    | The codebase interacts with external systems such as Transformers, PyTorch, and ChatGPTAPI to support model training and code documentation generation. The integration with external libraries occurs through Python import statements.                        |
| **📶 Scalability**     | The system's scalability depends on the underlying architecture and the use of external libraries. Transformer models can handle large volumes of data and scale efficiently. However, the specific scalability of this codebase is not explicitly stated. |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                                                                                           | Summary                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ---                                                                                            | ---                                                                                                                                                                                                                                                                                                                                                                                                                          |
| [t5_vicuna_3b.py](https://github.com/turium23/test1/blob/main/t5_vicuna_3b.py)                 | The code provides details about "T5 Vicuna"-a model fine-tuned on the "ShareGPT" dataset in the "Vicuna style" using the "Flan-T5-XL" base. It includes parameters, VRAM usage, model hubs, default config, and a travel blog post generation example.                                                                                                                                                                       |
| [main.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\main.py)                 | This code is a console application for generating code documentation using ChatGPT. It takes a code file as input and uses the AutoDoc module to extract documentation using AI. The resulting documentation is added as comments in the code file.                                                                                                                                                                          |
| [autodoc.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\autodoc.py)   | Exception:                                                                                                                                                                                                                                                                                                                                                                                                                   |
| [divider.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\divider.py)   | The code defines a class named Divider that splits a given text based on specific patterns defined for different languages. The __init__ method initializes the text and language properties, while the divide method uses regular expressions to find start and end patterns in the text and splits it accordingly. The resulting splits are stored in the __splitted_content list, which is returned by the divide method. |
| [file.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\file.py)         | This code defines a File class that allows users to perform operations on files. It can retrieve the content of a file, determine its language, and create a new commented file with the given content.                                                                                                                                                                                                                      |
| [prompt.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\prompt.py)     | The code defines a Prompt class that takes a language and text as parameters. It has a create method that opens a text file based on the language parameter, replaces "CODE" with the text parameter, and returns the updated content.                                                                                                                                                                                       |
| [result.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\result.py)     | This code provides a Result class that takes in code, text comments, and a language. It uses regular expressions to extract comments and inserts them into the code based on language-specific formatting. For Python, it adds comments as docstrings, while for TypeScript and JavaScript, it adds comments as block comments.                                                                                              |
| [settings.py](https://github.com/turium23/test1/blob/main/AutoDoc-ChatGPT\modules\settings.py) | The code utilizes the colorama package for colored output. It defines constants for different colors and text styles. The Settings class contains a list of supported programming languages and regex patterns to identify the start and end points of code blocks in each language.                                                                                                                                         |

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
