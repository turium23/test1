
<div align="center">
<h1 align="center">
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
<br>test1
</h1>
<h3>◦ Test1: Empowering code mastery, one commit at a time!</h3>
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

The project is called AutoDoc and it is a console application that generates code documentation using AI chatbots. It automates the process of generating comments for code by leveraging an AI chatbot to provide comments based on the provided code. The core functionalities of the project include reading code files, detecting the programming language, connecting to the chatbot, dividing the code into smaller parts, asking the chatbot for comments, and merging the code with the comments to generate the final commented version. It aims to save developers time and effort by automating the cumbersome task of writing code documentation.

---

## ⚙️ Features

| Feature                | Description                                                                                                |
|------------------------|------------------------------------------------------------------------------------------------------------|
| **⚙️ Architecture**     | The codebase follows a modular architecture, with separate classes for File and AutoDoc.                             |
| **📖 Documentation**   | The codebase lacks comprehensive documentation. However, each file includes comments providing explanations for each class and function.                                            |
| **🔗 Dependencies**    | The codebase relies on several external libraries such as os, argparse, configparser, and RevChatGPT.                                                           |
| **🧩 Modularity**      | The codebase is well-organized into smaller, reusable components, such as the AutoDoc and File classes.                                                                  |
| **✔️ Testing**          | The codebase doesn't have explicit testing strategies or tools mentioned, making it difficult to assess the system's testing approach.                                      |
| **⚡️ Performance**      | The codebase doesn't explicitly focus on performance characteristics, such as speed or resource usage.                                                                 |
| **🔐 Security**        | The codebase doesn't address security measures directly, so security considerations might need to be added if necessary.                                               |
| **🔀 Version Control** | The codebase uses Git for version control. The link to the repository is provided, indicating version control practices are in place.                            |
| **🔌 Integrations**    | The codebase integrates with RevChatGPT library to generate comments based on the provided code.                                                            |
| **📶 Scalability**     | The codebase doesn't have specific scalability considerations mentioned, but it can be extended with new functionality.                                               |

---


## 📂 Project Structure




---

## 🧩 Modules

## AutoDoc-ChatGPT\main.py

This code script is for a console application called AutoDoc that generates code documentation using ChatGPT. The script imports necessary modules such as os, argparse, configparser, and several custom modules. It also reads configuration information from a config.ini file.

The auth variable is set by extracting email, password, and session_token values from the config.ini file.

The script defines an argparse.ArgumentParser object with a description for the AutoDoc application. It adds a command-line argument for the code file path.

The script checks if the code file specified exists. If not, it exits with an error message.

A File object is created using the specified code file path.

An AutoDoc object is created using the authentication information, the content of the file, and the detected language of the file.

The AutoDoc instance is used to start the documentation generation, and the result is saved.

A commented version of the original code file with the generated documentation is created using the File object.

Now, here are brief descriptions for each function and class:

- Function: args.file
   - Description: Retrieves the value of the -file argument specified in the command line.
   
- Class: File
   - Description: Represents a code file. It provides methods to read the file content, detect the language, and create a commented version with generated documentation.
   
- Class: AutoDoc
   - Description: Represents the AutoDoc application. It connects to ChatGPT for code documentation generation. It requires authentication, code content, and language information as parameters for initialization. It provides a method to start the documentation generation process.
   
- Function: exit
   - Description: Exits the script execution with an error message.
   
- Function: os.path.exists(path)
   - Description: Checks if a path exists on the file system.
## AutoDoc-ChatGPT\modules\autodoc.py

The code script is a Python program that automates the process of generating comments for code. It uses the RevChatGPT library to communicate with an AI chatbot and generate comments based on the code provided.

The main class in the script is `AutoDoc`, which takes a configuration, code, and language as inputs. The `__init__` method initializes the class with the provided inputs. It validates the code and language, and exits the program with an error message if there are any issues.

The private method `__ask` is used to communicate with the chatbot and retrieve a response. It takes the code as an input and returns the chatbot's response. If there is an error in the chatbot communication, it raises a `ValueError`.

The `start` method is the main entry point of the program. It divides the code into smaller parts using the `Divider` class. If the code is empty or cannot be divided, it exits with an error message. It then connects to the chatbot using the provided configuration (session token or email/password). After that, it iterates over the divided code parts and asks the chatbot for comments. The comments are stored in the `__comments` list. Finally, it merges the code and comments using the `Result` class and returns the commented code.

Overall, the `AutoDoc` class provides a convenient way to automate the process of generating comments for code using an AI chatbot.