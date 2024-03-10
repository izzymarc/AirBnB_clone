
# AirBnB Clone - The Console

## Table of Contents

- [Introduction](#introduction)
- [Environment](#environment)
- [Installation](#installation)
- [Testing](#testing)
- [Usage](#usage)
- [Authors](#authors)

## Introduction

This team project aims to build a clone of [AirBnB](https://www.airbnb.com/). The console is a command interpreter to manage the abstraction between objects and how they are stored. This includes creating new objects, retrieving objects from a file, performing operations on objects, and destroying objects.

For a fundamental background of the project, visit the [Wiki](https://github.com/izzymarc/AirBnB_clone/wiki).

### Storage

All classes are managed by the `Storage` engine in the `FileStorage` Class.

## Environment

The project is developed and tested on Ubuntu 20.04 LTS using Python 3.8.3. Editors used include VIM 8.1.2269, Visual Studio Code 1.6.1, and Atom 1.58.0. Version control is handled with Git 2.25.1.

Style guidelines:
- [pycodestyle (version 2.7.*)](https://pypi.org/project/pycodestyle/)
- [PEP8](https://pep8.org/)

## Installation

To install the console, clone the repository to your local machine by running:

```bash
git clone https://github.com/thisislaait/AirBnB_clone.git
# or
git clone https://github.com/izzymarc/AirBnB_clone.git
```

After cloning, change into the AirBnB directory:

```bash
cd AirBnB_clone
```

To start the console, run:

```bash
./console.py
```

### Execution

- **Interactive mode:**

  ```bash
  $ ./console.py
  (hbnb) help

  Documented commands (type help <topic>):
  ========================================
  EOF  help  quit

  (hbnb) quit
  $
  ```

- **Non-interactive mode:**

  ```bash
  $ echo "help" | ./console.py
  (hbnb)

  Documented commands (type help <topic>):
  ========================================
  EOF  help  quit
  (hbnb)
  $
  ```

## Testing

Tests are located in the `tests` folder. For documentation and unit tests:

- **Modules:** `python3 -c 'print(__import__("my_module").__doc__)'`
- **Classes:** `python3 -c 'print(__import__("my_module").MyClass.__doc__)'`
- **Functions:** Inside and outside a class: `python3 -c 'print(__import__("my_module").my_function.__doc__)'` and `python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'`

### Python Unit Tests

- Use the unittest module.
- File extension `.py`.
- Files and folders start with `test_`.
- For `models/base.py`, unit tests are in: `tests/test_models/test_base.py`.
- To run all tests: `python3 -m unittest discover tests`.

## Usage

### Starting the console

```bash
$ ./console.py
(hbnb)
```

### Available Commands

For a full list of commands, use the `help` command in the console.

## Authors

**Ezekiel Gwamna** & **Ugo Ogadi**

- Email: [izzymarc@gmail.com](mailto:izzymarc@gmail.com)
- Email: [ogadi.ugo@gmail.com](mailto:ogadi.ugo@gmail.com)

GitHub Repositories:
- [https://github.com/thisislaait/AirBnB_clone](https://github.com/thisislaait/AirBnB_clone)
- [https://github.com/izzymarc/AirBnB_clone](https://github.com/izzymarc/AirBnB_clone)

## Adding an AUTHORS File

To generate a list of authors from the git repository, use the following bash script:

```bash
#!/bin/sh

git shortlog -se \
  | perl -spe 's/^\s+\d+\s+//' \
  | sed -e '/^CommitSyncScript.*$/d' \
  > AUTHORS
```
