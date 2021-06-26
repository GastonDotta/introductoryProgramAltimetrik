! [img](https://lh3.googleusercontent.com/dnyDO-4zLMWbPGdEz7kMS1wtrTuzvEpNjWCswck1WAT9ADcoJHkxfB9I09hfUh69lv2VPggt3tbqLj_HaxjAWGvtP7yIj0Y0U2GmyaQ2BRRQdNklrWnFx27ZXNdJn-4-svnyZmID)

# Git: 
Git is the most popular open source Version Control System on the market.

## Branches:
A branch in Git is simply a lightweight movable pointer to one of these commits. The default branch name in Git is master.
## Branching Strategies & Flows: 
! [img](https://salesforcegraells.files.wordpress.com/2017/10/gitflow-workflow.jpg)
This Flowchart is usually the most commonly used (“Gitflow”) and proposes the division with 2 types of essential branches the "Master" branch, and the "Develop" branch, to which can be added the "Feature" branches, "Release" branches and "Hotfix" branches.

### The Master branch:
Usually contains the "Versions", so very few changes are usually made.
### Develop branch:
This is where the main work is done where once the changes made are "stable" and checked, a "merge" is made to a new version in the Master branch.
### Feature branches:
As the word indicates, are used to develop new program features.
### Release Branch:
In this branch the function is "tested", bugs are fixed, and the metadata is worked on in order to release a new version in the future. 
### Hotfix Branches
It is a branch that comes directly from the "Master" and is usually used to fix severe bugs.
## Commits and Tags:
A 'commit' or 'revision' is a modification that is applied to the repository. The first commit is called "Head" and new commits are always direct children of the last commit.
These files at that point may all be tagged with a user-friendly, meaningful name or revision number.
## Stash command:
“Stash'' comes from the word chest or cache, this command creates a ''box'' where the changes made without committing are saved.
## Hooks:
These are mechanisms that trigger scripts that are intended to automate actions within git.
## Rebase and squash: 
Rebase is the process of moving or combining a sequence of commits into a new base commit.
Squash refers to gathering several commits into one (from the same branch).
## Merge vs rebase:
Rebase unifies the branches leaving a linear tree “making it neater''. The merge still leaves ''alive'' the graphic of the branches.
