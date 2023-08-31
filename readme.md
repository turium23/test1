
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Streamline Documentation with AutoDoc-ChatGPT!</h3>
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

The AutoDoc-ChatGPT project is a console application that generates documentation for code using an AI-based chatbot. Its purpose is to automate the process of documenting code, saving developers time and effort. By taking a code file as input and using ChatGPT, it generates comments for different parts of the code and adds them as comments within the code file itself. This streamlines the documentation process and improves code readability, making it easier for developers to understand and maintain the code.Overall, the project provides a valuable solution for developers who want to quickly generate accurate and comprehensive documentation for their code, reducing the manual effort required and improving code comprehension.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| ⚙️ Architecture        | The codebase follows a modular design pattern, with separate modules for different functionalities such as code division, file operations, comments generation, and prompt generation. The AutoDoc class is the main component that utilizes other modules to generate code documentation using ChatGPT. The overall architecture allows for easy extensibility and maintainability. |
| 📖 Documentation       | The codebase has comprehensive and well-documented code. Each module and class contains descriptive comments explaining its purpose and functionality. The file structure provides an organized view of the codebase. Proper naming conventions are followed, making it easier to understand the code and its logic. |
| 🔗 Dependencies        | The codebase relies on external libraries like ChatGPT API and regular expressions. It uses Python's built-in modules such as os for file operations. The system also relies on certain language-specific conventions for dividing, commenting, and formatting code. |
| 🧩 Modularity          | The codebase is organized into smaller, interchangeable modules, allowing for easy reuse and maintenance. Modules such as autodoc.py, file.py, prompt.py, divider.py, and result.py encapsulate specific functionalities and can be used independently in other projects. |
| ✔️ Testing             | The codebase does not include explicit testing methodologies or tools. However, due to its structured design and clear separation of concerns, it can be easily tested using unit testing frameworks like pytest or unittest. |
| ⚡️ Performance         | The system performance depends on the ChatGPT API response time and the size of the code being processed. The codebase itself does not have significant performance-related optimization tactics. However, the modularity allows for potential scalability enhancements. |
| 🔐 Security            | The codebase does not explicitly handle security aspects. However, the use of ChatGPT API suggests that security measures must be in place on the ChatGPT side to protect against attacks like injection or code tampering. Proper file handling practices help maintain data integrity. |
| 🔀 Version Control     | The codebase tracks changes and versions using Git version control. It effectively manages multiple branches, commits, and merges to ensure collaboration and codebase integrity among multiple developers. |
| 🔌 Integrations        | The codebase integrates with the ChatGPT API to generate code documentation using natural language processing. It also integrates with language-specific conventions for code division, commenting, and formatting. |
| 📶 Scalability         | The codebase's modular design enables easy scalability with the addition of new functionality or support for additional programming languages. It can handle increased code size by utilizing external resources like ChatGPT API for computationally intensive tasks, making it scalable for larger codebases. |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| main.py                | The code is a console application for generating code documentation using ChatGPT. It takes a code file as input and uses ChatGPT to create documentation for the code. The resulting documentation is then added as comments in the code file.                                                                                                                                                                                                      |
| autodoc.py             | The provided code snippet is for an AutoDoc class that generates comments for code. It takes a configuration, code, and language as input. It divides the code into parts, connects to a ChatGPT API, sends each part to the API for generating comments, and merges the comments with the code. The commented code is returned as output.                                                                                                           |
| divider.py             | The code defines a class called Divider that splits a given text into sections based on regex patterns. It uses regular expressions and settings from a module to identify the start and end points of each section. The divided sections are stored in a list and returned as the result.                                                                                                                                                           |
| file.py                | The code defines a File class that handles file operations. It initializes file path and extracts filename, dirname, and language. It can return the file content and create a new file with commented content.                                                                                                                                                                                                                                      |
| prompt.py              | The code defines a Prompt class that takes a language and text as inputs. The create() method reads a file specific to the language, replaces "CODE" with the provided text, and returns the modified content as a string.                                                                                                                                                                                                                           |
| result.py              | The code snippet is a Python class called Result that transforms code/comments based on language. The'get' method examines the language and invokes relevant private methods'__py' or'__ts'. These methods use regular expressions to extract code and comments specified within'|' characters. The code/comments are modified and formatted according to the language's conventions and returned as a single string.                                |
| settings.py            | The code snippet defines some constants and a class called Settings, which contains supported_languages, divide_start, and divide_end dictionaries. These dictionaries store regular expressions for dividing code files based on their respective starting and ending points for different programming languages (py, ts, js).                                                                                                                      |
| example_commented.js   | The provided code snippet defines a class called "User" with a constructor that takes a name as a parameter and sets it to the "name" property of the instance. The class also has a method called "getName" that returns the name of the user. An instance of a User is created with the name "John" and its "getName" function is called. The code snippet also checks if the instance belongs to the User class.                                  |
| autodoc_commented.py   | The provided code snippet is a class called AutoDoc, which generates comments for code using an AI-powered chatbot. It takes a session token, code, language, and an optional example code as input. The start method divides the code into parts, connects to the chatbot API, and generates comments for each part. The comments are then merged with the original code to create commented code. The generated comments are returned as a string. |
| divider_commented.py   | The code snippet defines a class called Divider that can split a given text string into sections based on language-specific separators. The class has a method called divide() which handles different languages, and currently supports Python language (indicated by "py"). The Python splitting is done based on class and function definitions. The code uses regular expressions to find and extract the sections of Python code.               |
| file_commented.py      | The provided code defines a class called "File" that represents a file object. It has methods to retrieve the content and language of the file, as well as to create a new file with commented content. The class uses the os module to interact with the file system and perform file operations.                                                                                                                                                   |
| prompt_commented.py    | This code snippet defines a `Prompt` class that generates prompts for coding exercises. It takes in a language, code text, and optional example text. The `create` method generates a prompt by replacing placeholders in a template file with the provided code and example text.                                                                                                                                                                   |
| result_commented.py    | The provided code snippet contains a class definition called "Result" that represents a code result with its associated text comment and language. The class has a method called "get" that modifies the code by including the text comments as docstrings for the appropriate class and function definitions in the code. The modification is specific to the Python language.                                                                      |
| settings_commented.py  | This code snippet defines a class called "Settings" that stores settings for a program. It includes a variable called "supported_languages" which is a list containing the supported programming languages, with "py" as the initial value.                                                                                                                                                                                                          |
| example_2_commented.ts | The provided code snippet is a TypeScript implementation of a server using the `http` module. It creates an instance of `http.Server` and handles GET requests. It has a constructor that takes functions to handle server response and error. It also has a `listen` method to start the server on a specified port.                                                                                                                                |
| example_commented.ts   | This code provides a `Pizza` class with a constructor to create `Pizza` objects with a name and an array of toppings. It also includes a `PizzaMaker` class with a static method `create` to create a new `Pizza` object. The code instantiates a `pizza` object using the `PizzaMaker` class, with a name of'Inferno' and toppings of'cheese' and'peppers'.                                                                                         |

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
