
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>test1
</h1>
<h3>◦ Unleash the future: test1, where innovation meets code.</h3>
<h3>◦ Developed with the software and tools listed below.</h3>

<p align="center">
<img src="https://img.shields.io/badge/Python-3776AB.svg?style&logo=Python&logoColor=white" alt="Python" />
</p>
<img src="https://img.shields.io/github/languages/top/turium23/test1?style&color=5D6D7E" alt="GitHub top language" />
<img src="https://img.shields.io/github/languages/code-size/turium23/test1?style&color=5D6D7E" alt="GitHub code size in bytes" />
<img src="https://img.shields.io/github/commit-activity/m/turium23/test1?style&color=5D6D7E" alt="GitHub commit activity" />
<img src="https://img.shields.io/github/license/turium23/test1?style&color=5D6D7E" alt="GitHub license" />
</div>

---

## 📒 Table of Contents
- [📒 Table of Contents](#-table-of-contents)
- [📍 Overview](#-overview)
- [⚙️ Features](#-features)
- [📂 Project Structure](#project-structure)
- [🧩 Modules](#modules)

---


## 📍 Overview

The project is an implementation of a code documentation tool called AutoDoc. It utilizes the ChatGPT API to generate documentation from code files, currently supporting Python. The tool takes a code file as input, interacts with the ChatGPT API to generate comments, and then creates a new commented version of the code file. The core functionalities include parsing code files, generating comments using AI-powered chatbot, and providing a convenient way to improve code documentation. This tool simplifies the documentation process and enhances code readability, saving time for developers and improving code collaboration.

---

## ⚙️ Features

| Feature                | Description                                                                                                                     |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a simple console application design pattern, where the AutoDoc class interacts with the ChatGPT API to generate code documentation.                                           |
| **📖 Documentation**    | The codebase lacks comprehensive documentation. Additional comments within the code itself would improve code understanding and maintenance.                                                |
| **🔗 Dependencies**    | The codebase has external dependencies on the os, argparse, configparser, colorama, and revChatGPT libraries. It also relies on the ChatGPT API for the documentation generation.          |
| **🧩 Modularity**      | The codebase demonstrates modularity by separating functionality into multiple files, allowing for easier maintenance and component reuse.                                                |
| **✔️ Testing**          | The codebase doesn't have explicit testing strategies or tools mentioned. Incorporating unit tests would enhance code robustness and reduce the chance of bugs in the future.            |
| **⚡️ Performance**      | Performance is difficult to assess without benchmarks. However, the system mainly relies on the external ChatGPT API for documentation generation, which could affect performance. |
| **🔐 Security**        | The codebase doesn't showcase any specific security measures. However, secure storage and transmission of authentication credentials should be ensured to protect sensitive information. |
| **🔀 Version Control** | Version control is implemented using the Git system, as evident from the repository. Additional details on branching and workflow conventions are not provided in the given information. |
| **🔌 Integrations**    | The system integrates with the ChatGPT API to generate code documentation. Configurable options via the "config.ini" file allow for easy integration with different setups.          |
| **📶 Scalability**     | Scalability is not a key objective of the codebase, but it can handle code files of varying lengths. Expanding language support and optimizing API usage could enhance scalability.      |

---


## 📂 Project Structure




---

## 🧩 Modules

## AutoDoc-ChatGPT\main.py

The code script is a console application called AutoDoc that generates code documentation using ChatGPT. It currently supports Python as a language. The application takes a code file as input and uses the ChatGPT API to generate the documentation. It then creates a new commented file with the generated documentation.

The code script starts by importing necessary modules and classes, such as os, argparse, AutoDoc, File, and configparser. It also reads a configuration file called "config.ini" to get authentication credentials.

Then, it defines a command-line argument parser with a description of the application. The "-file" argument is required and represents the path to the code file.

Next, it checks if the specified code file exists. If it doesn't exist, the script exits with an error message.

After that, it creates an instance of the File class using the specified code file. The File object provides methods to read and write to the code file.

The script then creates an instance of the AutoDoc class with authentication credentials, the content of the code file, and the language of the code. The AutoDoc object is responsible for interacting with the ChatGPT API and generating the documentation.

Finally, it calls the start method of the AutoDoc object to generate the documentation. The result is then used to create a new commented version of the code file using the file.create_commented_file method.

Overall, the code script is a simple implementation of a document generation tool using the ChatGPT API for code documentation.
## AutoDoc-ChatGPT\modules\autodoc.py

The code script begins with importing necessary modules and packages such as `os`, `time`, `colorama`, `revChatGPT.V1`, `Prompt`, `Divider`, `Settings`, `Result`, and `Console`. It initializes the colorama module and defines a Tech Lead class called `AutoDoc`. 

The `AutoDoc` class has an initializer that takes three parameters: `config` (a string containing the configuration details), `code` (a string representing the code to be documented), and `language` (a string indicating the programming language used in the code).

The initializer checks the validity of the input parameters, ensuring that the code is a non-empty string and the language is supported. 

The class also has a private method `__ask` that sends a prompt to the chatbot and receives a response. 

The `start` method is the main entry point of the code. It handles the processing of the code and generating the documentation. It displays the progress of the documentation generation in the console.

The code is divided into separate parts using the `Divider` class. If the code is empty or there is nothing to comment, the program exits. 

The code connects to the `revChatGPT` chatbot using the provided configuration details (session token or email/password). 

Each part of the code is sent to the chatbot to generate comments. The comments are stored in a list. 

The code and comments are merged using the `Result` class to create the commented code. 

Finally, the commented code is returned and displayed in the console.