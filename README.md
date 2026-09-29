# File-Management
# 📁 File Management App

A simple command-line file manager written in Python. It lets you create, view, read, edit, and delete files from an interactive menu, using only the standard library.

## Features

- **Create** a new empty file
- **View** all files in the current directory
- **Read** the contents of a file
- **Edit** a file by appending text to it
- **Delete** a file
- Error handling for missing files, existing files, and other unexpected errors

## Usage

Run the program:

```bash
python main.py
```

You will see this menu:

```
FILE MANAGEMENT APP
1: Create file
2: View all files
3: Delete file
4: Read file
5: Edit file
6: Exit
```

Enter a number from 1 to 6 and follow the prompts.

## Example

```
Enter your choice (1-6) = 1
Enter the file name to create = notes.txt
File 'notes.txt' created successfully!

Enter your choice (1-6) = 5
Enter file name to edit = notes.txt
Enter data to add = Hello, world!
Content added to 'notes.txt' successfully!

Enter your choice (1-6) = 4
Enter file name to read = notes.txt
Content of 'notes.txt':
Hello, world!
```

## Project Structure

```
file-management-app/
├── main.py
└── README.md
```

## How It Works

| Function        | Description                                              |
|-----------------|----------------------------------------------------------|
| `create_file`   | Creates a new file (fails if it already exists)          |
| `view_all_files`| Lists everything in the current directory                |
| `delete_file`   | Removes the specified file                               |
| `read_file`     | Prints the contents of the specified file                |
| `edit_file`     | Appends user-entered text to the specified file          |
| `main`          | Runs the menu loop until the user chooses to exit        |

## Notes

- The app works in the directory where you run it.
- Editing uses append mode, so existing content is never overwritten.
- Deleting a file is permanent, so use it carefully.

## Future Improvements

- Overwrite/replace file content option
- Rename and copy file features
- Filter to show only files (not folders)
- Confirmation prompt before deleting

## Author

Riya Uikey
