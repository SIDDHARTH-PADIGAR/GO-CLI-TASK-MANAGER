# Todo List CLI Application

A simple Command Line Interface (CLI) Todo List application written in Go. This project demonstrates basic operations like adding, deleting, editing, and toggling todos, and it stores the todo list in a JSON file.

## Installation

1. Clone the repository
   ```sh
   git clone https://github.com/your_username/todo-cli.git
   cd todo-cli
Run the application

sh
go run ./ -list
Usage
Here are the available commands for the application:

Add a new todo

sh
go run ./ -add "Title of your todo"
List all todos

sh
go run ./ -list
Edit a todo by index

sh
go run ./ -edit "index:new title"
Toggle the completion status of a todo by index

sh
go run ./ -toggle index
Delete a todo by index

sh
go run ./ -del index
Example
sh
$ go run ./ -add "Walk the dog"
$ go run ./ -list
Output:

#	Title	Completed	Created At	Completed At
0	Walk the dog	❌	Wed, 20 Nov 2024 18:37	
File Structure
main.go: Entry point of the application

todo.go: Contains the Todo struct and related methods

command.go: Handles command line flags and operations

storage.go: Manages loading and saving of todos to a JSON file

License
Distributed under the MIT License. See LICENSE for more information.
