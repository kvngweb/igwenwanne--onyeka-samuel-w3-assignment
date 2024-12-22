# igwenwanne--onyeka-samuel-w3-assignment
Version Control

Version control is a system for managing changes to files over time. It helps developers to:

Track Changes: Keep a record of who changed what and when.

Collaborate: Allow multiple people to work on the same project simultaneously.

Restore Previous Versions: Roll back to earlier versions if needed.

Experiment Safely: Use branching to test new ideas without disrupting the main project.

Difference Between Git and GitHub
Git:

A distributed version control system.
Manages your project's code history on your local machine.
Offers commands like commit, branch, merge, and push.

GitHub:

A cloud-based platform for hosting Git repositories.
Provides additional collaboration tools like issue tracking, pull requests, and web-based interfaces.

Acts as a central hub for sharing and managing Git repositories online.
3 GitHub Alternatives
GitLab:

A Git repository hosting service with built-in CI/CD pipelines.
Supports self-hosting and private repositories.
Bitbucket:

A Git and Mercurial repository platform.
Well-integrated with Atlassian products like Jira.
SourceForge:

Offers Git and Subversion (SVN) hosting.
Focuses on open-source projects.

Difference Between git fetch and git pull
git fetch:

Downloads changes from the remote repository to your local repository but does not update your working branch.

Useful to preview changes before merging them.
git pull:

Combines git fetch and git merge in one step.
Downloads changes and immediately merges them into your current branch.
Git Rebase (Simple Terms)

What it does:
Rebase re-applies your branch's commits on top of another branch to create a cleaner, linear history.

Example:

Before rebasing:
mathematica
Copy code
main:    A---B---C  
feature:       D---E  

After rebasing feature onto main:

mathematica
Copy code
main:    A---B---C  
feature:             D'---E'  
Command:

bash
Copy code
git checkout feature  
git rebase main  
When to use:

To clean up commit history before merging.
Git Cherry-Pick (Simple Terms)

What it does:
Cherry-pick applies a specific commit from one branch to another without merging the entire branch.

Example:

Original feature branch:
mathematica
Copy code
feature: A---B---C---D  
Cherry-pick commit C onto main:
vbnet
Copy code
main:    X---Y---Z---C'  
Command:

bash
Copy code
git checkout main  
git cherry-pick <commit-hash>  
When to use:

To pick a bug fix or feature from another branch without including unrelated commits.
