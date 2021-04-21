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
    --help </br>
    ![image](https://user-images.githubusercontent.com/80945113/115553601-43ca2180-a2b6-11eb-95ca-319738ff2bf6.png) </br>
    man </br>
    ![image](https://user-images.githubusercontent.com/80945113/115553965-a9b6a900-a2b6-11eb-89c4-5378ab9bc3b8.png) </br>
    info </br>
    ![image](https://user-images.githubusercontent.com/80945113/115554156-d8cd1a80-a2b6-11eb-9259-e7e507ea47a4.png)
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
1) ✓ Examine the tree command. Master the technique of applying a template, for example, display all files that contain a character c, or files that contain a specific sequence of characters. List subdirectories of the root directory up to and including the second nesting level.</br>
    ![image](https://user-images.githubusercontent.com/80945113/115087111-4293a000-9f16-11eb-8f91-519735e917f2.png)

2) ✓ What command can be used to determine the type of file (for example, text or binary)? Give an example.
    ![image](https://user-images.githubusercontent.com/80945113/115087874-bc785900-9f17-11eb-88d4-872c97a80ad5.png)

3) ✓ Master the skills of navigating the file system using relative and absolute paths. How can you go back to your home directory from anywhere in the filesystem?</br>
    using relative path: </br>
    ![image](https://user-images.githubusercontent.com/80945113/115088060-0feaa700-9f18-11eb-94dc-fc41bfa16a2c.png)</br>
    using absolute path: </br>
    ![image](https://user-images.githubusercontent.com/80945113/115088115-2abd1b80-9f18-11eb-9742-4ba4f669754d.png)

4) ✓ Become familiar with the various options for the ls command. Give examples of listing directories using different keys. Explain the information displayed on the terminal using the -l and -a switches.
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
    
5) ✓ Perform the following sequence of operations: 
    -  create a subdirectory in the home directory;
    -  in this subdirectory create a file containing information about directories located in the root directory (using I/O redirection operations);
    -  view the created file; </br>
       ![image](https://user-images.githubusercontent.com/80945113/115455193-4d0dac80-a22a-11eb-9a43-623b5b32f5c5.png)
    -  copy the created file to your home directory using relative and absolute addressing </br>
       ![image](https://user-images.githubusercontent.com/80945113/115455432-a1189100-a22a-11eb-9fec-87381cfb45d1.png)
    -  delete the previously created subdirectory with the file requesting removal;
    -  delete the file copied to the home directory. </br>
       ![image](https://user-images.githubusercontent.com/80945113/115455702-f48adf00-a22a-11eb-9d51-46f15784eea8.png)

6) ✓ Perform the following sequence of operations:
    -  create a subdirectory test in the home directory;
    -  copy the .bash_history file to this directory while changing its name to labwork2;
    -  create a hard and soft link to the labwork2file in the test subdirectory; </br>
       ![image](https://user-images.githubusercontent.com/80945113/115457078-a37bea80-a22c-11eb-82b1-8eca3843284e.png)
    -  how to define soft and hard link, what do these concepts;
       hard link copies file by value (creates mirror copy). Copied file has same inode number and permission</br>
       soft link copies file by reference. Copied file has different inode number and permission</br>
       ![image](https://user-images.githubusercontent.com/80945113/115457453-3e74c480-a22d-11eb-9578-0636b1745d34.png)
    -  change the data by opening a symbolic link. What changes will happen and why 
       let's change file through soft link</br>
       ![image](https://user-images.githubusercontent.com/80945113/115457755-93183f80-a22d-11eb-9b25-de9ece8e6a17.png)
       Changes were aplied for origin file (lab2work)
    -  rename the hard link file to hard_lnk_labwork2;
    -  rename the soft link file to symb_lnk_labwork2 file; 
    -  then delete the labwork2. What changes have occurred and why? </br>
       ![image](https://user-images.githubusercontent.com/80945113/115458386-526cf600-a22e-11eb-937d-3bd17c2615eb.png)
       Now I try to use hard link file (everything ok): </br>
       ![image](https://user-images.githubusercontent.com/80945113/115458475-6dd80100-a22e-11eb-8925-1519a64d357c.png)
       But can't open symbolic link: </br>
       ![image](https://user-images.githubusercontent.com/80945113/115459068-46cdff00-a22f-11eb-8521-dd226172cc88.png)
       symbolic links is (unexpectedly) link to original file. If you delete original file link points nowhere. Hardlink is just mirror copy
7) ✓ Using the locate utility, find all files that contain the squid and traceroute sequence.
8) ✓ Determine which partitions are mounted in the system, as well as the types of these partitions.
   using lsblk command we can watch all blocks mounted into system, including disk partitions </br>
   ![image](https://user-images.githubusercontent.com/80945113/115459698-058a1f00-a230-11eb-999b-913154c8d49e.png)
9) ✓ Count the number of lines containing a given sequence of characters in a given file.
   as example let's count frequency of using different commands</br> 
   ![image](https://user-images.githubusercontent.com/80945113/115462023-ce693d00-a232-11eb-98bc-493c7ed5482e.png)

10) ✓ Using the find command, find all files in the /etc directory containing the host character sequence. </br>
   ![image](https://user-images.githubusercontent.com/80945113/115460575-171ff680-a231-11eb-82c7-de14f7f1c07d.png)
12) ✓ List all objects in /etc that contain the ss character sequence. How can I duplicate a similar command using a bunch of grep? 
   use [grep ss *] command, result: </br>
   ![image](https://user-images.githubusercontent.com/80945113/115463384-6b78a580-a234-11eb-8fcc-26b40e14d932.png)
13) ✓ Organize a screen-by-screen print of the contents of the /etc directory. Hint: You must use stream redirection operations.
14) ✓ What are the types of devices and how to determine the type of device? Give examples.
    types of devices:
      - character based (data stream is transfered and handled) 1 character(byte) at a time
      - block type(hard drives for example) transfer data in blocks
      - pipes
      - sockets
      We can determine device's type by letter(b-block / c-character) or by it's major number(8 - block, 4 - chracter) </br>
      ![image](https://user-images.githubusercontent.com/80945113/115551429-bb4a8180-a2b3-11eb-8770-a91727e99417.png)
15) ✓ List the first 5 directory files that were recently accessed in the /etc directory
     ls -1t | head -5 </br>
     ![image](https://user-images.githubusercontent.com/80945113/115553202-cef6e780-a2b5-11eb-89d4-83a48115a326.png) </br>
16) ✓ How to determine the type of file in the system, what types of files are there?
   ![image](https://user-images.githubusercontent.com/80945113/115551821-4297f500-a2b4-11eb-93fc-08164a340fad.png)
