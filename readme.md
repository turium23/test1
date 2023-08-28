
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ AutoDoc-ChatGPT: Revolutionizing documentation with AI!</h3>
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

The AutoDoc-ChatGPT project is a console application that uses a chatbot AI called ChatGPT to generate code documentation. By providing a code file path as input, the program divides the code into sections and sends prompts to ChatGPT to generate relevant comments for each section. The generated comments are then inserted as documentation in the original code file. The project's core functionality lies in automating the tedious task of writing code documentation, saving developers time and effort while ensuring comprehensive and accurate documentation for their code.

---

## ⚙️ Features

| **Feature**           | **Description** |
|-------------------------|------------------------------------|
| **⚙️ Architecture**     | The system follows a modular architecture, with separate modules for code manipulation, text processing, file operations, and interacting with the ChatGPT service. It uses classes and functions to encapsulate functionality, allowing for easy extension and reusability. |
| **📖 Documentation**   | The codebase includes comments and docstrings to explain the purpose and functionality of different components. However, there is scope for improvement in terms of more comprehensive and structured documentation. |
| **🔗 Dependencies**    | The system relies on external libraries such as colorama and the os module for certain functionalities. Additionally, it interacts with the ChatGPT service for generating comments.|
| **🧩 Modularity**      | The system is divided into various modules, each responsible for a specific functionality. It allows for separate development and maintenance of different components, making the codebase more organized and modular. |
| **✔️ Testing**          | The codebase does not explicitly mention testing. It might be beneficial to add automated tests to ensure the correctness and robustness of the code. |
| **⚡️ Performance**      | As the system interacts with external services like the ChatGPT API and involves file operations, performance primarily depends on the response time of these external services and the size of input files. The system does not explicitly mention any performance optimization strategies. |
| **🔐 Security**        | The codebase does not implement any explicit security measures. It might be crucial to validate user input, check for file and API access permissions and potentially sanitize code inputs to prevent potential security vulnerabilities. |
| **🔀 Version Control** | The codebase is version-controlled using Git, which helps track changes, collaborate, and facilitate code maintenance. It allows developers to work concurrently on different branches and efficiently manage code versions. |
| **🔌 Integrations**    | The system integrates with the ChatGPT service to generate comments for code documentation. It likely requires a secure API key or authentication mechanism to access the service. |
| **📶 Scalability**     | The system's scalability capability depends on external services like the ChatGPT API and the underlying infrastructure that stores and runs the codebases. If these systems can handle a large volume of requests, the system should be able to scale effectively. |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| main.py                | This code snippet is a console application called AutoDoc. It generates code documentation using ChatGPT and supports Python language. It takes a code file path as input, checks if the file exists, reads the file content, and starts generating documentation using the ChatGPT service. The generated documentation is then saved by creating commented lines in the original file.                                                                                                                                                                                                                                                                                            |
| autodoc.py             | This code snippet is for an Auto Documentation tool. It takes in a configuration, code, and programming language as inputs. It divides the code into parts, connects to a ChatGPT chatbot, generates comments for each part of the code using the chatbot, and merges the comments back into the code. The tool provides an automated way to generate comments for code documentation.                                                                                                                                                                                                                                                                                              |
| divider.py             | This code defines a class called "Divider" that splits a given text based on predefined start and end patterns. It uses regular expressions and a settings module to determine the split points. The resulting split content is stored in a list and returned as the output.                                                                                                                                                                                                                                                                                                                                                                                                        |
| file.py                | The code snippet defines a class for manipulating files. It provides methods for getting file content, getting the file's language, and creating a new file with commented content. The class uses the os module for file operations.                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| prompt.py              | The code snippet defines a class called Prompt that takes a language and text as inputs. It has a create() method that opens a file specific to the language and replaces placeholder text with the provided code text. The method returns the modified text as a string.                                                                                                                                                                                                                                                                                                                                                                                                           |
| result.py              | This code snippet defines a Result class that takes code, text comments, and a language as input. The'get' method returns a modified version of the code with comments inserted as documentation. The code handles both Python and TypeScript/JavaScript languages, extracting comments surrounded by'| |' delimiters and inserting them as comments or docstrings in the code.                                                                                                                                                                                                                                                                                                     |
| settings.py            | The code snippet imports colorama for colored output and defines constants for various colors and styles. It includes a Settings class that contains supported languages and patterns for dividing code sections.                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| example_commented.js   | The code snippet defines a User class that represents a user with a name property. It has a constructor that takes in a name and creates a new User instance with that name. The getName method returns the name of the user. An instance of User class is created with the name'John'. The user's name is retrieved via the getName method. Lastly, instanceof is used to check if the user object is an instance of the User class.                                                                                                                                                                                                                                               |
| autodoc_commented.py   | The provided code snippet is an implementation of a class called AutoDoc that generates comments for a given code using an AI-powered chatbot. It takes a session token, code, language, and an optional example as arguments. It uses the chatbot API to send prompts and obtain responses for generating comments. The __init__ function initializes the AutoDoc instance with the given inputs. The __ask function sends a prompt to the chatbot API and returns the response. The start function divides the code into parts, connects to the chatbot API, generates comments for each part, and merges the comments with the code. The commented code is returned as a result. |
| divider_commented.py   | This code snippet defines a class called Divider that can split a text string into sections based on language-specific separators. It currently supports Python code and splits it based on class and function definitions. The __py method uses regular expressions to find the start and end positions of these definitions and then adds the corresponding sections to a list. The divide method checks the language and calls the appropriate splitting method. The sections are returned as a list of strings.                                                                                                                                                                 |
| file_commented.py      | The provided code snippet defines a File class that represents a file object. It has methods to retrieve the content and language of the file, as well as create a new file with commented content. It uses the os module to handle file paths and operations.                                                                                                                                                                                                                                                                                                                                                                                                                      |
| prompt_commented.py    | The provided code snippet defines a class called "Prompt" that generates prompts for coding exercises in a specified language. The class has a constructor method to initialize the language, code, and optional example text. It also has a method called "create" that generates the prompt using the given language, code, and example text (if provided). The class reads the prompt template from a file and replaces placeholders with the code and example text to create the final prompt.                                                                                                                                                                                  |
| result_commented.py    | This code snippet defines a class called `Result` that represents a code result with its associated text comment and language. It provides a `get()` method that modifies the code by including the text comments as docstrings for the appropriate class and function definitions in Python code.                                                                                                                                                                                                                                                                                                                                                                                  |
| settings_commented.py  | The code defines a settings class to store program settings, with a "supported_languages" variable that holds a list of supported languages.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| example_2_commented.ts | This code snippet is a TypeScript class that creates an HTTP server using the http module. It handles GET requests, parses the request body, and calls functions to handle server response and error. The server can be started by specifying the port number.                                                                                                                                                                                                                                                                                                                                                                                                                      |
| example_commented.ts   | The provided code defines two classes, "Pizza" and "PizzaMaker". The "Pizza" class represents a pizza with a given name and an array of toppings. The "PizzaMaker" class has a static method called "create" that creates a new Pizza object using the given name and toppings. The "const pizza" creates a new Pizza object using the "PizzaMaker" class and provides it with the name "Inferno" and toppings "cheese" and "peppers".                                                                                                                                                                                                                                              |

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
