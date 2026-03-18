# Bandit Level 6 → Level 7

### Goal
The password for the next level is stored somewhere on the server and has all of the following properties:
- Owned by user `bandit7`
- Owned by group `bandit6`
- 33 bytes in size

### Solution
To find a file with these specific properties across the entire system, we use the `find` command starting from the root directory `/`.

1. **Find the file using multiple criteria:**
```bash
find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
```

2>/dev/null is used to hide "Permission denied" errors for directories we don't have access to.  

The search identifies the file at: /var/lib/dpkg/info/bandit7.password.  

2.Read the password:
```bash
cat /var/lib/dpkg/info/bandit7.password
```
Password for Level 7  
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

### Screenshot
![Level 1 Password Solution](./Image/bandit6_pass.png)
