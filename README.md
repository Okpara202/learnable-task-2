# learnable task 2 - Favour Okpara (FE)

1. Explain version control

    Version control is a system that helps you manage changes to code, documents, or other digital content over time. It's a crucial tool for developers, writers, and teams to collaborate, track changes, and maintain a record of all modifications.

    ## Key Concepts:
    - Repository (Repo): A central location where all the files, folders, and history of changes are stored.
    - Commits: Snapshots of changes made to the code or content at a particular point in time.
    - Versions: A series of commits that represent the evolution of the code or content.
    - Branches: Separate lines of development that allow multiple versions of the code or content to coexist.

    ## Version Control Workflow:

    - Create a repository: Initialize a new repository, either locally or remotely (e.g., on GitHub).
    - Add files: Add files to the repository, which creates an initial commit.
    - Make changes: Modify files, add new ones, or delete existing ones.
    - Commit changes: Create a new commit that captures the changes made since the last commit.
    - Push changes: Upload the new commit to the remote repository (if applicable).
    - Pull changes: Download changes from the remote repository (if applicable) and merge them into the local repository.
    - Merge branches: Combine changes from different branches into a single branch.
    - Tag releases: Mark specific commits as releases, making it easier to track changes and maintain a record of updates.

    ## Benefits of Version Control:

    - Collaboration: Multiple developers can work on the same project simultaneously without conflicts.
    - Change tracking: A complete history of changes is maintained, making it easy to identify and revert changes if needed.
    - Backup and recovery: Version control systems provide a backup of the code or content, allowing for easy recovery in case of data loss or corruption.
    - Flexibility: Version control enables the creation of multiple branches, making it easy to experiment with new features or bug fixes without affecting the main codebase.

    ## Popular Version Control Systems:

    - Git
    - Mercurial
    - Subversion (SVN)
    - Perforce

    Git is one of the most widely used version control systems, and it's the one used by GitHub, GitLab, and many other popular platforms.

2. Explain difference between git and github

    Git and GitHub are two related concepts in the world of version control and software development. Although they always work together, they are quite different from each other.

    ## Git

    Git is a free, open-source version control system created by Linus Torvalds in 2005. It's a decentralized system that allows developers to track changes made to their code, collaborate with others, and maintain a record of all modifications.

    ## Key Features of Git:

    - Distributed version control system
    - Tracks changes made to code
    - Allows collaboration and branching
    - Fast and efficient
    - Supports large-scale projects

    ## GitHub

    GitHub is a web-based platform that provides a centralized location for Git repositories. Founded in 2008, GitHub allows developers to host, manage, and share their Git repositories with others. It provides a user-friendly interface for Git operations, as well as additional features like issue tracking, project management, and collaboration tools.

    ## Key Features of GitHub:

    - Web-based platform for Git repositories
    - Centralized location for code management
    - Collaboration tools and issue tracking
    - Project management and version control
    - Large community of developers and open-source projects

    ## Key Differences

    Here are the main differences between Git and GitHub:

    - Git is a version control system, while GitHub is a platform for hosting Git repositories.
    - Git is decentralized, while GitHub is centralized.
    - Git is primarily used for version control, while GitHub provides additional features like collaboration tools and issue tracking.

    In summary, Git is the underlying version control system, while GitHub is a platform that provides a user-friendly interface for Git operations and additional features for collaboration and project management.

3. List three other github alternatives

    Three other github alternatves are:

    - GitLab
    - Bitbucket
    - Azure DevOps


4. Explain the difference between git fetch and git pull

    Git fetch and Git pull are two closely related but very different Git commands.

    **Git fetch**

    Git fetch is a command that downloads the latest data from a remote repository, but it doesn't automatically merge it with your local data. It updates your local repository's knowledge of the remote repository's branches, tags, and commits. When you run git fetch, Git performs the following steps:

    - Connects to the remote repository.
    - Downloads the latest commits, branches, and tags from the remote repository.
    - Updates your local repository's refs (references) to match the remote repository's refs.
    - Doesn't merge the downloaded data with your local data.

    **Git pull**

    Git pull is a command that downloads the latest data from a remote repository and automatically merges it with your local data. It's essentially a combination of git fetch and git merge. When you run git pull, Git performs the following steps:

    - Connects to the remote repository.
    - Downloads the latest commits, branches, and tags from the remote repository (just like git fetch).
    - Merges the downloaded data with your local data (using git merge).
    - Updates your local repository's refs to match the remote repository's refs.

    **Key differences**

    Here are the main differences between git fetch and git pull:

    - git fetch only downloads data from the remote repository, while git pull downloads and merges the data.
    - git fetch doesn't change your local data, while git pull updates your local data by merging the downloaded changes.

    **When to use each command:**

    - Use git fetch when you want to update your local repository's knowledge of the remote repository's branches, tags, and commits without changing your local data.
    - Use git pull when you want to download and merge the latest changes from the remote repository into your local data.

5. Explain in simple terms git rebase and the command for it

    Git Rebase is a way to update your local branch with the latest changes from a remote branch, while keeping your commit history clean and linear.

    ## How does Git Rebase work?

    Imagine you're working on a feature branch, and you've made some commits. Meanwhile, someone else has made changes to the main branch (e.g., master). When you want to update your feature branch with those changes, you can use Git Rebase.

    Here's what happens during a rebase:

    - Git temporarily removes your local commits.
    - Git updates your local branch with the latest changes from the remote branch.
    - Git reapplies your local commits on top of the updated branch.

    **Git Rebase Command:**

    The basic command for Git Rebase is: `git rebase <branch-name>`

    Replace <branch-name> with the name of the branch you want to rebase onto (e.g., master, main, etc.).

6. Explain in simple terms git cherry-pick and the command for it

    Git Cherry-Pick is a way to apply a single commit from one branch to another branch.

    **How does Git Cherry-Pick work?**

    Imagine you have two branches: feature and master. You've made a commit on the feature branch that fixes a bug, and you want to apply that same fix to the master branch without merging the entire feature branch.

    Here's what happens during a cherry-pick:

    - Git finds the commit you want to cherry-pick.
    - Git applies the changes from that commit to your current branch.

    ## Git Cherry-Pick Command:

    The basic command for Git Cherry-Pick is: `git cherry-pick <commit-hash>`


    Replace <commit-hash> with the hash of the commit you want to cherry-pick. You can find the commit hash using git log.