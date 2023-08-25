
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Automating Knowledge with AutoDoc ChatGPT!</h3>
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

The project, located in the AutoDoc-ChatGPT repository, is an Auto Documentation tool that uses the ChatGPT API to generate comments for code files in different programming languages. The tool takes a configuration file, code file, and the programming language as inputs. It then merges the generated comments with the original code to generate a commented code file. This automated process aims to save developers time and effort by eliminating the need for manual code documentation, ensuring code details are readily available for better understanding and maintainability.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular architecture, with separate modules for AutoDoc (code documentation generation), Divider (text splitting), File (file handling), Prompt (text prompt generation), Result (code comment processing), and Settings (language settings). This allows for easy separation of concerns and scalability.    |
| **📖 Documentation**   | The codebase provides inline documentation for each module, explaining their functionality and usage. This helps developers understand and maintain the codebase effectively. However, additional external documentation, such as a README file, would further enhance the comprehensiveness of the documentation.    |
| **🔗 Dependencies**    | The codebase imports the following external libraries: `colorama` for color formatting and `re` for regular expressions. There are no other major external dependencies, which helps keep the codebase lightweight and easily portable.    |
| **🧩 Modularity**      | The codebase is organized into separate modules, each responsible for a specific task. This modular design allows for easy interchangeability and reuse of components in other projects. Future modifications and updates can be isolated to their respective modules, minimizing the impact on other parts of the codebase.    |
| **✔️ Testing**          | The codebase does not include explicit details about testing strategies or tools. However, to ensure the stability and reliability of the system, comprehensive unit tests are recommended for each module. The use of a testing framework like `pytest` would streamline the testing process.    |
| **⚡️ Performance**      | As the codebase focuses on code documentation and text manipulation, performance considerations should be taken into account, such as optimizing regular expression patterns for efficiency and minimizing API calls to the ChatGPT API. Thorough profiling and benchmarking can help identify areas for performance optimization.    |
| **🔐 Security**        | The codebase does not explicitly mention security measures. To enhance security, it is recommended to sanitize user inputs when interacting with the file system. Additionally, ensuring the confidentiality and privacy of any API tokens or sensitive information is crucial to maintaining system security.    |
| **🔀 Version Control** | The codebase is stored in a Git repository on the local machine under the given path. Utilizing version control tools like Git enables proper tracking of changes, collaboration across team members, and easy rollback to previous versions if necessary.    |
| **🔌 Integrations**    | The system integrates with the ChatGPT API to generate code comments. No other external systems or services are mentioned in the codebase. Considering potential integrations with code documentation tools or version control systems could further enhance the capabilities of the system.    |
| **📶 Scalability**     | The modular design of the codebase allows for easy scalability. New modules can be added or existing ones modified as per requirements. However, to cater to high scalability needs, optimization and caching mechanisms could be considered to handle increased load and maintain performance.    |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| main.py                | The code snippet reads from a configuration file, takes user arguments from the command line, validates the existence of a code file, and uses a module to generate code documentation based on the file's content and language. The generated documentation is then saved in a commented file.                                                                                                                                                                                                    |
| autodoc.py             | This code snippet is for an Auto Documentation tool. It takes a configuration, code, and language as inputs. It uses the ChatGPT API to generate comments for each part of the code. The comments are then merged with the original code to generate commented code.                                                                                                                                                                                                                               |
| divider.py             | The provided code defines a class called Divider that splits a text into different sections based on specified start and end patterns. The class has a divide() method that uses regular expressions to find the start and end positions and retrieves the divided sections.                                                                                                                                                                                                                       |
| file.py                | This code snippet defines a File class that represents a file. It has methods to retrieve the file's content, language, and create a new commented file based on the original.                                                                                                                                                                                                                                                                                                                     |
| prompt.py              | The code initializes a Prompt class with language and text inputs. The create method opens a file based on the language and replaces "CODE" with the provided text. The method returns the resulting string.                                                                                                                                                                                                                                                                                       |
| result.py              | This code snippet defines a Result class with the ability to process code and text comments in Python and TypeScript/JavaScript. It extracts specific information from comments and integrates it into the code as comments in a desired format.                                                                                                                                                                                                                                                   |
| settings.py            | This code snippet defines settings for syntax highlighting in different programming languages. It sets up color codes for different text styles and provides regex patterns for dividing code blocks by language.                                                                                                                                                                                                                                                                                  |
| example_commented.js   | The provided code creates a class called "User" with a name property. It has a constructor to initialize the name, a method to retrieve the name, and an instance of User called "user.                                                                                                                                                                                                                                                                                                            |
| autodoc_commented.py   | This code snippet defines a class called AutoDoc that generates comments for code using an AI-powered chatbot. It takes a token, code, language, and optional example as input. It initializes the instance with error checking, sends prompts to the chatbot API, and generates comments. The start() method divides the code, connects to the chatbot, generates comments for each part, merges the code and comments, and returns the commented code.                                           |
| divider_commented.py   | The provided code snippet implements a class called `Divider` that splits a given text into sections based on language-specific separators. It currently supports the "py" language for Python. The `divide()` method uses regular expressions to split the Python code into sections based on class and function definitions. The sections are then returned as a list of strings.                                                                                                                |
| file_commented.py      | The provided code snippet defines a class called "File" which represents a file object. It has methods to retrieve the content and language of the file, and to create a new file with commented content. The class takes a path argument during initialization, and the content can be retrieved with the "content" method. You can also get the language of the file using the "language" method. The "create_commented_file" method allows you to create a new file with the commented content. |
| prompt_commented.py    | This code snippet defines a class called Prompt, which is used to generate prompts for coding exercises in a specified programming language. It has a constructor that takes the language, code, and optional example text as arguments. The create method generates the prompt by replacing placeholders in a template file with the code and example text.                                                                                                                                       |
| result_commented.py    | This code snippet defines a class "Result" that represents a code result with associated text comments and language. It provides a method to modify the code by including the text comments as docstrings for appropriate class and function definitions.                                                                                                                                                                                                                                          |
| settings_commented.py  | The code snippet defines a class, "Settings", that stores the supported_languages variable, which is a list of supported programming languages. The snippet also imports color formatting features from the "colorama" module.                                                                                                                                                                                                                                                                     |
| example_2_commented.ts | The provided code snippet creates a server using Node.js's HTTP module. It listens for GET requests, parses the request body, and handles response and error functions. The server can be started by calling the listen method with a specified port number.                                                                                                                                                                                                                                       |
| example_commented.ts   | The code snippet defines a Pizza class, with a constructor to initialize its name and toppings. There is also a PizzaMaker class with a static method to create a new Pizza object. The create method takes a Pizza object as a parameter and returns a newly created Pizza object. The code then uses the PizzaMaker class to create a pizza with the name "Inferno" and toppings "cheese" and "peppers".                                                                                         |

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
