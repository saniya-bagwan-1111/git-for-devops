# Step 1: Create a directory and navigate into it
mkdir git-for-devops

cd git-for-devops/

# Step 2: Initialize a Git repository
git init

# Step 3: Configure Git user settings
git config --global user.name "usename"

git config --global user.email "email"

# Step 4: Create a file, add it to the staging area, and commit
touch nibba.txt

git add nibba.txt'

git commit -m "Adding files"

# Step 5: Check the status, remove the file, and restore it
git status

rm nibba.txt

git restore nibba.txt

git status

# Step 6: Create a new file, add it, and commit the changes
touch nibbi.txt

git add nibbi.txt

git commit -m "Adding modified version"

# Step 7: Create and switch to a new branch
git checkout -b dev

# Step 8: Add a new file on the dev branch, stage it, and commit it
touch nibbu.txt

git add nibbu.txt

git commit -m "Adding nibbu"

# Step 9: Switch between branches and modify files
git checkout master

git checkout dev

# Step 10: Create another branch from dev and modify a file
git checkout -b from-dev

echo "Modified content" > nibbu.txt

git add nibbu.txt

git commit -m "Modifying nibbu"

# Step 11: Check commit history and list branches
git log --oneline

git branch
