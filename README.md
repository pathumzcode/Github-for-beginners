# 🐙 GitHub for Beginners — Hands-On Workshop

Welcome to **GitHub for Beginners!** 🚀

This repository is designed to help beginners learn Git and GitHub through practical, step-by-step activities. You will learn how to create branches, manage files, commit changes, push code, and contribute to a repository using Pull Requests.

Instead of only learning theory, you will complete each activity by working directly with files and commands.

![GitHub for Beginners Banner](images/banner.jpg)

## 🎯 What You Will Learn

* Understand the difference between Git and GitHub.
* Create and manage GitHub repositories.
* Fork and clone repositories.
* Create and switch between branches.
* Create, edit, and organize project files.
* Stage and commit changes.
* Push branches to GitHub.
* Create and review Pull Requests.
* Work with GitHub Issues.
* Collaborate with other developers.

## 📍 Prerequisites

Before starting the workshop, make sure you have the following:

| Requirement         | Description                                                         |
| ------------------- | ------------------------------------------------------------------- |
| GitHub Account      | A GitHub account to fork repositories and create Pull Requests.     |
| Git                 | Installed and configured on your computer.                          |
| Visual Studio Code  | Recommended editor for working with project files.                  |
| Terminal            | Windows PowerShell, Command Prompt, macOS Terminal, or Linux shell. |
| Internet Connection | Required to access GitHub.                                          |

## 🛠️ Installation Guide

### 1. Install Git

#### For Windows

1. Download Git from [git-scm.com](https://git-scm.com/download/win).
2. Run the installer and follow the setup wizard.
3. Use the default settings if you are a beginner.
4. Open Command Prompt or PowerShell.
5. Verify the installation:

```bash
git --version
```

#### For macOS

Install Git using Homebrew:

```bash
brew install git
```

Alternatively, download Git from [git-scm.com](https://git-scm.com/download/mac).

Verify the installation:

```bash
git --version
```

#### For Linux

Install Git using your distribution's package manager.

For Ubuntu or Debian:

```bash
sudo apt update
sudo apt install git
```

Verify the installation:

```bash
git --version
```

### 2. Install Visual Studio Code

1. Download VS Code from [code.visualstudio.com](https://code.visualstudio.com/).
2. Install the application for your operating system.
3. Follow the official guide to enable the [VS Code command-line tool](https://code.visualstudio.com/docs/editor/command-line).

Verify that the `code` command works:

```bash
code --version
```

## 🚀 Getting Started

### Step 1: Fork This Repository

A **Fork** creates your own copy of another person's repository under your GitHub account.

1. Open the original workshop repository.
2. Click the **Fork** button.
3. Select your GitHub account as the destination.
4. Complete the fork process.
5. Open your fork and verify that it was created successfully.

> 💡 **Best Practice:** Create a folder called `workshop` on your Desktop to organize your workshop projects.


### Step 2: Open Your Terminal

Open PowerShell, Command Prompt, or your preferred terminal.

Navigate to your workshop folder.

For Windows:

```powershell
cd Desktop
mkdir workshop
cd workshop
```

If the folder already exists, simply navigate into it instead of creating it again.

### Step 3: Clone Your Fork

**Clone** downloads a copy of your repository to your computer.

Replace `your-username` with your actual GitHub username.

```bash
git clone https://github.com/your-username/Github-for-beginners.git
```

Navigate into the project directory:

```bash
cd Github-for-beginners
```

Open the project in VS Code:

```bash
code .
```

Verify the repository status:

```bash
git status
```

> 💡 **Tip:** Since you cloned your fork, `origin` normally points to your fork on GitHub.

## 🌿 Branch Practice Exercises

### Exercise 1: Create Your First Branch

A **branch** allows you to work on changes separately without directly modifying the `main` branch.

Create a branch using your name:

```bash
git switch -c feature/your-name-introduction
```

For example:

```bash
git switch -c feature/pathum-introduction
```

Check your current branch:

```bash
git branch
```

The current branch is marked with an asterisk (`*`).

**Your task:**

* Create a feature branch using your name.
* Confirm that you are working on the new branch.

### Exercise 2: Create and Edit Your First File

1. Open the repository in VS Code.
2. Find the `student-introductions.md` file.
3. Open the file.
4. Add your introduction using the template below.
5. Save your changes.

If the file does not exist, create it in the repository root.

#### Introduction Template

Add the following Markdown content and replace the example details with your own information:

```markdown
## Your Name

- **GitHub Username:** your-username
- **Role:** Student / Developer
- **Interests:** Web Development, Java, GitHub
- **About Me:** Write a short introduction about yourself.
- **What I Want to Learn:** Git, GitHub, and Open Source.
```

**Your task:**

* Add your introduction.
* Use Markdown formatting correctly.
* Save the file.

### Exercise 3: Check Your Changes

Before committing, check which files have changed.

```bash
git status
```

Review the differences:

```bash
git diff
```

These commands help you understand what you changed before saving the changes in Git history.

**Your task:**

* Check the modified files.
* Review your introduction.
* Make sure you have not accidentally changed unrelated files.

### Exercise 4: Stage and Commit Your Changes

**Staging** selects the changes that will be included in your next commit.

Stage the introduction file:

```bash
git add student-introductions.md
```

Alternatively, stage all changes:

```bash
git add .
```

Check the staged changes:

```bash
git status
```

Commit your changes with a meaningful message:

```bash
git commit -m "Add introduction for your-name"
```

For example:

```bash
git commit -m "Add introduction for Pathum"
```

> ⚠️ **Troubleshooting:** If Git asks you to configure your identity, follow the [Git Configuration Troubleshooting Guide](https://github.com/nisalgunawardhana/Github-for-beginners/blob/main/support%20md%20files/Git-Configuration-Troubleshooting.md).

**Your task:**

* Stage your changes.
* Create at least one commit.
* Use a clear commit message.

### Exercise 5: Create a Second Branch

Practice creating another branch.

First, return to your original branch:

```bash
git switch main
```

Create a new branch:

```bash
git switch -c feature/add-learning-goals
```

Create a file named `learning-goals.md` and add:

```markdown
# My Learning Goals

- Learn Git commands.
- Understand GitHub repositories.
- Practice branching and merging.
- Create Pull Requests.
- Contribute to open-source projects.
```

Stage and commit the file:

```bash
git add learning-goals.md
git commit -m "Add personal learning goals"
```

**Your task:**

* Create a second branch.
* Add a new Markdown file.
* Commit the changes separately from your introduction branch.

### Exercise 6: Push Your Branches to GitHub

A **push** uploads your local commits to a remote repository.

Push your first branch:

```bash
git push -u origin feature/your-name-introduction
```

Push your second branch:

```bash
git push -u origin feature/add-learning-goals
```

Replace `feature/your-name-introduction` with the actual branch name you created.

Open your fork on GitHub and verify that both branches are available.

**Your task:**

* Push both branches.
* Confirm that your commits appear on GitHub.

### Exercise 7: Create Your First Pull Request

A **Pull Request (PR)** allows you to propose changes from one branch to another.

1. Open your fork on GitHub.
2. Select the `feature/your-name-introduction` branch.
3. Click **Compare & pull request**, if displayed.
4. Set the original workshop repository as the **base repository**.
5. Set `main` as the base branch.
6. Select your fork as the **head repository**.
7. Select your feature branch as the compare branch.
8. Add a meaningful title and description.
9. Click **Create pull request**.

Example title:

```text
Add introduction for Pathum
```

Example description:

```markdown
## Changes Made

- Added my introduction to student-introductions.md.
- Followed the provided Markdown template.

## Purpose

This Pull Request is part of the GitHub for Beginners workshop.
```

> 💡 **Important:** When contributing to the original workshop repository, ensure the Pull Request targets the original repository, not just another branch in your fork.

### Pull Request Screenshots

![Compare and Pull Request](https://github.com/nisalgunawardhana/Github-for-beginners/raw/main/images/pr-image1.png)

![Review Pull Request](https://github.com/nisalgunawardhana/Github-for-beginners/raw/main/images/pr-image2.png)

![Create Pull Request](https://github.com/nisalgunawardhana/Github-for-beginners/raw/main/images/pr-image3.png)

**Your task:**

* Create at least one Pull Request.
* Check the target repository and branch.
* Review your changes before submitting.

### Exercise 8: Learn About GitHub Issues

An **Issue** is used to report bugs, suggest improvements, ask questions, or track tasks.

1. Open the original workshop repository.
2. Select the **Issues** tab.
3. Click **New issue**.
4. Enter a descriptive title.
5. Explain your suggestion or report.
6. Submit the Issue.

Example title:

```text
Suggest an improvement to the beginner guide
```

Example description:

```markdown
## Suggestion

Add another example explaining how Git branches work.

## Reason

This could help beginners understand branching more easily.
```

**Your task:**

* Create an Issue on the original repository, if you have permission and Issues are enabled.
* If you do not have permission to create an Issue, follow the workshop organizer's submission instructions instead.

## 🏆 Submission Guidelines

After completing the exercises, submit your work using the workshop's official submission process, if one is provided.

Before submitting, make sure you have the following information ready:

* Your GitHub username.
* A link to your fork.
* Links to your Pull Requests.
* A link to your Issue, if applicable.
* Screenshots showing your completed work.
* A short reflection describing what you learned.

### Submission Steps

1. Open the original workshop repository.
2. Navigate to the submission instructions.
3. Open the designated submission Issue template, if available.
4. Provide your GitHub username and relevant links.
5. Attach screenshots or other requested evidence.
6. Submit your completion details.

![Submission Issue](https://github.com/nisalgunawardhana/Github-for-beginners/raw/main/images/issue1.png)

![Submission Details](https://github.com/nisalgunawardhana/Github-for-beginners/raw/main/images/issue2.png)

> **Note:** Follow the current instructions provided by the workshop organizers. Do not assume that a submission template or badge is available unless the repository provides one.

## 📋 Checklist for Completion

Use this checklist to track your progress.

* [ ] Created or accessed a GitHub account.
* [ ] Installed Git.
* [ ] Installed Visual Studio Code.
* [ ] Forked the workshop repository.
* [ ] Cloned the fork to my computer.
* [ ] Created at least two feature branches.
* [ ] Added my introduction to `student-introductions.md`.
* [ ] Created an additional Markdown file.
* [ ] Staged and committed my changes.
* [ ] Used meaningful commit messages.
* [ ] Pushed my branches to GitHub.
* [ ] Created at least one Pull Request to the original repository.
* [ ] Reviewed the Pull Request changes.
* [ ] Created an Issue on the original repository, if permitted.
* [ ] Prepared the required submission details.

## 📚 Useful Git Commands

| Command                          | Purpose                                |
| -------------------------------- | -------------------------------------- |
| `git --version`                  | Check the installed Git version        |
| `git clone URL`                  | Clone a repository                     |
| `git status`                     | Check repository status                |
| `git branch`                     | List local branches                    |
| `git switch -c branch-name`      | Create and switch to a branch          |
| `git switch main`                | Switch to the `main` branch            |
| `git add filename`               | Stage a specific file                  |
| `git add .`                      | Stage changes in the current directory |
| `git commit -m "message"`        | Commit staged changes                  |
| `git diff`                       | View unstaged changes                  |
| `git log --oneline`              | View commit history                    |
| `git push -u origin branch-name` | Push a branch and set its upstream     |
| `git pull`                       | Fetch and integrate remote changes     |
| `git remote -v`                  | Display configured remote repositories |

## 🚀 Keep Learning and Building!

Congratulations on completing the GitHub for Beginners hands-on workshop!

Keep practicing with personal projects, explore open-source repositories, and collaborate with other developers.

**Learn. Practice. Collaborate. Contribute. 🐙💻**
