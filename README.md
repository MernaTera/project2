 project 2
# How to Remove Branches Locally and Remotely

## Remove a Branch Locally
git checkout main
git branch -d dev


## Remove a Branch Remotely
git push origin --delete dev

#####

# Annotated tags vs Lightweight Tags
## Annotated Tags
Purpose:
Typically used for release versions (e.g., v1.0.0) or important commits where metadata is needed.

Data Stored:

Tag message (annotation)
Tagger's name and email
Date and time of tagging

command to create:

git tag -a <tag-name> -m "message of tag"

## Lightweight Tags
Purpose:
Used for temporary tags or when you only need a simple pointer to a commit.

Data Stored:

Only the tag name and the associated commit hash.
No additional metadata (e.g., tag message, tagger information, or date).

Command to create:

git tag <tag-name>


######


# how to list tags

command to use:

to list all tags:
git tag  

to list tags with commit:
git show <tag-name>
git tag -n

to list tags with matching pattern:
git tag -l 'tag-name*'


######

# how to delete tag locally and remotely
## Delete a tag Locally

git tag -d <tag-name>

## Delete a tag Remotely

git push origin --delete <tag-name>


######

# When to use Rebase

for a clean and linear Git history where that is critical

for cleaning a messy Git History

to Avoid merge confusion in feature branches

######

# adding an image via URL 
![Bonus](https://png.pngtree.com/png-clipart/20220206/original/pngtree-bonus-icon-on-transparent-background-png-image_7264198.png)


