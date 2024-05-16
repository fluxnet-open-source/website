# Version Control, Git, GitHub, and GitHub Desktop

## What is Version Control?

Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later. It allows multiple people to collaborate on a project, keeps track of every modification to the code, and can help revert to a previous version if necessary, but even if you are working alone, it can make things so much easier:

![Comic: a PhD student sends "FINAL.doc" to their supervisor, but after several increasingly intense and frustrating rounds of comments and revisions they end up with a file named "FINAL_rev.22.comments49.corrections.10.#@$%WHYDIDCOMETOGRADSCHOOL????.doc" - source: https://phdcomics.com/comics/archive.php?comicid=1531](fig/phd101212s.png)

### Key Features of Version Control:

- **History Tracking**: Keeps a record of every change made to the files.
- **Collaboration**: Multiple people can work on the same project simultaneously without overwriting each other's work.
- **Branching and Merging**: Allows you to create branches to work on different features or fixes independently and merge them back into the main codebase when ready.
- **Backup and Restore**: Helps in restoring files to a previous state in case of accidental deletion or errors.

## What is Git?

Git is a distributed version control system designed to handle everything from small to very large projects with speed and efficiency. It allows developers to track changes, revert to previous stages, and work simultaneously on multiple branches.

### Key Features of Git:

- **Distributed System**: Every developer has a complete history of the project on their local machine.
- **Performance**: Fast and efficient handling of projects of any size.
- **Branching and Merging**: Flexible branching and merging capabilities, making it easier to experiment and integrate new features.
- **Integrity**: Ensures the integrity of the code by storing every change in a cryptographic hash.

## Why Should You Use Version Control and Git?

### 1. **Collaboration**

Version control allows multiple developers to work on the same project simultaneously without overwriting each other's work. Git makes it easy to merge changes and resolve conflicts.

### 2. **History and Backup**

Every change made to the project is recorded, providing a complete history of the project. This is crucial for understanding what changes were made, by whom, and why. It also acts as a backup, allowing you to revert to previous versions if needed.

![Graphic: Changes Are Saved Sequentially - source: https://github.com/swcarpentry/git-novice](fig/play-changes.svg)

### 3. **Branching and Experimentation**

Git allows you to create branches to work on new features, bug fixes, or experiments without affecting the main codebase. 

![Graphic: Different Versions Can be Saved - source: https://github.com/swcarpentry/git-novice](fig/versions.svg)

Once the work is complete and tested, you can merge the branch back into the main codebase.

![Graphic: Multiple Versions Can be Merged - source: https://github.com/swcarpentry/git-novice](fig/merge.svg)


## What is GitHub?

GitHub is a web-based platform that uses Git for version control and provides a collaborative environment for developers. It hosts your repositories and allows you to manage your projects with additional features such as issue tracking, project management tools, and continuous integration.

## What is GitHub Desktop?

GitHub Desktop is a user-friendly application that provides a graphical interface to interact with Git and GitHub. It simplifies the process of managing your repositories, making it accessible even for those who are not familiar with the command-line interface.
