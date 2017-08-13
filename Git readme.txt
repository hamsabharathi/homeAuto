You have now been introduced to the fundamental Git workflow. You learned a lot! Let's take a moment to generalize:

Git is the industry-standard version control system for web developers
Use Git commands to help keep track of changes made to a project:
git init creates a new Git repository
git status inspects the contents of the working directory and staging area
git add <filename> adds files from the working directory to the staging area
git diff shows the difference between the working directory and the staging area
git commit permanently stores file changes from the staging area in the repository
git log shows a list of all previous commits

Congratulations! You've learned three different ways to backtrack in Git. You can use these skills to undo changes made to your Git project.

Let's take a moment to review the new commands:

git checkout HEAD filename: Discards changes in the working directory.
git reset HEAD filename: Unstages file changes in the staging area.
git reset SHA: Can be used to reset to a previous commit in your commit history.
Additionally, you learned a way to add multiple files to the staging area with a single command:

git add filename_1 filename_2

Let's take a moment to review the main concepts and commands from the lesson before moving on.

Git branching allows users to experiment with different versions of a project by checking out separate branches to work on.
The following commands are useful in the Git branch workflow.

git branch: Lists all a Git project's branches.
git branch branch_name: Creates a new branch.
git checkout branch_name: Used to switch from one branch to another.
git merge branch_name: Used to join file changes from one branch to another.
git branch -d branch_name: Deletes the branch specified

The workflow for Git collaborations typically follows this order:

1.Fetch and merge changes from the remote
2.Create a branch to work on a new project feature
3.Develop the feature on your branch and commit your work
4.Fetch and merge from the remote again (in case new commits were made while you were working)
5.Push your branch up to the remote for review
Steps 1 and 4 are a safeguard against merge conflicts, which occur when two branches contain file changes that cannot be merged

We also learned the following commands

git clone: Creates a local copy of a remote.
git remote -v: Lists a Git project's remotes.
git fetch: Fetches work from the remote into the local copy.
git merge origin/master: Merges origin/master into your local branch.
git push origin <branch_name>: Pushes a local branch to the origin remote