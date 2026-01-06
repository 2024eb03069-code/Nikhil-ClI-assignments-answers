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
 I used the **pwd** command to display the current working directory. To view all files and folders present in that directory with detailed information such as permissions, ownership, and file size, I executed the **ls -l** command.

Command: pwd and ls -l
<img width="1122" height="716" alt="Screenshot (626)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/2.png" />

3. Environment Confirmation File:
 To create the file and insert the required text, I used the echo command along with output redirection (>). This method creates the file automatically if it does not already exist and writes the given text into it.
To verify the content, I used the **cat** command to display the file contents.

Command: **echo "Linux user environment verified" > user_info.txt**
<img width="1088" height="686" alt="Screenshot (629)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/4(i).png" /> 

4. File Integrity Check:
 To determine the total number of characters in the file, I used the **wc -m** command. The output confirmed that the file contains 32 characters.

Command: **wc -m user_info.txt**

<img width="1065" height="677" alt="Screenshot (640)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/4(ii).png" />

5. Learning the Tools:
 I accessed the manual page of the mkdir command using **man mkdir**. Since the Coursera lab environment did not display the manual page correctly, I ran the command on my Kali Linux system.

A particularly useful option is -p, which automatically creates parent directories if they do not exist. Using this option, I created both the parent and child directories in a single command and verified their creation using **ls and cd**.

Command: **man mkdir & mkdir -p /home/coder/parent/child**
<img width="1083" height="675" alt="Screenshot (630)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/5.png" />

6. Home Directory Inspection:
 The home directory is represented by the **~** (tilde) symbol.
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
 To display the Linux kernel version currently running on the system, I used the uname -r command.

Command: **uname -r**
<img width="1051" height="667" alt="Screenshot (636)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/8.png" />

9. Network Connectivity Test:
 To verify network connectivity, I used the ping command.
This command sends ICMP echo request packets to the destination host and waits for replies.

Command: **ping www.google.com**

<img width="1051" height="685" alt="Screenshot (637)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/9.png" />

10. System Health Awareness:
 I used the **uptime** command to display system health information.

Uptime duration: Time since the last system boot

Number of users: Currently logged-in users
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%201/10.png" />

<h2>Question 2</h2>
You are working as a junior system administrator responsible for organizing project-related files in your home directory.
Your supervisor wants you to demonstrate your understanding of Linux file and directory management commands.
1. Project Workspace Setup: 
```bash
mkdir documents
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%202/1.png" />

### Task 2: File Creation
```bash
cd documents && touch plan.txt
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%202/2.png" />

### Task 3: Content Addition
```bash
echo "Your project notes here" > plan.txt
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%202/3.png" />

### Task 4: File Metadata Verification
```bash
ls -l plan.txt
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%202/4.png" />

**Explanation:** Displays long format listing showing permissions, owner, size, and timestamp.

### Task 5: File Duplication
```bash
cp plan.txt plan_copy.txt
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%202/5.png" />

### Task 6: Directory Renaming
```bash
cd ..
mv documents project_documents
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%202/6.png" />
### Task 7: Archival Structure
```bash
mkdir project_documents/archive
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%202/7.png" />

### Task 8: File Organization
```bash
mv project_documents/plan_copy.txt project_documents/archive/
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%202/8.png" />

### Task 9: Recursive Listing
```bash
ls -R project_documents
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%202/9.png" />
**Explanation:** Displays directory tree showing all subdirectories and files recursively.

### Task 10: Path Verification
```bash
readlink -f project_documents/archive/plan_copy.txt
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%202/10.png" />
**Explanation:** Shows the full absolute path of the file, resolving any symbolic links.

---

## QUESTION 3: Links & Disk Usage (10 Tasks - 5 Points)

Navigate to Question_3 folder and execute:

### Task 1: File Creation
```bash
echo "Sample data content" > sample_data.txt
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%203/1.png" />


### Task 2: Hard Link Creation
```bash
ln sample_data.txt sample_hard.txt
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%203/2.png" />

### Task 3: Symbolic Link Creation
```bash
ln -s sample_data.txt sample_soft.txt
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%203/3.png" />

### Task 4: Inode Verification
```bash
ls -i sample_data.txt sample_hard.txt sample_soft.txt
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%203/4.png" />
**Explanation:** Shows inode numbers - hard link shares same inode, symbolic link has different inode.

### Task 5: Inode Analysis
**Explanation:** The hard link (sample_hard.txt) and original file (sample_data.txt) share the same inode number because they point to the same data block. The symbolic link has a different inode as it's a separate file containing just the path reference.
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%203/5.png" />

### Task 6: File Metadata Inspection
```bash
stat sample_data.txt
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%203/6.png" />
**Explanation:** Displays detailed file information including inode, permissions, size, access/modify times, and more.

### Task 7: Disk Usage Check
```bash
du -h ~
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%203/7.png" />
**Explanation:** Shows disk usage summary of home directory in human-readable format (KB, MB, GB).

### Task 8: File Size Overview
```bash
ls -lh ~
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%203/8.png" />
**Explanation:** Lists home directory files with sizes in human-readable format.

### Task 9: Link Deletion Test
```bash
rm sample_soft.txt
ls sample_data.txt
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%203/9.png" />
**Explanation:** Removing symbolic link doesn't affect the original file. Removing hard link decrements link count but preserves data if other links exist.

### Task 10: Disk Utility Demonstration
```bash
du -sh ~/*
df -h
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%203/10.png" />
**Explanation:** Shows disk usage summary for each item in home directory and filesystem disk space utilization in human format.

---

## QUESTION 4: System Monitoring (10 Tasks - 5 Points)

Navigate to Question_4 folder and execute:

### Task 1: System Uptime Verification
```bash
uptime
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%204/1.png" />

### Task 2: User Process Listing
```bash
ps aux --user=$USER
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%204/2.png" />
**Explanation:** Lists all processes running under current user account with detailed information.

### Task 3: CPU Usage Analysis
```bash
ps aux --user=$USER --sort=-%cpu | head -5
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%204/3.png" />
**Explanation:** Shows top 5 processes consuming most CPU resources, sorted by %CPU usage.

### Task 4: Background Process Execution
```bash
sleep 300 &
jobs
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%204/4.png" />
**Explanation:** Starts background process (300 second sleep) and lists active background jobs.

### Task 5: Process Priority Management
```bash
renice +5 -p <PID>
ps -p <PID> -o pid,ni,cmd
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%204/5.png" />

**Explanation:** Changes process priority (nice value) and displays the modified process with new priority level.

### Task 6: Memory Usage Monitoring
```bash
free -h
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%204/6.png" />
**Explanation:** Displays memory usage statistics in human-readable format showing total, used, free, and cache memory.

### Task 7: Disk Space Inspection
```bash
df -h /home
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%204/7.png" />
**Explanation:** Shows disk space usage for /home filesystem including total, used, available space, and usage percentage.

### Task 8: Shell Identification
```bash
echo $SHELL
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%204/8.png" />
**Explanation:** Displays the current user's login shell (usually /bin/bash or /bin/zsh on macOS).

### Task 9: Output Redirection
```bash
uname -a > system_report.txt
cat system_report.txt
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%204/9.png" />
**Explanation:** Redirects system information output to file, then displays file contents to verify redirection worked.

### Task 10: Disk Usage Visualization
```bash
du -sh ~/* | sort -hr
```
<img width="1058" height="667" alt="Screenshot (638)" src="https://github.com/2024eb03069-code/Nikhil-ClI-assignments-answers/blob/main/images/Qno%204/10.png" />
**Explanation:** Shows disk usage for each directory in home, sorted by size in descending order.

---



