# Task 5.1 report

## Task1.Part1
1) ✓ Log in to the system as root. </br>
   ![image](https://user-images.githubusercontent.com/80945113/115000468-75ed1500-9eab-11eb-8390-1c38d5afe0ca.png)
2) ✓ Use the passwd command to change the password. Examine the basic parameters of the command. What system file does it change *?</br>
   ![image](https://user-images.githubusercontent.com/80945113/115001248-2b1fcd00-9eac-11eb-8b95-3c9434fe2435.png)</br>
   file /etc/shadow stores info about paswwords</br>
   ![image](https://user-images.githubusercontent.com/80945113/115002175-1bed4f00-9ead-11eb-800c-484e15f29225.png)
3) ✓ Determine the users registered in the system, as well as what commands they execute. What additional information can be gleaned from the command execution?</br>
   let's open (/etc/passwd) using vim: </br>
   ![image](https://user-images.githubusercontent.com/80945113/115005602-b4d19980-9eb0-11eb-98d3-07c8c23d1e1b.png) </br>
   .bash_history file contains all commands executed by partcular user. By entering "Vim /home/<user_name>/.bash_history" we can see: </br>
   ![image](https://user-images.githubusercontent.com/80945113/115006524-a637b200-9eb1-11eb-9e58-d5ed64418c31.png)
4) ✓ Change personal information about yourself.</br>
   ![image](https://user-images.githubusercontent.com/80945113/115007512-b8feb680-9eb2-11eb-8d17-e1205dfa0c66.png)
5) ✓ Become familiar with the Linux help system and the man and info commands. Get help on the previously discussed commands, define and describe any two keys for these commands. Give examples.</br>
6) ✓ Explore the more and less commands using the help system. View the contents of files .bash* using commands.</br>
   ![image](https://user-images.githubusercontent.com/80945113/115009599-1eec3d80-9eb5-11eb-8998-e428c5ef6d83.png)</br>
    less command does almost same things, but is faster because it does not load the entire file at once and allows navigation though file using page up/down keys.
    Also you can search word in file as in example: </br>
    ![image](https://user-images.githubusercontent.com/80945113/115010463-206a3580-9eb6-11eb-90e2-40bf0e39fd67.png)
    ![image](https://user-images.githubusercontent.com/80945113/115010403-0fb9bf80-9eb6-11eb-8612-19f17ace48e3.png)
7) ✓ Describe in plans that you are working on laboratory work 1. Tip: You should read the documentation for the finger command.</br>
    ![image](https://user-images.githubusercontent.com/80945113/115032902-81076b80-9ed2-11eb-9208-d4156c8f6f3f.png)
9) ✓ List the contents of the home directory using the ls command, define its files and directories. Hint: Use the help system to familiarize yourself with the ls command.</br>
    on Ubuntu Server: </br>
    ![image](https://user-images.githubusercontent.com/80945113/115034614-5f0ee880-9ed4-11eb-906a-3c917eb4e48e.png) </br>
    on Ubuntu Desktop (files and directories I've created for previous labs): </br>
    ![image](https://user-images.githubusercontent.com/80945113/115035351-2cb1bb00-9ed5-11eb-848e-bf91e48e67bf.png)
## Task1.Part2
1) Examine the tree command. Master the technique of applying a template, for example, display all files that contain a character c, or files that contain a specific sequence of characters. List subdirectories of the root directory up to and including the second nesting level. 
    ![image](https://user-images.githubusercontent.com/80945113/115087111-4293a000-9f16-11eb-8f91-519735e917f2.png)

2) What command can be used to determine the type of file (for example, text or binary)? Give an example.
    ![image](https://user-images.githubusercontent.com/80945113/115087874-bc785900-9f17-11eb-88d4-872c97a80ad5.png)

3) Master the skills of navigating the file system using relative and absolute paths. How can you go back to your home directory from anywhere in the filesystem?</br>
    using relative path: </br>
    ![image](https://user-images.githubusercontent.com/80945113/115088060-0feaa700-9f18-11eb-94dc-fc41bfa16a2c.png)</br>
    using absolute path: </br>
    ![image](https://user-images.githubusercontent.com/80945113/115088115-2abd1b80-9f18-11eb-9742-4ba4f669754d.png)

4) Become familiar with the various options for the ls command. Give examples of listing directories using different keys. Explain the information displayed on the terminal using the -l and -a switches.
    List only directories:</br>
    ![image](https://user-images.githubusercontent.com/80945113/115088437-d36b7b00-9f18-11eb-977e-4f2acad2557e.png)</br>
    List directories with subdirectories: </br>
    ![image](https://user-images.githubusercontent.com/80945113/115088552-1594bc80-9f19-11eb-8956-b8a644528840.png)</br>
    List files recursively </br>
    ![image](https://user-images.githubusercontent.com/80945113/115088616-378e3f00-9f19-11eb-8fa8-fd55a185057d.png)</br>
    ls -l. Shows files as table, where column1 - permisssion status, 2 - links to file, 3 - owner of the file, 4 - group of owners, </br>
    5 - size of the content in bytes, 6 - last modify name, 7- name </br>
    ![image](https://user-images.githubusercontent.com/80945113/115088958-f3e80500-9f19-11eb-979c-7835bf10e952.png)</br>
    -a flag also shows hidden files (starting from point) </br>
    ![image](https://user-images.githubusercontent.com/80945113/115089027-20038600-9f1a-11eb-8ceb-e1b4c3aef24d.png)
    
5) Perform the following sequence of operations: -  create a subdirectory in the home directory;
    -  in this subdirectory create a file containing information about directories located in the root directory (using I/O redirection operations);
    -  view the created file;-  copy the created file to your home directory using relative and absolute addressing.
    -  delete the previously created subdirectory with the file requesting removal;
    -  delete the file copied to the home directory.

6) Perform the following sequence of operations:
    -  create a subdirectory testin the home directory;
    -  copy the .bash_historyfile to this directory while changing its name to labwork2;
    -  create a hard and soft link to the labwork2file in the test subdirectory; 
    -  how to define soft and hard link, what do theseconcepts;
    -  change the data by opening a symbolic link. What changes will happen and why 
    -  rename the hard link file to hard_lnk_labwork2;
    -  rename the soft link file to symb_lnk_labwork2 file; 
    -  then delete the labwork2. What changes have occurred and why?
7) Using the locate utility, find all files that contain the squid and traceroute sequence.
8) Determine which partitions are mounted in the system, as well as the types of these partitions.
9) Count the number of lines containing a given sequence of characters in a given file.
10) Using the findcommand, find all files in the /etc directory containing the host character sequence.
11) List all objects in /etc that contain the ss character sequence. How can I duplicate a similar command using a bunch of grep? 
12) Organize a screen-by-screen print of the contents of the /etc directory. Hint: You must use stream redirection operations.
13) What are the types of devices and how to determine the type of device? Give examples.
14) How to determine the type of file in the system, what types of files are there?
15) * List the first 5 directory files that were recently accessed in the /etcdirectory
