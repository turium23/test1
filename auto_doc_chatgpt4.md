
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Automate documentation with AutoDoc-ChatGPT!</h3>
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

The project is a command-line tool for generating code documentation using an AI-powered chatbot. It can automatically generate comments for code in Python and TypeScript/JavaScript files by parsing the code and connecting to the chatbot API to generate comments for each code segment. The resulting commented code is returned, providing developers with an efficient way to document their code and improve code readability. The tool optimizes the code documentation process by leveraging advanced AI capabilities, saving developers time and effort.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The system follows a modular architecture with separate classes for different functionalities. The `AutoDoc` class interacts with other modules like `Divider`, `File`, `Prompt`, and `Result` to generate code documentation using an AI-powered chatbot. The codebase also includes a `Settings` module for language-specific settings. Overall, the architecture facilitates code separation and reusability.    |
| **📖 Documentation**   | The codebase includes comments and docstrings that provide explanations and descriptions of various functionality and classes. It explains the purpose and usage of each file/module, making it easier for developers to understand the codebase. However, the documentation could be improved by including more detailed explanations and examples.    |
|**🔗 Dependencies**    | The system relies on the `colorama` library for defining color and style constants in the `settings.py` module. It also leverages the external AI-powered chatbot for generating code comments. Additionally, it depends on common libraries like regular expressions and file I/O for various functionalities.    |
|**🧩 Modularity**      | The system is well-organized into smaller interchangeable components represented by individual classes/modules like `AutoDoc`, `Divider`, `File`, `Prompt`, `Result`, and `Settings`. Each component has a specific responsibility and can be easily extended or modified without impacting the entire system. This modular design promotes maintainability and testability.    |
|**✔️ Testing**          | The codebase does not explicitly mention a testing strategy or provide dedicated tests. Incorporating a testing framework such as `pytest` and adding unit tests would help ensure the correctness and reliability of the system's functionality. |
|**⚡️ Performance**      | Based on the provided information, it is challenging to analyze the system's performance characteristics comprehensively. Performance can vary depending on the size and complexity of the code files being processed, the external chatbot API's response time, and other factors. To assess performance accurately, benchmarking and profiling techniques could be applied. Efficiency tuning might be possible by optimizing code splitting algorithm in the `Divider` module or parallelizing certain operations if applicable.   |
|**🔐 Security**        | The codebase lacks specific security measures and does not mention any implementation for securing data and maintaining functionality. Depending on the environment and usage scenario, potential security risks may include unauthorized access to code/content, confidential information exposure/display, and secure creditentials handling when working with external services. Specific security practices such as input validation, authentication, secure communication, and access controls should be considered and implemented when deploying the codebase.    |
|**🔀 Version Control** | The codebase is version controlled using Git, as evident from the given local file path. However, the Git repository details or actual version control practices (such as branching strategies, pull request review process) are not provided. A structured and organized version control workflow, using practices like feature branching, code reviews, and continuous integration, could improve collaboration, code stability, and prevent unintentional errors.   |
|**🔌 Integrations**    | The system relies on external integration with an AI-powered chatbot for generating code

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| main.py                | The code snippet is a command-line tool for generating code documentation using ChatGPT. It reads a configuration file, sets authentication credentials, parses command-line arguments, checks if the provided code file exists, creates a wrapper around the file, and uses the AutoDoc module to generate documentation. The resulting documentation is then appended to the code file.                                                                                                                                                                                                                           |
| autodoc.py             | The provided code snippet defines a class called'AutoDoc' that automatically generates comments for code. It initializes with a config, code, and language. The'start' method divides the code, connects to a chatbot, generates comments for each divided part using the chatbot, merges the comments with the code, and returns the commented code.                                                                                                                                                                                                                                                               |
| divider.py             | The code defines a class called "Divider" that splits a given text based on start and end patterns using regular expressions. It stores the divided content in a list variable. The "divide" method performs the splitting and returns the list. The code relies on the "Settings" module for language-specific patterns.                                                                                                                                                                                                                                                                                           |
| file.py                | The provided code snippet defines a File class that encapsulates a file's functionalities. It can retrieve the content of a file, determine its language, and create a new file with commented content based on the original file's path and language.                                                                                                                                                                                                                                                                                                                                                              |
| prompt.py              | The Prompt class has an init method that sets the language and text variables.The create method reads a text file corresponding to the language and replaces "CODE" with the stored text.                                                                                                                                                                                                                                                                                                                                                                                                                           |
| result.py              | This code snippet defines a class called "Result" that processes code and comments in Python and TypeScript/JavaScript files. It extracts comments from a specific format and embeds them as docstrings or JSDoc comments in the code. The processed code is then returned.                                                                                                                                                                                                                                                                                                                                         |
| settings.py            | The code snippet is defining some color and style constants using the colorama library. It also defines a Settings class with supported programming languages and regular expressions to divide code blocks in different languages.                                                                                                                                                                                                                                                                                                                                                                                 |
| example_commented.js   | The code snippet defines a User class with a constructor that takes a name parameter. It has a getName() method that returns the user's name. The code creates a new User instance, assigns it the name "John", and then calls the getName() method on the user object. Finally, it checks whether the user instance is an instance of the User class.                                                                                                                                                                                                                                                              |
| autodoc_commented.py   | The provided code snippet is for a class called AutoDoc, which generates comments for code using an AI-powered chatbot. It takes inputs such as a session token, code string, language string, and an optional example string. The class handles input validation and initializes the necessary variables. It also includes methods for interacting with the chatbot API and generating comments for the code. The start method divides the code into parts, connects to the chatbot, generates comments for each part, and merges the comments with the original code. The commented code is returned as a string. |
| divider_commented.py   | The code snippet defines a class called `Divider` that can split a text string into sections based on language-specific separators. It currently supports python code splitting, based on class and function definitions. The `divide` method splits the text using regular expressions and returns a list of sections.                                                                                                                                                                                                                                                                                             |
| file_commented.py      | The provided code snippet defines a File class that represents a file object. It has methods to retrieve the content and language of the file, as well as create a new file with commented content. The class takes a file path as an argument and provides methods to access and manipulate the file.                                                                                                                                                                                                                                                                                                              |
| prompt_commented.py    | The provided code snippet defines a `Prompt` class that generates prompts for coding exercises in a specified language. It takes in the language, code, and an optional example usage as input. The main functionality is the `create` method, which returns a prompt with the code and example text placeholders filled in from a template file specific to the given language.                                                                                                                                                                                                                                    |
| result_commented.py    | The code provides a class called "Result" that represents a code result. It includes functionalities to modify the code by adding text comments as docstrings to appropriate class and function definitions. Currently, it supports Python language only. The "__init__" method initializes the instance with code, text comment, and language. The "get" method returns the modified code. The "__py" method is a helper method for modifying the Python code by adding comments as docstrings.                                                                                                                    |
| settings_commented.py  | The code snippet defines a Settings class that stores the settings for a program. It includes a variable called supported_languages which holds a list of supported languages, with "py" as the initial value.                                                                                                                                                                                                                                                                                                                                                                                                      |
| example_2_commented.ts | The code snippet provides a Server class that creates an HTTP server using Node.js. It handles incoming GET requests, parses the request body, sets the response content type to JSON, and executes serverResponse or serverError functions accordingly. The listen method starts the server on a specified port.                                                                                                                                                                                                                                                                                                   |
| example_commented.ts   | The code defines a `Pizza` class with properties for a pizza's name and toppings, and a `PizzaMaker` class with a static method to create a `Pizza` object. The code also creates and assigns a `pizza` object with a specific name and toppings using `PizzaMaker.create()`.                                                                                                                                                                                                                                                                                                                                       |

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
