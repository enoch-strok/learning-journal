# Git vs GitHub

##### What is Git and GitHub?
- Git is the **verson control software** and GitHub is the **cloud manager/collaboration**.
- In the past, version controlling was done locally only.
- VCS (Version Control System)
- CVCS (Centralized Version Control System)
- DVCS (Distributed Version Control System) Has multiple backups so that multiple mirrored repositores could be worked on at the same time. Helps with collaboration.
- Git tracks all changes and corruptions or loss of information.
- Git stores information in 3 stages.
  - Committed (Equivalent to "Save As"/Takes Snapshot)
    - Data is securely stored in a local database
  - Modified
    - File has been changed but not committed to the database
  - Staged
    - Flagged a file’s changed version to be committed in the next snapshot

##### Default Text Editor
Without configuration of a default text editor, Git will use the system’s default editor–most likely Vim. To configure a different text editor, such as Emacs, type the following into your Terminal or Command Line:

$ git config --global core.editor emacs

##### Using Seperate Users Per Project
*By using the –global option, these Git settings apply to anything on the system. To use different identity settings for a specific project, change the working directory to the desired local Git repository and repeat the steps above without using –global.

##### Terms & Info
- HEAD = The label meaning "You Are Here" (Latest version of the master file).
- Usually a message is added with a commit.

##### ACP
- **A** Add
  - `git add filename`
  - "Staging"
- **C** Commit
  - `git commit -m "why message`
- **P** Push
  - `git push origin master` or `git push`
