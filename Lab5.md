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
### **\**
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
