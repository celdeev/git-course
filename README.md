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




