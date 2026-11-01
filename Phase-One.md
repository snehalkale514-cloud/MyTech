\# PHASE ONE – GIT AND GITHUB PRACTICAL



\## Aim

To create a Git repository, upload a Python program to GitHub, create a new branch, add another Python program, and demonstrate the difference between branches.



\---



\## REQUIREMENTS

1\. Computer or laptop

2\. Git installed

3\. GitHub account

4\. Python installed

5\. Internet connection



\---



\# PART 1: CREATE A GITHUB REPOSITORY



\### Step 1: Open GitHub

1\. Open https://github.com

2\. Login to your GitHub account.

3\. Click the \*\*+\*\* icon.

4\. Select \*\*New repository\*\*.

5\. Enter repository name: `MyTech`

6\. Select \*\*Public\*\*.

7\. Click \*\*Create repository\*\*.



Keep the repository page open.



\---



\# PART 2: OPEN GIT BASH



\### Step 2: Create a folder



Open Git Bash and type:



```bash

mkdir MyTech

cd MyTech

```



\### Step 3: Configure Git



```bash

git config --global user.name "Snehal"

git config --global user.email "snehalkale514@gmail.com"

```



\### Step 4: Initialize Git



```bash

git init

```



This command creates a Git repository in the folder.



\---



\# PART 3: CREATE THE FIRST PYTHON PROGRAM



\### Step 5: Create a Python file



```bash

notepad program1.py

```



Paste this code into Notepad:



```python

n = int(input("Enter a number: "))



for i in range(1, 11):

&#x20;   print(n, "x", i, "=", n\*i)

```



Save the file and close Notepad.



\### Step 6: Run the program



```bash

python program1.py

```



Example output:



```text

Enter a number: 5

5 x 1 = 5

5 x 2 = 10

5 x 3 = 15

5 x 4 = 20

5 x 5 = 25

5 x 6 = 30

5 x 7 = 35

5 x 8 = 40

5 x 9 = 45

5 x 10 = 50

```



\### Step 7: Add and commit the file



```bash

git add program1.py

git commit -m "Add multiplication table program"

```



\### Step 8: Connect GitHub repository



```bash

git branch -M main

git remote add origin https://github.com/snehalkale514-cloud/MyTech.git

```



\### Step 9: Push the code to GitHub



```bash

git push -u origin main

```



Now open GitHub and refresh the repository. You should see `program1.py`.



\---



\# PART 4: CREATE A NEW BRANCH



\### Step 10: Create a branch



```bash

git checkout -b GIT-EXAM

```



This creates a new branch named GIT-EXAM and switches to it.



\### Step 11: Create the second Python program



```bash

notepad program2.py

```



Paste this code:



```python

a = int(input("Enter first number: "))

b = int(input("Enter second number: "))



if a > b:

&#x20;   print("First number is greater")

elif b > a:

&#x20;   print("Second number is greater")

else:

&#x20;   print("Both numbers are equal")

```



Save and close Notepad.



\### Step 12: Run the second program



```bash

python program2.py

```



Example output:



```text

Enter first number: 10

Enter second number: 5

First number is greater

```



\### Step 13: Add and commit the second program



```bash

git add program2.py

git commit -m "Add greatest of two numbers program"

```



\### Step 14: Push the new branch to GitHub



```bash

git push -u origin GIT-EXAM

```



Now the GIT-EXAM branch is also uploaded to GitHub.



\---



\# PART 5: DEMONSTRATE THE DIFFERENCE BETWEEN BRANCHES



\### Step 15: Switch to main branch



```bash

git checkout main

ls

```



Output:



```text

program1.py

```



\### Step 16: Switch to GIT-EXAM branch



```bash

git checkout GIT-EXAM

ls

```



Output:



```text

program1.py

program2.py

```



\### Result



\- Main branch contains `program1.py`.

\- GIT-EXAM branch contains `program1.py` and `program2.py`.



This demonstrates that different branches can contain different versions of a project.



\---



\# IMPORTANT GIT COMMANDS



| Command | Use |

|---|---|

| `git init` | Creates a Git repository |

| `git status` | Shows file status |

| `git add .` | Adds all changed files |

| `git add filename` | Adds a particular file |

| `git commit -m "message"` | Saves changes |

| `git push` | Uploads changes to GitHub |

| `git pull` | Downloads latest changes |

| `git branch` | Shows branches |

| `git checkout main` | Switches to main branch |

| `git checkout -b branchname` | Creates and switches to a new branch |

| `git remote -v` | Shows remote repository URL |

| `ls` | Shows files in the folder |



\---



\# VIVA QUESTIONS AND ANSWERS



\### Q1. What is Git?

Git is a tool used to track changes in files.



\### Q2. What is GitHub?

GitHub is an online platform used to store and share code.



\### Q3. What is a repository?

A repository is a place where project files and their history are stored.



\### Q4. What is Git Bash?

Git Bash is a command-line application used to run Git commands.



\### Q5. What is `git init`?

It creates a new Git repository.



\### Q6. What is `git add`?

It adds files for the next commit.



\### Q7. What is `git commit`?

It saves changes in the Git repository.



\### Q8. What is `git push`?

It uploads local commits to GitHub.



\### Q9. What is `git pull`?

It downloads the latest changes from GitHub.



\### Q10. What is a branch?

A branch is a separate version of a project.



\### Q11. What is the main branch?

It is the main branch of a repository.



\### Q12. Why do we create branches?

To work on different versions or features without directly changing the main branch.



\### Q13. What is `git checkout`?

It is used to switch between branches.



\### Q14. What is `git status`?

It shows the current status of files.



\### Q15. What is `git clone`?

It downloads an existing GitHub repository to our computer.



\### Q16. What is `git remote`?

It connects a local repository to a remote repository.



\### Q17. What is the difference between Git and GitHub?

Git is a version-control tool, while GitHub is an online platform for hosting Git repositories.



\### Q18. What is the use of `git branch`?

It displays the available branches.



\### Q19. What is the use of `git merge`?

It combines changes from one branch into another.



\### Q20. What is the difference between `git add` and `git commit`?

`git add` selects files, while `git commit` saves the selected changes.



\---



\# FINAL RESULT



Successfully created a Git repository, uploaded a Python multiplication-table program to GitHub, created a new branch named GIT-EXAM, added a program to find the greatest of two numbers, and demonstrated the difference between the main and GIT-EXAM branches.

