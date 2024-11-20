# Go Todos CLI

A simple and efficient CLI-based To-Do application written in Go. Manage your tasks with features like adding, editing, deleting, toggling completion, and listing todos.

---

## Features
- Add, edit, delete, or toggle the completion status of todos.
- Persistent storage using JSON files.
- Clean and user-friendly tabular output.
- Minimalistic CLI-based workflow.

---

## Getting Started

### Prerequisites
- Go installed (version 1.18 or later).

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/go-todos-cli.git
   cd go-todos-cli
   
### Run this application
```bash
go run ./
```

---

## Usage

### Commands:
- List all todos:
```bash
go run ./ -list
```
### Example Output:
![image](https://github.com/user-attachments/assets/de5db7f5-775a-4967-a730-badbf91a029a)
---
- Add a new todo:
```bash
go run ./ -add "Practice Go"
```
### Example Output:
![image](https://github.com/user-attachments/assets/fe0d1b17-2835-4e1e-8f7e-aacab20e156d)
---
- Edit a todo (format: id:new_title):
```bash
go run ./ -edit "1:Go to the gym"
```
### Example Output:
![image](https://github.com/user-attachments/assets/d66f2620-41c2-471b-8eaa-e6d6c952a64b)
---
- Toggle completion:
```bash
go run ./ -toggle 1
```
### Example Output:
![image](https://github.com/user-attachments/assets/13adf5cc-267d-478c-ab81-2bb38d1a45b3)
---
- Delete a todo:
```bash
go run ./ -del 0
```
### Example Output:
![image](https://github.com/user-attachments/assets/59cafecc-83cc-49d4-ac67-24647a68f2ed)

---

## JSON data format

Todos are stored persistently in a todos.json file in the following format:
```json
[
    {
        "Title": "Go to the gym",
        "Completed": true,
        "CreatedAt": "2024-11-20T13:36:45.7191398+05:30",
        "CompletedAt": "2024-11-20T19:15:19.2441337+05:30"
    },
    {
        "Title": "Go for a swim",
        "Completed": true,
        "CreatedAt": "2024-11-20T13:46:57.9514189+05:30",
        "CompletedAt": "2024-11-20T18:38:54.8653736+05:30"
    },
    {
        "Title": "Complete documentation",
        "Completed": false,
        "CreatedAt": "2024-11-20T18:37:24.8932658+05:30",
        "CompletedAt": null
    },
    {
        "Title": "Practice Go",
        "Completed": false,
        "CreatedAt": "2024-11-20T19:10:01.9222751+05:30",
        "CompletedAt": null
    }
]
```

---

## Technologies used:
- Go: Core programming language.
- JSON: Persistent storage for todos.
- Aquasecurity/Table: For clean tabular CLI outputs.

---

## Conclusion
**The Go Todos CLI is a simple, yet powerful command-line tool for managing your tasks. This project marks my first foray into using Go, and it’s been an exciting journey learning the language while building a useful tool. With its easy-to-use commands and persistent storage, it’s perfect for anyone looking to keep track of their to-dos in a minimalistic way. Whether you're managing personal tasks or experimenting with Go, this project offers a solid foundation for learning and productivity.**



