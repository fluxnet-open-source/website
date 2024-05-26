# Chapter: Using .gitignore in GitHub Desktop

In this chapter, you'll learn about the `.gitignore` file, why it's important, and how to use it in your Git repository. 

## Table of Contents

1. [What is .gitignore?](#what-is-gitignore)
2. [Why Use .gitignore?](#why-use-gitignore)
3. [Creating a .gitignore File](#creating-a-gitignore-file)
4. [Example .gitignore File](#example-gitignore-file)

## What is .gitignore?

The `.gitignore` file is a special file in Git that tells the version control system which files and directories to ignore in a repository. This means that the specified files and directories will not be tracked by Git, and any changes made to them will not be committed.

## Why Use .gitignore?

Imagine you are working on a project with raw data you use for processing. The raw data is many gigabytes in size and changes frequently, while the processed data is a much more manageable size. You don't want to commit this data to your repository because it will bloat the repository size and slow down operations like cloning and fetching (plus many remote Git providers like GitHub have limits to repo sizes). By adding the data directory to the `.gitignore` file, you can exclude the raw data from version control, while versioning the processed data.

Another example, many text editors and IDEs create configuration files or directories while you are working on a project specific to that editor. These files are not necessary for the project and can be safely ignored. By adding patterns to ignore these temporary files to the `.gitignore` file, you can keep your repository clean and avoid committing unnecessary files.

One final example, many languages create build artifacts, dependencies, or virtual environments when you compile or run your code. These files are not needed in the repository as they can be regenerated from the source code. By ignoring these build directories, you can avoid committing unnecessary files and keep your repository focused on the source code. Python for example compiles its code to `.pyc` bytecode files, which can be ignored.

## Creating a .gitignore File

1. Open GitHub Desktop and navigate to your repository.
2. Click on the `Repository` menu and select `Open in <Your Default Editor>` to open the repository in your text editor.
3. In your text editor, create a new file named `.gitignore` if it is not already created.
4. Add the files and directories you want to ignore to the `.gitignore` file. Each pattern to ignore should be on a new line.

## Example .gitignore File

Here's an example of a `.gitignore` template for R projects: 

```plaintext
# History files
.Rhistory
.Rapp.history

# Session Data files
.RData
.RDataTmp

# User-specific files
.Ruserdata

# Example code in package build process
*-Ex.R

# Output files from R CMD build
/*.tar.gz

# Output files from R CMD check
/*.Rcheck/

# RStudio files
.Rproj.user/

# produced vignettes
vignettes/*.html
vignettes/*.pdf

# OAuth2 token, see https://github.com/hadley/httr/releases/tag/v0.3
.httr-oauth

# knitr and R markdown default cache directories
*_cache/
/cache/

# Temporary files created by R markdown
*.utf8.md
*.knit.md

# R Environment Variables
.Renviron

# translation temp files
po/*~

# RStudio Connect folder
rsconnect/

```

## Adding .gitignore to Your Repository

1. Save the `.gitignore` file in your text editor.
2. Return to GitHub Desktop. You should see the `.gitignore` file listed under the `Changes` tab.
3. In the `Summary` field, write "Add .gitignore file" or another commit summary.
4. Click the `Commit to main` button to commit the `.gitignore` file to your repository.



By following these steps, you can create and use a `.gitignore` file in your Git repository to keep your project clean, secure, and manageable. This file is essential for any project to ensure that only relevant and necessary files are tracked by Git.
