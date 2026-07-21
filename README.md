# 🔄 GitLab ↔ GitHub Repository Mirroring

This project demonstrates how to mirror a GitLab repository with GitHub so that all changes made in GitLab are automatically synchronized to GitHub.

## 📌 Project Objective

The objective of this project is to understand:

- GitLab Repository Management
- GitHub Repository Integration
- Repository Mirroring
- Branch Management
- Merge Requests
- Automatic Synchronization between GitLab and GitHub

---

## 🛠️ Technologies Used

- Git
- GitLab
- GitHub
- SSH Authentication

---

## 📂 Repository Structure

```
mirror-repo-gitlab/
├── README.md
├── index.html
└── contact.html
```

---

# 🚀 Steps Performed

## Step 1 - Create GitLab Repository

- Created a new GitLab repository named **mirror-repo-gitlab**
- Initialized the repository with a README file

---

## Step 2 - Configure SSH Authentication

Generated an SSH key:

```bash
ssh-keygen -t ed25519 -C "your-email@example.com"
```

Copied the public key:

```bash
cat ~/.ssh/id_ed25519.pub
```

Added the SSH key to:

**GitLab → User Settings → SSH Keys**

Verified SSH connection:

```bash
ssh -T git@gitlab.com
```

---

## Step 3 - Clone Repository

```bash
git clone git@gitlab.com:maliuday/mirror-repo-gitlab.git
```

---

## Step 4 - Configure Repository Mirroring

Configured repository mirroring so that:

```
GitLab
     │
     ▼
```
---

## Step 5 - Create Initial HTML File

Created:


Checked repository status:

```bash
git status
```

Added files:


Committed changes:

```bash
git commit -m "Add index.html"
```

Pushed to GitLab:

```bash
git push origin main
```

Verified that the same changes appeared automatically on GitHub.

---

## Step 6 - Create Development Branch

Created a new branch:

```bash
git checkout -b dev
```

Created:

```
contact.html
```

Added changes:

```bash
git add .
```

Committed changes:

```bash
git commit -m "Add contact page"
```

Pushed branch:

```bash
git push origin dev
```

---

## Step 7 - Merge Branch

Created a Merge Request in GitLab.

Merged:

```
dev
   │
   ▼
main
```

---

## Step 8 - Verify Mirroring

After merging into **main**, all changes were automatically synchronized to GitHub.

Verified that:

- ✅ index.html
- ✅ contact.html
- ✅ Commit History
- ✅ Branch Updates

were successfully mirrored to GitHub.

---

# 🔄 Workflow

```
Developer
     │
     ▼
GitLab Repository
     │
     ▼
Create Branch (dev)
     │
     ▼
Develop Features
     │
     ▼
Commit
     │
     ▼
Push
     │
     ▼
Merge Request
     │
     ▼
Merge to Main
     │
     ▼
Repository Mirroring
     │
     ▼
GitHub Repository
```

---

# 📚 Git Commands Used

```bash
git clone
git status
git branch
git checkout -b dev
git add .
git commit -m ""
git push origin main
git push origin dev
git pull
```

---

# ✅ Learning Outcomes

- Created a GitLab repository
- Configured SSH authentication
- Connected GitLab with GitHub
- Configured Repository Mirroring
- Worked with Git branches
- Created and merged Merge Requests
- Understood GitLab workflow
- Verified automatic synchronization between GitLab and GitHub

---

## 📷 Demo

- Repository created in GitLab
- Repository mirrored to GitHub
- Branch creation
- Merge Request
- Successful synchronization

---

## 👨‍💻 Author

**Uday Mali**

- GitHub: https://github.com/Maliuday
- GitLab: https://gitlab.com/maliuday
- LinkedIn: https://www.linkedin.com/in/uday-mali-7aa1b7286/```bash
git add .
```
```
index.html
```

Every push to GitLab is automatically synchronized with GitHub.


