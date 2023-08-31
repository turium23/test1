
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Smart code docs + friendly chat-bot: AutoDoc-ChatGPT!</h3>
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

The AutoDoc-ChatGPT project is an auto documentation tool that generates comments for code using an AI-powered chatbot. It takes a code file as input and generates comments for each part of the code based on the provided language. The resulting commented code helps developers understand the functionality and purpose of the code more easily and saves them time in writing manual documentation. The project simplifies the process of documenting code, improving code readability and maintainability.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular design pattern with separate modules for different functionalities such as parsing, code generation, and file operations. The AutoDoc module uses a ChatGPT model for generating comments. |
| **📖 Documentation**   | The codebase has comprehensive documentation, providing explanations of each file's purpose and functionality through code comments. |
| **🔗 Dependencies**    | The codebase relies on external dependencies such as Python's `re` module for regular expressions and `pathlib` module for file operations. |
| **🧩 Modularity**      | The system is highly modular, divided into separate components for parsing, generating comments, dividing code, file operations, and retrieving prompts. Components can be easily replaced or extended. |
| **✔️ Testing**          | While the codebase does not have specific information on testing strategies and tools mentioned, the modularity of the system enables easy testing of individual components. Unit tests can be implemented for each module. |
| **⚡️ Performance**      | The system's performance is highly dependent on the efficiency of the ChatGPT model for generating comments. Other operations such as parsing, file operations, and code division are generally standard and efficient. |
| **🔐 Security**        | The codebase does not have explicit security measures mentioned. However, as a static code analysis tool, it is unlikely to have specific security risks unless there are vulnerabilities in the external dependencies. Input validation should be implemented to minimize security risks. |
| **🔀 Version Control** | The codebase is tracked using Git version control, stored on a local repository. Regular commits and branching strategies can be employed to manage changes effectively. |
| **🔌 Integrations**    | The system integrates with a ChatGPT model to generate code comments. It can also integrate with other components of larger software projects to automate the documentation process. |
| **📶 Scalability**     | The codebase is fairly scalable as it can handle different programming languages for generating code comments. It can be extended to support additional languages and integrated with existing codebases of any size. |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| main.py                | The code snippet reads a configuration file, parses command line arguments, checks if a code file exists, and uses an AutoDoc module to generate code documentation. The resulting documentation is then used to create a commented file.                                                                                                                                                                                                                                                                                                                                             |
| autodoc.py             | This code snippet is for an Auto Documentation tool. It takes a code, language, and configuration as input. It divides the code into parts, connects to a ChatGPT model, generates comments for each part using the model, and merges the comments with the code. The output is the commented code.                                                                                                                                                                                                                                                                                   |
| divider.py             | The code defines a class called "Divider" that splits a given text based on specified start and end patterns. It uses regular expressions and settings from module "settings" to identify the divisions. The divided content is stored and returned as a list.                                                                                                                                                                                                                                                                                                                        |
| file.py                | This code snippet defines a class `File` that encapsulates functionalities related to file operations. It can retrieve the file's content, determine its language, and create a new file with additional comments based on the given content.                                                                                                                                                                                                                                                                                                                                         |
| prompt.py              | The provided code snippet defines a class called "Prompt" with two attributes: language and text. It has a create() method that reads a specified file based on the language attribute and replaces the word "CODE" with the text attribute's value. The method returns the modified content as a string.                                                                                                                                                                                                                                                                             |
| result.py              | This code snippet defines a class called `Result` which takes in code, text comments, and a programming language as input. It provides a `get()` method that processes and modifies the given code based on the specified language. The `get()` method uses regular expressions and string manipulations to extract comments and insert them into the code in the appropriate format for both Python and TypeScript (or JavaScript) languages.                                                                                                                                        |
| settings.py            | The code snippet defines setting constants and a class named "Settings". It stores supported programming languages and regex patterns to divide code blocks within the languages.                                                                                                                                                                                                                                                                                                                                                                                                     |
| example_commented.js   | The code snippet defines a User class that represents a user with a name property. It provides a constructor to create a new User instance with the given name, and a getName method to return the name of the user. An instance of User is created with the name'John' and the getName method is called on it. Finally, it checks if the user instance is an instance of the User class.                                                                                                                                                                                             |
| autodoc_commented.py   | The code snippet provides the implementation of the AutoDoc class, which generates comments for code using an AI-powered chatbot. It takes a session token, code string, language string, and an optional example code string as inputs. The __init__ method initializes the AutoDoc instance and performs input validation. The __ask method sends a prompt to the chatbot API and returns the response. The start method divides the code into parts, connects to the chatbot, generates comments for each part, merges the comments with the code, and returns the commented code. |
| divider_commented.py   | This code snippet is a class called `Divider` that takes a text string and a language string. It has a method called `divide()` that splits the text into sections based on language-specific separators. For the given code snippet, the language separator used is "py" for Python, and the `__py()` method splits the Python code into sections based on class and function definitions. The result is a list of strings representing the sections of the Python code.                                                                                                             |
| file_commented.py      | This code provides a File class with methods to retrieve the content and language of a file using its path, as well as create a new file with commented content. The content() method reads and returns the content of the file, the language() method returns the language of the file, and the create_commented_file() method writes the commented content into a new file.                                                                                                                                                                                                         |
| prompt_commented.py    | The provided code snippet defines a class called Prompt for generating prompts for coding exercises. It takes in the language of the prompt, the code to be used, and an optional example usage of the code. The create() method generates the prompt by replacing placeholders in a template file with the provided code and example text.                                                                                                                                                                                                                                           |
| result_commented.py    | The code snippet defines a class called "Result" that represents a code result with a text comment and a language. The class has a "get" method that modifies the code by including the text comments as docstrings for the appropriate class and function definitions. The modification is specifically designed for Python code.                                                                                                                                                                                                                                                    |
| settings_commented.py  | The code snippet defines a `Settings` class that stores the settings for a program. It has a `supported_languages` variable which is a list of supported languages. There are no functions defined in this class.                                                                                                                                                                                                                                                                                                                                                                     |
| example_2_commented.ts | The provided code snippet is a class that creates an HTTP server using the Node.js "http" module. It accepts server response and error handling functions and can be started by invoking the "listen" method with the desired port number. The server listens for GET requests and responds with a JSON formatted data after processing the request.                                                                                                                                                                                                                                  |
| example_commented.ts   | The provided code snippet defines a class called `Pizza` that represents a pizza with a name and a list of toppings. It also includes a class called `PizzaMaker` with a static method to create a new `Pizza` object. Finally, it demonstrates the usage of the `PizzaMaker` class to create a `Pizza` object named "Inferno" with toppings "cheese" and "peppers".                                                                                                                                                                                                                  |

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
