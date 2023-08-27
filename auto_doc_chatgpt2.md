
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Streamline docs effortlessly!</h3>
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

The AutoDoc-ChatGPT project aims to automate the process of generating documentation for code with the help of an AI-powered chatbot. The codebase consists of modules that extract code content, divide it into parts, connect to a ChatGPT model, and generate comments for each part. These comments are then merged with the original code to generate a commented version of the code file. This project saves developers time and effort by automating the documentation process and ensuring that code is well-documented for improved maintainability and code comprehension.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The system follows a modular design pattern with separate modules for different functionalities such as file handling, prompting, result parsing, and AutoDoc generation. It uses composition to combine these modules.     |
| **📖 Documentation**   | The codebase lacks extensive inline documentation. However, each file has a brief description of its purpose. Additional documentation on classes, methods, and code logic would enhance the understanding of the codebase.    |
| **🔗 Dependencies**    | The codebase relies on external libraries such as os, colorama for file operations and colorful output, respectively. It also uses ChatGPT as a dependency for generating comments.    |
| **🧩 Modularity**      | The codebase is organized into individual modules that encapsulate specific functionality. These modules can be easily interchanged or extended with minimal impact on other components.     |
| **✔️ Testing**          | The codebase does not include any explicit testing strategies or tools. The absence of unit tests limits the ability to ensure code correctness and reliability. Adding a test suite would improve the long-term maintainability of the project.    |
| **⚡️ Performance**      | The performance characteristics of the system are difficult to analyze based solely on the codebase. Factors such as network latency and computational resources required by the ChatGPT API will have a significant impact on the overall performance.     |
| **🔐 Security**        | From the provided codebase, no specific security-related measures can be identified. Security considerations will depend on external systems used, such as the secure handling of authentication details and ensuring safe communication with the ChatGPT API.    |
| **🔀 Version Control** | The codebase is stored in a Git repository, enabling version control with tools like git log, branches, and easy collaboration. However, the specific version control strategies and branching workflows used are not evident from the codebase.    |
| **🔌 Integrations**    | The system integrates with the ChatGPT API to generate comments. No other integration points are apparent from the provided codebase.    |
| **📶 Scalability**     | The codebase itself does not demonstrate explicit scalability features. The scalability of the system would depend on the performance and availability of external dependencies (such as ChatGPT) and the underlying infrastructure used to deploy and execute the system.    |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| main.py                | This code snippet is a console application for generating code documentation using ChatGPT. It takes a code file as input, checks its existence, extracts its content and language. It then initiates the AutoDoc module with authentication details and code information. Finally, it generates documentation using ChatGPT and creates a commented version of the code file with the documentation.                                                          |
| autodoc.py             | The code snippet initializes an AutoDoc class to generate comments for a given code. It divides the code into parts, connects to a ChatGPT model, and generates comments for each part using the chatbot. The comments are merged with the code to create commented code. Finally, the commented code is returned.                                                                                                                                             |
| divider.py             | The code defines a class called "Divider" that splits text based on the starting and ending patterns specified in the Settings module for a given language. The text is divided into separate parts and stored in a list, which is returned as the result.                                                                                                                                                                                                     |
| file.py                | The code snippet defines a File class with functionalities to get the content of a file, determine its language, and create a commented version of the file. It uses the os module to manipulate file paths and perform file operations.                                                                                                                                                                                                                       |
| prompt.py              | The code snippet defines a class Prompt with a constructor that takes a language and a text parameter. It has a create method that reads a file based on the language and replaces "CODE" with the given text. The method returns the modified text as a string.                                                                                                                                                                                               |
| result.py              | The code snippet includes a Result class with language-specific methods (__py and __ts) that parse a text_comment and modify the code accordingly. The __py method extracts specific parts from the comment, replaces corresponding sections in the code, and adds descriptive comments. The __ts method does a similar process for TypeScript code, adding comment blocks. The get method chooses the relevant parsing method based on the language provided. |
| settings.py            | This code snippet defines a Settings class with supported_languages and regex patterns for dividing code blocks in different languages. It also imports colorama for colorful output.                                                                                                                                                                                                                                                                          |
| example_commented.js   | The code snippet defines a User class with a name property. It includes a constructor to create a user object with a given name and a getName method to retrieve the user's name. An instance of the User class is created with the name'John', and the getName method is invoked on that instance. The code snippet also checks if the user object belongs to the User class.                                                                                 |
| autodoc_commented.py   | The provided code snippet is for the AutoDoc class, which is responsible for generating comments for code using an AI-powered chatbot. It takes a session token, code, language, and an optional example as input. The code is divided into parts and sent to the chatbot API to get comments. The comments are then merged with the original code to generate the commented code. The start() method initiates the process and returns the commented code.    |
| divider_commented.py   | This code snippet defines a class called `Divider` that can split a text string into sections based on language-specific separators. In the current implementation, it supports Python (indicated by the provided language string "py"). The `divide` method utilizes regular expressions to split Python code into sections based on class and function definitions. The resulting sections are returned as a list of strings.                                |
| file_commented.py      | The code snippet provides a class called File, which represents a file object. It has methods to retrieve the content and language of the file, as well as to create a new file with commented content. The class takes a file path as an argument when initializing an instance. The content(), language(), and create_commented_file() methods retrieve the content, language, and create a new commented file, respectively.                                |
| prompt_commented.py    | This code snippet defines a class called Prompt that generates prompts for coding exercises in a specified language. It allows the user to provide the language, code, and optional example text. The prompt is generated by reading from a template text file and replacing placeholders with the provided code and example text. The create method returns the generated prompt as a string.                                                                 |
| result_commented.py    | This code snippet defines a class called "Result" that represents a code result with its associated text comment and language. It provides a method to modify the code by including the text comments as docstrings for the appropriate class and function definitions in the code. This functionality is implemented specifically for Python language.                                                                                                        |
| settings_commented.py  | This code snippet defines a Settings class with a supported_languages variable that stores a list of supported languages. No functions are defined in this class. The colorama import statement allows for text color styling in the terminal.                                                                                                                                                                                                                 |
| example_2_commented.ts | The provided code snippet imports the'http' module and defines a Server class that creates an instance of an HTTP server. It has methods for handling server responses and errors. The server listens on a specified port and can handle GET requests with JSON data.                                                                                                                                                                                          |
| example_commented.ts   | This code snippet defines a Pizza class with properties for name and toppings. It also includes a PizzaMaker class with a static method to create a new Pizza object. Finally, it creates a pizza object using the PizzaMaker class.                                                                                                                                                                                                                           |

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
