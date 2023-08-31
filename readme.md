
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ ChatGPT: Automate your documentation! #AutoDocChatGPT</h3>
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

The AutoDoc-ChatGPT project is an automated documentation tool aimed at generating code comments using a language model called ChatGPT. The project allows users to input a code file and a configuration file, then processes the code and generates comments for each part of the code. These comments are merged with the code, creating a commented version. The tool aims to save time and effort by automating the code documentation process, helping developers understand the codebase and improving collaboration.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The system follows a modular architecture where different modules like `autodoc.py`, `divider.py`, `file.py`, `prompt.py`, `result.py`, and `settings.py` handle specific functionality, contributing to a clear separation of concerns and reusability. |
| **📖 Documentation**   | The codebase includes inline comments and docstrings throughout the modules, providing clear explanations of the code's functionality, inputs, and outputs. The documentation ensures code comprehension and enables code maintenance. |
| **🔗 Dependencies**    | The system relies on external libraries for functionalities like pattern matching, file management, and AI-powered chatbot capabilities. The dependencies include the ChatGPT model, regular expressions, and potentially additional libraries specific to the chosen programming language. |
| **🧩 Modularity**      | Each module contains (or represents) distinct entities or functionalities, such as AutoDoc, Divider, File, Prompt, Result, and Settings. This modularity promotes flexibility, code reusability, and easier maintenance or extension of specific components. |
| **✔️ Testing**          | There is no mention of specific testing strategies or tools in the provided information. Additional analysis is required to evaluate the system's testing approach and the presence of test cases or frameworks. |
| **⚡️ Performance**      | Without additional information or direct performance measurement, it is challenging to assess the system's performance. Its efficiency can depend on factors like the size of the codebase, AI model execution time, and network latency if API calls are involved. |
| **🔐 Security**        | The provided codebase details don't mention specific security measures. To ensure data security and functionality, additional analysis involving secure coding practices, input validation, and secure network communication is required. |
| **🔀 Version Control** | The codebase uses Git for version control, as evident from the repository path. Git enables effective collaboration among developers, facilitates change tracking, and provides features like branching, merging, and history management. |
| **🔌 Integrations**    | The integration with the ChatGPT model is a crucial component of the system, enabling code documentation generation. The specific details about the integration mechanism and potential integration with other systems are not provided in the information. |
| **📶 Scalability**     | Limited information is available to evaluate the system's scalability. The system's scalability depends on factors like handling large codebases, managing chatbot API scalability, and potential parallel execution. In-depth analysis is necessary for accurate scalability assessment. |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| main.py                | This code snippet reads a configuration file, takes user input for a code file, and generates code documentation using ChatGPT, storing the documentation as comments in the code file.                                                                                                                                                                                                                                                                                      |
| autodoc.py             | This code snippet is for an Auto Documentation tool. It takes in code, config, and language as input. It divides the code into parts, connects to a ChatGPT model, and generates comments for each part. Finally, it merges the comments with the code to create a commented version of the code.                                                                                                                                                                            |
| divider.py             | The code defines a class called Divider, which takes in a text and language. It uses regular expressions to find specific patterns for dividing the text into sections. The dividing rules are specified in the Settings module. The divided sections are stored in a list and returned.                                                                                                                                                                                     |
| file.py                | The code provides a class called File that manages file path, directory, basename, and language. It can read file content, retrieve the language, and create a commented version of the file.                                                                                                                                                                                                                                                                                |
| prompt.py              | The code snippet defines a class called "Prompt" with an init method and a create method. The init method initializes the object with a language and text parameter. The create method reads a file using the language parameter and replaces a placeholder with the text parameter. It returns the modified text as output.                                                                                                                                                 |
| result.py              | This code snippet defines a class Result with three private attributes: code, text_comment, and language. The class has a get() method that returns modified code based on the language specified. If the language is "py", it replaces specific text comments in the code with corresponding descriptions. If the language is "ts" or "js", it adds comments to the code based on the specified names and comments in the text_comment. The modified code is then returned. |
| settings.py            | The code snippet provides color schemes and regular expressions for supported programming languages. It defines start patterns for class and function definitions and end patterns for each language. These settings can be used to divide code into smaller sections based on language-specific patterns.                                                                                                                                                                   |
| example_commented.js   | The code defines a User class that represents a user with a name property. The class has a constructor that accepts a name parameter and sets it as the user's name. The class also has a method called getName() that returns the user's name. An instance of the User class is created with the name'John' and its getName() method is called. The code also checks if the user instance is an instance of the User class.                                                 |
| autodoc_commented.py   | The provided code snippet is a Python class called AutoDoc. It utilizes an AI-powered chatbot to generate comments for a given code string. The class takes in a token, code, language, and optional example code as parameters. The code is divided into parts and sent to the chatbot API for generating comments. The comments are then merged with the original code. The start() method initiates the comment generation process.                                       |
| divider_commented.py   | The provided code snippet defines a class called Divider that splits a text string into sections based on language-specific separators. It currently supports Python code division, where it identifies class and function definitions as separators. The divided sections are returned as a list of strings.                                                                                                                                                                |
| file_commented.py      | This code snippet defines a `File` class that represents a file object. It provides methods to retrieve the content and language of the file, as well as create a new file with commented content. The `content` method reads the file's content, the `language` method returns the file's language, and the `create_commented_file` method writes the commented content to a new file.                                                                                      |
| prompt_commented.py    | The code snippet provides a class called `Prompt` that generates prompts for coding exercises in a specified language. It takes in the language, code, and an optional example text as arguments. The `create` method generates the prompt by replacing placeholders in a template file with the provided code and example text.                                                                                                                                             |
| result_commented.py    | The provided code snippet defines a class called "Result" that represents a code result with a text comment and language. The class has a method "get" that modifies the code by including the text comments as docstrings in the appropriate class and function definitions. The modification is specific to Python code and is achieved using regular expressions. The modified code is then returned.                                                                     |
| settings_commented.py  | The provided code snippet defines a class called `Settings` that stores the settings for a program. It has a variable `supported_languages` which is a list containing supported programming languages.                                                                                                                                                                                                                                                                      |
| example_2_commented.ts | This code snippet is a TypeScript class that represents a server by creating an instance of the HTTP server.It handles GET requests, parses the request body, sets the response headers, and calls the provided callback functions for successful and error responses.                                                                                                                                                                                                       |
| example_commented.ts   | The code snippet defines a Pizza class with a constructor that initializes the name and toppings properties. It also includes a PizzaMaker class with a static create method that creates a new Pizza object. The code creates a new Pizza object called "pizza" using the PizzaMaker class with the name "Inferno" and toppings "cheese" and "peppers".                                                                                                                     |

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
