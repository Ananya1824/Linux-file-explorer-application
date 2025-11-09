# 🐧 Linux File Explorer Application

A comprehensive **console-based File Explorer application** written in **C++** for Linux operating systems.  
This project provides complete file management — navigation, manipulation, search, and permission control — all from the terminal.

---

## 📋 Project Overview

**Assignment:** Capstone Project — File Explorer Application  
**Language:** C++  
**Platform:** Linux OS  
**Development Duration:** 5 Days  

---

## 🎯 Features

### 🗓️ Day 1: Basic Operations
- ✅ List files in current directory (simple and detailed views)
- ✅ Display file information with color coding
- ✅ Show file sizes, modification times, and types

### 🗓️ Day 2: Navigation
- ✅ Change directories (absolute and relative paths)
- ✅ Navigate to parent directory
- ✅ Display current working directory
- ✅ Real-time directory tracking

### 🗓️ Day 3: File Manipulation
- ✅ Create new files and directories
- ✅ Delete files/directories (supports recursive deletion)
- ✅ Copy and move files/directories (recursive and cross-filesystem support)
- ✅ Rename files and directories

### 🗓️ Day 4: Search Functionality
- ✅ Recursive file search
- ✅ Case-insensitive filename matching
- ✅ Display results with full paths

### 🗓️ Day 5: Permission Management
- ✅ View permissions (symbolic & octal)
- ✅ Change file permissions (`chmod`)
- ✅ Change ownership (`chown`)
- ✅ Display owner/group information

---

## 🛠️ Prerequisites

- Linux OS (Ubuntu, Debian, Fedora, etc.)
- G++ compiler (`v4.8+`)
- `make` utility
- Standard C++ libraries
- `sudo` access (optional for permission tasks)

---

## 📦 Installation

### 1️⃣ Clone or Download the Project
```bash
git clone https://github.com/your-username/linux-file-explorer.git
cd linux-file-explorer
```

### 2️⃣ Compile the Application
**Using Make:**
```bash
make
```

**Manual Compilation:**
```bash
g++ -Wall -Wextra -std=c++11 -O2 -o file_explorer file_explorer.cpp
```

### 3️⃣ Run the Application
```bash
./file_explorer
```

### 4️⃣ Optional: Install System-wide
```bash
sudo make install
```
Then run it anywhere:
```bash
file_explorer
```

---

## 🎮 Usage Guide

### 🧭 Main Menu
```
📂 Navigation & Listing:
  1. List files (simple)
  2. List files (detailed)
  3. Change directory
  4. Go to parent directory

📁 File Operations:
  5. Create file
  6. Create directory
  7. Delete file/directory
  8. Copy file/directory
  9. Move file/directory
  10. Rename file/directory

🔍 Search:
  11. Search files

🔐 Permissions:
  12. View file permissions
  13. Change permissions (chmod)
  14. Change owner/group (chown)

⚙️ Other:
  15. Display current path
  0. Exit
```

Each menu provides clear emoji-based feedback for user-friendly interaction.

---

## 🎨 Enhanced UI Features

### Visual Improvements
- **📍 Current Directory Display** — always visible
- **🌈 Color Coding:**
  - Blue: Directories 📁  
  - Green: Executables ⚡  
  - White: Regular files 📄  
  - Red: Errors ❌  
  - Yellow: Warnings ⚠️  
  - Cyan: Info ℹ️  

### Usability
- Grouped, clear menu organization  
- Real-time path updates  
- Safe recursive operations  
- Confirmation prompts for destructive actions  

---

## 🧠 Technical Details

### System Calls Used
- `opendir()`, `readdir()`, `closedir()`
- `stat()`, `mkdir()`, `rmdir()`, `unlink()`
- `rename()`, `chmod()`, `chown()`
- `getcwd()`, `chdir()`

### Permission Formats
- **Symbolic:** `drwxr-xr-x`
- **Octal:** `755`

```
Owner  Group  Others
rwx    r-x    r-x
421    421    421
```

---

## 🔐 Permissions & Privileges

### Normal Operations
- Reading, listing, and searching  
- Creating/copying files (write permission)  

### Admin Operations
- Ownership change via `chown`
- System-level permission modifications

---

## 🐛 Error Handling

Handles:
- Invalid directory paths  
- Permission denied  
- File not found  
- Invalid input  
- Recursive deletion warnings  

---

## 🚀 Advanced Features

- Recursive file search  
- Smart file size formatting (B, KB, MB, GB)  
- User confirmation for critical actions  
- Cross-path support (absolute & relative)  

---

## 📊 Project Structure
```
File Explorer/
├── file_explorer.cpp   # Main source
├── Makefile            # Build config
└── README.md           # Documentation
```

---

## 🔧 Build Options

### Debug Build
```bash
g++ -Wall -Wextra -std=c++11 -g -o file_explorer_debug file_explorer.cpp
```

### Optimized Build
```bash
g++ -Wall -Wextra -std=c++11 -O3 -o file_explorer file_explorer.cpp
```

---

## 📚 Learning Outcomes

- Mastery of **Linux System Programming**
- Deep understanding of **File System APIs**
- Implementation of **process and permission management**
- Use of **modern C++ features**
- **Robust error handling**
- Development of **interactive CLI tools**

---

## 📅 Day-wise Implementation Summary

| Day | Focus Area | Status |
|------|-------------|--------|
| 1 | Basic Operations | ✅ Complete |
| 2 | Navigation | ✅ Complete |
| 3 | File Manipulation | ✅ Complete |
| 4 | Search Functionality | ✅ Complete |
| 5 | Permission Management | ✅ Complete |

---

## ⚠️ Important Notes

- Use `sudo` for restricted operations.  
- Deletion works recursively only with confirmation.  
- Copy operations overwrite existing files.  
- Symbolic links appear as regular files in simple view.

---

## 🔄 Future Enhancements

- Recursive deletion improvements  
- File preview support  
- Zip/tar integration  
- Sorting & filtering  
- Favorites/bookmarks  
- Batch operations  
- Command history  

---

## 📄 License

This is an **educational project** developed as part of the Capstone Assignment.

---

## 👨‍💻 Developer Information

**Developer:** Ananya Kumari Panda
**Duration:** 5 Days  
**Tested On:** Ubuntu Linux  
**Compiler:** G++ (C++11)  
**GitHub:** [https://github.com/Ananya1824](https://github.com/Ananya1824)

---

## 🎓 Conclusion

This **Linux File Explorer Application** provides a fully functional and feature-rich file management system via the command line.  
It demonstrates strong proficiency in **C++ programming, Linux system calls, and software design principles**.

> **Happy Exploring! 🚀**
