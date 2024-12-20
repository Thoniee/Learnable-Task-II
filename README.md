# Learnable-Task-II

# Explain Version Control

Version control is a system that manages changes to files, code, or projects over time. It allows multiple people to work on a project simultaneously, tracks changes, and provides a history of revisions. Popular tools like Git enable users to collaborate, revert to previous versions, and resolve conflicts efficiently, ensuring consistent progress and minimizing errors.

# Explain difference between git and github

Git is the tool for version control, while GitHub is a platform for hosting and collaborating on Git repositories.

# List 3 other github alternatives

1. GitLab

An open-source platform offering similar features to GitHub, including repository hosting, CI/CD, and project management tools.
Available as both a cloud-hosted service and a self-hosted option.

2. Bitbucket

Developed by Atlassian, it supports Git repositories and integrates seamlessly with other Atlassian products like Jira and Trello.
Offers both cloud-based hosting and on-premises solutions with Bitbucket Server.

3. SourceForge

One of the oldest platforms for hosting open-source projects.
Provides Git, Subversion (SVN), and Mercurial repository hosting, along with project management and distribution tools.

# Explain the difference between git fetch and git pull

 git fetch is used when you want to review changes before merging. While, git pull is used when you’re confident and want to update your branch directly without separate review.

 # Explain in simple terms git rebase and the command for it
  
Git rebase is a way to move or "reapply" your commits on top of another branch. It reorganizes your commit history to make it linear and cleaner, avoiding unnecessary merge commits.

In simple terms:  
- Imagine two people (you and a teammate) working on the same project in separate branches.  
- While you were working, your teammate made updates on the main branch.  
- To update your branch with their changes and keep the history neat, you "rebase" your branch onto the main branch.

Instead of merging the branches (which creates a "merge commit"), rebasing moves your changes to the latest commit of the main branch, as if they were made after your teammate’s changes.

- Command for Rebase 

git rebase <branch_name>

- For example;

git checkout feature-branch  
git rebase main  

This takes the commits from `feature-branch` and replays them on top of the `main` branch.

# Explain in simple terms git cherry-pick and the command for it
 
Git cherry-pick is a command used to apply a specific commit from one branch to another. Instead of merging or rebasing all the changes, cherry-pick allows you to "pick" a single commit you want and apply it to your current branch.

In simple terms:  
- Imagine someone made a useful change in their branch that you want in yours, but you don’t want all their other changes.  
- You can use cherry-pick to grab just that specific change and apply it to your branch.

- Command for Cherry-Pick  

git cherry-pick <commit_hash>

- Steps:  
1. Find the commit hash you want to cherry-pick (use `git log` to see the history).  
2. Run the `git cherry-pick` command with that hash.  

- For example:  
git cherry-pick 3a1b2c3d

This applies the changes from the commit `3a1b2c3d` to your current branch.




