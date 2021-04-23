# Task2 Task  assignment.
1) ### Analyze the structure of the /etc/passwd and /etc/group file, what fields are present in it, what users exist on the system? Specify several pseudo-users, how to define them?
    * In passwd file there are such fields: </br>
      username : password(x indicates incrypted password) : user id(UID) : group id(GID) : user info : home directory : commandshell </br>
    * In group file there are such fields: </br>
      group name : password : GID : users </br>
    * there are a lot of users: </br>
      ![image](https://user-images.githubusercontent.com/80945113/115575641-6e72a500-a2cb-11eb-81b5-0ccf459a8920.png)
    * pseudo users are ones whos home directory is not located at /home
2) ### What are the uid ranges? What is UID? How to define it?
    UID ranges from 0 to 99 statically allocated by the system and cannot be created by applications
    UID ranges from 100 to 499 should be reserved for dynamic allocation by system administrators and post install sctipt
3) ### What is GID? How to define it?
   GID is group identifier (0-100 range is reserved for system use). To define it read /etc/group file.
4) ### How to determine belonging of user to the specific group? 
   command: group "username" </br>
   ![image](https://user-images.githubusercontent.com/80945113/115910826-fc8a8f00-a475-11eb-8040-66b1badda40e.png)
5) ### What are the commands for adding a user to the system? What are the basic parameters required to create a user?
   useradd [options] username
   after creation of user, add user's password: </br>
   ![image](https://user-images.githubusercontent.com/80945113/115912403-f39abd00-a477-11eb-9400-a6932d7fb154.png) </br>
   Some basic parameters:
      * -d "path" specify home directory (/home by default)
      * -u "UID" (-g "GID") specify UID or GID for new user
      * -G "group1, group2, ..." specify groups for new user 
      * -M to create user without home directory

6) ### How do I change the name (account name) of an existing user?
   usermod -l new-name old-name
7) ### What is skell_dir? What is its structure?
   /etc/skel is used to initiate home directory when a user is first created </br>
   ![image](https://user-images.githubusercontent.com/80945113/115913779-b59e9880-a479-11eb-90ab-1b9cfb9ae8d3.png)
8) ### How to remove a user from the system (including his mailbox)?
   userdel -r username (-r to delete with mail)
9) ### What commands and keys should be used to lock and unlock a user account?
   * to lock a user: usermod -L username
   * to unlock a user: usermod -U username
10) ### How to remove a user's password and provide him with a password-free login for subsequent password change?
   to make password for user expired: passwd --expire username
   to verify expiration: chage -l username
11) ### Display the extended format of information about the directory, tell about the information columns displayed on the terminal.
   to get extend info about directory I call ls command with such parameters combined:
   * -a - show hidden files
   * -h - show size of files in readable format
   * -i -show inode number </br>
   ![image](https://user-images.githubusercontent.com/80945113/115925122-5183d080-a489-11eb-902f-44091ca6dcac.png)
12) ### What access rights exist and for whom (i. e., describe the main roles)? Briefly describe the acronym for access rights.
   access is discribe by 3 letters(rwx). r - read, w - write, x - execute. Each file has certain access mode for user(file owner), </br>
   group and other(everyone else who has access to a file)
13) ### What is the sequence of defining the relationship between the file and the user?
   to get relationship between file and user call "ls -l filenane". It shows user and group who own a file.
14) ### What commands are used to change the owner of a file (directory), as well as the mode of access to the file? Give examples, demonstrate on the terminal.
   "chown username:group file". To change permission for directoy use -R key: "chown -R username:group directory"
15) ### What is an example of octal representation of access rights? Describe the umask command.
   octal form of permission is decimal representation of binary number, which describes rwx. For example: </br>
   r  w  x     octal                meaning                       </br>
   1  1  1       7       read, write and execute is available     </br>
   1  0  1       5               read and execute                 </br>
   0  1  1       3              write and execute                 </br>
16) ### Give definitions of sticky bits and mechanism of identifier substitution. Give an example of files and directories with these attributes.
   sticky bits - is a permission bit that is set on a file or a directory that lets only the owner of the file/directory or the root user to delete or rename the file. <.br>
   to add sticky bit: "chmod +t directory/" </br>
   in this example I create directory, set 777 permission, add sticky bit: </br>
   ![image](https://user-images.githubusercontent.com/80945113/115929171-fdc8b580-a48f-11eb-91ae-b0eb80e9b9d8.png)
