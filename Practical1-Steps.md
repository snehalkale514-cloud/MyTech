\# Practical 1: Git and GitHub



\## Phase 1: Create GitHub Repository

1\. Open github.com and sign in.

2\. Click +, then New repository.

3\. Enter repository name: MyTech.

4\. Select Public.

5\. Leave Add README unchecked.

6\. Click Create repository.



\## Phase 2: Configure Git in Git Bash

1\. Open Git Bash.

2\. Check Git: git --version

3\. Set name: git config --global user.name "Your Name"

4\. Set email: git config --global user.email "your-email@example.com"



\## Phase 3: Create and Connect Local Folder

1\. Create folder: mkdir MyTech

2\. Enter folder: cd MyTech

3\. Start Git: git init

4\. Connect repository: git remote add origin YOUR\_REPOSITORY\_URL



\## Phase 4: Create First Program

1\. Create program1.py in Notepad.

2\. Write a multiplication-table program.

3\. Save the file.

4\. Run: python program1.py



\## Phase 5: Commit and Upload First Program

1\. git add program1.py

2\. git commit -m "Add multiplication table program"

3\. git branch -M main

4\. git push -u origin main



\## Phase 6: Create Exam Branch

1\. git checkout -b GIT-EXAM



\## Phase 7: Create Second Program

1\. Create program2.py in Notepad.

2\. Write a program to find the greater of two numbers.

3\. Save the file.

4\. Run: python program2.py



\## Phase 8: Commit and Upload Second Program

1\. git add program2.py

2\. git commit -m "Add greatest of two numbers program"

3\. git push -u origin GIT-EXAM



\## Phase 9: Demonstrate Branch Difference

1\. git checkout main

2\. ls

3\. git checkout GIT-EXAM

4\. ls



Expected:

\- main has program1.py

\- GIT-EXAM has program1.py and program2.py

