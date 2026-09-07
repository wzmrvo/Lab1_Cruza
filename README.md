# Lab 1 - Git and GitHub

## Student Information

**Name:** Cruza Daniel L.
**Course:** Bachelor of Science in Information Technology (BSIT)

---

# Step-by-Step Git and GitHub Process

## Step 1: Configure Git

First, Git was configured with the user's name and email.

```bash
git config user.name "Your Name"
git config user.email "your@email.com"
```

The configuration was checked using:

```bash
git config user.name
git config user.email
```

## Step 2: Create the Project Folder

A project folder named `Cruza_BSIT` was created.

The project was opened in Visual Studio Code.

## Step 3: Initialize the Git Repository

Git was initialized inside the project folder:

```bash
git init
```

This created a local Git repository for the project.

## Step 4: Create the Initial HTML

The initial webpage was created using HTML.

The main file was:

```text
main.html
```

The initial version contained the basic HTML structure without styling.

## Step 5: Add and Commit the Initial Version

The initial HTML file was added to Git:

```bash
git add .
```

Then it was committed:

```bash
git commit -m "Initial HTML version"
```

## Step 6: Create the `no-style` Branch

A separate branch was created for the HTML-only version:

```bash
git switch -c no-style
```

The purpose of this branch was to preserve the original webpage without CSS and JavaScript.

The branch was checked using:

```bash
git ls-tree --name-only HEAD
```

The `no-style` branch contains:

```text
main.html
```

## Step 7: Return to the `main` Branch

After preserving the HTML-only version, the project was switched back to the main branch:

```bash
git switch main
```

## Step 8: Add CSS and JavaScript

The complete webpage was developed on the `main` branch.

The project files became:

```text
main.html
main.css
main.js
```

CSS was used to style the webpage and make it responsive.

JavaScript was used to add interactive features such as the theme toggle, mobile menu, and contact form interaction.

## Step 9: Add the Updated Files

The completed files were added to Git:

```bash
git add main.html main.css main.js
```

## Step 10: Commit the Completed Version

The completed webpage was committed:

```bash
git commit -m "Create modern responsive portfolio"
```

## Step 11: Connect the Local Repository to GitHub

The local repository was connected to the GitHub repository using:

```bash
git remote add origin https://github.com/wzmrvo/Lab1_Cruza.git
```

## Step 12: Push the `main` Branch

The completed `main` branch was uploaded to GitHub:

```bash
git push -u origin main
```

## Step 13: Push the `no-style` Branch

The HTML-only branch was also uploaded:

```bash
git switch no-style
git push -u origin no-style
```

## Step 14: Verify the Branches

The available branches were checked using:

```bash
git branch -a
```

The repository contains:

```text
main
no-style
remotes/origin/main
remotes/origin/no-style
```

## Step 15: Final Project Structure

The final project contains two versions.

### `main` branch

```text
main
├── main.html
├── main.css
└── main.js
```

This is the complete styled and interactive version.

### `no-style` branch

```text
no-style
└── main.html
```

This is the original HTML-only version.

---

# Technologies Used

* HTML5
* CSS3
* JavaScript
* Git
* GitHub
* Visual Studio Code

# Conclusion

This laboratory activity demonstrated how to use Git for version control and GitHub for remote repository management. Branching was used to preserve the original HTML-only version while the `main` branch was developed into a complete webpage with CSS styling and JavaScript functionality.
