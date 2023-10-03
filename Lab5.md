# Lecture Note on Shell Commands - Part 2
## I/O Redirection
### **>**
  Redirects the output of shell command and saves it into the text file
  #### **cat**
  Shows the content of text file
  
  <img width="1012" alt="스크린샷 2023-10-03 오후 2 11 30" src="https://github.com/H0JunP/reppopotamus/assets/134226638/58348872-efd7-45c6-97a6-313dba662a72">

  ```sh
  $ [command you want to type in] > [text file you want to save output to]
  ```
---
### **>>**
  Appends the output of shell command into the existing file
  
  *If file doesn't exist, it creates new text file and saves it into that text file*

  <img width="991" alt="스크린샷 2023-10-03 오후 2 17 16" src="https://github.com/H0JunP/reppopotamus/assets/134226638/7e65bb2e-0c1e-4f4b-8288-d6510bec6d2c">

  ```sh
  $ [command you want to type in] >> [text file you want to save/append output to]
  ```
---
### **<**
  redirect input of shell command from text file

  *You can use **<**, **>** and **>>** into one command at the same time*

  <img width="991" alt="스크린샷 2023-10-03 오후 2 20 16" src="https://github.com/H0JunP/reppopotamus/assets/134226638/c70d1ab8-e6e8-41c8-85c1-a4c7a789cd18">

  ```sh
  $ [command you want to type in] < [text file you want to import input from]
  ```
---
### **|**
  pipelines the output of previous comamnd into the input of next command

  ```sh
  $ [command 1]|[command 2]|[command 3]|......
  ```
---
### **\\**
  Ignores the input of enter in shell commands in order to write long commands into multiple lines
  
  <img width="1041" alt="스크린샷 2023-10-03 오후 2 28 40" src="https://github.com/H0JunP/reppopotamus/assets/134226638/805c77e8-c15c-4469-af2b-bdbd016cd822">

  #### Without Using **\**
  ```sh
  $ python3 --version
  ```

  #### Using **\**
  ```sh
  $ python3 \
  > --version
  ```
---
## Permissions
Because Linux is a multi-user system, files and directories have a permission assigned differently to owner/group/others
<img width="710" alt="스크린샷 2023-10-03 오후 2 56 30" src="https://github.com/H0JunP/reppopotamus/assets/134226638/2921a9a3-1462-4330-b6da-e49cab3306a2">

### **ls -l**
  Checking the permission of file/directory
  
  <img width="710" alt="스크린샷 2023-10-03 오후 3 00 12" src="https://github.com/H0JunP/reppopotamus/assets/134226638/6bee2bfc-fc24-4126-857a-f044270cd099">

  ```sh
  $ ls -l [File or Directory]
  ```
---
### **chmod**
  Changes permission of file/directory
  #### Permission Setting
  <img width="378" alt="스크린샷 2023-10-03 오후 3 05 18" src="https://github.com/H0JunP/reppopotamus/assets/134226638/31bbeda2-313a-4556-89d4-4abf8e55e4c3"><img width="1047" alt="스크린샷 2023-10-03 오후 3 05 40" src="https://github.com/H0JunP/reppopotamus/assets/134226638/c2a1c15e-fcc0-4411-8726-ecbcf82b6be9">

<img width="518" alt="스크린샷 2023-10-03 오후 3 07 49" src="https://github.com/H0JunP/reppopotamus/assets/134226638/6d96bde3-02ff-489d-8e1e-a450b532b4c2">

  ```sh
  $ chmod [Permission Setting] [File/Directory location]
  ```
---
### **sudo**
  Executes command with superuser previllages

  
  *Type **exit** in shell command to exit out of superuser prompt*
  ```sh
  $ sudo [command you want to execute]
  ```
---
## Text Editors
There's a lot of kinds of text editors you can choose in Linux, each of them has different characteristics.
<img width="1219" alt="스크린샷 2023-10-03 오후 3 52 26" src="https://github.com/H0JunP/reppopotamus/assets/134226638/bc1d3e65-4cf3-4f38-8f54-1f3334bbab95">

### Saving Shell Commands into the Text File
  You can save commands into the text file and execute them in command prompt
  *The text file needs to be saved as **.sh** file*

  <img width="377" alt="스크린샷 2023-10-03 오후 3 56 56" src="https://github.com/H0JunP/reppopotamus/assets/134226638/9c1bdfac-2fee-40ef-9e19-4c7ba8528046">
  <img width="847" alt="스크린샷 2023-10-03 오후 3 57 19" src="https://github.com/H0JunP/reppopotamus/assets/134226638/2e4d3ee0-d3fa-424c-827b-ed6808260322">
  <img width="847" alt="스크린샷 2023-10-03 오후 3 57 38" src="https://github.com/H0JunP/reppopotamus/assets/134226638/90a5c3ff-845a-42de-b1ef-03b75df9139e">

  #### Creating shell command text file
  ```sh
  $ nano [name of text file].sh
  ```

  #### Executing shell command from text file
  ```sh
  $ sh [name of text file].sh
  ```
---
## Checking Command History
### **history**
  You can either see the command history directly from command prompt, or you can save it into the text file using **>** or **>>**
  
  <img width="449" alt="스크린샷 2023-10-03 오후 4 02 31" src="https://github.com/H0JunP/reppopotamus/assets/134226638/44c34f2d-b7dc-4968-9d84-62eaac1f9282">

  #### Viewing history directly from command prompt
  ```sh
  $ history
  ```
  #### Saving history into the text file
  ```sh
  $ history > [text file you want to save the history into]
  ```
