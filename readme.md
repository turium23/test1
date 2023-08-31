
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ AutoDoc-ChatGPT: Revolutionizing Technical Documentation</h3>
<h3>◦ Developed with the software and tools listed below.</h3>

<p align="center">
<img src="https://img.shields.io/badge/JavaScript-F7DF1E.svg?style&logo=JavaScript&logoColor=black" alt="JavaScript" />
<img src="https://img.shields.io/badge/Python-3776AB.svg?style&logo=Python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/TypeScript-3178C6.svg?style&logo=TypeScript&logoColor=white" alt="TypeScript" />
<img src="https://img.shields.io/badge/Markdown-000000.svg?style&logo=Markdown&logoColor=white" alt="Markdown" />
</p>
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

The AutoDoc-ChatGPT project provides a way to generate code documentation using an AI-powered chatbot. The project's core functionality includes dividing code into manageable parts, connecting to the chatbot API to generate comments for each part, and merging the comments with the original code. The purpose of the project is to automate the documentation process, saving time and effort for developers. The value proposition lies in the ability for developers to quickly and easily generate comprehensive code documentation without the need for extensive manual work.

---

## ⚙️ Features

| Feature                | Description                                                                                     |
| ---------------------- | ----------------------------------------------------------------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular architecture, dividing functionality into separate modules.       |
| **📖 Documentation**   | The codebase has descriptive inline comments that explain the purpose and functionality of each component.                         |
| **🔗 Dependencies**    | The codebase relies on external libraries such as Colorama for color and style constants.                                |
| **🧩 Modularity**      | The codebase is organized into smaller, interchangeable modules that handle specific tasks such as code division, file handling, and result processing. |
| **✔️ Testing**          | The codebase does not have information about testing strategies or tools.                                    |
| **⚡️ Performance**      | Since there is no performance information provided, the performance characteristics are unknown. |
| **🔐 Security**        | There is no mention of specific security measures in the codebase.                                   |
| **🔀 Version Control** | The codebase uses Git for version control.                                                          |
| **🔌 Integrations**    | The codebase integrates with ChatGPT to generate code documentation through a conversation with a chatbot. |
| **📶 Scalability**     | The codebase does not provide information regarding scalability aspects.                          |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| main.py                | The code snippet configures and executes a console application called AutoDoc. It uses ChatGPT to generate code documentation for a specified Python file. The application takes inputs through command-line arguments and reads configurations from a config.ini file. It checks if the specified code file exists, creates an AutoDoc instance, generates documentation, and creates a new file with comments based on the generated documentation.                                                                         |
| autodoc.py             | The code snippet is a part of an AutoDoc program. It allows users to generate comments for code based on a conversation with a chatbot. It divides the code into multiple parts, connects to the chatbot, generates comments using the chatbot, and merges the comments with the original code. The resulting commented code is returned.                                                                                                                                                                                     |
| divider.py             | The provided code snippet defines the "Divider" class, which is responsible for dividing a text into smaller portions based on specified start and end patterns. It uses regular expressions to identify the start and end positions of each portion in the text for a given language. The divided portions are stored in the "__splitted_content" list and returned as a result.                                                                                                                                             |
| file.py                | This code snippet defines a class called "File" that represents a file on the file system. It has functionality to retrieve the file's content, determine its language based on the file extension, and create a commented version of the file by adding a suffix to its name.                                                                                                                                                                                                                                                |
| prompt.py              | The code snippet defines a class "Prompt" that takes a language and text as input. It has a "create" method that reads a file based on the language and replaces the placeholder "CODE" with the provided text. The method returns the modified content as a string.                                                                                                                                                                                                                                                          |
| result.py              | The provided code snippet defines a Result class with methods to process and modify code comments in Python and JavaScript/TypeScript. It uses regular expressions to identify comment sections within the code and extracts the comments. The comments are then formatted and added back to the code.                                                                                                                                                                                                                        |
| settings.py            | The provided code snippet defines various color and style constants from the Colorama library. It also defines the supported languages and regular expressions to divide code blocks based on language-specific patterns.                                                                                                                                                                                                                                                                                                     |
| example_commented.js   | The code defines a User class with a name property. It has a constructor to initialize the name, and a method to get the user's name. It also creates an instance of User with the name'John' and checks if it is an instance of the User class.                                                                                                                                                                                                                                                                              |
| autodoc_commented.py   | The provided code snippet defines a class called AutoDoc that generates comments for code using an AI-powered chatbot. The class takes a session token, code to generate comments for, language of the code, and an optional example code. It initializes the instance with the provided inputs and sends code prompts to the chatbot API to generate comments for each part of the code. The comments and the original code are merged to create commented code. The start() method executes the comment generation process. |
| divider_commented.py   | Exception:                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| file_commented.py      | The provided code snippet defines a File class that represents a file object. It has functionalities to retrieve the file's content and language, and create a new file with commented content. The class includes methods such as content(), language(), and create_commented_file(). The class is dependent on the os module for file operations.                                                                                                                                                                           |
| prompt_commented.py    | This code snippet defines a Prompt class that generates prompts for coding exercises in a specified programming language. It takes in the language, code, and an optional example text as arguments. It provides a create() method that generates a prompt string by replacing placeholders in a template file with the code and example text. The prompt can be customized for different languages by using language-specific template files.                                                                                |
| result_commented.py    | The code snippet provides a Result class that represents a code result. It takes in code, text comment, and language as arguments. The get() method returns a modified version of the code with the text comments included as docstrings for the appropriate class and function definitions in Python code. The __py() method handles the parsing and modification of the Python code.                                                                                                                                        |
| settings_commented.py  | The provided code snippet defines a `Settings` class that stores the settings for a program. It has a `supported_languages` variable which is a list of supported languages, currently only containing "py" (Python).                                                                                                                                                                                                                                                                                                         |
| example_2_commented.ts | The code snippet is a TypeScript class that creates and starts an HTTP server, handling GET requests. It allows defining custom response and error handling functions.                                                                                                                                                                                                                                                                                                                                                        |
| example_commented.ts   | The code defines a Pizza class with a constructor to initialize its name and toppings. It also defines a PizzaMaker class with a static method that creates a new Pizza object using the provided name and toppings. The final code snippet uses the PizzaMaker class to create a new Pizza object named "Inferno" with toppings "cheese" and "peppers".                                                                                                                                                                      |

</details>

---

## 🚀 Getting Started

### ✔️ Prerequisites

Before you begin, ensure that you have the following prerequisites installed:
> - `ℹ️ Requirement 1`
> - `ℹ️ Requirement 2`
> - `ℹ️ ...`

### 📦 Installation

1. Clone the AutoDoc-ChatGPT repository:
```sh
git clone F:\autoapi\AutoDoc-ChatGPT
```

2. Change to the project directory:
```sh
cd AutoDoc-ChatGPT
```

3. Install the dependencies:
```sh
pip install -r requirements.txt
```

### 🎮 Using AutoDoc-ChatGPT

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
