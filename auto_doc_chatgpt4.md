
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Code smarter, document faster.</h3>
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

The AutoDoc-ChatGPT project is a code documentation tool powered by an AI chatbot. Its core functionality includes parsing code files, generating comments for each part of the code using ChatGPT, and combining the comments with the code to create a commented version. The project's purpose is to automate the code documentation process and improve code understanding by providing informative comments. Its value proposition lies in reducing the manual effort required for code documentation and enhancing code readability and maintainability.

---

## ⚙️ Features

| Feature          | Description                                                                                                                                                               |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **⚙️ Architecture** | The codebase follows a modular architecture pattern and is organized into several modules. It effectively separates concerns and allows for easy maintenance and extensibility.                                               |
| **📖 Documentation**    | The codebase has well-documented code snippets that provide detailed explanations of their functionality and usage. However, additional high-level documentation of the overall system design may be beneficial.                                                                |
| **🔗 Dependencies** | The system relies on external libraries such as `ChatGPT` for generating comments, and it may have dependencies on programming language-specific libraries for parsing and manipulating code.                                |
| **🧩 Modularity**   | The codebase is highly modular, with each module responsible for a specific functionality. This design enables code reuse, maintainability, and easier testing of individual components.                           |
| **✔️ Testing**       | The codebase does not provide specific information about the testing strategies or tools used. Further information is needed to assess whether comprehensive testing is implemented.                                          |
| **⚡️ Performance**   | The performance of the system may vary depending on the underlying language models used by `ChatGPT` and the size of the codebase being analyzed. Additionally, resource usage may depend on the number of code files being processed concurrently. |
| **🔐 Security**     | The codebase does not explicitly address security measures. Safeguarding user information and potential vulnerabilities should be considered in terms of data privacy and code execution.                                   |
| **🔀 Version Control** | The codebase is stored in a Git repository. However, specific version control strategies and tools are not mentioned. Implementing best practices such as branching, code reviews, and tags can enhance collaboration and code maintenance.    |
| **🔌 Integrations**   | The system interacts with external services such as `ChatGPT` for generating comments. It may benefit from integrating with version control systems or code hosting platforms to streamline workflows.                                   |
| **📶 Scalability**    | The system's scalability depends on the external services it relies on, such as `ChatGPT`, and the performance of the code parsing and comment generation processes. Load balancing and optimization may be necessary for handling increased traffic and larger codebases.    |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| main.py                | This code snippet is a command-line application for generating code documentation using ChatGPT. It parses command-line arguments, reads configuration values, and creates an authenticated session. It then reads the specified code file, generates documentation using ChatGPT, and creates a commented version of the code file with the generated documentation.                                                                                                                                                                                                                                                     |
| autodoc.py             | This code snippet is for an AutoDoc tool that generates comments for code. It connects to ChatGPT to generate comments for each part of the code, divides the code into parts, and merges the comments with the code. The result is the commented code.                                                                                                                                                                                                                                                                                                                                                                   |
| divider.py             | This code snippet defines a `Divider` class that takes in a `text` and `language` parameter. It uses regular expressions and settings from an external module to divide the text into parts based on start and end patterns. The divided content is stored in a list and returned.                                                                                                                                                                                                                                                                                                                                        |
| file.py                | This code defines a File class that represents a file on the system. It can retrieve the file content, extract the language from the file extension, and create a new commented version of the file by appending "_commented" to its name.                                                                                                                                                                                                                                                                                                                                                                                |
| prompt.py              | The code defines a `Prompt` class that takes in a language and a text as inputs. The `create` method replaces the "CODE" placeholder with the given text by reading a file specific to the language. The resulting string is returned.                                                                                                                                                                                                                                                                                                                                                                                    |
| result.py              | This code snippet defines a class called "Result" with a constructor that takes three parameters: code (a string representing code), text_comment (a string representing comments related to the code), and language (a string specifying the programming language). The class has a "get" method that returns the modified code based on the language. The "__py" method handles Python code while the "__ts" method handles TypeScript/JavaScript code. These methods parse the text_comment using regular expressions and modify the code by adding comments in a specific format. The modified code is then returned. |
| settings.py            | The code snippet defines constants for different colors and settings. It also defines regular expressions for dividing code based on programming languages.                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| example_commented.js   | The code defines a User class with a name property. It has a constructor to set the name and a method getName() to retrieve the name. An instance of User is created with the name'John'. User instanceof User returns true.                                                                                                                                                                                                                                                                                                                                                                                              |
| autodoc_commented.py   | The provided code snippet creates an AutoDoc class that uses an AI-powered chatbot to generate comments for code. It takes in a token, code, language, and optional example code. It sends prompts to the chatbot API and receives responses. The start() method divides the code into parts, connects to the chatbot, and generates comments for each part using the ask() method. Finally, it merges the comments with the original code and returns the commented code.                                                                                                                                                |
| divider_commented.py   | The provided code snippet defines a class called "Divider" that splits a given text string into sections based on language-specific separators. It currently supports the "py" language. The "divide" method is used to initiate the splitting process, while the "__py" method specifically handles splitting Python code based on class and function definitions. The resulted sections are returned as a list of strings.                                                                                                                                                                                              |
| file_commented.py      | The provided code snippet defines a class called "File" that represents a file object. It provides methods to retrieve the content and language of the file and to create a new file with commented content.                                                                                                                                                                                                                                                                                                                                                                                                              |
| prompt_commented.py    | The provided code snippet defines a'Prompt' class that generates coding exercise prompts in a specified language. It takes in inputs for the language, code, and example text, and has a'create' method to generate the prompt text by substituting placeholders in a template file with the provided code and example text.                                                                                                                                                                                                                                                                                              |
| result_commented.py    | This code snippet defines a Result class that encapsulates a code result along with its associated text comment and language. The class has a method "get()" that returns a modified version of the code with the text comments included as docstrings for the appropriate class and function definitions in Python code. The implementation is specific to Python language.                                                                                                                                                                                                                                              |
| settings_commented.py  | The provided code snippet defines a class named "Settings" that stores the settings for a program. It has a variable called "supported_languages" that is initialized with a list containing only the string "py". This class does not have any functions defined.                                                                                                                                                                                                                                                                                                                                                        |
| example_2_commented.ts | The code snippet defines a Server class that creates an HTTP server and handles incoming GET requests. It takes server response and server error functions as parameters and starts the server on a specified port.                                                                                                                                                                                                                                                                                                                                                                                                       |
| example_commented.ts   | The code snippet defines two classes: `Pizza` and `PizzaMaker`. The `Pizza` class represents a pizza and has properties for name and toppings. The `PizzaMaker` class has a static method to create a `Pizza` object. The provided code creates a `Pizza` object named "Inferno" with toppings "cheese" and "peppers" using the `PizzaMaker` class.                                                                                                                                                                                                                                                                       |

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
