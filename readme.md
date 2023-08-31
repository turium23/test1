
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Automated Docs. Smarter Conversations.</h3>
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

The AutoDoc-ChatGPT project is a code documentation generation tool that automates the process of adding comments to code. It leverages the power of an AI-powered chatbot to generate meaningful comments for different parts of code written in various programming languages. This tool saves developers time and effort by automatically generating descriptive comments that improve code readability, support effective collaboration, and enhance maintainability. It offers a valuable solution for easily adding comprehensive documentation to code without manual intervention, improving the overall development experience.

---

## ⚙️ Features

Below is a comprehensive technical analysis of the codebase and its components of the project "AutoDoc-ChatGPT".

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The system follows a modular architecture with different components like `AutoDoc`, `Divider`, `File`, `Prompt`, `Result`, and `Settings`. The `AutoDoc` class is the main component that orchestrates the generation of code comments using the `ChatGPT` AI model. Limit: 200 characters.    |
| **📖 Documentation**   | The codebase has descriptive and well-commented code that provides guidance and clarity on how each component works. Additionally, there are a few example files in the `results` folder that showcase the usage of the various classes. Limit: 200 characters.    |
| **🔗 Dependencies**    | The codebase relies on external libraries such as `re`, `requests`, and `colorama`. It also relies on the `ChatGPT` model for generating code comments. Limit: 200 characters.    |
| **🧩 Modularity**      | The codebase follows a modular design by separating different functionalities into classes. Each class has a specific responsibility and can be used independently or swapped out for alternative implementations. Limit: 200 characters.    |
| **✔️ Testing**          | The codebase does not have explicit test cases or test frameworks mentioned. Limit: 200 characters.    |
| **⚡️ Performance**      | The system's performance largely depends on the response time of the `ChatGPT` API for generating code comments. Other functionalities like file handling and processing comments are expected to be efficient due to their relatively simple operations. Limit: 200 characters.    |
| **🔐 Security**        | There is no specific information available regarding security measures used in the codebase. Limit: 200 characters.    |
| **🔀 Version Control** | The codebase has Git as the version control system, allowing the tracking of changes and collaboration among multiple developers. Limit: 200 characters.    |
| **🔌 Integrations**    | The codebase integrates with the `ChatGPT` API to generate comments and relies on the file system for reading and writing files. Limit: 200 characters.    |
| **📶 Scalability**     | While the codebase itself does not provide explicit scalability features, the separation of concerns into modular components can facilitate future enhancements and modifications. Limit: 200 characters.    |

Based on the given information, these are the key characteristics and design choices observed in the codebase:

1. The codebase follows an object-oriented approach, utilizing classes and encapsulation for specific functionalities.
2. The project employs the use of various language-specific modules to divide code blocks, retrieve file content, and generate prompts.
3. The integration with `ChatGPT` API enables human-like code comment generation, making use of AI models.
4. The codebase includes example files in the `results` folder, providing concrete use cases and demonstrations of the code's capabilities.
5. The system does not have explicit unit tests or automated testing frameworks mentioned, indicating a potential area of improvement for testing

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| main.py                | This code snippet reads a configuration file, authenticates the user, and generates code documentation based on a provided code file using an AutoDoc class. The resulting documentation is then written to a new commented file.                                                                                                                                                                                                                                                                                                              |
| autodoc.py             | The provided code snippet is for an AutoDoc class which automatically generates comments for code. It initializes with a configuration, code, and language. It divides the code into parts, connects to a ChatGPT for generating comments, and merges the comments with the code. The start() function executes these steps.                                                                                                                                                                                                                   |
| divider.py             | The code snippet defines a class Divider that takes in text and language as inputs. It splits the text based on start and end patterns specific to each language, as defined in the Settings module. Resultant content sections are stored in a list called splitted_content, which is returned as the output.                                                                                                                                                                                                                                 |
| file.py                | The code defines a File class that encapsulates a file path, name, and language. It can retrieve and return file content, as well as create a new commented file based on the original file's content using a specific naming convention.                                                                                                                                                                                                                                                                                                      |
| prompt.py              | The code defines a class called Prompt that takes a language and text as inputs. It has a create method that opens a file corresponding to the language, reads its contents, replaces "CODE" with the provided text, and returns the modified string.                                                                                                                                                                                                                                                                                          |
| result.py              | The code snippet defines a class that processes code comments and adds them as docstrings based on the programming language. It uses regular expressions to extract comment sections, formats and inserts them as docstrings in Python code. For TypeScript/JavaScript code, it adds comment blocks before the respective lines.                                                                                                                                                                                                               |
| settings.py            | This code includes settings for supported languages and regular expressions to divide code blocks in each language based on keywords. It imports color settings for terminal styling. Sure.                                                                                                                                                                                                                                                                                                                                                    |
| example_commented.js   | The code snippet defines a "User" class with a "name" property and a constructor that takes a name parameter to create a new user instance. It also has a "getName()" method that returns the user's name. The code then creates a new user object with the name "John" and calls the "getName()" method. Finally, it checks if the user object is an instance of the User class.                                                                                                                                                              |
| autodoc_commented.py   | The provided code snippet defines a class called `AutoDoc` which generates code comments using an AI-powered chatbot. It takes inputs such as a session token, code string, language, and optional example code. The class has methods like `start()` to initiate the comment generation process. It divides the code into parts, connects to the chatbot API, sends prompts, and retrieves responses to generate comments for each part of the code. The comments are then merged with the original code to produce the final commented code. |
| divider_commented.py   | This code snippet defines a class called "Divider" that splits a given text string into sections based on language-specific separators. It currently supports Python language and splits the code based on class and function definitions. The divide() method returns a list of strings representing the sections of the code.                                                                                                                                                                                                                |
| file_commented.py      | The provided code snippet defines a class called `File` that represents a file object. It has methods to retrieve the content and language of a file, as well as create a new file with commented content. The `__init__` method initializes the file with the provided path. The `content()` method retrieves the content of the file, the `language()` method retrieves the language of the file, and the `create_commented_file()` method creates a new file with commented content.                                                        |
| prompt_commented.py    | The provided code snippet defines a class called "Prompt" which is used to generate prompts for coding exercises. The class takes in the language, code, and example text as parameters. The "create" method generates the prompt by reading a template file specific to the language and replacing placeholders with the code and example text.                                                                                                                                                                                               |
| result_commented.py    | The code snippet provides a class called "Result" that represents a code result with its associated text comment and language. It has a method, "get", that modifies the code by including the text comments as docstrings for the appropriate class and function definitions in the code. This functionality is implemented specifically for the Python language.                                                                                                                                                                             |
| settings_commented.py  | The code snippet defines a class called Settings that stores the settings for a program. It includes a list variable called supported_languages, which contains the supported programming languages. No functions are defined in this class.                                                                                                                                                                                                                                                                                                   |
| example_2_commented.ts | This code snippet defines a Server class that creates an HTTP server instance using the'http' module. It handles incoming GET requests, parses the request body, sets the response content type to JSON, and executes the serverResponse or serverError functions accordingly. The server can be started on a specified port using the listen method.                                                                                                                                                                                          |
| example_commented.ts   | The provided code snippet defines two classes:'Pizza' and'PizzaMaker'. The'Pizza' class represents a pizza object with a name and toppings. The'PizzaMaker' class has a static method that creates a new pizza object using the given name and toppings. The code then uses the'PizzaMaker' class to create a new pizza object named'Inferno' with cheese and peppers toppings.                                                                                                                                                                |

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
