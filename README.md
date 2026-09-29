# File Management  
A simple command-line file manager written in Python. It lets you create, view, read, edit and 
delete text files from a menu. 
This is a first-year student project made to practise Python file handling and exception handling. 
## Features
 - Create a new file
 - View all files in the current folder
 - Read the content of a file
 - Add text to a file
 - Delete a file
- Friendly error messages (file already exists, file not found, etc.) 
 
## How to Run 
1. Download `file_manager.py` and save it in any folder. 
2. Open a terminal in that folder. 
3. Run: 
``` 
python file_manager.py 
``` 
## Menu Options 
| Option | What it does | 
|--------|--------------| 
| 1 | Create a new file | 
| 2 | View all files in the folder | 
| 3 | Delete a file | 
| 4 | Read a file | 
| 5 | Add text to a file | 
| 6 | Exit | 
## Example 
``` 
FILE MANAGEMENT APP 
1: Create file 
2: View all files 
3: Delete file 
4: Read file 
5: Edit file 
6: Exit 
Enter your choice (1-6) = 1 
Enter the file name to create = notes.txt 
File 'notes.txt' created successfully! 
Enter your choice (1-6) = 5 
Enter the file name to edit = notes.txt 
Enter data to add = Hello world 
Content added to 'notes.txt' successfully! 
Enter your choice (1-6) = 4 
Enter the file name to read = notes.txt 
Content of 'notes.txt': 
Hello world 
``` 
## How It Works 
| Function | What it uses | 
|----------|--------------| 
| `create_file` | `open(filename, 'x')` creates a file and fails if it already exists | 
| `view_all_files` | `os.listdir()` lists everything in the folder | 
| `read_file` | `open(filename, 'r')` reads the content | 
| `edit_file` | `open(filename, 'a')` adds text at the end | 
| `delete_file` | `os.remove()` deletes the file | 
Errors such as `FileExistsError` and `FileNotFoundError` are handled with `try/except`, so the 
program shows a message instead of crashing. 
## Notes 
- Deleting a file is permanent.
- The app works only in the folder where you run it. 
## Concepts Used 
Functions, loops, conditions, file handling, `with` statement, exception handling, and the `os` 
module. 
## Author 
Riya Uikey 
 
