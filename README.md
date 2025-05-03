**1️⃣ Navigate to Your Local Project Folder**
cd /home/ubuntu/new_folder

**2️⃣ Initialize Git (If Not Already Initialized)**
git init

**3️⃣ Add the Remote Repository (Even If the Names Differ)**
git remote add origin <your-repo-url>
git remote add origin https://ssh path present with repository

**4️⃣ Add and Commit Files**
git add .
git commit -m "Initial commit"

**5️⃣ Push to the Repository**
If pushing to the main branch: default is main branch present in git
git branch -M main
git push -u origin main

**6 Push to the Repository**
If you want to remove a Git remote from your repository, use:
git remote remove <remote-name>

ex- git remote remove origin

**Pull with rebase (recommended for cleaner history)**
git pull --rebase origin main
git push origin main
