# Bandit Level 0 

### Goal
The goal is to log into the game using SSH and find the password for the next level.

### Solution
1. **Connect to the server:**
   ```bash
   ssh -p 2220 bandit0@bandit.labs.overthewire.org

2. **Password: bandit0**

3.Finding the next password:
After logging in, list the files and read the readme file

```ls```  
```cat``` readme  

Password for Level 1  
ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If  

### Screenshots
![Step 1 - Login](./Image/bandit0_ssh.png)
![Step 2 - Password](./Image/bandit0_pass.png)
