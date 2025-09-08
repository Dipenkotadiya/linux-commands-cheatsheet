# Solutions – File Permissions Exercises

### Exercise 1: Create a file only accessible by its owner
$ touch mysecret.txt
$ chmod 600 mysecret.txt
$ ls -l mysecret.txt
-rw------- 1 kingcobra kingcobra 0 Sep 8 19:00 mysecret.txt

Explanation:
- chmod 600 sets permissions so only the owner can read/write.

---

### Exercise 2: Allow group to edit the file, others cannot read
$ touch project.txt
$ chmod 660 project.txt
$ ls -l project.txt
-rw-rw---- 1 kingcobra kingcobra 0 Sep 8 19:05 project.txt

Explanation:
- chmod 660 allows the owner and group to read/write.
- Others have no permissions.

---

### Exercise 3: Add a user to a group and verify permissions
$ sudo useradd devuser
$ sudo groupadd devteam
$ sudo usermod -aG devteam devuser
$ groups devuser
devuser : devteam

$ touch shared.txt
$ chgrp devteam shared.txt
$ chmod 660 shared.txt
$ ls -l shared.txt
-rw-rw---- 1 kingcobra devteam 0 Sep 8 19:10 shared.txt

Explanation:
- The file shared.txt is owned by group 'devteam'.
- Users in the group can read and write the file.
- 'devuser' can now access the file after being added to 'devteam'.
