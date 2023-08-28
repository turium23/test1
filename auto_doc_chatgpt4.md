
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ AutoDoc-ChatGPT: Unleash the power of AI for automated documentation!</h3>
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

The AutoDoc-ChatGPT project aims to automatically generate comments for code snippets using an AI-powered chatbot. The core functionality involves splitting the code into smaller parts, connecting to a chatbot API, generating comments, and merging them with the original code. This project fulfills the purpose of providing developers with an automated and efficient way to document their code, reducing the manual effort required for writing comments. Its value proposition lies in saving time and improving the readability/documentation of code, making it easier for others to understand and maintain.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular architecture with separate modules for different functionalities such as code division, comment generation, file operations, and prompt generation. The architecture promotes separation of concerns and reusability. |
| **📖 Documentation**   | The codebase includes adequate documentation for each module, class, and function describing their purpose and usage. The documentation improves maintainability and readability of the codebase. |
| **🔗 Dependencies**    | The codebase relies on external libraries/tools for language-specific pattern matching (regex), API interaction, and color styling for output. These dependencies enhance the functionality and usability of the codebase. |
| **🧩 Modularity**      | The codebase is well-organized into smaller modules, each focusing on a specific feature. This modular approach promotes code reusability, maintainability, and easy debugging. |
| **✔️ Testing**          | The codebase does not have information about testing strategies and tools. Implementing automated testing with frameworks like pytest or unittest could improve code quality and reliability. |
| **⚡️ Performance**      | The codebase does not mention specific performance optimizations. However, the efficiency can be improved by optimizing API calls and code parsing algorithms if required. |
| **🔐 Security**        | The codebase does not provide information about specific security measures. Measures like input validation, secure API communication, and access control can be implemented to enhance system security. |
| **🔀 Version Control** | The codebase uses Git for version control. It allows for easy collaboration, code history tracking, and codebase management, ensuring a controlled and organized development process. |
| **🔌 Integrations**    | The codebase incorporates integration with the ChatGPT API to generate comments for code snippets. This integration enhances code documentation capabilities with AI-powered natural language processing. |
| **📶 Scalability**     | The codebase does not have specific scalability features mentioned. However, being built in a modular and organized manner promotes scalability by allowing easy addition of new features and supporting future enhancements. |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| main.py                | The code snippet imports necessary modules and settings, reads configuration from a file, parses command line arguments, checks if the code file exists, creates a commented version of the code file using AutoDoc, and saves the result.                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| autodoc.py             | This code snippet defines a class called AutoDoc, which generates comments for code based on user input. It divides the code into smaller parts, connects to a ChatGPT API for comment generation, and merges the comments with the original code.                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| divider.py             | This code defines a "Divider" class that splits a text into multiple segments based on start and end patterns defined in a language-specific settings module. The "divide" method uses regular expressions to find these patterns in the text and appends the segmented content to a list, which is returned as the output of the method.                                                                                                                                                                                                                                                                                                                                                         |
| file.py                | The code defines a class'File' that represents a file. It initializes with the file path and has methods to retrieve file content and language. Additionally, it has a method to create a new file with commented content based on the original file's path and name.                                                                                                                                                                                                                                                                                                                                                                                                                             |
| prompt.py              | The code snippet defines a class called Prompt. It has an initializer that takes a language and text as parameters. The main function is "create" which reads a file with the given language and replaces the word "CODE" with the provided text, returning the result as a string.                                                                                                                                                                                                                                                                                                                                                                                                               |
| result.py              | The provided code snippet defines a class named "Result" with three properties: code, text_comment, and language. It also has two private methods (__py and __ts) that manipulate the code based on language-specific logic. The get method calls either __py or __ts method depending on the language property and returns the manipulated code. The manipulation involves parsing comments from the text_comment property and inserting them as comments in the code.                                                                                                                                                                                                                           |
| settings.py            | This code snippet defines a class with settings for supported languages and patterns for dividing code blocks based on language-specific keywords. It also imports and defines styling variables for colored output.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| example_commented.js   | The provided code snippet defines a class called User which represents a user with a name property. It has a constructor to set the name and a method to get the name. The code also creates an instance of the User class, assigns the name'John' to it, and then retrieves the name and checks if the user object is an instance of the User class.                                                                                                                                                                                                                                                                                                                                             |
| autodoc_commented.py   | The provided code snippet is a part of a Python application called "AutoDoc". It takes in a code string, a language string, and a token string and uses an AI-powered chatbot to generate comments for the code. The code initializes an instance of the AutoDoc class with the given token, code, language, and an optional example. The code also contains methods to interact with the chatbot API, send prompts, and generate comments for the code. The start() method initiates the process of generating comments by dividing the code into parts, connecting to the chatbot API, generating comments for each part, merging the comments with the code, and returning the commented code. |
| divider_commented.py   | The provided code snippet defines a class called Divider that splits a text string into sections based on language-specific separators. Currently, it supports Python language and splits the text based on class and function definitions. The divided sections are returned as a list of strings.                                                                                                                                                                                                                                                                                                                                                                                               |
| file_commented.py      | This code defines a class called "File" with methods to retrieve a file's content and language, and create a new file with commented content. The class takes a file path as an argument and initializes variables for the path's directory, basename, and file language. The "content" method reads and returns the file's content. The "language" method returns the file's language. The "create_commented_file" method takes a string parameter representing the commented content, creates a new file with the commented content, and saves it in the same directory as the original file with a suffix of "_commented".                                                                     |
| prompt_commented.py    | This code snippet defines a class called "Prompt" that allows the generation of prompts for coding exercises in a specified language. The class has an initializer that takes in language, code, and optional example text. It also has a "create" method that generates the prompt by replacing placeholders with the provided code and example text, if any.                                                                                                                                                                                                                                                                                                                                    |
| result_commented.py    | This code snippet defines a Result class that represents a code result with its associated text comment and language. The get() method returns a modified version of the code, where the text comments are included as docstrings for the appropriate class and function definitions in the code. The code mainly focuses on Python language.                                                                                                                                                                                                                                                                                                                                                     |
| settings_commented.py  | The provided code snippet defines a class called Settings that stores settings for a program. It includes a variable called supported_languages, which is a list containing the supported programming languages (e.g., "py").                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| example_2_commented.ts | The provided code snippet is a server class implementation using the http module in Node.js. It creates an HTTP server, handles GET requests, and allows custom response and error handling. It can be started on a specified port using the listen() method.                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| example_commented.ts   | The provided code snippet defines a Pizza class with a name and toppings property, and a PizzaMaker class with a static create method that creates a new Pizza object. The code then creates a new Pizza object using the PizzaMaker class called "Inferno" with toppings "cheese" and "peppers".                                                                                                                                                                                                                                                                                                                                                                                                 |

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
