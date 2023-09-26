
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>test1
</h1>
<h3>◦ Test beyond limits, Test1 delivers!</h3>
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

The AutoDoc project is a command-line application that uses the ChatGPT language model to automatically generate code documentation. It supports the Python language and requires a code file as input. The core functionality involves extracting information from the code file, interacting with the ChatGPT model to generate comments, and merging the comments with the original code to produce a commented version. This project provides a valuable tool for developers to save time and effort in documenting their code.

---

## ⚙️ Features

| Feature                | Description                                                                                       |
| ---------------------- | ------------------------------------------------------------------------------------------------- |
| **⚙️ Architecture**     | The codebase follows a modular design pattern with separate files for different functionalities.   |
| **📖 Documentation**   | The codebase lacks comprehensive documentation, making it difficult for new contributors to understand the purpose and functionality of each component.             |
| **🔗 Dependencies**    | The codebase relies on external libraries such as os, argparse, configparser, etc.                   |
| **🧩 Modularity**      | The codebase is organized into smaller components like autodoc.py and main.py for ease of understanding and maintainability.                |
| **✔️ Testing**          | There is no information available about the testing strategies or tools used in the codebase.                          |
| **⚡️ Performance**      | The performance of the system is dependent on the underlying models it interacts with, namely ChatGPT.                            |
| **🔐 Security**        | The codebase does not contain specific measures for data protection or security.                                            |
| **🔀 Version Control** | The codebase is hosted on GitHub, indicating the use of Git for version control.                                             |
| **🔌 Integrations**    | The codebase integrates with ChatGPT to generate code documentation based on the given code file.                     |
| **📶 Scalability**     | The codebase does not contain specific features or considerations for scalability.                                                 |

---


## 📂 Project Structure




---

## 🧩 Modules

## AutoDoc-ChatGPT\main.py

The code is a command-line application called AutoDoc, which is used for generating code documentation using ChatGPT. It supports Python language and requires a code file as input.

The code first imports necessary modules and packages such as os, argparse, configparser, and the custom modules autodoc, file, and settings. It then reads configuration settings from a config.ini file, which includes authentication details like email, password, and session token.

Next, an argument parser is defined to handle command-line arguments. It specifies that the user must provide a path to the code file using the "-file" flag. If the file does not exist, the program exits with an error message.

The code then creates a File object using the provided code file path. This object reads the content of the file and determines the language of the code.

An AutoDoc object is then created, passing in the authentication details, the content of the code file, and the detected language. This object is used to interact with a ChatGPT model for generating the code documentation.

The "start" method of the AutoDoc object is called, which generates the documentation based on the code. The result obtained is used to create a new commented file using the File object.

Overall, the code performs the task of generating code documentation using the ChatGPT model and saves the commented file with the documentation.
## AutoDoc-ChatGPT\modules\autodoc.py

The code script is an implementation of an Auto Documentation tool called AutoDoc. It takes in a configuration file, code, and language as input parameters. The code is then divided into multiple parts using the Divider module. The divided parts are then sent to the ChatGPT language model to generate comments for each part. The comments are merged with the code using the Result module to create a commented version of the code. Finally, the commented code is returned as the output.

There are no newly defined functions or classes in this code script.