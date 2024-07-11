# Microsoft: First Steps with Rust - Capstone

Welcome to the final code repository for the Capstone Project of the Microsoft introductory Rust course. The project involves implementing a CLI application named Rusty-Journal to manage daily tasks. This application is controlled via the command line, eliminating the need for a GUI. The app is designed to handle command-line arguments and appropriately interpret user actions. The application supports the following actions:

Add a new task to the list.

Remove a completed task from the list.

Display all current tasks.

The program saves all tasks in a text file with data encoded in JSON format. It consists of two modules: CLI and Tasks, which manage the specified functionalities. The main module integrates these components and handles potential errors.

# The CLI Module

The CLI module processes user input and parses it into a struct that can be utilized by the main function. Key components include:

CommandLineArgs Struct: Contains the actions (add, remove, list tasks) defined in the Action enum.

Journal File Path: An optional argument allowing users to specify a different journal file.

# The Tasks Module

The Tasks module manages and displays tasks. Key features include:

Task Struct: Contains the task description and a timestamp (using the chrono crate).

Task List: Modeled as a vector (Vec<Task>), where completed tasks are simply removed from the vector.

This setup ensures efficient task management and clear separation of concerns within the application.
