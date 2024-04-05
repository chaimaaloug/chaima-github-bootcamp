--- { "layout" : "center" }

# GitHub Bootcamp

<img width="580" alt="spidertocat.png" src="https://octodex.github.com/images/mona-the-rivetertocat.png">

---

### How to initialise a new repository

1- Open your terminal or command prompt where you want to create the new repository.

```bash
$ cd /path/to/your/project
```

2- Use the following command to initialize a new Git repository.

```bash
$ git init
```

---

3- If you have an existing repository on a platform like GitHub, you can add a remote.

```bash
$ gra origin https://github.com/your-username/your-repository.git
```

4- Add your files to the staging area and commit them.

```bash
$ gaa
$ gcmsg "Initial commit"
```

5- If you added a remote, push your changes to the remote repository.

```bash
$ gp -u origin master
```

---

### How to review changes

To view <span style='color:yellow'>unstaged changes</span> in your working directory, you can use:

```bash
$ gd
```

To review the commit history, including the changes made in each commit, you can use:

```bash
$ glg
```

---

To review changes for a specific file, you can use:

```bash
$ gd <filename>
```

---

### How to commit changes

Before committing changes, you need to stage them. This command adds all changes in your working directory to the staging area.

```bash
$ gaa
```

Once you've staged your changes, it's time to commit them with a meaningful message that describes the purpose of the commit.

```bash
$ gcmsg "Your commit message here"
```

---

### Create a new branch

To create a new branch and switch to it, use the following command:

```bash
$ gcb new-branch-name
```

If you're using a more recent version of Git (2.23 and later), you can also use the git switch command:

```bash
$ gswc new-branch-name
```

---

### Merge branch on main

Before merging, ensure you are on the main branch:

```bash
$ gco main
```

To merge a branch into the main branch, use:

```bash
$ gm main
```

---

### Delete a branch

To delete a branch locally, use:

```bash
$ git branch -d branch-name
```

If the branch was pushed to a remote repository and you want to delete it there:

```bash
$ git push origin --delete branch-name
```

---

Verify that the branch is deleted locally and, if applicable, on the remote repository.

```bash
$ git branch
```

This command lists all local branches, and the deleted branch should not be in the list.

---

### Pushing changes to remote

This command sends your commits to the remote repository on platforms like GitHub.

```bash
git push <remote-name> <branch-name>
git push origin main
```

Tips 💡:

- Always pull changes before pushing to avoid conflicts.
- Push regularly to keep your remote up-to-date.

---

### Pulling changes from remote

This command fetches changes from the remote and merges them into your current branch.

```bash
git pull <remote-name> <branch-name>
```

Tips 💡:

- Pull regularly to stay updated with remote changes.
- Resolve any conflicts that may arise during the pull.

---

### WHAT ARE GIT AND GITHUB?

Git is a particular implementation of version control originally designed by Linus Torvalds in 2005 as a way of managing the Linux kernel. Git manages the evolution
of a set of files – called a repository or repo

Git is the software you will use locally
to record changes to a set of files. GitHub is a
hosting service that provides a Git-aware home for
such projects on the internet

---

### Repositories

- Often referred to as a repo, this a collection of all your files and
  the history of those files (i.e. commits)

- Can live on a local machine or on a remote server (e.g. GitHub)

- The act of copying a repo from a remote server is called cloning

--- { "layout" : "center" }

### Git Push Pull Commands

<img width="730" alt="github.png" src="https://edav.info/images/git/pull-request-2.png">

---

# Git Basics

## "Branching Strategies in Git"

> "In Git, every commit is like a snapshot of your project at a specific point in time, making it easy to navigate and collaborate."

---

# Code

```python
print("Hello, Spectacle!")
```

---

# Making a commit

- Make some changes to a file
- Use the git add command or Atom to add files to the staging area
- Type a commit message (that shortly describes the changes you made since the last commit) into the commit message box, and click the Commit button.

---

# How to apply commit

- Stage Changes: Use git add <file> to stage modifications for the next commit.
- Commit Changes: Utilize git commit -m "Your commit message" to commit staged changes.
- Review Changes: Always review modifications before committing to ensure accuracy.
- Push Changes: If collaborating, push commits to the remote repository using git push.

---

### How to use git fragments

---

### This one will be reverted

---

### How to fix the last commit message

---

### How to rebase
