
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ AutoDoc-ChatGPT: Unlocking automated documentation bliss!</h3>
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

The AutoDoc-ChatGPT project is a console application that utilizes the ChatGPT model to automatically generate code documentation. It takes a code file as input, processes it through the AutoDoc module, and generates commented documentation that is appended to the original code. The project's core purpose is to streamline the documentation process by automating the generation of descriptive comments, improving code readability, and reducing developer effort. This value proposition saves developers valuable time and ensures consistent and comprehensive code documentation.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The system follows a modular and object-oriented design, with separate modules for different functionalities. Objects are used to represent files, prompts, and results. The architecture allows for flexibility and extensibility. |
| **📖 Documentation**   | The codebase has comprehensive documentation with detailed explanations of each component and its functionalities. The documentation also includes examples and usage instructions, providing valuable assistance to developers. |
| **🔗 Dependencies**    | The system relies on external libraries such as colorama for color and style codes and revChatGPT for generating comments using a Chatbot. These dependencies enhance the system's functionality and contribute to its overall performance. |
| **🧩 Modularity**      | The system is organized into smaller and interchangeable components such as Autodoc, Divider, File, Prompt, and Result. Each component focuses on a specific task, promoting modularity, and easy maintenance. |
| **✔️ Testing**          | The codebase does not explicitly mention testing strategies or tools. It is recommended to implement a testing framework, such as unit tests, to ensure the reliability and stability of the system. |
| **⚡️ Performance**      | The system's performance depends on the efficiency and speed of the external libraries it utilizes, such as ChatGPT and colorama. However, without specific information on resource usage or benchmarks, it is challenging to provide a comprehensive analysis. |
| **🔐 Security**        | Security measures are not explicitly mentioned in the codebase itself. To enhance security, it is recommended to implement measures such as input validation, access control, and encryption of credentials or sessions. |
| **🔀 Version Control** | The codebase is stored in a Git repository, indicating the use of version control for tracking changes and collaborating with other developers. It allows for easy code collaboration, versioning, and rollback if necessary. |
| **🔌 Integrations**    | The system integrates effectively with external systems and services, such as ChatGPT, to generate code documentation. The use of external libraries and APIs demonstrates a seamless integration of third-party functionalities. |
| **📶 Scalability**     | The system's scalability depends on factors like resource utilization, design flexibility, and performance optimizations. Implementing strategies like load balancing, caching, and scalability patterns can help ensure the system's ability to handle growth. |


---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| main.py                | The code snippet is a console application that generates code documentation using ChatGPT. It takes a code file's path as an argument, reads the file, and passes it to AutoDoc along with authentication details. AutoDoc then generates the documentation using the ChatGPT model and the provided code. The resulting documentation is saved in a commented file.                                                                                                                                    |
| autodoc.py             | This code snippet is for an AutoDoc class that generates comments for code. It divides the code into parts, connects to a ChatGPT model to generate comments, and merges the comments with the original code. The comments are generated using a Chatbot object from the revChatGPT.V1 module. The code also handles error checking and authentication with credentials or a session token.                                                                                                             |
| divider.py             | This code defines a class called `Divider` with a method `divide()` that splits a given text based on start and end patterns specific to a given language. The resulting divided sections are stored in a list and returned.                                                                                                                                                                                                                                                                            |
| file.py                | The code defines a File class that represents a file on the system. It has methods to fetch the file's content, determine its programming language, and create a new commented file with a given content.                                                                                                                                                                                                                                                                                               |
| prompt.py              | The code snippet represents a Prompt class that initializes with a language and text. It has a create method that reads a template file specific to the language, replaces "CODE" with the provided text, and returns the modified template as a string.                                                                                                                                                                                                                                                |
| result.py              | The provided code snippet defines a class called "Result" with methods for generating documentation comments for Python and TypeScript/JavaScript code. The "__py()" method parses a text comment and inserts formatted comments based on specific markers in the code. The "__ts()" method performs a similar operation for TypeScript/JavaScript code, creating JSDoc-style comments. The "get()" method determines the programming language and invokes the corresponding comment generation method. |
| settings.py            | This code snippet defines various color and style codes from the colorama library. It also creates a Settings class with supported languages and regular expressions for identifying dividing points in code.                                                                                                                                                                                                                                                                                           |
| example_commented.js   | The code snippet defines a `User` class that represents a user with a name. The class has a constructor that takes the name parameter and sets it as an instance variable. There is also a `getName` method that returns the name of the user. An instance of the `User` class is created with the name'John', and the `getName` method is called to get the name. The code also checks if the instance `user` is an instance of the `User` class.                                                      |
| autodoc_commented.py   | The provided code snippet is for an Autodoc class that takes code, language, and a token as inputs and generates comments for the code using an AI-powered chatbot. The start() method divides the code into parts, connects to the chatbot, and generates comments for each part. The comments are then merged with the original code to produce the commented code.                                                                                                                                   |
| divider_commented.py   | The code snippet provides a class called Divider that takes a text string and language string as inputs. It splits the text into sections based on language-specific separators. Currently, it supports Python code and splits it based on class and function definitions. The divide() method is called to initiate the splitting process. The output is a list of strings representing the sections of the text.                                                                                      |
| file_commented.py      | This code snippet defines a class called "File" that represents a file object. It has methods to retrieve the content and language of the file, as well as create a new file with commented content. The file path is provided as an argument to the class constructor.                                                                                                                                                                                                                                 |
| prompt_commented.py    | This code snippet includes a class called Prompt, which is used for generating prompts for coding exercises in a specified language. It takes in the language, code text, and an optional example text as arguments. The create() method generates the prompt by replacing placeholders in a template text file with the actual code and example text provided.                                                                                                                                         |
| result_commented.py    | This code snippet defines a class called "Result" that represents a code result. It initializes the Result instance with code, text comment, and language. It provides a "get" method to return a modified version of the code with the text comments included as docstrings for appropriate class and function definitions in Python code.                                                                                                                                                             |
| settings_commented.py  | The code snippet imports required modules, defines color constants, and initializes a class `Settings` with a single variable `supported_languages` to store supported programming languages.                                                                                                                                                                                                                                                                                                           |
| example_2_commented.ts | This code snippet defines a Server class that creates an HTTP server using the http module. It handles GET requests, parses request body, sets response headers, and calls response/error handlers. The server can be started by calling the listen method and providing a port number.                                                                                                                                                                                                                 |
| example_commented.ts   | The provided code snippet defines a Pizza class with a constructor that initializes the name and toppings properties. It also includes a PizzaMaker class with a static method to create a Pizza object. The create method takes a Pizza event as input and creates a new Pizza object with the given name and toppings. Finally, the code creates a new Pizza object called "pizza" using the PizzaMaker class.                                                                                        |

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
