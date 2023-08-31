
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ AutoDoc-ChatGPT: Simplifying code documentation effortlessly</h3>
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

The AutoDoc project is a console application that aims to automate code documentation generation using ChatGPT. It takes a code file as input, divides it into parts, and sends each part to a ChatGPT model to generate comments. These comments are then merged with the original code, resulting in commented documentation. This automation saves time and effort for developers by eliminating the need for manual documentation and enhances the overall code understanding for future maintenance and collaboration purposes.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The system follows a modular architecture, with files and modules organized according to their functions. It utilizes a code parsing module and connects to a ChatGPT model for comment generation. |
| **📖 Documentation**   | The codebase has thorough documentation, with comments explaining the functions and purpose of each file and module. The documentation helps in understanding the codebase's functionalities and features. |
| **🔗 Dependencies**    | The system relies on external dependencies such as the ChatGPT model for comment generation. It also utilizes libraries for file handling and code parsing. |
| **🧩 Modularity**      | The codebase is organized into smaller, interchangeable components. Each file/module has a specific functionality and can be used independently, promoting reusability and maintainability. |
| **✔️ Testing**          | The codebase documentation does not mention specific testing strategies or tools. Therefore, the testing strategies/approaches implemented in the project are unknown. |
| **⚡️ Performance**      | No specific performance metrics or benchmarks are mentioned in the documentation. Therefore, a detailed analysis of performance cannot be provided. |
| **🔐 Security**        | The codebase does not include specific security measures mentioned in the documentation. Security measures regarding data protection and maintaining functionality are unknown. |
| **🔀 Version Control** | The codebase utilizes Git for version control. The usage of Git enables tracking changes, collaborative development, and easier code maintenance. |
| **🔌 Integrations**    | The system integrates with the ChatGPT model for comment generation. It also interacts with file handling modules and code parsing modules for processing input code files. |
| **📶 Scalability**     | The scalability of the system, in terms of handling growth, is not mentioned in the documentation. Therefore, a detailed analysis of scalability cannot be provided. |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| main.py                | This code snippet is a console application called AutoDoc. It generates code documentation using ChatGPT. It takes a code file as input and processes it to create commented documentation. It utilizes authentication credentials, reads configuration settings from a file, and interacts with other modules for file handling and code parsing.                                                                                                                                                                                                                                               |
| autodoc.py             | This code snippet is a tool called "AutoDoc" that automatically generates comments for code. It divides the code into parts, connects to a ChatGPT model, sends each part to the model for comment generation, merges the comments with the code, and returns the commented code as output.                                                                                                                                                                                                                                                                                                      |
| divider.py             | The code snippet defines a Divider class with a constructor that takes in a text and language. It divides the text based on predefined start and end patterns specific to the language. The divided portions are stored in the __splitted_content attribute. The divide() method performs the division and returns the divided portions.                                                                                                                                                                                                                                                         |
| file.py                | The code snippet defines a class called "File" which takes a file path as input. It provides functionalities to retrieve the content of the file, determine its language, and create a new file with commented content based on the original file's path.                                                                                                                                                                                                                                                                                                                                        |
| prompt.py              | The code defines a class Prompt that takes in a language and text parameter. It has a create method that reads a file based on the language and replaces the placeholder "CODE" with the given text.                                                                                                                                                                                                                                                                                                                                                                                             |
| result.py              | The code snippet is a class called Result that encapsulates functionality to modify code comments based on regular expressions and language-specific rules. It has methods to process Python (py) and TypeScript or JavaScript (ts/js) comments, extracting specific comment sections and inserting them as code comments in the appropriate format. The get method determines the language and calls the respective private method. The code modification involves finding specific comment sections, extracting them, and inserting them as code comments. The modified code is then returned. |
| settings.py            | This code provides settings for highlighting and categorizing code snippets based on supported languages and division points (start and end). It includes color codes for styling output.                                                                                                                                                                                                                                                                                                                                                                                                        |
| example_commented.js   | The code snippet defines a User class with a name property. The class has a constructor to set the name and a function to retrieve the name. It also creates an instance of the User class, assigns a name to it, and verifies if it is an instance of the User class.                                                                                                                                                                                                                                                                                                                           |
| autodoc_commented.py   | The provided code is for a class called AutoDoc, which generates comments for a given code using an AI-powered chatbot. It takes a code string, a language string, and a token string as input. The code uses the RevChatGPT API to communicate with the chatbot. The start() method divides the code into parts, connects to the chatbot, generates comments for each part, and then merges the comments with the original code. The commented code is returned as a string.                                                                                                                    |
| divider_commented.py   | This code snippet defines a class called "Divider" that takes a text string and a language string. It includes a method called "divide()" that splits the text into sections based on language-specific separators. Currently, it only supports splitting Python code based on class and function definitions. The resulting sections are stored in a list and returned.                                                                                                                                                                                                                         |
| file_commented.py      | The provided code snippet contains a `File` class that represents a file object. It has methods to retrieve the content and language of the file, as well as create a new file with commented content. The `__init__` method initializes the file object with a given path. The `content` method retrieves the content of the file. The `language` method retrieves the language of the file. The `create_commented_file` method creates a new file with the commented content.                                                                                                                  |
| prompt_commented.py    | The provided code snippet is a class called "Prompt" which generates prompts for coding exercises in a specific programming language. It takes in the language, code text, and an optional example text as input. The "create" method generates the prompt by replacing placeholders in a template file with the code and example text.                                                                                                                                                                                                                                                          |
| result_commented.py    | This code snippet defines a class called "Result" that represents a code result with its associated text comment and language. The "Result" class has a method called "get()" that returns a modified version of the code with the text comments included as docstrings for the appropriate class and function definitions in the code, specifically for the Python language.                                                                                                                                                                                                                    |
| settings_commented.py  | The provided code defines a `Settings` class that stores the settings for a program. It has a variable `supported_languages` which is a list containing supported languages. It doesn't have any defined functions.                                                                                                                                                                                                                                                                                                                                                                              |
| example_2_commented.ts | This code snippet defines a Server class that utilizes the http module to create an HTTP server. It handles GET requests and passes the request body to a specified response function. The server can be started by calling the listen method and providing a port number.                                                                                                                                                                                                                                                                                                                       |
| example_commented.ts   | The provided code snippet includes two classes:'Pizza' and'PizzaMaker'. The'Pizza' class represents a pizza object and has properties like name and toppings. The'PizzaMaker' class has a static method,'create', which creates a new pizza object using the'Pizza' class. The code snippet then creates a new pizza object ('Inferno') using the'PizzaMaker' class.                                                                                                                                                                                                                             |

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
