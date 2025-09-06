# Linux Navigation & File Operations — Exercises

1. Navigate to your home directory and confirm with `pwd`.
2. Create a folder called `devops-practice`.
3. Inside it, create a file named `notes.txt`.
4. Add text "My first DevOps file" using `nano` or `vim`.
5. Display content using `cat`.
6. Create a subfolder `archive` and move `notes.txt` into it.
7. Delete `notes.txt` from `archive`.

---

# Hands-on mini-exercises (try them *before* peeking solutions)

**Exercise A — Basic quick run (10–15 min)**

1. Create working folder and switch to it
2. Create two files and list them
3. Edit one file in `nano`, add 3 lines, save
4. Show the contents with `cat`
5. Delete the second file

**Commands to attempt (write them yourself first):**

- Create folder `devops-day2-practice`
- `touch` two files
- Edit with `nano`
- `cat` to view
- `rm` to delete

---

**Exercise B — Structured practice (20–30 min)**

Goal: produce a small folder with a file that contains a one-line script/log and a README for the exercise.

Tasks:

1. `mkdir day2-project && cd day2-project`
2. `mkdir logs scripts`
3. Create `scripts/hello.txt` and add a line using nano/vim
4. `cat` the file to confirm content
5. Remove the `logs` directory (if empty) or remove `scripts/hello.txt` then the dir

---

**Exercise C — Comfort with editors (30 min)**

1. Open `notes.txt` in `vim`. Add three bullet points about what you learned. Save + exit.
2. Re-open the file in `nano`, append one more line, save.
3. Show file with `cat -n` to confirm line numbers.
