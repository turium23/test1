
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Automate Docs with ChatGPT!</h3>
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

The AutoDoc-ChatGPT project is a console application designed to generate code documentation using ChatGPT, an AI-powered chatbot. It takes a code file as input and uses the AutoDoc module to generate comments for each part of the code. These comments are then merged back into the code file. The project's core functionality lies in automating the documentation process, saving developers valuable time and effort while enhancing code comprehension and maintainability. It provides a valuable proposition by leveraging AI technology to generate informative comments directly within the codebase.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular design pattern, with separate modules for AutoDoc, Divider, File, Prompt, Result, and Settings. It uses a class-based approach to organize code into reusable components.    |
| **📖 Documentation**   | The codebase includes comprehensive documentation for each module, explaining their purpose and functionality. Methods and classes are well-documented with clear descriptions and usage examples.    |
| **🔗 Dependencies**    | The codebase relies on external libraries such as RevChatGPT for generating comments using the Chatbot class. It also uses regular expressions for pattern matching and manipulation.    |
| **🧩 Modularity**      | The codebase is well-organized into separate modules, each responsible for a specific functionality. This allows for easy maintenance, reusability, and clear separation of concerns.    |
| **✔️ Testing**          | The codebase does not have explicit testing implemented. However, implementing unit tests using a framework such as pytest would ensure the correctness and stability of the codebase.    |
| **⚡️ Performance**      | The performance of the system depends on the performance of the external libraries and services it relies on, such as RevChatGPT for generating code comments. Timely responses and efficient resource usage are crucial in maintaining good performance.    |
| **🔐 Security**        | The codebase does not have specific security measures. However, if the system interacts with any sensitive data or services, implementing security measures such as secure authentication and encryption would be necessary.    |
| **🔀 Version Control** | The codebase is managed using Git version control. The project is hosted in a local Git repository, enabling easy collaboration, code sharing, and version tracking for better code organization and development workflows.    |
| **🔌 Integrations**    | The system integrates with the RevChatGPT library to generate comments using the AI-powered chatbot. It also interacts with external files and directories to read and write code files.    |
| **📶 Scalability**     | The system's scalability largely depends on the scalability of the external services it relies on. As the codebase is modular, it allows for easy addition of new modules or improvements to existing ones, promoting scalability with minimal impact on the rest of the system.    |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| main.py                | This code snippet is a console application that generates code documentation using ChatGPT. It reads configurations from a config file, authenticates the user, and takes a code file as input. The code file is processed by AutoDoc, which generates documentation using ChatGPT. Finally, the generated documentation is saved as comments in the code file.                                                                                                                                                                                                                                      |
| autodoc.py             | This code snippet defines a class called AutoDoc, which is responsible for generating comments for a given code. It uses the Chatbot class from the revChatGPT module to generate comments using a prompt based on the code and language. The code is divided into parts, and the Chatbot is used to generate comments for each part. The comments are then merged with the original code to create a commented version.                                                                                                                                                                             |
| divider.py             | The code snippet defines a `Divider` class that divides a text into sections based on specified start and end patterns. It uses regular expressions and settings from an imported module. The `divide` method finds the start and end patterns and splits the text accordingly, storing the sections in a list before returning it.                                                                                                                                                                                                                                                                  |
| file.py                | The code snippet defines a File class that provides core functionalities for working with files. It can initialize a file object with a given path, retrieve the file's content, determine its language, and create a new file with commented content based on the original file's path.                                                                                                                                                                                                                                                                                                             |
| prompt.py              | This code snippet defines a class called Prompt that takes in a language and text as arguments in its constructor. The create method reads and replaces a placeholder, CODE, in a file named after the language specified, located in a models directory. The method returns the modified content as a string.                                                                                                                                                                                                                                                                                       |
| result.py              | This code snippet defines a Result class with a constructor and a'get' method. The'get' method returns modified code based on the specified language. In Python, it extracts comments from text and inserts them as multiline string comments. In TypeScript or JavaScript, it adds comments as block comments above the corresponding code.                                                                                                                                                                                                                                                         |
| settings.py            | This code snippet defines global constants and a Settings class, which stores supported languages and regular expressions for dividing code blocks.                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| example_commented.js   | The code snippet defines a User class with a name property. The class has a constructor that accepts a name parameter to create a new User instance. It also has a getName method that returns the name of the user. An instance of the User class is created and its getName method is called. Finally, an instanceof operation is performed on the user instance to check if it is an instance of the User class.                                                                                                                                                                                  |
| autodoc_commented.py   | This code snippet is for a Python class called AutoDoc, which generates comments for code using an AI-powered chatbot. It takes a session token, code, language, and an example as input. The class has methods to initialize the instance, send a prompt to the chatbot API, and generate comments for the code. The start() method divides the code into parts, connects to the chatbot, sends prompts, generates comments, and merges the comments with the code. The commented code is then returned.                                                                                            |
| divider_commented.py   | The provided code snippet defines a class called "Divider" that splits a given text into sections based on language-specific separators. It currently supports only one language, Python ("py"). The split is done based on class and function definitions using regular expressions. The divided sections are stored in a list and returned.                                                                                                                                                                                                                                                        |
| file_commented.py      | The code provides a class called "File" that represents a file object. It has methods to retrieve the file's content and language, and create a new file with commented content. The class takes a file path as an argument and initializes its attributes based on the path. The "content" method reads and returns the content of the file. The "language" method returns the language of the file. The "create_commented_file" method creates a new file with the provided commented content. The file will be saved in the same directory with a modified name indicating it has been commented. |
| prompt_commented.py    | This code snippet defines a class called "Prompt" that generates prompts for coding exercises in a specified language. It takes in arguments like the language, code, and example text. The "create" method generates the prompt by replacing placeholders in a template file with the provided code and example text. This allows for customization and flexibility in generating prompts for different programming languages.                                                                                                                                                                      |
| result_commented.py    | This code snippet defines a class called `Result`, which represents a code result with a text comment and a language. It has a method `get()` that modifies the code by including the text comments as docstrings for class and function definitions in Python code. The class uses regular expressions to identify the text comments and update the code accordingly.                                                                                                                                                                                                                               |
| settings_commented.py  | The provided code snippet defines a class, Settings, that stores program settings. It has a variable, supported_languages, which is a list of supported languages, initially set to ["py"]. The class does not have any functions defined.                                                                                                                                                                                                                                                                                                                                                           |
| example_2_commented.ts | The provided code snippet is a TypeScript class that represents a server using the http module. It handles GET requests, receives the request body, and responds with JSON. It includes methods to start the server by listening on a specified port.                                                                                                                                                                                                                                                                                                                                                |
| example_commented.ts   | The code snippet defines a Pizza class with properties for name and toppings. It also includes a PizzaMaker class with a static method to create Pizza objects. The snippet demonstrates creating a pizza object using the PizzaMaker class.                                                                                                                                                                                                                                                                                                                                                         |

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
