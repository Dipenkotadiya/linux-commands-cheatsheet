**Exercise 1**
$ pwd
/home/ubuntu


**Exercise 2**
$ mkdir devops-practice
$ ls
devops-practice


**Exercise 3**
$ cd devops-practice
$ touch notes.txt
$ ls
notes.txt


**Exercise 4**
$ nano notes.txt   # (added "My first DevOps file")
$ cat notes.txt
My first DevOps file


---

### — SOLUTIONS (run only after attempting)

**Solution A — commands**
mkdir ~/devops-day2-practice
cd ~/devops-day2-practice
touch file1.txt file2.txt
nano file1.txt   # type "This is file1" -> Ctrl+O Enter -> Ctrl+X
cat file1.txt
rm file2.txt


**Solution B — commands**
mkdir day2-project
cd day2-project
mkdir logs scripts
nano scripts/hello.txt   # write "Hello from Day 2" -> save & exit
cat scripts/hello.txt
rm -r logs


**Solution C — vim + nano**
vim notes.txt
# press i, type "- Learn pwd, ls, cd", "- Learned nano", "- Learned vim basics"
# Esc then :wq
nano notes.txt
# add "Practice done on <date>" -> Ctrl+O -> Enter -> Ctrl+X
cat -n notes.txt
