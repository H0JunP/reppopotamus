# Lecture Note on Shell Commands
## How to launch Shell Terminal
- **Linux / MacOS**

  Search for **"Terminal"** in the apps and launch it!
- **Windows**

  Install the application called **"[Git Bash](https://git-scm.com/)"** (Because Windows doesn't use standard shell commands in default shell terminal)

## Some Shell Commands That May be Helpful to Know

## Directory Commands
### **pwd**

  Shows the current path in a hierarchical directory

  ![pwd example](https://github.com/H0JunP/reppopotamus/assets/134226638/f053b70f-2306-4eb0-9437-bdc8a42a39f6)
  ```sh
  $ pwd
  ```
---
### **cd**

  Changes the directory you're currently in
  #### Arguments
  - **[directory name]**
  - **/** : change directory to root folder
  - **.** : change directory in current folder
  - **..** : change to upper-level directory
  - **/[directory name]** : set the absolute path
  - **./[directory name]** : set the relative path
  - **../[directory name]** : set the relative path
 
  ![cd example](https://github.com/H0JunP/reppopotamus/assets/134226638/42d1ab88-12c6-4ed1-988b-350e6f9d2a87)
  ```sh
  $ cd (The path of directory you want to go)
  ```
---
### **ls**

  Shows the files located in current directory
  #### Options
  - **-l** : Shows detailed information (long format)
  - **-lh** : Same as above, but shows file size in units
  - **-la** : Shows all files (even hidden files)
  #### Long Format
  ![long format explanation](https://github.com/H0JunP/reppopotamus/assets/134226638/0a6acb48-371c-4618-9e0a-a5a94e7f8f5d)

  ![ls example](https://github.com/H0JunP/reppopotamus/assets/134226638/52a3b91a-6b81-4dc0-8515-b8ce974ce6dd)
  ```sh
  $ ls (directory you want to see contents of)
  $ ls -l (directory you want to see contents of)
  $ ls -la (directory you want to see contents of)
  ```
---
## Manipulation Commands
```diff
- WARNING: THESE COMMANDS MAY DELETE OR OVERWRITE YOUR FILES AND DIRECTORIES!
- MAKE SURE TO MAKE BACKUP BEFORE USING THESE COMMANDS AND USE IT AT YOUR OWN RISK!
```
---
### Wildcards
- **\*** : All filenames
- **g\*** : All filenames that begin with the character "g"
- **b\*.txt** : All filenames that begin with the character "g" and end with the characters ".txt"
- **Data???** : Any filename that begins with the characters "Data" followed by exactly 3 more characters
---
### **cp**

  Copy files and directories
  
  #### Options
  - **-i** : if the file with same name exists, the user is prompted before it is overwritten
  - **-r** : if file does not exist, it is created, Otherwise, it creates a file

  ![cp example](https://github.com/H0JunP/reppopotamus/assets/134226638/48bfe81c-0973-4d57-9f0c-75004401c920)
  ```sh
  $ cp (original file/directory) (destination file/directory)
  $ cp -i (original file/directory) (destination file/directory)
  $ cp -r (original file/directory) (destination file/directory)
  ```
---  
### **mv**

  Move files and directories or rename them

  #### Options
  - **-i** : if the file with same name exists, the user is prompted before it is overwritten
  
  ![IMG_1894315A30A8-1](https://github.com/H0JunP/reppopotamus/assets/134226638/dd97fe50-7bd0-4e58-a32f-32821ae233e2)
  ```sh
  $ mv (original file/directory) (destination file/directory)
  $ mv -i (original file/directory) (destination file/directory)
  $ mv (original file/directory) (original file/directory) (destination directory)
  ```
---
### **rm**

  Delete files and directories
  
  ```diff
    - WARNING: THESE OPERATIONS DELETE FILES AND DIRECTORIES AND IT'S IRREVERSIBLE!
    - MAKE SURE TO MAKE BACKUP BEFORE USING THESE COMMANDS AND USE IT AT YOUR OWN RISK!
  ```

  #### Options
  - **-i** : user is prompted before each file is deleted
  - **-r** : deletes all of its contents within

  ![IMG_DA06D295EC92-1](https://github.com/H0JunP/reppopotamus/assets/134226638/09b7168c-4222-4138-95ee-89d8b8865e60)
  ```sh
  $ rm (files or directories)
  $ rm -i (files or directories)
  $ rm -r (directories)
  ```
---
### **mkdir**

  Makes a new directory

  ![IMG_28C148E9ACF7-1](https://github.com/H0JunP/reppopotamus/assets/134226638/e3f3ffd2-55e0-4ce2-bdd2-33512513c0a6)

  ```sh
  $ mkdir (directory name)
  ```
---
## Help Commands
### **help**
  ![IMG_64DE9EAEA0EE-1](https://github.com/H0JunP/reppopotamus/assets/134226638/9a46d8ca-6a61-4ba1-8001-f14d719e4851)
  
  ```sh
  $ help (command name)
  ```
---
### **man**
  ![IMG_9A9C65CA29D8-1](https://github.com/H0JunP/reppopotamus/assets/134226638/b85df4a8-45c6-4071-ac6a-e0071c07666a)

  ```sh
  $ man (command name)
  ```
---
## Exiting Terminal
### **exit**
  ```sh
  $ exit
  ```
