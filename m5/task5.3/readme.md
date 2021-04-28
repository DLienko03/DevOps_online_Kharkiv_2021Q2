# TASK5.3 REPORT
## Part1
1. How many states could has a process in Linux?
  5 states:
  * Running/Runable(R) 
  * Sleeping: process waiting for a recource to be available (I/O operation to complete) or event to happen. The difference between process in Interruptible Sleep(S) and Ininterruptible Sleep (D)  
  * Stopped (T): provess becomes stopped when it recives SIGSTOP signal
  * Zombie (Z): 
2. Examine the pstree command. Make output (highlight) the chain (ancestors) of the current process.
  ![image](https://user-images.githubusercontent.com/80945113/116395885-5bad2280-a82d-11eb-9a30-023ff5cc9fcf.png)
3. What is a proc file system?
  It is pseudo-filesystem which provides an interface to kernel data structures. 
4. Print information about the processor (its type, supported technologies, etc.).
  ![image](https://user-images.githubusercontent.com/80945113/116396634-497fb400-a82e-11eb-91d8-ee90e83da7eb.png)
5. Use the ps command to get information about the process. The information should be as follows: the owner of the process, the arguments with which the process was launched for execution, the group owner of this process, etc. 
  ![image](https://user-images.githubusercontent.com/80945113/116399319-7a151d00-a831-11eb-8f41-1b8053f40b75.png)
6. How to define kernel processes and user processes?
  
7. Print the list of processes to the terminal. Briefly describe the statuses of the processes. What condition are they in, or can they be arriving in  
  ![image](https://user-images.githubusercontent.com/80945113/116400198-71711680-a832-11eb-8678-46f6e2bf8ee2.png)

8. Display only the processes of a specific user. 
  ![image](https://user-images.githubusercontent.com/80945113/116400807-23104780-a833-11eb-94e7-9497aac37cd9.png)

9. What utilities can be used to analyze existing running tasks (by analyzing the help for the ps command)?
  

10. What information does top command display?
  Top command displays list of processes or threds currently being managed by the Linux kernel.

11. Display the processes of the specific user using the top command.
  ![image](https://user-images.githubusercontent.com/80945113/116404045-ef372100-a836-11eb-8dbb-4626d82e00cc.png)

12. What interactive commands can be used to control the top command? Give a couple of examples.
  d - set delay between screen updates
  ![image](https://user-images.githubusercontent.com/80945113/116405598-80f35e00-a838-11eb-9043-ef081f622b02.png)
  H - threads-mode operation
13. Sort the contents of the processes window using various parameters (for example, the amount of processor time taken up, etc.)
  

14. Concept of priority, what commands are used to set priority?

15. Can I change the priority of a process using the top command? If so, how?

16. Examine the kill command. How to send with the kill commandprocess control signal? Give an example of commonly used signals.

17. Commands jobs, fg, bg, nohup. What are they for? Use the sleep, yes command to demonstrate the process control mechanism with fg, bg

## Part2
1. Check the implementability of the most frequently used OPENSSH commands in the MS Windows operating system. (Description of the expected result of the commands + screenshots: command – result should be presented)
2. Implement basic SSH settings to increase the security of the client-server connection (at least 
3. List the options for choosing keys for encryption in SSH. Implement 3 of them.
4. Implement port forwarding for the SSH client from the host machine to the guest Linux virtual machine behind NAT.
5*. Intercept (capture) traffic (tcpdump, wireshark) while authorizing the remote client on the server using ssh, telnet, rlogin. Analyze the result. 
