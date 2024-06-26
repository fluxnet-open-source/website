# 1: Pre Workshop: Setup GitHub Desktop on Windows, macOS, or Ubuntu

## Introduction

There are many ways to interact with Git and GitHub, both through the command line and through a graphical user interface (GUI), but in this tutorial we will be using GitHub Desktop. We chose GitHub Desktop because it is free, provides a graphical interface which can be easier to use for beginners, and is not tied to a specific IDE or text editor.

There are many alternatives to GitHub Desktop, such as GitKraken or integrations with IDEs like Visual Studio Code, but GitHub Desktop is a good choice if you're new to Git and GitHub. Other tools may offer more advanced features or integration with your preferred IDE, so may be worth exploring once you're more comfortable with Git.

- [GitKraken](https://www.gitkraken.com): A popular Git GUI application that offers a wide range of features, including features not present in GitHub Desktop such as a Git log tree, AI commit messages, and more.
- [Visual Studio Code](https://code.visualstudio.com): A popular code editor that includes built-in Git support, allowing you to perform common Git operations directly from the editor.
- Any other IDE or text editor you prefer may have Git integration built-in or available as an extension.

This guide will walk you through the installation process for Windows, macOS, and Linux. 

## Table of Contents

1. [Creating a GitHub Account](#creating-a-github-account)
1. [Installing GitHub Desktop](#installing-github-desktop)
    - [Windows](#windows)
    - [macOS](#macos)
    - [Linux](#linux)
1. [Install IDE (Integrated Development Environment) or Text Editor](#install-ide-integrated-development-environment-or-text-editor)

## Creating a GitHub Account

You will need an account for [GitHub](https://github.com) to use GitHub Desktop. Here's how to create one:

1. Go to <https://github.com> and follow the "Sign up" link at the top-right of the window.
2. Follow the instructions to create an account.
3. Verify your email address with GitHub.
4. Configure multifactor authentication (see below).

### Multi-factor Authentication

In 2023, GitHub introduced a requirement for 
all accounts to have 
[multi-factor authentication (2FA)](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/about-two-factor-authentication) 
configured for extra security.
Several options exist for setting up 2FA, you can find 2FA setup instructions for GitHub [here](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication).

## Installing GitHub Desktop

### Windows

#### Step 1: Download GitHub Desktop

1. Open your web browser and go to the [GitHub Desktop website](https://desktop.github.com/).
2. Click the `Download for Windows` button.

#### Step 2: Install GitHub Desktop

1. Once the download is complete, locate the `GitHubDesktopSetup.exe` file in your downloads folder and double-click it to start the installation.
2. Follow the on-screen instructions to complete the installation.

#### Step 3: Launch GitHub Desktop

1. After the installation is complete, GitHub Desktop should launch automatically. If it doesn’t, you can find it in your Start menu and launch it from there.
2. Sign in to your GitHub account or create a new one if you don’t have an account.

### macOS

#### Step 1: Download GitHub Desktop

1. Open your web browser and go to the [GitHub Desktop website](https://desktop.github.com/).
2. If you have an Apple Silicon (M1, M2, etc.) Mac, click the `Download for Apple Silicon` button. If you have an Intel-based Mac, click the `Download for MacOS` button.
  - If you're not sure which version you have, you can check by clicking the Apple logo in the top-left corner of your screen, selecting `About This Mac`. 
  - You can also download the intel version on an Apple Silicon Mac (the `Download for MacOS` button), but it will run a little slower.

#### Step 2: Install GitHub Desktop

1. Once the download is complete, locate the `GitHub Desktop.zip` file in your downloads folder and double-click it to extract the application if it did not extract automatically. Click the extracted `GitHub Desktop` application to open it.
2. Drag the `GitHub Desktop` application into your `Applications` folder.

#### Step 3: Launch GitHub Desktop

1. Open the `Applications` folder and double-click `GitHub Desktop` to launch it.
2. Sign in to your GitHub account or create a new one if you don’t have an account.

### Linux

GitHub Desktop is not officially available for Linux, but because the source code is open-source, there is a fork for linux called [ShiftKey GitHub Desktop](https://github.com/shiftkey/desktop). Installation instructions for your distribution can be found on the [ShiftKey GitHub Desktop page](https://github.com/shiftkey/desktop)

## Install Git - Optional

GitHub Desktop comes with its own trimmed down version of Git, so you don't need to install Git separately. However, this version of Git is not accessible from the command line. If you want to use Git from the command line, you can install Git separately.
You can find instructions for installing Git on Windows, macOS, and Linux [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). 

On macOS and Linux, Git is often pre-installed, so you may not need to install it, you can check by opening a terminal and typing `git --version`.

## Install IDE (Integrated Development Environment) or Text Editor - Optional

To work with your code, you will need an IDE or text editor. You may already have one installed that you are comfortable with such as Visual Studio Code (VS Code), PyCharm, RStudio, or another. If you don't have one installed, here are some popular options:

- [Visual Studio Code](https://code.visualstudio.com/)
  - works with many languages and has a large number of extensions available
- [PyCharm](https://www.jetbrains.com/pycharm/)
  - Python focused, but works with other languages as well
- [RStudio](https://www.rstudio.com/)
  - R focused, but works with other languages as well

For this tutorial, if you don't want to install an IDE or text editor, you can use any text editor you are comfortable with, such as Notepad (Windows), TextEdit (macOS), or Gedit (Linux).

## Configure GitHub Desktop - Optional

Once you have GitHub Desktop installed, there are a few settings you may want to configure:

- Default editor: You can set your preferred text editor or IDE as the default editor for opening files in GitHub Desktop.
  -  instructions found [here](https://docs.github.com/en/desktop/configuring-and-customizing-github-desktop/configuring-a-default-editor-in-github-desktop)
