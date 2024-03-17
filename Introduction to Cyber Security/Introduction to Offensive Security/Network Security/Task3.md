### Open terminal
- click open terminal
### Recon
- `nmap`: network mapper, a network scanner that help us discover running machines and any programs running on them that are visible to the outside world.

![nmap](https://github.com/MarcuXNg/Introduction_to_Cyber_Security_Writeup/assets/95072521/059b3562-feec-484e-aaa7-7409c49fa62c)

- As we can see on the screen, three services are running:
  + FTP server: stands for File Transfer Protocol, is used to transfer files between machines
  + SSH server: stands for Secure Shell, is used for secure remote login(allows you to execute commands on a remote system securely).
  + HTTP server: stands for Hypertext Transfer Protocol, is used for the web. Whenever you are browsing the web, you are using HTTP or HTTPS. HTTPS is the secure (encrypted) version of HTTP.
- Nmap reports on whether the host is up based on whether it receives any response from it. This is useful to know when no ports are open or accessible.

### Gather more information about the FTP server
1. `ftp 10.10.173.123`: connect to the target FTP server
2. log in using the login `anonymous` to see if this FTP server supports anonymous logins
3. use `ls` to get a list of the filenames along with their details
4. To download file use command `get FILENAME`. (get secret.txt).
5. to quit the FTP client: use command `bye` or `exit`

![ftp](https://github.com/MarcuXNg/Introduction_to_Cyber_Security_Writeup/assets/95072521/73e8c8bd-c6de-47ae-988f-18db195248da)

+ `txt`: text files
+ `epub`: ebooks
+ `sh`: shell script (usually contains a group of commands that needs to be performed repetitively)

6. Concatenate the downloaded file using `cat FILENAME` (cat secret.txt)
7. Login as root using the password that gather from the FTP server (the password is ABC789xyz123)

![step 6](https://github.com/MarcuXNg/Introduction_to_Cyber_Security_Writeup/assets/95072521/8943d337-3709-4c3c-8c05-8d426f3ba808)

=> have complete control over the target server, have full access to all files, including user files. 
8. Use command:
  + `pwd`: print working directory, to see where we are in the system
  + `ls`: to list file
  + `cat FILENAME`: concatenate file

![step 7](https://github.com/MarcuXNg/Introduction_to_Cyber_Security_Writeup/assets/95072521/73ed980d-58f9-46c7-be4e-631f17db3c05)

9. Use command:
  + `cd /DIRECTORY`: change directory
  + `ls`: list everything in the directory
  + `pwd`: printout working directory
  + `cat`: concatente file

[Example]: 
  1. `cd /home`
  2. `ls`
  3. `cd librarian/`
  4. `pwd` 
  5. `ls`
  6. `cat flag.txt`

![step 9](https://github.com/MarcuXNg/Introduction_to_Cyber_Security_Writeup/assets/95072521/d4822d4e-8086-429c-bc46-e7ef05795420)
