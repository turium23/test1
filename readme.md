
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Automate docs, chat smartly</h3>
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

The AutoDoc-ChatGPT project is a code documentation generator that utilizes the ChatGPT model to create commented documentation for code files. It takes a code file path as input and connects to the ChatGPT API to generate comments for different parts of the code. The resulting comments are then merged with the code, providing developers with automatically generated documentation, saving them time and effort in documenting their code.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular architecture with clearly defined components. It uses a class-based approach for code organization.   |
| **📖 Documentation**   | The codebase includes comprehensive inline documentation for each component and method, making it easy to understand the functionality.    |
| **🔗 Dependencies**    | The codebase relies on external libraries like colorama for text styling and regular expressions for pattern matching.   |
| **🧩 Modularity**      | The system is well-organized into separate modules for different tasks such as generating comments, dividing code, handling files, and managing app settings. This enables easy maintainability and reusability.   |
| **✔️ Testing**          | The codebase doesn't provide information about testing strategies or tools. Additional information is required to evaluate its testing approach.   |
| **⚡️ Performance**      | The performance of the system depends on the underlying hardware and the efficiency of the ChatGPT API for generating comments. No specific performance optimizations are mentioned in the codebase.  |
| **🔐 Security**        | The system uses email, password, and session token as authentication credentials for the ChatGPT API. Additional details are required to fully assess the security measures in place.    |
| **🔀 Version Control** | The codebase is version-controlled using Git. Further information regarding the specific version control strategies and tools used isn't provided.   |
| **🔌 Integrations**    | The system integrates with the ChatGPT API to generate comments for code snippets. No other external system or service integrations are mentioned in the codebase.   |
| **📶 Scalability**     | The system's scalability isn't explicitly addressed in the provided information. Additional details are needed to evaluate its ability to handle growth.   |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| main.py                | The provided code snippet is a console application called AutoDoc that generates code documentation using the ChatGPT model. It takes a code file path as input and creates commented documentation for the code. The application authenticates with ChatGPT using email, password, and session token provided in a config file.                                                                                                                                                                |
| autodoc.py             | The provided code snippet is for an AutoDoc class that generates comments for a given code. It divides the code into parts, connects to a ChatGPT (chatbot) to generate comments for each part, and merges the comments with the code. The start method initiates this process.                                                                                                                                                                                                                 |
| divider.py             | The code snippet defines a class called Divider that splits a given text into segments based on specific start and end patterns. It uses regular expressions and a settings module for customization. The divide() method uses iterators to find the start and end points, handle overlapping patterns, and store the divided segments. The resulting segments are returned as a list.                                                                                                          |
| file.py                | This code snippet defines a File class that handles operations on a file. It extracts information about the file path, content, and language. It can also create a new file with the commented version of the provided content.                                                                                                                                                                                                                                                                 |
| prompt.py              | The code defines a Prompt class that takes a language and a text input. The create method reads a file based on the language and replaces the word "CODE" with the input text from the object. The method returns the modified file content.                                                                                                                                                                                                                                                    |
| result.py              | The provided code snippet defines a class `Result` with three private attributes: `code`, `text_comment`, and `language`. The `get` method checks the language and calls either the `__py` or `__ts` private methods to process the text comments in a custom format and insert them as code annotations. The `__py` method processes comments in Python code, while the `__ts` method processes comments in TypeScript or JavaScript code. The processed code is returned by the `get` method. |
| settings.py            | This code snippet defines various text styles and settings for the colorama library. It includes color constants, a Settings class with supported languages, regex patterns to identify class and function definitions, and patterns to mark the end of these definitions in different languages.                                                                                                                                                                                               |
| example_commented.js   | This code snippet defines a User class with a name property. It has a constructor to setup the user's name. It also has a getName() method to retrieve the user's name. An instance of the User class is created with the name'John'. The code snippet calls the getName() method and checks if the instance is an instanceof the User class.                                                                                                                                                   |
| autodoc_commented.py   | The provided code snippet defines a class called AutoDoc that generates comments for code using an AI-powered chatbot. It takes a session token, code string, language, and an optional example as inputs. The class has methods for sending prompts to the chatbot API and generating comments for the code. The code is divided into parts, and for each part, the chatbot is used to generate a comment. The comments are then merged with the original code to produce the commented code.  |
| divider_commented.py   | The code defines a class called Divider that splits a given text into sections based on language-specific separators. It currently supports Python ("py") language and uses regular expressions to identify class and function definitions as separators. The divide() method calls the appropriate language-specific method, in this case __py(), and returns a list of the sections.                                                                                                          |
| file_commented.py      | The code snippet provides a File class that represents a file object. It has methods to retrieve the content and language of the file, as well as create a new file with commented content. The path to the file is passed as an argument to initialize the File instance.                                                                                                                                                                                                                      |
| prompt_commented.py    | The code defines a Prompt class for generating coding exercise prompts. It takes in arguments for the language, code text, and an optional example text. The create() method generates the prompt by reading a template file and replacing specific placeholders with the given code and example text.                                                                                                                                                                                          |
| result_commented.py    | The provided code snippet includes a class called'Result' that represents a code result with its associated text comment and language. The'Result' class has a'get' method that returns a modified version of the code with the text comments included as docstrings for the appropriate class and function definitions. The code implementation includes the splitting and modification of Python code based on the provided text comment. The modified code is then returned.                 |
| settings_commented.py  | The code snippet defines a Settings class that manages the supported_languages setting. Currently, only the "py" (Python) language is supported. This class does not contain any functions. The code also imports colorama to provide color styling options.                                                                                                                                                                                                                                    |
| example_2_commented.ts | The provided code snippet defines a Server class that creates an HTTP server and listens on a specified port. It handles GET requests, parses the request data, and invokes serverResponse to handle successful responses and serverError to handle errors.                                                                                                                                                                                                                                     |
| example_commented.ts   | The provided code snippet consists of two classes: `Pizza` and `PizzaMaker`. The `Pizza` class represents a Pizza object with a name and toppings. The `PizzaMaker` class provides a static `create` method that creates a new Pizza object based on the provided parameters. The snippet includes an example of creating a new pizza object using the `PizzaMaker` class.                                                                                                                      |

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
