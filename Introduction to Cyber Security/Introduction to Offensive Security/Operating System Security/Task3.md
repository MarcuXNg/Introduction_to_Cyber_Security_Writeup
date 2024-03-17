### Overall
- Tricking the target into running a malicious file or by obtaining a username and a password. 
- After discovering a username, we will try to “guess” the password; furthermore, we will try to escalate our privileges to a system administrator.
- This account is called root on Android, Apple, and Linux systems. While, on MS Windows systems, this account is called administrator. (The accounts root and administrator have complete unrestricted access to a system).

### Open terminal

![Untitled](https://github.com/MarcuXNg/Introduction_to_Cyber_Security_Writeup/assets/95072521/745fd51b-9fb5-4623-8987-17c018f175c1)

### Log in to Sammie's account
- ssh sammie@10.10.27.219
- password: dragon (cannot see the password are being typed)

![login to sammie](https://github.com/MarcuXNg/Introduction_to_Cyber_Security_Writeup/assets/95072521/03b549c0-aac1-4659-9340-c5552a28b959)

### Using whoami, ls, cat command

- whoami: who am i? (the user that login) => return sammie
- ls: list, show all the files in the current directory unless they are hidden
- cat FILENAME: concatenate, print all the cntents of the file on the screen

![Using whoami, ls, cat](https://github.com/MarcuXNg/Introduction_to_Cyber_Security_Writeup/assets/95072521/6d7aa342-a438-4695-8058-2f8474c10fe9)

### Using history command

- history: prints the commands used by the user.
![Using history](https://github.com/MarcuXNg/Introduction_to_Cyber_Security_Writeup/assets/95072521/4bf14037-c67f-4327-9607-296117a1111a)

### To login as other user if you are already login 
- su - USERNAME
- su - root: switch to root
Ex: su - johnny

### Answering question
- password login is abc123
- The root password: happyHack!NG
![Practice](https://github.com/MarcuXNg/Introduction_to_Cyber_Security_Writeup/assets/95072521/c200b6f9-b6e8-4d3e-9683-aec6d8719660)
- The content of the file: THM{YouGotRoot}
