
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Automate documentation with AI wizardry 🧙‍♂️</h3>
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

The AutoDoc-ChatGPT project is aimed at automatically generating code documentation by leveraging the ChatGPT model. It provides a set of modules that handle tasks such as parsing code files, generating comments for code sections, and creating a new version of the code with the generated documentation. The project's value proposition lies in significantly reducing the effort required to generate comprehensive code documentation, which can improve code readability, maintainability, and collaboration among developers.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| ⚙️ Architecture     | The system follows a modular design with separate files for different functionalities. It uses a class-based approach for encapsulating related code. The main.py file acts as an entry point for the code generation process.    |
| 📖 Documentation   | The codebase contains comprehensive and well-documented code. Each file has clear descriptions of its functionalities and how it fits into the overall system. The README file provides an overview of the project and instructions for running it.    |
| 🔗 Dependencies    | The system relies on the ChatGPT model for generating comments. It also uses libraries such as regular expressions (`re`), colorama, and http for various functionalities. These dependencies are well-managed and documented in the codebase.    |
| 🧩 Modularity      | The system is well-organized into smaller modules that handle specific tasks such as parsing code, generating comments, managing files, and handling prompts. This modularity allows for easy maintenance, debugging, and extensibility.   |
| ✔️ Testing          | The codebase does not explicitly mention any specific testing strategies or tools. Further testing details might be available in the existing test cases or test directories. Comprehensive testing is essential to validate the functionality and detect potential issues.    |
| ⚡️ Performance      | The analysis of performance aspects is not evident from the codebase alone. Performance considerations such as speed, efficiency, and resource usage could be assessed by profiling and load testing the system with representative inputs.    |
| 🔐 Security        | The security measures employed by the system are not explicitly addressed in the codebase. To ensure data security and maintain functionality, guidelines such as secure coding practices, input validation, and access control should be followed. Analyzing the codebase alone does not provide insight into specific security measures.    |
| 🔀 Version Control | The project's Git codebase indicates the use of version control to manage changes to the codebase. The system leverages version control tools such as Git to track modifications, collaborate with team members, and maintain a history of changes made to the project. Proper branch management, pull requests, and code reviews could enhance collaboration.    |
| 🔌 Integrations    | The codebase does not explicitly mention the integration with other systems or services. Additional integrations may exist in environmental configuration files or APIs not available in the displayed codebase. Any interdependencies should be monitored, maintained, and their documentation should be appropriately communicated for smooth functioning.    |
| 📶 Scalability     | The codebase does not provide explicit information regarding the system's ability to handle growth. Scalability in terms of code complexity, load, or user base might be improved by proper design patterns, architectural choices, and optimization techniques. Assessing scalability requires additional information, such as performance benchmarks and future plans.    |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| main.py                | The code snippet reads a configuration file, takes command line inputs to specify a code file, checks if the file exists, parses the file, generates code documentation using an AI-powered tool, and creates a new commented version of the file with the documentation.                                                                                                                                                                                                                                     |
| autodoc.py             | This code snippet is a script for generating comments for code using a ChatGPT model. It divides the code into sections, connects to ChatGPT, and generates comments for each section. The comments are then merged into the code. The script requires a configuration, code, and language as input.                                                                                                                                                                                                          |
| divider.py             | The provided code defines a class "Divider" that divides a given text based on start and end patterns specific to a language. The "divide" method uses regular expressions to find the start and end positions, splits the text accordingly, and returns a list of divided segments.                                                                                                                                                                                                                          |
| file.py                | The code defines a File class that manages file-related functionalities: getting the file path, file name and file extension, reading the file content, retrieving the file language, and creating a new commented version of the file.                                                                                                                                                                                                                                                                       |
| prompt.py              | The code defines a class, Prompt, with a constructor that takes a language and text. It has a create method that reads from a file corresponding to the language, replaces a placeholder with the text, and returns the result.                                                                                                                                                                                                                                                                               |
| result.py              | This code snippet defines a Result class that takes in code, text comments, and a language as input. The get method processes the code and returns the modified code based on the language. For the "py" (Python) language, it extracts names and descriptions from the text comments and inserts them as comments in the code. For the "ts" or "js" (TypeScript or JavaScript) language, it extracts names and comments from the text comments and inserts them as block comments in the code.               |
| settings.py            | The code snippet defines color constants and a Settings class with language-specific regular expressions called'divide_start' and'divide_end' for code parsing purposes. These patterns are used to divide code into sections such as classes and functions based on the supported languages.                                                                                                                                                                                                                 |
| example_commented.js   | The provided code snippet defines a User class that represents a user with a name property. It has a constructor to create a new User instance with a given name, a getName method to return the name of the user, and an instance of User object is created with a name'John' and its getName method is called. The instanceof operator is used to check if the user object is an instance of the User class.                                                                                                |
| autodoc_commented.py   | The provided code snippet is for an AutoDoc class that generates comments for a given code using an AI-powered chatbot. It takes a session token, code string, language, and an optional example code. The class has methods to divide the code into parts, connect to the chatbot API, send prompts to the chatbot, and merge the code with generated comments. The start method executes the entire process and returns the code with generated comments.                                                   |
| divider_commented.py   | The code snippet defines a class "Divider" that splits a text string into sections based on language-specific separators. It currently supports Python code splitting, using class and function definitions as separators.                                                                                                                                                                                                                                                                                    |
| file_commented.py      | The provided code snippet defines a class called `File` that represents a file object. It has methods to retrieve the content and language of the file, and to create a new file with commented content. The class takes a file path as an argument and initializes various attributes based on the path. The `content` method returns the content of the file, the `language` method returns the language of the file, and the `create_commented_file` method creates a new file with the commented content. |
| prompt_commented.py    | The provided code snippet defines a class called Prompt, which generates prompts for coding exercises. It accepts the language, the code text, and an optional example text as arguments. The create() method generates a prompt by filling in placeholders for the code and example text in a predefined template based on the language.                                                                                                                                                                     |
| result_commented.py    | This code snippet defines a class called "Result" that represents a code result with its associated text comment and language. The main functionality of the code is the "get" method, which modifies the code by including the text comments as docstrings for the appropriate class and function definitions in Python code. The "__py" method is a private method used internally to split the Python code based on the text comment separators.                                                           |
| settings_commented.py  | The code snippet defines a Settings class that stores the supported_languages variable as a list of supported programming languages. It uses the colorama library to define constants for different text colors and styles. This class does not have any functions defined.                                                                                                                                                                                                                                   |
| example_2_commented.ts | The provided code snippet defines a Server class that creates an instance of an HTTP server using the built-in http module. It takes in functions for handling server response and server error. It listens to GET requests on a specified port and call the serverResponse function with the request data or the serverError function if an error occurs.                                                                                                                                                    |
| example_commented.ts   | The code snippet provides classes and a static method to create a Pizza object. The Pizza class has a constructor that initializes the name and toppings. The PizzaMaker class has a create method that returns a new Pizza object with the given name and toppings. The code snippet creates a new Pizza object named "Inferno" with the toppings "cheese" and "peppers".                                                                                                                                    |

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
