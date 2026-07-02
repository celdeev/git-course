install git
git --version
git config --global user.name "celestial"
git config --global user.email "kcelestial78@gmail.com"
 git config --list--------------TO check if username and password s created/check configuration

---------Create a repository-------
mkdir git-course
cd git-course
 git init
git status

----------- create a readme file----------
echo "# My First Git Project" > README.md

add the readme file------------

git add README.md

------------update readme file when changes are made--------
git commit -m "Update README"

After updating add readme file again-------
git add README.md
git log --oneline

----------make your first commit------

git commit -m "First commit"

---------git diff shows the changes you have made that are not yet staged.----------

git diff

---------flow---------
Edit file
    ↓
git add
    ↓
git commit
-----------------git workflow-----------
Edit file
    ↓
Working Directory
    ↓
git add
    ↓
Staging Area
    ↓
git commit
    ↓
Repository History
---------------suppose project contains-----------

git-practice/
│
├── README.md
├── app.py
├── .gitignore
├── debug.log
├── secret.env
└── node_modules/

-----------.gitignore file not found error solution----------
.gitignore secret.env

error: .gitignore secret.env
bash: .gitignore: command not found

solution:

Create the file:----

How to create a .gitignore file
Option 1 (Git Bash)

Create the file:

touch .gitignore

Then open it with Notepad:

notepad .gitignore

Add the following:

*.log
.env

Save and close the file.
Verify it works

Create a test log file:

echo "test" > test.log

Then run:

git status
If you want to commit the latest version of README.md and include .gitignore, run:

git add README.md
git add .gitignore

or simply:

git add .

Then check:

git status

You should see only:

Changes to be committed:
    modified: README.md
    new file: .gitignore

Finally, commit everything:

git commit -m "Update README and add .gitignore"








