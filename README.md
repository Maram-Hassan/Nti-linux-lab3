# Nti-linux-lab3
1.	List all of the unix available shells.
![Screenshot from 2024-10-05 10-21-01](https://github.com/user-attachments/assets/d00a4c01-ac12-4300-bbdc-7ac529e96ef6)

2.	What are the differences between the unix shells?
```
Bash (Bourne Again Shell): A widely used default shell on Linux; compatible with the original Bourne shell (sh) but with many enhancements.
Zsh (Z shell): Extends bash with many more interactive features like better auto-completion, syntax highlighting, and customization options.
Ksh (Korn shell): Known for its scripting improvements over Bourne shell, with enhanced job control and arithmetic functions.
Tcsh (Tenex C shell): Similar to C shell (csh) but adds tab completion and command history.
Dash: Lightweight, POSIX-compliant, often used for scripting to ensure portability.
```
3.	List Linux commands in /usr/bin that start with letter “w”
![Screenshot from 2024-10-05 10-22-07](https://github.com/user-attachments/assets/c23318aa-fc93-4687-b1a6-4f0825750c9f)

4.	Starting from /etc, find files owned by lp user.
![Screenshot from 2024-10-05 10-23-13](https://github.com/user-attachments/assets/59f38c00-3618-4419-8e25-dcbec495a123)

5.	Find all directories in your home directory.
![Screenshot from 2024-10-05 10-24-04](https://github.com/user-attachments/assets/3e9bd331-a249-49b0-985c-bfc90a0abbb3)

6.	Write a command to search for all files on the system that, its name is “.bash_profile”.
```
find ~ -type d
```
7.	Identify the file types of the following: /etc/passwd, /dev/pts/0, /etc.
![Screenshot from 2024-10-05 10-25-17](https://github.com/user-attachments/assets/60862172-bd31-4543-b9d1-e1a1095e834a)

8.	 List the inode numbers of /, /etc, /etc/hosts, /etc/rc/, /etc/rc.d/rc.d.
![Screenshot from 2024-10-05 10-28-17](https://github.com/user-attachments/assets/f72ce625-dfdb-4c91-814e-1c816a38c5ee)

9.	 What happens if you execute: 

a.	cat filename1 | cat filename2
```
it will list the content of both files
```
b.	ls | rm
```
This will try to execute rm with no arguments, which will fail because rm needs filenames to delete.
```
c.	ls /etc/passwd | wc –l
```
This will return 1 because ls will just output /etc/passwd, and wc -l will count this as one line.
```
10.	Create a bash shell alias named ls for the “ls –l” command

11.	List the user commands and redirect the output to /tmp/commands.list
![Screenshot from 2024-10-05 10-47-13](https://github.com/user-attachments/assets/481d61fa-bd7a-49a5-a30a-63ea849a65ff)

12.	Get all the users names whose first character in their login is ‘g’.
![Screenshot from 2024-10-05 10-47-39](https://github.com/user-attachments/assets/cc96bb84-0d7a-4192-93eb-1e50ebc4a599)

13.	Write two commands: first: to search for all files on the system that named .bash_profile. Second: sorts the output of ls command on / recursively, Saving their output and error in 2 different files and sending them to the background.
```
find / -name ".bash_profile"
ls -R / > output.txt 2> error.txt &
```
14.	Display lines 7 to line 10 of /etc/passwd file

![Screenshot from 2024-10-05 10-09-33](https://github.com/user-attachments/assets/62eeac01-5016-458d-86c1-319ef5aaed6c)

15.	List the environment variables in your current shell.

![Screenshot from 2024-10-05 10-10-15](https://github.com/user-attachments/assets/da26ffa9-4cbc-4389-819d-4d59ee7230ae)

16.	What are the commands that list the values of all the variables?
![Screenshot from 2024-10-05 10-10-15](https://github.com/user-attachments/assets/da26ffa9-4cbc-4389-819d-4d59ee7230ae)

17.	What are the commands that list the value of a specific variable?

![Screenshot from 2024-10-05 10-11-33](https://github.com/user-attachments/assets/b55599e4-8423-4c14-a4ea-ecbe15ee1d89)

18.	Display your current shell.
![Screenshot from 2024-10-05 10-10-15](https://github.com/user-attachments/assets/7c5ff7da-8d58-4032-933a-0b48aae16f72)

19.	What is the difference between startup files and initialization files?
```
    Startup files are executed when a shell starts. These include /etc/profile, ~/.bash_profile, and ~/.bashrc (for bash).
    Initialization files set up the environment, paths, and other configurations for your shell.

Startup file of bash:

    /etc/profile
    ~/.bash_profile
    ~/.bash_login
    ~/.profile

Initialization file of bash:

    ~/.bashrc
```
20.	State the startup file of: bash.
```
/etc/profile
~/.bash_profile
~/.bash_login
~/.profile
```
22.	State the initialization file of:  bash.
```
~/.bashrc
```
23.	Edit in your profile to display date at login and change your prompt permanently.
![Screenshot from 2024-10-05 10-44-47](https://github.com/user-attachments/assets/bfaf186e-ad7e-4fea-96dd-8ebf5357966f)

24.	Execute the following command :

echo \   then  press enter

Notice the prompt what is that and how can you change it.
```
This creates a multi-line prompt because the backslash \ tells the shell that the command continues on the next line.
```
24.	Issue the command sleep 100.
![Screenshot from 2024-10-05 09-45-31](https://github.com/user-attachments/assets/63bc624a-8880-4366-b667-8b4627d61230)

25.	 Stop the last command.
![Screenshot from 2024-10-05 09-45-31](https://github.com/user-attachments/assets/e965deae-1649-4c24-8e93-f54a8777cce9)

26.	Resume the last command in the background
![Screenshot from 2024-10-05 09-56-17](https://github.com/user-attachments/assets/d4b45594-29c7-4a8c-87d3-cfcea5a26d12)

27.	Issue the jobs command and see its output.
![Screenshot from 2024-10-05 09-58-04](https://github.com/user-attachments/assets/8403192a-0ab7-4363-a40c-a1d190e07944)

28.	Send the sleep command to the foreground and send it again to the background.
```
fg
```
```
bg
```
29.	Kill the sleep command.
![Screenshot from 2024-10-05 09-58-30](https://github.com/user-attachments/assets/11da154e-61e2-41ed-a109-bbf626e774ac)

30.	Display your processes only
![Screenshot from 2024-10-05 09-52-16](https://github.com/user-attachments/assets/8accbb7c-bc51-40ba-9e33-488b8cb8d6ad)

31.	Display all processes except yours

32.	Use the pgrep command to list your processes only
![Screenshot from 2024-10-05 09-54-51](https://github.com/user-attachments/assets/3183a351-5b59-4c53-bb92-ac8fdf5433fb)

33.	Kill your processes only.
    ```
    pkill -u maram
```
                    	





