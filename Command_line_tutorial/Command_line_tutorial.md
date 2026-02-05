## Self-Guided Command Line Tutorial (Beginner, Mac, ~30 min)

Welcome! This hands-on tutorial will help you build confidence with the command line in your VS Code terminal on a Mac. Work through each step, typing the commands in your terminal. Read the explanations and try the suggested experiments.

### 1. Navigating Directories

- **See where you are:**  
  ```bash
  pwd
  ```
  This prints your "present working directory".

- **List files and folders:**  
  ```bash
  ls
  ```
  Try adding the `-l` flag for more detail:  
  ```bash
  ls -l
  ```

- **Move into a directory:**  
  ```bash
  cd Documents
  ```
  Replace `Documents` with any folder you see from `ls`.

- **Go up one level:**  
  ```bash
  cd ..
  ```

- **Go to your home directory:**  
  ```bash
  cd ~
  ```

- **Tab completion:**  
  Start typing a folder or file name, then press `Tab` to auto-complete. Try:  
  ```bash
  cd Doc<Tab>
  ```

### 2. Making Directories and Files

- **Create a new directory:**  
  ```bash
  mkdir test_folder
  ```

- **Move into your new directory:**  
  ```bash
  cd test_folder
  ```

- **Create an empty file:**  
  ```bash
  touch hello.txt
  ```

- **Edit a file (opens in VS Code):**  
  ```bash
  code hello.txt
  ```
  *(If `code` doesn't work, open from VS Code's File menu.)*

- **Write text to a file:**  
  ```bash
  echo "This is my first file!" > hello.txt
  ```

- **View file contents:**  
  ```bash
  cat hello.txt
  ```

### 3. Copying, Moving, and Renaming

- **Copy a file:**  
  ```bash
  cp hello.txt copy.txt
  ```

- **Move (rename) a file:**  
  ```bash
  mv copy.txt renamed.txt
  ```

- **Move a file to another directory:**  
  ```bash
  mkdir subfolder
  mv renamed.txt subfolder/
  ```

- **Check your work:**  
  ```bash
  ls
  ls subfolder
  ```

### 4. Removing Files and Directories

- **Remove a file:**  
  ```bash
  rm hello.txt
  ```

- **Remove an empty directory:**  
  ```bash
  rmdir subfolder
  ```
  *(If not empty, use `rm -r subfolder` to remove folder and contents.)*

- **Remove a directory and all its contents (dangerous!):**  
  ```bash
  rm -r test_folder
  ```

### 5. Flags and Help

- **Flags modify command behavior.**  
  Try:  
  ```bash
  ls -a
  ```
  (`-a` shows hidden files)

- **See help for a command:**  
  ```bash
  man ls
  ```
  *(Press `q` to quit the manual.)*

- **Quick help:**  
  ```bash
  ls --help
  ```

### 6. Practice Challenge

1. In your home directory, create a folder called `practice`.
2. Inside `practice`, create two files: `one.txt` and `two.txt`.
3. Write your name into `one.txt` and today's date into `two.txt`.
4. Copy both files into a new folder called `backup`.
5. Delete `one.txt` from `practice`.
6. Move `two.txt` from `practice` to `backup`.
7. Remove the `practice` folder (should now be empty).
8. List the contents of `backup` to confirm both files are there.

Try to do this without looking back at the commands above. If you get stuck, refer to the relevant section.

---

**Congratulations!**  
You've completed the basics of the command line. Practice these skills regularly—they are essential for bioinformatics and data science.
