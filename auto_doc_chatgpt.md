
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Code smarter, document faster!</h3>
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

The AutoDoc-ChatGPT project is a console application that generates code documentation using an AI-powered chatbot called ChatGPT. It supports multiple programming languages and automates the process of generating comments for code segments. By providing the code file as input, the tool connects to the chatbot and generates comments based on specific patterns for different programming languages. The generated comments are then merged with the code, resulting in a commented version of the file, saving developers valuable time and effort in the documentation process.

---

## ⚙️ Features

| Feature                | Description                                                                                                                                                                                                                                                               |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular design, with separate modules for each functionality. The core architecture revolves around generating code documentation using an AI-powered chatbot. The system is implemented as a console application.                   |
| **📖 Documentation**   | The codebase includes documentation comments within the code files, which provides an overview of the purpose and functionality of each module. However, the documentation could be more comprehensive, especially explaining the internal workings of the system.               |
| **🔗 Dependencies**    | The system uses external dependencies such as ChatGPT (a language model chatbot) and colorama module. The system requires authentication with given credentials or a session token for the chatbot API.                                                                                 |
| **🧩 Modularity**      | The codebase is well-organized into smaller, interchangeable components. Each module focuses on a specific task, such as dividing code, creating prompts, generating documentation, or handling files. This modular approach promotes code maintainability and reusability. |
| **✔️ Testing**          | The codebase does not provide information about testing strategies or tools. The presence of automated tests is essential to ensure the code functionality and avoid potential regressions in the future.                                                                     |
| **⚡️ Performance**      | Performance considerations are not explicitly mentioned in the codebase. However, the system's performance heavily relies on the efficiency of the AI chatbot and the processing time required for generating documentation for larger codebases.                                   |
| **🔐 Security**        | Security measures are not explicitly addressed in the codebase. However, ensuring secure credential handling during the authentication process and applying input validation to prevent any potential security vulnerabilities should be considered.                   |
| **🔀 Version Control** | The codebase is stored in the Git version control system. However, details about specific version control strategies and tools utilized are not provided. Utilizing appropriate branching and tagging conventions would facilitate collaboration and codebase management.     |
| **🔌 Integrations**    | The system interacts with external dependencies, such as the ChatGPT language model chatbot, to generate code documentation. It also requires user input for authentication credentials or a chatbot session token, integrating the user into the process.                                 |
| **📶 Scalability**     | The codebase does not provide clear indications of scalability considerations. Scaling the system could involve optimizing the code for efficient processing of larger codebases, evaluating the performance impact of AI chatbot interactions, and handling concurrent usage.                 |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| main.py                | The code snippet is a console application called AutoDoc that generates code documentation using ChatGPT. It takes a code file as input, authenticates with given credentials, processes the file content, generates documentation, and creates a commented version of the code file with the generated documentation.                                                                                                                                                                                                                                                                                                                                                       |
| autodoc.py             | This code snippet is the implementation of a Tech Lead's automated documentation tool. It divides the provided code into smaller parts, connects to a language model chatbot (ChatGPT), generates comments for each part of the code using the chatbot, and merges the code with the generated comments. The tool supports multiple languages and requires login details or a session token for the chatbot. It provides progress updates during the process and returns the commented code as the final output.                                                                                                                                                             |
| divider.py             | The provided code defines a class called "Divider" that takes a text string and a language as input. It uses regular expressions to find specific patterns in the text and divides it accordingly. The divided content is stored in a list, which is returned as the output of the "divide" method.                                                                                                                                                                                                                                                                                                                                                                          |
| file.py                | This code snippet defines a class that represents a file. Its core functionalities include: 1. Initializing the file object with the provided path and extracting its directory, basename, and language.2. Retrieving the content of the file as a string.3. Retrieving the language of the file.4. Creating a new file with commented content based on the original file.                                                                                                                                                                                                                                                                                                   |
| prompt.py              | The code snippet defines a class Prompt that takes a language and text as input. It has a create method that reads a model text file specific to the language, replaces "CODE" in the file with the text input, and returns the modified text.                                                                                                                                                                                                                                                                                                                                                                                                                               |
| result.py              | The provided code snippet defines a class called "Result" that takes in code, text comments, and the programming language as parameters. The "get" method of the class returns the modified code based on the language. For Python code, it looks for specific patterns in the comments and inserts the corresponding description in the code using indentation.For TypeScript and JavaScript code, it also looks for specific patterns in the comments and inserts the corresponding description as block comments above the identified code blocks.The code focuses on parsing and modifying code comments based on specific patterns for different programming languages. |
| settings.py            | This code snippet imports the colorama module and defines some color constants. It also creates a Settings class with supported languages and patterns for dividing code sections.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| example_commented.js   | The code snippet defines a User class that represents a user with a name property. It has a constructor to initialize the user's name, a getName method to retrieve the user's name, and an instance creation and method invocation at the end.                                                                                                                                                                                                                                                                                                                                                                                                                              |
| autodoc_commented.py   | The provided code snippet defines an AutoDoc class that takes a code string, a language string, and a token string. It generates comments for the code using an AI-powered chatbot. The start() method initiates the process by dividing the code into segments, connecting to the chatbot API, and generating comments for each segment. The comments are merged with the code, resulting in the commented code as the output.                                                                                                                                                                                                                                              |
| divider_commented.py   | The provided code snippet defines a class called'Divider' that takes a text string and a language string as input. It has a'divide' method that splits the text into sections based on language-specific separators. The code currently supports Python language, where it splits the text based on class and function definitions. The split sections are returned as a list of strings.                                                                                                                                                                                                                                                                                    |
| file_commented.py      | The code snippet defines a class called `File`, which represents a file object. It has methods to retrieve the content and language of the file, and to create a new file with commented content based on the original file. The class takes a file path as an argument and provides methods like `content`, `language`, and `create_commented_file` to interact with the file.                                                                                                                                                                                                                                                                                              |
| prompt_commented.py    | This code snippet defines a class called Prompt that generates coding prompts in a specified language. It takes in the language, code, and an optional example, and can generate the prompt with placeholders filled in. The prompt is read from a text file specific to the language. The core functionality lies in the create method, which replaces placeholders in the prompt text with the provided code and example.                                                                                                                                                                                                                                                  |
| result_commented.py    | This code snippet defines a class called Result that represents a code result with associated text comments and language. It has a method called get() that modifies the code by adding text comments as docstrings to the appropriate class and function definitions. Currently, it only supports Python (language "py") and uses regular expressions to split the code and extract the comments.                                                                                                                                                                                                                                                                           |
| settings_commented.py  | The code snippet defines a class called "Settings" that stores the settings for a program. It includes a variable "supported_languages" that is a list of supported languages, with the initial value being ["py"]. No functions are defined in this class.                                                                                                                                                                                                                                                                                                                                                                                                                  |
| example_2_commented.ts | The code defines a Server class that creates an HTTP server instance using Node.js' http module. It listens for GET requests, extracts the request body, and processes the request using serverResponse and serverError functions. It exposes a listen method to start the server on a specified port.                                                                                                                                                                                                                                                                                                                                                                       |
| example_commented.ts   | The provided code snippet defines two classes, `Pizza` and `PizzaMaker`. The `Pizza` class represents a pizza and has properties for name and toppings. The `PizzaMaker` class has a static method `create` that creates a new `Pizza` object with the given name and toppings. Finally, a new `Pizza` object is created using the `create` method of `PizzaMaker`.                                                                                                                                                                                                                                                                                                          |

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
