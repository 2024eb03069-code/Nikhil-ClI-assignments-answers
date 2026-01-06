# Nikhil-CLI-assignments-answers
This repository contains the completed assignment of the Command Line Interface and Scripting Graded Lab Assignment done by Fathima Sabu.

**Coursera Labs** was used to complete this assignment.

<h2>Question 1</h2>
You have just joined IxD Systems as a junior systems engineer. On your first day, the Linux administrator asks you to perform a basic environment verification on the lab machine using your own login account.

1. User Identity Verification: 
Display your currently logged-in username and all groups your user account belongs to.
Your name or login ID must appear in the output.


**Answer 1:** I used the whoami command to check the username of the currently logged-in account. To view my user ID (UID) and all the groups associated with my account, I used the id command.
Command: **whoami** and **id**
<img width="1790" height="895" alt="Screenshot (625)" src= "https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/1.png?raw=true" />
I am using the **clear** command after each question so that the commands looking clean.

2. Workspace Validation:
3. I used the **pwd** command to display the current working directory. To view all files and folders present in that directory with detailed information such as permissions, ownership, and file size, I executed the **ls -l** command.

Command: pwd and ls -l
<img width="1122" height="716" alt="Screenshot (626)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/2.png" />

3. Environment Confirmation File:
4. To create the file and insert the required text, I used the echo command along with output redirection (>). This method creates the file automatically if it does not already exist and writes the given text into it.
To verify the content, I used the **cat** command to display the file contents.

Command: **echo "Linux user environment verified" > user_info.txt**
<img width="1088" height="686" alt="Screenshot (629)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/3.png" /> 

4. File Integrity Check:
5. To determine the total number of characters in the file, I used the **wc -m** command. The output confirmed that the file contains 32 characters.

Command: **wc -m user_info.txt**
<img width="1065" height="677" alt="Screenshot (640)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/4(i).png" />
<img width="1065" height="677" alt="Screenshot (640)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/4(ii).png" />

5. Learning the Tools:
6. I accessed the manual page of the mkdir command using **man mkdir**. Since the Coursera lab environment did not display the manual page correctly, I ran the command on my Kali Linux system.

A particularly useful option is -p, which automatically creates parent directories if they do not exist. Using this option, I created both the parent and child directories in a single command and verified their creation using **ls and cd**.

Command: **man mkdir & mkdir -p /home/coder/parent/child**
<img width="1083" height="675" alt="Screenshot (630)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/5.png" />

6. Home Directory Inspection:
7. The home directory is represented by the **~** (tilde) symbol.
To list all contents of the home directory, I used the **ls ~** command.
By default, ls displays files and directories in alphabetical order.

Command: **ls ~**
<img width="1064" height="683" alt="Screenshot (642)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/6.png" />
7. Log Investigation: 
To search for the word "admin" inside the file log.txt, I used the grep command, which searches for specific patterns and displays only the matching lines.

Since the file was not already present, I created and edited it before performing the search.

Command: **grep -n "admin" log.txt**
<img width="1065" height="667" alt="Screenshot (634)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/7.png" />

8. System Information Check:
9. To display the Linux kernel version currently running on the system, I used the uname -r command.

Command: **uname -r**
<img width="1051" height="667" alt="Screenshot (636)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/8.png" />

9. Network Connectivity Test:
10. To verify network connectivity, I used the ping command.
This command sends ICMP echo request packets to the destination host and waits for replies.

Command: **ping www.google.com**

<img width="1051" height="685" alt="Screenshot (637)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/9.png" />

10. System Health Awareness:
11. I used the **uptime** command to display system health information.

Uptime duration: Time since the last system boot

Number of users: Currently logged-in users
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/10.png" />

<h2>Question 2</h2>
You are working as a junior system administrator responsible for organizing project-related files in your home directory.
Your supervisor wants you to demonstrate your understanding of Linux file and directory management commands.
1. Project Workspace Setup: 



