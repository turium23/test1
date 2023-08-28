
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ AutoDoc-ChatGPT: Automatic Documentation, Effortless Communication</h3>
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

The AutoDoc-ChatGPT project is designed to generate code documentation by using the power of GPT-based chatbots. It achieves this by autonomously generating comments for different segments of code. The project supports multiple programming languages and provides a user-friendly interface to authenticate and connect with the chatbot API. These code comments enhance readability and understanding by providing context and explanations, saving developers time and effort. With its ability to generate comprehensive and accurate documentation, the AutoDoc-ChatGPT project streamlines the code documentation process and improves collaborative development.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular design pattern, with separate modules for autodoc functionality, code division, file handling, prompts, results processing, and settings. It uses object-oriented programming to organize functionality within each module, enhancing code reusability and maintainability.|
| **📖 Documentation**   | The codebase includes detailed inline comments in each module, explaining the purpose and functionality of the code. Additionally, there is a README file that provides an overview of the project and instructions on how to use it. The documentation is comprehensive and helps new contributors understand the codebase.|
| **🔗 Dependencies**    | The project relies on external libraries such as ChatGPT for generating comments, regular expressions for pattern matching, and the standard Python libraries for file handling. These dependencies are well-documented and specified within the code.|
| **🧩 Modularity**      | The codebase is well-organized into multiple modules, each responsible for a specific functionality. This modularity makes the codebase easy to understand, maintain, and extend. The modular design promotes code reuse and separation of concerns.|
| **✔️ Testing**          | The codebase does not appear to have a dedicated testing framework or tests included. There is room for implementing proper testing strategies such as unit tests or integration tests to ensure code correctness and maintainability.|
| **⚡️ Performance**      | In terms of performance, the codebase primarily relies on external systems like ChatGPT for the comment generation process. The performance of the overall system depends on the response time of the external systems and the efficiency of the codebase in handling large code files.|
| **🔐 Security**        | The codebase does not appear to have specific security measures implemented. It should be cautious when handling user input, authentication credentials, or interacting with external systems to avoid vulnerabilities such as injection attacks or data breaches.|
| **🔀 Version Control** | The code is managed using Git version control. The repository has a well-structured commit history that allows tracking changes, collaboration, and easy rollbacks. Git provides a reliable way to ensure code integrity and manage code versions efficiently.|
| **🔌 Integrations**    | The codebase integrates with ChatGPT for generating comments and uses external libraries for functionalities like regular expression pattern matching. It could benefit from added integrations with other code analysis tools or APIs to enhance the documentation generation process.|
| **📶 Scalability**     | The codebase can handle scalability to some extent due to its modular design. However, it may face challenges when dealing with very large code files, as it heavily relies on an external system (ChatGPT) for comment generation. Ensuring optimal resource usage and implementing optimizations can improve scalability.|

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| main.py                | The code snippet is a console application for generating code documentation using ChatGPT. It takes a code file path as input and uses the AutoDoc module to extract the content and language of the file. It then authenticates with ChatGPT using the credentials provided in the config file. Finally, it generates code documentation using the AutoDoc module and creates a new file with comments added to the original code file.                                                                                                                                                                                                                                                       |
| autodoc.py             | This code snippet is for an AutoDoc tool that generates comments for code. It uses a ChatGPT model to generate comments for different parts of the code by dividing it into segments. The tool connects to the ChatGPT, generates comments for each segment, and merges them with the original code to create commented code as the output. It supports different programming languages and requires login details or a session token for authentication.                                                                                                                                                                                                                                      |
| divider.py             | The provided code snippet defines a class called Divider that divides a given text based on start and end patterns specific to a given language. The divide() method searches for start and end patterns in the text using regular expressions, and appends the extracted content to a list. The divided content is then returned as a result.                                                                                                                                                                                                                                                                                                                                                 |
| file.py                | This code provides a File class that represents a file and offers functionalities to retrieve its content, language, and create a new commented file. The path of the file is normalized and stored, and various file details are extracted. File content can be retrieved, and a new commented file can be created based on provided content.                                                                                                                                                                                                                                                                                                                                                 |
| prompt.py              | This code snippet defines a Prompt class that takes a language and text as input. It has a create method that opens a file specific to the language and replaces "CODE" with the provided text. The method returns the modified text as a string.                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| result.py              | The provided code includes a class called Result that processes code snippets and comments in different programming languages (Python, TypeScript, and JavaScript). It extracts names and corresponding comments from a multi-line comment pattern found within the text_comment. It then inserts the comments back into the code at the appropriate locations in a specific format based on the programming language being processed. The get() method returns the updated code.                                                                                                                                                                                                              |
| settings.py            | This code snippet defines a Settings class and contains constants for text coloring. It also defines dictionaries for dividing code based on supported languages and specific patterns.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| example_commented.js   | The code snippet defines a User class with a name property. It has a constructor to set the name when creating a new instance, and a getName() method to retrieve the name. The code also creates a user instance named'John' and calls the getName() method. Finally, it checks if the user instance is an instance of the User class.                                                                                                                                                                                                                                                                                                                                                        |
| autodoc_commented.py   | The provided code snippet represents a class called AutoDoc, which uses an AI-powered chatbot to generate comments for a given code. The class takes in a session token, code string, language, and an optional example code. It validates the inputs and initializes the necessary variables. The class has a private method, __ask, that sends a prompt to the chatbot API and returns the response. The start method generates comments for the code by dividing the code into parts, connecting to the chatbot API, and generating comments for each part. It then merges the comments with the original code. The commented code with generated comments is returned by the start method. |
| divider_commented.py   | The provided code snippet is a class called Divider that splits a text string into sections based on language-specific separators. It currently supports Python code by detecting class and function definitions as separators. The divide() method returns a list of strings representing the sections of the text.                                                                                                                                                                                                                                                                                                                                                                           |
| file_commented.py      | This code snippet defines a File class that represents a file object. It has methods to retrieve the content and language of the file, and to create a new file with commented content.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| prompt_commented.py    | This code snippet provides a class called Prompt that generates prompts for coding exercises in a specified language. It takes in the language, code, and example text as input. The create() method generates the prompt by replacing placeholders in a template file with the actual code and example text. It returns the generated prompt as a string.                                                                                                                                                                                                                                                                                                                                     |
| result_commented.py    | The provided code snippet defines a class called "Result" which represents a code result with its associated text comment and language. The class has a constructor that initializes the code, text comment, and language. It has a "get" method that returns a modified version of the code with the text comments included as docstrings for the appropriate class and function definitions in the code. This functionality is specific to the Python language. The private method "__py" is responsible for splitting the Python code into sections based on the text comment separators and adding the comments as docstrings in the code.                                                 |
| settings_commented.py  | The code snippet defines a Settings class that stores program settings, specifically the supported languages. It initializes a list of supported languages with the language "py". This class does not include any functions.                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| example_2_commented.ts | The code snippet is a TypeScript implementation of a server class using the'http' module. It creates an HTTP server, handles incoming GET requests, and allows listening on a specified port number.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| example_commented.ts   | The provided code snippet defines a Pizza class with properties for name and toppings. It also includes a PizzaMaker class with a static method for creating Pizza objects. The code snippet creates a new Pizza object using the PizzaMaker method.                                                                                                                                                                                                                                                                                                                                                                                                                                           |

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
