# The AirBnB Clone Project
![AirBnB Logo](https://www.pngitem.com/pimgs/m/132-1322125_transparent-background-airbnb-logo-hd-png-download.png)

## Project Description
This signifies the inaugural stage of the AirBnB clone project, emphasizing backend development and integration with a console application leveraging Python's cmd module.

Data, represented as Python objects, is generated and stored within a JSON file, accessible via the Python json module.

## Description of the Command Interpreter:
The application's interface mirrors that of the Bash shell, featuring a concise set of commands tailored for AirBnB website functionality.

Acting as the frontend for the web application, this command-line interpreter enables users to interact with the backend developed using Python's object-oriented programming (OOP) capabilities.

Some of the available commands include:
- show
- create
- update
- destroy
- count

Through this command-line interpreter and the backend, users can engage in various actions such as:
- Creating new objects (e.g., User or Place instances)
- Retrieving objects from files or databases
- Performing operations on objects (e.g., counting or computing statistics)
- Updating object attributes
- Deleting objects

## How to Get Started
Use the following instructions to set up the project on your local Linux machine for development and testing purposes.

## Installation

Clone the project repository from GitHub. This repository contains the simple shell program and its dependencies.

```
git clone https://github.com/Ojay16/AirBnB_clone.git
```

After cloning, you will have a folder named "AirBnB_clone" containing various files that enable the program's functionality.

> /console.py: The primary executable for the project, serving as the command interpreter.
>
> models/engine/file_storage.py: A class responsible for serializing instances to a JSON file and deserializing JSON files to instances.
> 
> models/__ init __.py: Contains a unique `FileStorage` instance for the application.
> 
> models/base_model.py: Defines common attributes and methods shared by other classes.
> 
> models/user.py: Represents the User class, which inherits from BaseModel.
> 
> models/state.py: Represents the State class, which inherits from BaseModel.
>
> models/city.py: Represents the City class, which inherits from BaseModel.
>
> models/amenity.py: Represents the Amenity class, which inherits from BaseModel.
>
> models/place.py: Represents the Place class, which inherits from BaseModel.
>
> models/review.py: Represents the Review class, which inherits from BaseModel.

## How to Use It
The program can operate in two modes: Interactive and Non-interactive.

**Interactive Mode:** In this mode, the console displays a prompt (hbnb) where users can enter and execute commands. After executing a command, the prompt reappears, waiting for the next command. This cycle continues until the user exits the program.

**Non-interactive Mode:** To run the shell in non-interactive mode, you pipe a command into its execution. In this mode, no prompt is displayed, and no further input is expected from the user.

## Command Input Format
You can input commands into the console by directly typing them in interactive mode or by utilizing an echo command in non-interactive mode. It's important to separate commands with spaces.

Examples:

Interactive Mode:
```
$ ./console.py
(hbnb) help
Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
(hbnb) 
(hbnb) quit
$
```

Non-interactive Mode:
```
$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
```

## Available Commands and Their Functions
The console runs the following commands:

| Command | Description |
| ------- | ----------- |
| **quit or EOF** | Exits the program. |
| **help** | Provides information on how to use a specific command. |
| **create** | Creates a new instance of a specified `Class`, saves it to the JSON file, and prints the `id`. Valid classes include BaseModel, User, State, City, Amenity, Place, and Review. |
| **show** | Prints the string representation of an instance based on the class name and `id`. |
| **destroy** | Deletes an instance based on the class name and `id` (saves the change to the JSON file). |
| **all** | Prints string representations of all instances based on the class name or all objects if no class name is specified. |
| **update** | Updates an instance based on the class name and `id` by adding or updating attributes (saves the changes to the JSON file). |
| **count** | Retrieves the number of instances of a class. |

## Authors
Ojemare Julius | [GitHub](https://github.com/Ojay16)

