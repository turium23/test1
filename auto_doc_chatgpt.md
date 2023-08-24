
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Automate documentation with precision!</h3>
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

The core functionalities of the project involve automatically generating code documentation using AI-powered chatbots. The purpose of the project is to provide a streamlined and efficient process for generating code comments by utilizing natural language processing techniques. This saves developers time and effort in manually writing documentation, allowing them to focus more on coding. The project's value proposition lies in its ability to improve code readability, maintainability, and collaboration by automatically generating meaningful comments for code files.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular architecture, with separate modules for different functionalities such as file handling, code division, prompt creation, result processing, and autodoc generation. |
| **📖 Documentation**   | The codebase is well-documented with comprehensive comments in each file, explaining the purpose and functionality of the code. It enables easy understanding and maintenance of the system.    |
| **🔗 Dependencies**    | The codebase relies on external libraries such as ChatGPT for code documentation generation. It also utilizes regular expressions for text splitting and Python's built-in libraries for file handling.    |
| **🧩 Modularity**      | The codebase is organized into separate modular components, enabling individual reusability and interchangeability. Each module focuses on a specific functionality, allowing easy maintenance and extensibility of the system.    |
| **✔️ Testing**          | The codebase lacks explicit information about testing strategies and tools. However, the modular structure facilitates the implementation of unit tests for each module, ensuring the correctness and robustness of the system.    |
| **⚡️ Performance**      | The codebase primarily depends on the efficiency and response time of the external ChatGPT model for code documentation generation. The code itself appears to be well-optimized and does not show any significant performance issues. Further evaluation would require benchmarking. |
| **🔐 Security**        | The codebase does not involve any security-sensitive operations or data storage. However, proper attention should be given to the handling of potentially malicious input files to prevent vulnerabilities or code execution risks.    |
| **🔀 Version Control** | The system utilizes Git as the version control system, enabling easy tracking of changes, collaboration, and code maintenance. The codebase's repository could benefit from developing a clear versioning strategy and maintaining a consistent branching model for smooth development workflows.    |
| **🔌 Integrations**    | The system integrates with the ChatGPT API for code documentation generation using AI-powered chatbots. Apart from that, there are no evident integrations with other systems or services.    |
| **📶 Scalability**     | The codebase's modular structure and separation of concerns provide a solid foundation for handling future growth and scalability. The system can accommodate new functionalities or languages by extending the existing modules or creating new ones. The potential scalability bottleneck lies in the reliance on the external ChatGPT API, which should be monitored with increasing workload.  |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| main.py                | This code snippet is a console application for generating code documentation. It reads a code file path as input, checks if the file exists, extracts the content and language from the file, and initiates the code documentation generation process using ChatGPT. Finally, the generated documentation is added as code comments to the original file.                                                                                                                                                        |
| autodoc.py             | The code snippet provided initializes and runs an AutoDoc program that generates comments for given code. It divides the code into parts, connects to a ChatGPT model for generating comments, and merges the comments with the original code. The commented code is then returned as the output.                                                                                                                                                                                                                |
| divider.py             | The code implements a Divider class with a divide() method that splits a given text based on patterns defined in the Settings class. It uses regular expressions to find start and end positions, handles cases where the end is before the start, and returns the divided content as a list.                                                                                                                                                                                                                    |
| file.py                | This code snippet defines a class called'File' that encapsulates file-related operations. It can retrieve the content and language of a file, as well as create a commented version of the file with a modified filename.                                                                                                                                                                                                                                                                                        |
| prompt.py              | The code snippet defines a'Prompt' class with a constructor taking a language and text parameter. It has a'create' method that reads a file specific to the language, replaces "CODE" with the text, and returns the modified content as a string.                                                                                                                                                                                                                                                               |
| result.py              | The code snippet is a class called "Result" that processes code and comments in different programming languages. It extracts specific comments enclosed in "|" characters and inserts formatted comments into the code using Python and TypeScript/JavaScript specific logic.                                                                                                                                                                                                                                    |
| settings.py            | The code snippet sets global variables for text styles and defines a Settings class with supported languages and regex patterns for splitting code blocks. It enables coloring and formatting printed output in Python, TypeScript, and JavaScript.                                                                                                                                                                                                                                                              |
| example_commented.js   | The code defines a class called User representing a user with a name property. It has a constructor to initialize the name and a getName method to retrieve the name. An instance of the User class is then created, and the name is retrieved using the getName method. Want to confirm the object is an instance of the User class.                                                                                                                                                                            |
| autodoc_commented.py   | The provided code snippet defines a class named AutoDoc, which generates comments for code using an AI-powered chatbot. It takes a token, code, language, and an optional example as input. The comments are generated by sending prompts to the chatbot API and receiving responses. The code is divided into parts, and the chatbot generates comments for each part. Finally, the comments are merged with the code. The `start()` method initiates the process and returns the code with generated comments. |
| divider_commented.py   | The provided code snippet defines a class called Divider that splits a text string into sections based on language-specific separators. It currently supports Python (language code = "py") and splits the text based on class and function definitions. The divide method performs the splitting and returns a list of strings representing the sections of the text.                                                                                                                                           |
| file_commented.py      | The provided code snippet defines a class called `File` with methods to retrieve the content and language of a file, and create a new file with commented content. The `__init__` method initializes the file path and extracts the directory name, base name, and language. The `content` method retrieves the file content, the `language` method returns the file language, and the `create_commented_file` method creates a new file with commented content.                                                 |
| prompt_commented.py    | This code snippet provides a class called Prompt that generates prompts for coding exercises in a specified language. It takes in the language, code, and an optional example text as arguments. The create() method generates the prompt by replacing placeholders for the code and example text in a template file specific to the language.                                                                                                                                                                   |
| result_commented.py    | This code snippet defines a class called "Result" that represents a code result with associated text comments and a language. The class has a method called "get" that modifies the code by including the text comments as docstrings for appropriate class and function definitions. It currently supports the "py" language.                                                                                                                                                                                   |
| settings_commented.py  | The provided code defines a class called Settings, which stores the settings for a program. It includes a variable'supported_languages' that contains a list of supported languages. Example usage shows how to access the supported_languages variable.                                                                                                                                                                                                                                                         |
| example_2_commented.ts | The provided code snippet is a class that represents an HTTP server using the `http` module. It creates an instance of `http.Server` and provides functionalities for handling server responses and errors. It supports the GET method, listens on a specified port, and can be extended to handle other HTTP methods as well.                                                                                                                                                                                   |
| example_commented.ts   | The provided code snippet defines two classes-Pizza and PizzaMaker. The Pizza class represents a pizza with a name and toppings. The PizzaMaker class has a static method to create a new Pizza object. The snippet then creates a new Pizza object using the PizzaMaker class with the name "Inferno" and toppings "cheese" and "peppers".                                                                                                                                                                      |

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
git clone F:/autoapi/AutoDoc-ChatGPT
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
