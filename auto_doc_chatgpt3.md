
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ Automate documentation brilliance, with AutoDoc-ChatGPT!</h3>
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

The project is a Python console application that generates code documentation using an AI-powered chatbot. It takes a code file as input, connects to the chatbot API, and generates comments for each part of the code. The comments are then added to the code file, providing valuable documentation for developers. The project aims to automate the often time-consuming task of writing documentation and improve code understanding and maintainability.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular architecture, with separate modules for generating documentation, splitting text, file handling, prompt generation, and processing comments. The code is well-organized and focuses on separation of concerns.    |
| **📖 Documentation**   | The codebase is adequately self-documented with informative variable and method names. However, there is no extensive external documentation apart from the commenting within the code.    |
| **🔗 Dependencies**    | The codebase has a dependency on the ChatGPT API for generating comments. It also relies on regular expressions and the os module from the standard library for text parsing and file handling operations.    |
| **🧩 Modularity**      | The system is divided into individual modules, each responsible for a specific functionality. This modular approach allows components to be easily understood, maintained, and replaced if needed.    |
| **✔️ Testing**          | The codebase lacks explicit testing strategies or tools. Proper unit tests, integration tests, and test coverage should be implemented to ensure the code's reliability and functionality.    |
| **⚡️ Performance**      | The system's performance is dependent on the effectiveness and efficiency of the underlying ChatGPT API and external services. Local code execution appears to be lightweight and efficient.    |
| **🔐 Security**        | The codebase does not possess any substantial measures for data security or access control. Care should be taken to ensure credentials and sensitive data are securely managed.    |
| **🔀 Version Control** | The system uses Git for version control, as evident from the provided codebase. Leveraging Git allows for effective collaboration, tracking changes, and managing the project's development history.    |
| **🔌 Integrations**    | The system integrates with the ChatGPT API for generating comments from code. No other explicit external system integrations are observed.    |
| **📶 Scalability**     | The codebase appears to be potentially scalable as each component can be individually extended or replaced. However, the scalability of the overall system depends on the scalability and performance of the external dependencies.    |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| main.py                | The provided code snippet is a Python console application for generating code documentation. It takes a code file as input, authenticates with ChatGPT using email, password, and session token from a config file, analyzes the code file, and generates documentation using ChatGPT. The resulting documentation is then added as comments to the code file.                                                                                                                                                                                                   |
| autodoc.py             | This code snippet implements a AutoDoc class that generates comments for code using ChatGPT. It divides the code into parts, connects to ChatGPT, and asks for comments for each part. It then merges the comments with the original code to create commented code.                                                                                                                                                                                                                                                                                              |
| divider.py             | The code defines a class called Divider that splits a given text based on regular expressions specified in the Settings module. The divide method finds the start and end matches in the text and extracts the content between them, storing it in the __splitted_content list. The divided content is returned as a list.                                                                                                                                                                                                                                       |
| file.py                | This code snippet defines a File class, allowing users to access the content of a file, get its language, and create a new file with commented content. The class utilizes the os module to handle file path operations.                                                                                                                                                                                                                                                                                                                                         |
| prompt.py              | The code defines a Prompt class with an initializer accepting a language and text parameter. The create method returns the content of a file, replacing the string "CODE" with the provided text, based on the specified language.                                                                                                                                                                                                                                                                                                                               |
| result.py              | This code snippet defines a Result class with methods for processing code comments. It supports two languages: Python and TypeScript/JavaScript.-The `get` method determines the language and calls the appropriate method.-The `__py` method processes Python code comments.-The `__ts` method processes TypeScript/JavaScript code comments.Overall, the code parses comment sections, extracts names and comments, and inserts formatted comments into the code.                                                                                              |
| settings.py            | The code snippet defines various settings for syntax highlighting, including supported languages and delimiters for dividing code blocks.                                                                                                                                                                                                                                                                                                                                                                                                                        |
| example_commented.js   | The provided code snippet is a class called "User" that represents a user with a name property. It has a constructor that creates a new User instance with a given name. It also has a method called "getName()" which returns the name of the user. Lastly, it instantiates a new User object with the name'John', calls the getName() method, and checks if the user instance is of the User class.                                                                                                                                                            |
| autodoc_commented.py   | The provided code snippet is for an AutoDoc class that generates comments for code using an AI-powered chatbot. It takes a code string, a language string, and a token string as inputs. The class initializes instance variables and checks the validity of the inputs. It also has methods to send prompts to the chatbot API and generate comments for the code. The start() method divides the code into parts, connects to the chatbot, and generates comments for each part. Finally, it merges the comments with the code and returns the commented code. |
| divider_commented.py   | The provided code snippet includes a class called "Divider" that takes a text string and a language string as input. It has a "divide" method that splits the text into sections based on the language-specific separators. Currently, it only supports Python language, where it separates the text based on class and function definitions. The output is a list of strings representing the sections of the text.                                                                                                                                             |
| file_commented.py      | The provided code snippet defines a'File' class with methods for retrieving the content and language of a file, and creating a new file with commented content. It takes a file path as an argument upon initialization. The'content' method retrieves the file's content, the'language' method returns the file's language, and the'create_commented_file' method writes a new file with the commented content provided as an argument.                                                                                                                         |
| prompt_commented.py    | The provided code snippet defines a Prompt class that generates prompts for coding exercises in a specified language. It takes in the language, code, and an optional example usage. The create() method generates the prompt by replacing placeholders in a text file with the provided code and example. The class aims to provide a flexible and reusable way to create prompts for different programming languages.                                                                                                                                          |
| result_commented.py    | The code provides a Result class that takes code, text comment, and language inputs. The get() method modifies the code by adding text comments as docstrings to the appropriate class and function definitions in the code. Currently, the implementation supports only Python language. The __py() method splits the Python code into sections based on a given separator in the text comment. The code then replaces specific sections with the modified comments. The modified code is returned.                                                             |
| settings_commented.py  | The code snippet defines a class called "Settings" that stores program settings. It has a variable called "supported_languages" that is a list containing a single value, "py".                                                                                                                                                                                                                                                                                                                                                                                  |
| example_2_commented.ts | The code snippet creates a server using the Node.js `http` module, enabling GET requests. The server can be started on a specified port number.                                                                                                                                                                                                                                                                                                                                                                                                                  |
| example_commented.ts   | The code snippet defines a Pizza class that has a name and toppings property. It also has a static method in the PizzaMaker class to create a new Pizza object. The static method takes an object with a name and toppings and returns a new Pizza object. Finally, the code creates a new Pizza object using the PizzaMaker class with a name value of'Inferno' and toppings of'cheese' and'peppers'.                                                                                                                                                           |

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
