
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Automated docs, empowered conversations!</h3>
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

The AutoDoc-ChatGPT project aims to simplify the process of generating code documentation using an AI-powered chatbot. It provides a console application that takes in a code file, interacts with ChatGPT to generate comments, and saves the documentation as comments in a new file. Core functionalities include dividing the code into sections, connecting to the chatbot, generating comments for each section, merging comments with the code, and returning the commented code. This saves development time, enhances code readability, and helps developers understand the code without needing extensive explanations.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular architecture with components such as Main, AutoDoc, Divider, File, Prompt, Result, and Settings. The system is designed to take an input code file, generate documentation using the AutoDoc class, and save the documentation as comments in a new file. It utilizes the ChatGPT library for generating comments. |
| **📖 Documentation**   | The codebase is adequately documented, with each file providing a summary of its functionality. However, further documentation detailing the APIs and key classes would enhance the codebase's usability. |
| **🔗 Dependencies**    | The codebase relies on external libraries such as ChatGPT and modules such as os, re, and console for various functionalities. ChatGPT library provides AI-powered chatbot functionality, while os and re are used for file path manipulation, regex operations, and division pattern matching. The console module helps in displaying progress during code generation. |
| **🧩 Modularity**      | The codebase exhibits good modularity by organizing functionality into separate modules/classes, focusing on single responsibilities. Components like AutoDoc, Divider, File, Prompt, Result, and Settings encapsulate specific functionalities, promoting code reuse and maintainability. |
| **✔️ Testing**          | The codebase doesn't mention specific testing strategies or tools. However, due to the modular design, individual components can be unit tested to verify their functionality. This could potentially be enhanced with automated testing tools and a comprehensive test suite. |
| **⚡️ Performance**      | The code efficiency depends on the performance of external libraries like ChatGPT, as they handle the generation of comments. File operations and code parsing might have performance implications based on the size of the codebase. Overall, the codebase's performance should be assessed and improved based on specific use cases. |
| **🔐 Security**        | Given the codebase's purpose, security measures seem focused on maintaining functionality rather than securing data. Handling user input and file operations should consider potential security vulnerabilities like code injection or unauthorized file access. Proper input validation and file access controls would improve security. |
| **🔀 Version Control** | The code is stored in a local Git repository, allowing for effective version control. However, specific details regarding branching strategies, commit practices, and collaboration are not mentioned. Following best practices in version control would improve project maintenance and collaboration. |
| **🔌 Integrations**    | The codebase integrates with the ChatGPT library, which provides AI-generated comments. Being an AI integration, any additional system integration specifics are not mentioned. Documentation or further discussions with developers would shed light on potential integrations with editors, development environments, or CI/CD pipelines. |
| **📶 Scalability**     | The codebase's scalability primarily depends on the performance of external libraries and the hardware infrastructure used. While the modular design allows for adding new features or improving existing ones, evaluating and optimizing system performance under heavy workloads is essential for seamless scalability. Load testing and resource monitoring are recommended for addressing scalability concerns. |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| main.py                | The code creates a console application called AutoDoc that generates code documentation using ChatGPT. It takes in a code file as input, checks if the file exists, and then uses AutoDoc to retrieve the code's documentation. Finally, the documentation is saved as comments in a new file.                                                                                                                                                                                                                                                            |
| autodoc.py             | The provided code snippet implements an AutoDoc class that generates comments for code. It initializes with a configuration, code, and programming language. It uses the ChatGPT library to interact with a chatbot for generating comments. The code is divided into parts, and for each part, the chatbot generates a comment. The comments are then merged with the code. The start method executes this process and returns the commented code.                                                                                                       |
| divider.py             | The code snippet defines a class called "Divider" that is responsible for dividing a text based on certain patterns defined in a Settings module. It uses regex to find the starting and ending positions of the divisions, and then creates a list of divided content.                                                                                                                                                                                                                                                                                   |
| file.py                | The code snippet defines a File class that represents a file. It provides methods to retrieve the file's content and language, as well as create a new commented version of the file. The file path is normalized and stored as private attributes.                                                                                                                                                                                                                                                                                                       |
| prompt.py              | The code defines a Prompt class with an initializer that takes a language and text parameter. It has a create method that reads a template file specific to the language, replaces "CODE" with the provided text, and returns the resulting contents as a string.                                                                                                                                                                                                                                                                                         |
| result.py              | This code snippet defines a class called "Result" with a constructor and two private methods. The "get" method checks the language and calls either the "__py" or "__ts" method. These methods parse text comments and modify code accordingly, adding formatted comments based on specific language syntax. The updated code is returned as a string.                                                                                                                                                                                                    |
| settings.py            | The code snippet defines settings for a syntax highlighter. It sets color codes for different programming language keywords and regex patterns to divide code sections. Languages supported are Python, TypeScript, and JavaScript.                                                                                                                                                                                                                                                                                                                       |
| example_commented.js   | This code defines a User class with a constructor that takes a name parameter. It also has a getName method that returns the name of the user. An instance of the User class is created with the name'John', and the getName method is called on that instance which returns'John'. The instanceof operator is used to check if the user instance is of type User, which returns true.                                                                                                                                                                    |
| autodoc_commented.py   | The provided code snippet is a Python class called "AutoDoc" that generates comments for a given code using an AI-powered chatbot. It takes a session token, code string, language string, and an optional example code string as arguments. The class has initialization, prompt sending, and result generation methods. The start method divides the code into parts, connects to the chatbot, generates comments for each part, merges the comments with the code, and returns the commented code. The console module is used for displaying progress. |
| divider_commented.py   | The code defines a class called "Divider" that splits a given text into sections based on language-specific separators. It currently supports Python code and splits it based on class and function definitions. The code first finds the start and end indices of each section using regular expressions, and then extracts the corresponding section from the original text. The result is a list of strings representing the sections of the text.                                                                                                     |
| file_commented.py      | The provided code snippet defines a class called "File" that represents a file object. It allows reading the file's content, retrieving its language, and creating a new file with commented content. The class provides methods such as `content()` to retrieve the file's content, `language()` to retrieve the file's language, and `create_commented_file()` to create a new file with commented content. The class utilizes the `os` module for file path manipulation and handling.                                                                 |
| prompt_commented.py    | This code snippet defines a class called Prompt, which is used to generate coding exercise prompts in a specified language. The class takes the language, code, and optional example text as inputs. It has a create method that generates the prompt by replacing placeholders in a template file with the code and example text.                                                                                                                                                                                                                        |
| result_commented.py    | The provided code snippet defines a "Result" class that represents a code result with associated text comment and language. It has a "get" method that modifies the code by including the text comments as docstrings in the appropriate class and function definitions. This functionality is specific to the Python language.                                                                                                                                                                                                                           |
| settings_commented.py  | This code snippet defines a `Settings` class that stores the settings for a program. It includes a variable `supported_languages` which is a list of supported programming languages. The example usage demonstrates accessing the `supported_languages` attribute.                                                                                                                                                                                                                                                                                       |
| example_2_commented.ts | The provided code snippet is a class that creates an HTTP server using the `http` module. It handles incoming GET requests by parsing the request body, setting the response Content-Type to JSON, and calling the `serverResponse` function. It also has a `listen` method to start the server on a specified port.                                                                                                                                                                                                                                      |
| example_commented.ts   | The provided code snippet includes two classes: `Pizza` and `PizzaMaker`. The `Pizza` class has a constructor that initializes the name and toppings of the pizza. The `PizzaMaker` class has a static method `create` that creates a new Pizza object with the given name and toppings. The code creates a new Pizza object using the `create` method from `PizzaMaker` class with the name'Inferno' and toppings'cheese' and'peppers'.                                                                                                                  |

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
