# 🛠️ Stima Engineer

![Updated Features](https://img.shields.io/badge/Features-Updated-brightgreen)

一個專為開發者設計的命令行工具，旨在高效管理和互動他們的專案。利用Stima API的強大功能，stima-engineer提供代碼生成、文件編輯、專案規劃和代碼審查等功能，以簡化您的開發流程。

## 🛠️ Updated Features

- **Enhanced File and Folder Management**: The `/add` and `/edit` commands now support adding and modifying both files and folders, providing greater flexibility in managing your project structure.
- **Project Planning**: Introducing the `/planning` command, which allows users to create comprehensive project plans that can be used to generate files and directories systematically.
- **Advanced Workflows**: New examples demonstrate how to integrate planning and creation commands for efficient project setup.

## ✨ Features

- **Automated Code Generation**: Generate code for your projects effortlessly.

- **File Management**: Add, edit, and manage project files directly from the command line.

- **Interactive Console**: User-friendly interface with rich text support for enhanced readability.

- **Conversation History**: Save and reset conversation histories as needed.

- **Code Review**: Analyze and review code files for quality and suggestions.

- **Enhanced File and Folder Management**: The `/add` and `/edit` commands now support adding and modifying both files and folders, providing greater flexibility in managing your project structure.

- **Project Planning**: Introducing the `/planning` command, which allows users to create comprehensive project plans that can be used to generate files and directories systematically.

## 💡 How the Script Works

1. **Initialization**: The script initializes global variables and sets up the OpenAI client using the provided API key.

2. **Handling User Commands**: It listens for user commands such as `/edit`, `/create`, `/add`, `/review`, and the new `/planning` command, processing them accordingly.

3. **Processing File and Folder Modifications**: Based on the user's instructions, the script modifies files and folders, adds new content, or creates new files and folders as needed. The `/add` and `/edit` commands have been enhanced to support both files and folders, providing greater flexibility in project management.

4. **Project Planning**: The newly introduced `/planning` command allows users to create comprehensive project plans, which the script can use to generate files and directories systematically using the `/create` command.

5. **AI-Generated Instructions**: The tool interacts with OpenAI's API to generate instructions and suggestions for code generation, editing, project planning, and reviewing.

6. **Applying Changes**: Changes are applied to the project files and folders based on the AI-generated instructions, ensuring that the project stays up-to-date and well-maintained.

7. **Managing Conversation History and Added Files**: The script manages the conversation history and keeps track of files and folders added to the context, allowing users to reset or modify the history as needed.

## 📥 Installation

### Prerequisites

- **Python**: Ensure you have Python 3.7 or higher installed. [Download Python](https://www.python.org/downloads/)

- **Stima API Key**: Obtain an API key from [Stima API](https://api.stima.tech).

### 🔧 Steps

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/stima-tech/stima-engineer.git
   ```

2. **Navigate to the Project Directory**:

   ```bash
   cd stima-engineer
   ```

3. **Install Dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

## 📚 Usage

Launch the application using the following command, and **Add API Key and Model Name  at the tail**:
If not specify model name, use **claude-3-5-sonnet-20240620** as default model.

```bash
python eng.py --api-key=sk-xxxxxxxxxx  --model MODEL_NAME# you have to type your Stima API Key and the model name you need
```

### 🎮 Available Commands

- `/edit`: Edit files or folders (followed by file or folder paths)

- `/create`: Create files or folders (followed by instructions)

- `/add`: Add files or folders to context (followed by file or folder paths)

- `/planning`: Plan project structure and tasks (followed by instructions)

- `/debug`: Print the last AI response

- `/reset`: Reset chat context and clear added files

- `/review`: Review and analyze code files for quality and potential improvements (followed by file or folder paths)

- `/quit`: Exit the program

### 🚀 Advanced Workflows

Here's an example workflow that demonstrates using `/planning` followed by `/create` to generate files based on the created plan:

1. **Planning the Project**:

   ```bash
   You: /planning Create a basic web application with the following structure:
   
   - A frontend folder containing HTML, CSS, and JavaScript files.
   
   - A backend folder with server-side scripts.
   
   - A README.md file with project documentation.
   ```

2. **Creating the Project Structure based on the Plan**:

   ```bash
   You: /create Generate the project structure based on the above plan.
   ```

This demonstrates how to use the new `/planning` command to define a project structure, and then `/create` to generate the files and folders accordingly.

### 📝 Examples

```bash
You: /add src/main.py src/utils/helper.py src/models/

You: /planning Outline a RESTful API project with separate folders for models, views, and controllers.

You: /create Set up the basic structure for a RESTful API project with models, views, and controllers folders, including initial files.

You: /edit src/main.py src/models/user.py src/views/user_view.py
```

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository.

2. Create a new branch (`git checkout -b feature/YourFeature`).

3. Commit your changes (`git commit -m 'Add some feature'`).

4. Push to the branch (`git push origin feature/YourFeature`).

5. Open a pull request.

## 🙏 Acknowledgments
- [o1-engineer](https://github.com/Doriandarko/o1-engineer)


