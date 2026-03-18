# Bandit Level 7 → Level 8

### Goal
The password for the next level is stored in the file `data.txt` next to the word `millionth`.

### Solution
The file `data.txt` is very large. Instead of reading it manually, we use the `grep` command to search for the specific keyword.

1. **Verify the file and its size:**
```bash
ls
wc data.txt
```
2.Search for the password:
```bash
grep "millionth" data.txt

# OR using a pipe

cat data.txt | grep millionth
```
Password for Level 8  
dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

### Screenshot
![Level 1 Password Solution](./Image/bandit7_pass.png)
