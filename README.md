# 🛠️ TaskCLI – Command-Line Task Tracker in C#

TaskCLI is a simple command-line task manager built using C# and .NET. It helps you manage your daily tasks directly from the terminal with a clean and minimal interface. All tasks are stored in a local JSON file, with support for adding, updating, deleting, and tracking task status (`todo`, `in-progress`, `done`).

---

## ✨ Features

- ✅ Add new tasks
- ✅ Update task descriptions
- ✅ Delete tasks by ID
- ✅ Mark tasks as in-progress or done
- ✅ List all tasks or filter by status
- ✅ Stores tasks in `tasks.json`
- ✅ Lightweight, no external libraries

---

## ⚙️ Requirements

- [.NET SDK](https://dotnet.microsoft.com/download) (Core 3.1 or later)
- C# 8.0+

---

## 🚀 Getting Started

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/task-cli.git
   cd task-cli
   ```

2. **Build the project:**

   ```bash
   dotnet build
   ```

3. **Run the CLI tool:**

   ```bash
   dotnet run -- <command> [arguments]
   ```

---

## 📘 Usage Examples

### ✅ Add a Task
```bash
dotnet run -- add "Buy groceries"
```

### ✏️ Update a Task
```bash
dotnet run -- update 1 "Buy groceries and cook dinner"
```

### ❌ Delete a Task
```bash
dotnet run -- delete 1
```

### 🔁 Change Task Status
```bash
dotnet run -- mark-in-progress 1
dotnet run -- mark-done 1
```

### 📋 List Tasks
```bash
dotnet run -- list              # List all tasks
dotnet run -- list todo         # Only todo tasks
dotnet run -- list in-progress  # Only in-progress tasks
dotnet run -- list done         # Only completed tasks
```

---

## 🗂️ Task Data Format

Each task is stored in a JSON file like this:

```json
{
  "id": 1,
  "description": "Buy groceries",
  "status": "todo",
  "createdAt": "2025-07-24T14:15:00",
  "updatedAt": "2025-07-24T14:15:00"
}
```

---

## 🔒 Error Handling

- Handles missing or invalid IDs
- Creates `tasks.json` if it doesn't exist
- Prevents crashes on invalid inputs

---

## 🧠 Optional Improvements (Future Ideas)

- `help` command
- Sort tasks by creation date or status
- Highlight output with colors
- Backup `tasks.json` before deleting

---

## 📄 License

MIT License — free for personal or commercial use.

---

## 👨‍💻 Author

**Bibek Chandra Dey**  
Junior .NET Developer  
🇧🇩 Bangladesh
