
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>AutoDoc-ChatGPT
</h1>
<h3>◦ AutoDoc-ChatGPT: Empowering seamless documentation with AI</h3>
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

The AutoDoc-ChatGPT project is a code documentation tool that uses ChatGPT, an AI-powered chatbot. It generates comments for code snippets in various programming languages by dividing the code into parts, connecting to the chatbot API, and generating comments for each part. The resulting comments are then merged with the code, providing automated documentation.The core functionality of the project is to automate the process of generating code documentation. It analyzes the code, interacts with the chatbot API to generate comments, and inserts the generated comments as docstrings or block comments into the code. This saves time for developers and ensures consistent and informative documentation for the codebase.The purpose of the project is to simplify the task of code documentation by leveraging machine learning and natural language processing capabilities. It eliminates the manual effort involved in writing and maintaining code comments, allowing developers to focus more on the actual development process. The value proposition lies in improving code readability, enabling better code understanding and faster onboarding for new team members.

---

## ⚙️ Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular design pattern, with each component focused on a specific task. The main module connects all the components to generate code documentation using ChatGPT as a chatbot interface.    |
| **📖 Documentation**   | The codebase is well-documented, with informative comments explaining the purpose, functionality, and usage of each module and class. It provides comprehensive explanations for developers.    |
| **🔗 Dependencies**    | The system relies on external libraries such as colorama for terminal text formatting. It also leverages ChatGPT as a dependency to generate comments using a chatbot interface.    |
| **🧩 Modularity**      | The codebase demonstrates a high level of modularity, with specialized modules for different functionalities. Each module handles a specific task, promoting code reusability and ease of maintenance.    |
| **✔️ Testing**          | The codebase does not have explicit mentions of testing strategies or tools. However, it is structured in a way that allows for easy unit testing, making it feasible to incorporate appropriate testing practices.    |
| **⚡️ Performance**      | The system's performance is subjective as it relies on external services like ChatGPT. However, the codebase minimizes unnecessary operations and appropriately customizes requests to optimize both speed and resource usage.    |
| **🔐 Security**        | The codebase itself does not seem to focus on security measures. However, the system should consider security concerns regarding the use of external dependencies like ChatGPT and handle potential vulnerabilities in data exchanges.    |
| **🔀 Version Control** | The codebase follows a version control strategy utilizing Git, utilizing the common Git commands "add", "commit", and "push" to manage changes. This enables collaboration, versioning, and easy tracking of code modifications.    |
| **🔌 Integrations**    | The system integrates with ChatGPT, leveraging its capabilities as a chatbot interface for generating code comments. It also incorporates colorama for formatting terminal text, enhancing user experience.    |
| **📶 Scalability**     | The system's scalability is indirectly affected by the scalability of ChatGPT and external API dependencies. However, the modular design allows for easy scalability of individual system components if needed in the future.    |

---


## 📂 Project Structure




---

## 🧩 Modules

<details closed><summary>Root</summary>

| File                   | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ---                    | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| main.py                | This code snippet is a console application called AutoDoc that generates code documentation using ChatGPT. It expects a code file path as input and uses the AutoDoc module to process and generate the documentation. The resulting documentation is then added as comments to the code file.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| autodoc.py             | The provided code is for an AutoDoc class that generates comments for code snippets. It initializes with a configuration, code, and language. It uses chatbot interaction to generate comments, dividing the code into parts, connecting to ChatGPT, generating comments for each part, and merging the comments with the code. The start method executes these processes and returns the commented code.                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| divider.py             | The code defines a class called "Divider" that divides a given text based on predefined patterns. It utilizes regular expressions to find start and end points in the text, which are defined in the "Settings" module. The divided content is stored in a list and returned as the result.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| file.py                | This code defines a `File` class that represents a file on the system. It provides methods to get the file's content, determine its language, and create a new commented file with a modified name. It uses the `os` module for file operations.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| prompt.py              | The provided code snippet defines a Prompt class with an initialize method that takes a language and text parameter. The class has a create method that reads a file corresponding to the language parameter and replaces the placeholder "CODE" with the provided text. The create method returns the modified content as a string.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| result.py              | The provided code snippet defines a "Result" class that takes code, text comments, and a language string as inputs.The "get" method checks the language and calls either the "__py" or "__ts" method.The "__py" method uses regular expressions to parse comments in Python-style code and inserts them as docstrings.The "__ts" method does a similar operation for TypeScript/JavaScript-style code, parsing comments and inserting them as block comments.The modified code is then returned.                                                                                                                                                                                                                                                                                                                                          |
| settings.py            | The provided code snippet defines color constants for formatting terminal text using colorama. It also includes settings for supported languages and delimiters for identifying start and end points in code blocks of different languages.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| example_commented.js   | The provided code snippet defines a User class that represents a user with a name property. The class has a constructor method to initialize the name property, a getName method to retrieve the user's name, and an instanceof check to determine if an object is an instance of the User class.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| autodoc_commented.py   | This code snippet defines a class called AutoDoc that generates comments for code using an AI-powered chatbot. It takes a session token, code, language, and optional example as input. The class provides methods to divide the code into parts, connect to the chatbot API, send prompts, and generate comments. The start() method generates comments for the code using the chatbot API and returns the original code with the generated comments.                                                                                                                                                                                                                                                                                                                                                                                    |
| divider_commented.py   | This code snippet defines a class called "Divider" that can split a given text string into sections based on language-specific separators. It currently supports Python ("py") as the only supported language. The "divide" method splits the text into sections using regular expressions based on class and function definitions. The resulting sections are returned as a list of strings.                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| file_commented.py      | The code snippet defines a class "File" that represents a file object. It provides methods to retrieve the content and language of the file, as well as create a new file with commented content. The class takes a file path as an argument and initializes its attributes. The "content" method reads and returns the content of the file, while the "language" method returns the language of the file. The "create_commented_file" method creates a new file with the commented content provided as an argument.                                                                                                                                                                                                                                                                                                                      |
| prompt_commented.py    | This code snippet provides a class called `Prompt` that generates prompts for coding exercises in a specified language. It takes in the language, code, and example text as arguments and has a `create` method that generates the prompt by replacing placeholders in a template file with the given code and example text. It allows for the example text to be optional.                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| result_commented.py    | The provided code snippet defines a class called "Result" with a constructor that takes code, text comment, and language arguments. The class has a "get" method that modifies the code by including the text comments as docstrings for the appropriate class and function definitions in Python code. The "py" method in the class handles the modification of Python code by splitting the code into sections based on the text comment. It then replaces the specified text with the comments as docstrings. Above that, the code leverages regular expressions for finding and extracting the relevant portions of text and uses string manipulation to perform the modifications. The modified code is returned as a string. Overall, this functionality can be useful for automatically documenting code with associated comments. |
| settings_commented.py  | The code snippet defines a class called `Settings` that stores program settings. It includes a `supported_languages` variable, which is a list containing one element, "py". This variable can be accessed and used in other parts of the program.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| example_2_commented.ts | The provided code snippet defines a Server class that creates an HTTP server using the'http' module. It handles incoming GET requests, collects the request body, and sends a JSON response. The class includes methods to handle serverResponse and serverError callbacks and to start the server on a specified port.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| example_commented.ts   | The provided code snippet defines two classes: `Pizza` and `PizzaMaker`. The `Pizza` class represents a type of pizza and has properties for the name and toppings of the pizza. The `PizzaMaker` class provides a static method `create` that takes a pizza object as input and returns a new `Pizza` object with the same name and toppings. The code then uses the `PizzaMaker` class to create a pizza object named'Inferno' with toppings'cheese' and'peppers'.                                                                                                                                                                                                                                                                                                                                                                      |

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
