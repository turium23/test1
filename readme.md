
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Simplify documentation with AutoDoc-ChatGPT!</h3>
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

The AutoDoc-ChatGPT project is a console application that utilizes the ChatGPT model to automatically generate code documentation. By taking a code file as input, the application divides the code into segments and connects with the ChatGPT model to generate comments based on each segment. These comments are then merged with the original code, resulting in comprehensive and meaningful documentation. This project offers a time-saving solution for developers by automating the often tedious task of documenting code, enhancing code readability and understanding.

---

## ⚙️ Features

|    Feature             |      Description                                                                                        |
|------------------------|---------------------------------------------------------------------------------------------------------|
| **⚙️ Architecture**     | The codebase follows a modular architecture with classes for different functionalities to provide code documentation. The main.py file serves as an entry point for the console application. Limited to 200 characters.|
| **📖 Documentation**    | The codebase has inline code comments explaining each class and method's purpose, enhancing understandability. The README file could provide additional documentation for usage and setup. Limited to 200 characters.|
| **🔗 Dependencies**     | The codebase doesn’t have external dependencies apart from the language-specific regular expressions/libraries. Limited to 200 characters.|
| **🧩 Modularity**       | The system is well-organized into modules and classes that encapsulate related functionality, increasing maintainability and reusability. Limited to 200 characters.|
| **✔️ Testing**          | The current codebase lacks evident testing strategies or committed tests which could suggest that testing might need improvements. Limited to 200 characters.|
| **⚡️ Performance**      | With the absence of specific performance metrics or benchmarks, it is challenging to evaluate the system's overall performance. Limited to 200 characters.|
| **🔐 Security**         | The provided codebase looks primarily focused on generating code documentation and doesn't seem to involve security-related functionality or measures for data protection. Limited to 200 characters.|
| **🔀 Version Control**  | The source code is version controlled using Git, but additional information regarding branching strategy, commit practices, or CI/CD would be necessary to provide a comprehensive assessment. Limited to 200 characters.|
| **🔌 Integrations**     | The codebase doesn't indicate any external integrations or collaborations with other systems, services, or APIs, making it self-contained. Limited to 200 characters.|
| **📶 Scalability**      | The scalability of the system is not apparent from the codebase provided. Structural decisions, extensibility, or performance optimizations could affect its scalability. Limited to 200 characters.|

Note: The given codebase snapshots only provide insight into the code structure and partial functionality. A deeper assessment would be possible by exploring the entire codebase, including omitted files and examining GitHub repository details.

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| main.py                | This code snippet is a console application called AutoDoc that generates code documentation using ChatGPT. It takes a code file as input and generates commented documentation based on it. The application uses an authentication mechanism and reads configurations from a config.ini file.                                                                                                                                                                                                                                                             |
| autodoc.py             | This code snippet defines an AutoDoc class that generates comments for code. It divides the code into segments, connects to a ChatGPT model to generate comments using each segment, and merges the comments with the code. The resulting commented code is returned.                                                                                                                                                                                                                                                                                     |
| divider.py             | The provided code snippet is a class called "Divider" that splits a given text based on start and end patterns specific to a chosen language using regular expressions. The divided sections are stored in a list called "__splitted_content" and returned as the final output.                                                                                                                                                                                                                                                                           |
| file.py                | The code defines a File class that performs several operations on a file. It normalizes the path, gets the directory name, base name, and language. It can read and return the content of the file. It can also create a new commented file based on a given content.                                                                                                                                                                                                                                                                                     |
| prompt.py              | The code defines a class called Prompt that takes a language and text as inputs. The create method reads a template file corresponding to the language and replaces "CODE" with the provided text.                                                                                                                                                                                                                                                                                                                                                        |
| result.py              | This code snippet defines a Result class with a constructor and a get method. The get method returns a modified version of code based on the language and comments provided. If the language is "py", the code is formatted by adding comments to specific code lines. If the language is "ts" or "js", the code is annotated with comments using block comments based on specific code lines.                                                                                                                                                            |
| settings.py            | This code snippet defines constants and a class called Settings that holds supported languages and regular expressions patterns for dividing code blocks based on language.                                                                                                                                                                                                                                                                                                                                                                               |
| example_commented.js   | This code snippet defines a class called User with a constructor that takes a name parameter. An instance of this class is created with the name'John'. The User class has a method called getName() which returns the user's name. The code also checks if the user instance is of type User.                                                                                                                                                                                                                                                            |
| autodoc_commented.py   | The provided code snippet is for a class called AutoDoc, which generates comments for code using an AI-powered chatbot. It takes a session token, code string, language string, and optional example code string as inputs. The code string is passed as a prompt to the chatbot API, which returns a response. The code is divided into multiple parts and the chatbot generates comments for each part. The comments are then merged with the original code. The start() method triggers the comment generation process and returns the commented code. |
| divider_commented.py   | The code snippet is a class called Divider that takes a text string and a language string as input. It divides the text into sections based on language-specific separators. Currently, it only supports Python (language="py") and splits the text based on class and function definitions. The sections are returned as a list of strings.                                                                                                                                                                                                              |
| file_commented.py      | The provided code snippet defines a class called "File" that represents a file object. It has methods to retrieve the content and language of the file, as well as create a new file with commented content. The class takes a path to a file as an argument when initialized.                                                                                                                                                                                                                                                                            |
| prompt_commented.py    | The code snippet provides a class called "Prompt", which generates coding exercise prompts in a specified language. It takes a language, code text, and optional example text as inputs. The "create" method replaces placeholders in a template file with the provided code and example text, returning the generated prompt as a string.                                                                                                                                                                                                                |
| result_commented.py    | This code snippet defines a Result class that encapsulates code, text comments, and language information. The'get' method modifies the code to include text comments as docstrings.'py' is the currently supported language.                                                                                                                                                                                                                                                                                                                              |
| settings_commented.py  | The code snippet defines a class called `Settings` that stores settings for a program. It has a variable `supported_languages` which is a list containing a single element (`"py"`) to indicate that Python is a supported language. It does not contain any functions.                                                                                                                                                                                                                                                                                   |
| example_2_commented.ts | The provided code snippet is a TypeScript class that represents a server using the http module. It creates an http.Server instance and handles GET requests by extracting the request body, setting the response header, and calling the serverResponse or serverError functions. The server can be started by calling its listen method and specifying the port number.                                                                                                                                                                                  |
| example_commented.ts   | The provided code snippet defines two classes: Pizza and PizzaMaker. The Pizza class has a constructor for initializing a pizza's name and toppings. The PizzaMaker class has a static method that creates a new Pizza object based on the provided name and toppings. The const pizza variable uses the PizzaMaker class to create a new pizza object named "Inferno" with toppings "cheese" and "peppers".                                                                                                                                              |

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
